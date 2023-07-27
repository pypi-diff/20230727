# Comparing `tmp/kfp-2.0.1.tar.gz` & `tmp/kfp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.CoJLbZ8K/kfp-2.0.1.tar", last modified: Wed Jun 21 00:23:29 2023, max compression
+gzip compressed data, was "kfp-2.1.1.tar", last modified: Thu Jul 27 17:15:22 2023, max compression
```

## Comparing `kfp-2.0.1.tar` & `kfp-2.1.1.tar`

### file list

```diff
@@ -1,250 +1,198 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-05-17 17:25:59.000000 kfp-2.0.1/MANIFEST.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-06-21 00:23:29.000000 kfp-2.0.1/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1972 2023-06-21 00:19:12.000000 kfp-2.0.1/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      882 2023-06-21 00:23:03.000000 kfp-2.0.1/kfp/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/cli_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5391 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/compile_.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/compile_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16229 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-03-14 22:48:17.000000 kfp-2.0.1/kfp/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/dsl.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/cli/utils/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/aliased_plurals_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/aliased_plurals_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/deprecated_alias_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/deprecated_alias_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/parsing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/cli/utils/parsing_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/client/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/client/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/client/auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66582 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/client/client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18470 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/client/client_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/client/set_volume_credentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/client/set_volume_credentials_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/client/token_credentials_base.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/client/token_credentials_base_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-05-19 17:00:33.000000 kfp-2.0.1/kfp/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3443 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   154348 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/compiler_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    33924 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/compiler_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1965 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/compiler_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85354 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/pipeline_spec_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/pipeline_spec_builder_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8163 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/compiler/read_write_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1321 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6055 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/base_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5432 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/base_component_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5995 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5489 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25321 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/component_factory.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6726 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/component_factory_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/constants.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1516 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/container_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1997 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/container_component_artifact_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1888 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/container_component_artifact_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1905 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/container_component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4574 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/container_component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15824 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/executor.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3649 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/executor_main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44835 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/executor_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11014 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6428 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/for_loop_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3399 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1015 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/importer_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5510 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/importer_node.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7662 2023-06-05 22:53:04.000000 kfp-2.0.1/kfp/components/importer_node_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/kfp_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13634 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/pipeline_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5981 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/pipeline_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6436 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/pipeline_context.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27240 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/pipeline_task.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12295 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/pipeline_task_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16441 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/placeholders.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    22066 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/placeholders_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1523 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/python_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44307 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    38004 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/structures_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-06-05 22:53:04.000000 kfp-2.0.1/kfp/components/task_final_status.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7711 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/tasks_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2851 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/tasks_group_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/components/types/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/types/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2415 2023-06-05 22:53:04.000000 kfp-2.0.1/kfp/components/types/artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8059 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/custom_artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16140 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/custom_artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7858 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/type_annotations.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7717 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/type_annotations_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19843 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    26536 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/types/type_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3679 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1740 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/v1_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/v1_modelbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27893 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/v1_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4214 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/components/yaml_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4324 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/components/yaml_component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/_auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-06-15 22:44:46.000000 kfp-2.0.1/kfp/deprecated/_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/_local_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/_runners.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/auth/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/auth/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/auth/_satvolumecredentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/auth/_tokencredentialsbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/aws.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/azure.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/components_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/_data_passing_rewriter.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/_data_passing_using_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/_default_transformers.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/_k8s_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/_op_to_template.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/v2_compat.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_airflow_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_component_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_data_passing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_dynamic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_key_value_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_naming.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_python_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_python_to_graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/_yaml_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/modelbase.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/components/structures/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/structures/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/type_annotation_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/components/type_annotation_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/containers/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_build_image_api.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_cache.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_component_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_container_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_gcs_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/_k8s_job_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/entrypoint.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/containers/entrypoint_utils.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_component_bridge.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_container_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_container_op_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_metadata.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_ops_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_pipeline_param.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_pipeline_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_resource_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_volume_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/_volume_snapshot_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/artifact.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/artifact_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/component_spec.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/component_spec_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/data_passing_methods.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/dsl_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/dsl_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/dsl/extensions/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/extensions/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/extensions/kubernetes.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-06-05 22:53:04.000000 kfp-2.0.1/kfp/deprecated/dsl/io_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/metrics_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/metrics_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/serialization_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/serialization_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-06-05 22:53:04.000000 kfp-2.0.1/kfp/deprecated/dsl/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/dsl/types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/gcp.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/deprecated/notebook/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/notebook/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/notebook/_magic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/deprecated/onprem.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7618 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/dsl/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/registry/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/registry/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/registry/context/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/registry/context/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/registry/context/default_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/registry/context/kfp_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/registry/registry_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/registry/registry_client_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp/v2/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-06-20 23:31:32.000000 kfp-2.0.1/kfp/v2/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/v2/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/v2/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-05-17 17:25:59.000000 kfp-2.0.1/kfp/v2/dsl.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7648 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/entry_points.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      451 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-06-21 00:23:29.000000 kfp-2.0.1/kfp.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1278 2023-06-20 23:31:32.000000 kfp-2.0.1/requirements.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-06-21 00:23:29.000000 kfp-2.0.1/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-06-20 23:31:32.000000 kfp-2.0.1/setup.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-21 00:23:29.000000 kfp-2.0.1/tests/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-03-14 22:48:17.000000 kfp-2.0.1/tests/test_kfp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921663 kfp-2.1.1/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-07-08 15:08:27.000000 kfp-2.1.1/MANIFEST.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-27 17:15:22.921509 kfp-2.1.1/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1972 2023-07-24 19:29:12.000000 kfp-2.1.1/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.895246 kfp-2.1.1/kfp/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      909 2023-07-27 01:00:40.000000 kfp-2.1.1/kfp/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.898441 kfp-2.1.1/kfp/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/cli_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5377 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/cli/compile_.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/compile_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16208 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/cli/component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.899704 kfp-2.1.1/kfp/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/dsl.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.900739 kfp-2.1.1/kfp/cli/utils/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/aliased_plurals_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/aliased_plurals_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/deprecated_alias_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/deprecated_alias_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/parsing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/cli/utils/parsing_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.902476 kfp-2.1.1/kfp/client/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66575 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/client/client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18470 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/client/client_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/set_volume_credentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/set_volume_credentials_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/token_credentials_base.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/client/token_credentials_base_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.903907 kfp-2.1.1/kfp/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3429 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   153764 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/compiler_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    33889 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/compiler_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1958 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/compiler/compiler_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85340 2023-07-27 17:14:48.000000 kfp-2.1.1/kfp/compiler/pipeline_spec_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/compiler/pipeline_spec_builder_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8175 2023-07-26 17:38:47.000000 kfp-2.1.1/kfp/compiler/read_write_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.904374 kfp-2.1.1/kfp/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1314 2023-07-24 19:29:12.000000 kfp-2.1.1/kfp/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6576 2023-07-26 00:11:33.000000 kfp-2.1.1/kfp/components/load_yaml_utilities.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5668 2023-07-26 00:11:33.000000 kfp-2.1.1/kfp/components/load_yaml_utilities_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.905912 kfp-2.1.1/kfp/deprecated/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-07-12 22:27:23.000000 kfp-2.1.1/kfp/deprecated/_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_local_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/_runners.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.906304 kfp-2.1.1/kfp/deprecated/auth/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/_satvolumecredentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/auth/_tokencredentialsbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/aws.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/azure.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.907810 kfp-2.1.1/kfp/deprecated/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/components_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.909141 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.910481 kfp-2.1.1/kfp/deprecated/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_data_passing_using_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_default_transformers.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_k8s_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/_op_to_template.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/v2_compat.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.912584 kfp-2.1.1/kfp/deprecated/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_airflow_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_component_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_data_passing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_dynamic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_key_value_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_naming.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_python_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_python_to_graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/_yaml_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/modelbase.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.912718 kfp-2.1.1/kfp/deprecated/components/structures/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/structures/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/type_annotation_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/components/type_annotation_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.913970 kfp-2.1.1/kfp/deprecated/containers/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_build_image_api.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_cache.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_component_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_container_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_gcs_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/_k8s_job_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/entrypoint.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/containers/entrypoint_utils.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919140 kfp-2.1.1/kfp/deprecated/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_component_bridge.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_container_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_container_op_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_metadata.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_ops_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline_param.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_pipeline_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_resource_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_volume_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/_volume_snapshot_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/artifact.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/artifact_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/component_spec.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/component_spec_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/data_passing_methods.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/dsl_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/dsl_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919398 kfp-2.1.1/kfp/deprecated/dsl/extensions/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/extensions/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/extensions/kubernetes.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/io_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/metrics_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/metrics_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/serialization_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/serialization_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/dsl/types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/gcp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.919673 kfp-2.1.1/kfp/deprecated/notebook/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/notebook/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/notebook/_magic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/deprecated/onprem.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.920106 kfp-2.1.1/kfp/registry/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.920552 kfp-2.1.1/kfp/registry/context/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/default_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/context/kfp_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/registry_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/registry/registry_client_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921110 kfp-2.1.1/kfp/v2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-07-08 15:08:27.000000 kfp-2.1.1/kfp/v2/dsl.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.896235 kfp-2.1.1/kfp.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3775 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5840 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/entry_points.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      466 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-07-27 17:15:22.000000 kfp-2.1.1/kfp.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1293 2023-07-27 01:00:40.000000 kfp-2.1.1/requirements.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-07-27 17:15:22.921710 kfp-2.1.1/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-07-12 22:27:24.000000 kfp-2.1.1/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 17:15:22.921257 kfp-2.1.1/tests/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-07-08 15:08:27.000000 kfp-2.1.1/tests/test_kfp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kfp-2.0.1/PKG-INFO` & `kfp-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.1
+Version: 2.1.1
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.0.1/README.md` & `kfp-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/__init__.py` & `kfp-2.1.1/kfp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # `kfp` is a namespace package.
 # https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
-__version__ = '2.0.1'
+__version__ = '2.1.1'
 
 TYPE_CHECK = True
 
+from kfp import components
 from kfp import dsl
 from kfp.client import Client
```

### Comparing `kfp-2.0.1/kfp/cli/__init__.py` & `kfp-2.1.1/kfp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/__main__.py` & `kfp-2.1.1/kfp/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/cli.py` & `kfp-2.1.1/kfp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/cli_test.py` & `kfp-2.1.1/kfp/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/compile_.py` & `kfp-2.1.1/kfp/cli/compile_.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import os
 import sys
 import types
 from typing import Callable, Dict, Optional
 
 import click
 from kfp import compiler
-from kfp.components import base_component
-from kfp.components import graph_component
+from kfp.dsl import base_component
+from kfp.dsl import graph_component
 
 
 def is_pipeline_func(func: Callable) -> bool:
     """Checks if a function is a pipeline function.
 
     Args:
         func (Callable): The function to check.
```

### Comparing `kfp-2.0.1/kfp/cli/compile_test.py` & `kfp-2.1.1/kfp/cli/compile_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/component.py` & `kfp-2.1.1/kfp/cli/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 _DOCKER_IS_PRESENT = True
 try:
     import docker
 except ImportError:
     _DOCKER_IS_PRESENT = False
 
 import kfp as kfp
-from kfp.components import component_factory
-from kfp.components import kfp_config
-from kfp.components import utils
+from kfp.dsl import component_factory
+from kfp.dsl import kfp_config
+from kfp.dsl import utils
 
 _REQUIREMENTS_TXT = 'runtime-requirements.txt'
 
 _DOCKERFILE = 'Dockerfile'
 
 # TODO: merge kfp_package_path into runtime-requirements.txt, once we have
 # kfp_runtime package that is dependency-free.
```

### Comparing `kfp-2.0.1/kfp/cli/component_test.py` & `kfp-2.1.1/kfp/cli/component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/__init__.py` & `kfp-2.1.1/kfp/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/dev_env.py` & `kfp-2.1.1/kfp/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/dev_env_test.py` & `kfp-2.1.1/kfp/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/gcp.py` & `kfp-2.1.1/kfp/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/gcp_test.py` & `kfp-2.1.1/kfp/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.1.1/kfp/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/utility.py` & `kfp-2.1.1/kfp/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me/utility_test.py` & `kfp-2.1.1/kfp/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/diagnose_me_cli.py` & `kfp-2.1.1/kfp/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/dsl.py` & `kfp-2.1.1/kfp/cli/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/experiment.py` & `kfp-2.1.1/kfp/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/output.py` & `kfp-2.1.1/kfp/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/pipeline.py` & `kfp-2.1.1/kfp/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/recurring_run.py` & `kfp-2.1.1/kfp/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/run.py` & `kfp-2.1.1/kfp/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/__init__.py` & `kfp-2.1.1/kfp/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/aliased_plurals_group.py` & `kfp-2.1.1/kfp/cli/utils/aliased_plurals_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/aliased_plurals_group_test.py` & `kfp-2.1.1/kfp/cli/utils/aliased_plurals_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/deprecated_alias_group.py` & `kfp-2.1.1/kfp/cli/utils/deprecated_alias_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/deprecated_alias_group_test.py` & `kfp-2.1.1/kfp/cli/utils/deprecated_alias_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/parsing.py` & `kfp-2.1.1/kfp/cli/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/cli/utils/parsing_test.py` & `kfp-2.1.1/kfp/cli/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/__init__.py` & `kfp-2.1.1/kfp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/auth.py` & `kfp-2.1.1/kfp/client/auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/client.py` & `kfp-2.1.1/kfp/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import warnings
 import zipfile
 
 from google.protobuf import json_format
 from kfp import compiler
 from kfp.client import auth
 from kfp.client import set_volume_credentials
-from kfp.components import base_component
+from kfp.dsl import base_component
 from kfp.pipeline_spec import pipeline_spec_pb2
 import kfp_server_api
 import yaml
 
 # Operators on scalar values. Only applies to one of |int_value|,
 # |long_value|, |string_value| or |timestamp_value|.
 _FILTER_OPERATIONS = {
```

### Comparing `kfp-2.0.1/kfp/client/client_test.py` & `kfp-2.1.1/kfp/client/client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/set_volume_credentials.py` & `kfp-2.1.1/kfp/client/set_volume_credentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/set_volume_credentials_test.py` & `kfp-2.1.1/kfp/client/set_volume_credentials_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/token_credentials_base.py` & `kfp-2.1.1/kfp/client/token_credentials_base.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/client/token_credentials_base_test.py` & `kfp-2.1.1/kfp/client/token_credentials_base_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/compiler/__init__.py` & `kfp-2.1.1/kfp/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/compiler/compiler.py` & `kfp-2.1.1/kfp/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 Implementation of KFP compiler that compiles KFP pipeline into Pipeline IR:
 https://docs.google.com/document/d/1PUDuSQ8vmeKSBloli53mp7GIvzekaY7sggg6ywy35Dk/
 """
 
 from typing import Any, Dict, Optional
 
 from kfp.compiler import pipeline_spec_builder as builder
-from kfp.components import base_component
-from kfp.components.types import type_utils
+from kfp.dsl import base_component
+from kfp.dsl.types import type_utils
 
 
 class Compiler:
     """Compiles pipelines composed using the KFP SDK DSL to a YAML pipeline
     definition.
 
     The pipeline definition is `PipelineSpec IR <https://github.com/kubeflow/pipelines/blob/2060e38c5591806d657d85b53eed2eef2e5de2ae/api/v2alpha1/pipeline_spec.proto#L50>`_, the protobuf message that defines a pipeline.
```

### Comparing `kfp-2.0.1/kfp/compiler/compiler_test.py` & `kfp-2.1.1/kfp/compiler/compiler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 from google.protobuf import json_format
 import kfp
 from kfp import components
 from kfp import dsl
 from kfp.cli import cli
 from kfp.compiler import compiler
 from kfp.compiler import compiler_utils
-from kfp.components import graph_component
-from kfp.components import pipeline_task
-from kfp.components import yaml_component
-from kfp.components.types import type_utils
 from kfp.dsl import Artifact
 from kfp.dsl import ContainerSpec
+from kfp.dsl import graph_component
 from kfp.dsl import Input
 from kfp.dsl import Model
 from kfp.dsl import Output
 from kfp.dsl import OutputPath
+from kfp.dsl import pipeline_task
 from kfp.dsl import PipelineTaskFinalStatus
+from kfp.dsl import yaml_component
+from kfp.dsl.types import type_utils
 from kfp.pipeline_spec import pipeline_spec_pb2
 import yaml
 
 VALID_PRODUCER_COMPONENT_SAMPLE = components.load_component_from_text("""
     name: producer
     inputs:
     - {name: input_param, type: String}
@@ -148,26 +148,14 @@
             compiler.Compiler().compile(
                 pipeline_func=simple_pipeline, package_path=target_json_file)
 
             self.assertTrue(os.path.exists(target_json_file))
             with open(target_json_file, 'r') as f:
                 f.read()
 
-    def test_compile_pipeline_with_dsl_graph_component_should_raise_error(self):
-
-        with self.assertRaisesRegex(
-                AttributeError,
-                "module 'kfp.dsl' has no attribute 'graph_component'"):
-
-            @dsl.graph_component
-            def flip_coin_graph_component():
-                flip = flip_coin_op()
-                with dsl.Condition(flip.output == 'heads'):
-                    flip_coin_graph_component()
-
     def test_compile_pipeline_with_misused_inputvalue_should_raise_error(self):
 
         upstream_op = components.load_component_from_text("""
         name: upstream compoent
         outputs:
         - {name: model, type: Model}
         implementation:
@@ -188,15 +176,15 @@
         """)
 
         with self.assertRaisesRegex(
                 TypeError,
                 ' type "system.Model@0.0.1" cannot be paired with InputValuePlaceholder.'
         ):
 
-            @dsl.pipeline(name='test-pipeline', pipeline_root='dummy_root')
+            @dsl.pipeline(name='test-pipeline')
             def my_pipeline():
                 downstream_op(model=upstream_op().output)
 
     def test_compile_pipeline_with_misused_inputpath_should_raise_error(self):
 
         component_op = components.load_component_from_text("""
         name: compoent with misused placeholder
@@ -209,24 +197,24 @@
             - {inputPath: text}
         """)
 
         with self.assertRaisesRegex(
                 TypeError,
                 ' type "String" cannot be paired with InputPathPlaceholder.'):
 
-            @dsl.pipeline(name='test-pipeline', pipeline_root='dummy_root')
+            @dsl.pipeline(name='test-pipeline')
             def my_pipeline(text: str):
                 component_op(text=text)
 
     def test_compile_pipeline_with_missing_task_should_raise_error(self):
 
         with self.assertRaisesRegex(ValueError,
                                     'Task is missing from pipeline.'):
 
-            @dsl.pipeline(name='test-pipeline', pipeline_root='dummy_root')
+            @dsl.pipeline(name='test-pipeline')
             def my_pipeline(text: str):
                 pass
 
     def test_compile_pipeline_with_misused_inputuri_should_raise_error(self):
 
         component_op = components.load_component_from_text("""
         name: compoent with misused placeholder
@@ -239,15 +227,15 @@
             - {inputUri: value}
         """)
 
         with self.assertRaisesRegex(
                 TypeError,
                 ' type "Float" cannot be paired with InputUriPlaceholder.'):
 
-            @dsl.pipeline(name='test-pipeline', pipeline_root='dummy_root')
+            @dsl.pipeline(name='test-pipeline')
             def my_pipeline(value: float):
                 component_op(value=value)
 
     def test_compile_pipeline_with_misused_outputuri_should_raise_error(self):
 
         component_op = components.load_component_from_text("""
         name: compoent with misused placeholder
@@ -260,15 +248,15 @@
             - {outputUri: value}
         """)
 
         with self.assertRaisesRegex(
                 TypeError,
                 ' type "Integer" cannot be paired with OutputUriPlaceholder.'):
 
-            @dsl.pipeline(name='test-pipeline', pipeline_root='dummy_root')
+            @dsl.pipeline(name='test-pipeline')
             def my_pipeline():
                 component_op()
 
     def test_compile_pipeline_with_invalid_name_should_raise_error(self):
 
         @dsl.pipeline(name='')
         def my_pipeline():
@@ -1307,15 +1295,16 @@
     pipeline_spec = spec.get('pipelineSpec', spec)
 
     if 'executors' in pipeline_spec['deploymentSpec']:
         for executor in pipeline_spec['deploymentSpec']['executors']:
             pipeline_spec['deploymentSpec']['executors'][
                 executor] = yaml.safe_load(
                     re.sub(
-                        r"'kfp==(\d+).(\d+).(\d+)(-[a-z]+.\d+)?'", 'kfp',
+                        r"'(kfp(-dsl)?)==(\d+).(\d+).(\d+)(-[a-z]+.\d+)?'",
+                        'kfp',
                         yaml.dump(
                             pipeline_spec['deploymentSpec']['executors']
                             [executor],
                             sort_keys=True)))
     return spec
```

### Comparing `kfp-2.0.1/kfp/compiler/compiler_utils.py` & `kfp-2.1.1/kfp/compiler/compiler_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # limitations under the License.
 """Utility methods for compiler implementation that is IR-agnostic."""
 
 import collections
 from copy import deepcopy
 from typing import DefaultDict, Dict, List, Mapping, Set, Tuple, Union
 
-from kfp.components import for_loop
-from kfp.components import pipeline_channel
-from kfp.components import pipeline_context
-from kfp.components import pipeline_task
-from kfp.components import tasks_group
+from kfp.dsl import for_loop
+from kfp.dsl import pipeline_channel
+from kfp.dsl import pipeline_context
+from kfp.dsl import pipeline_task
+from kfp.dsl import tasks_group
 
 GroupOrTaskType = Union[tasks_group.TasksGroup, pipeline_task.PipelineTask]
 
 ILLEGAL_CROSS_DAG_ERROR_PREFIX = 'Illegal task dependency across DSL context managers.'
 
 
 def additional_input_name_for_pipeline_channel(
```

### Comparing `kfp-2.0.1/kfp/compiler/compiler_utils_test.py` & `kfp-2.1.1/kfp/compiler/compiler_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 from absl.testing import parameterized
 from kfp.compiler import compiler_utils
-from kfp.components import pipeline_channel
+from kfp.dsl import pipeline_channel
 
 
 class TestAdditionalInputNameForPipelineChannel(parameterized.TestCase):
 
     @parameterized.parameters(
         {
             'channel':
```

### Comparing `kfp-2.0.1/kfp/compiler/pipeline_spec_builder.py` & `kfp-2.1.1/kfp/compiler/pipeline_spec_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
                     Union)
 import warnings
 
 from google.protobuf import json_format
 from google.protobuf import struct_pb2
 import kfp
 from kfp.compiler import compiler_utils
-from kfp.components import for_loop
-from kfp.components import pipeline_channel
-from kfp.components import pipeline_context
-from kfp.components import pipeline_task
-from kfp.components import placeholders
-from kfp.components import structures
-from kfp.components import tasks_group
-from kfp.components import utils
-from kfp.components.types import artifact_types
-from kfp.components.types import type_utils
+from kfp.dsl import for_loop
+from kfp.dsl import pipeline_channel
+from kfp.dsl import pipeline_context
+from kfp.dsl import pipeline_task
+from kfp.dsl import placeholders
+from kfp.dsl import structures
+from kfp.dsl import tasks_group
+from kfp.dsl import utils
+from kfp.dsl.types import artifact_types
+from kfp.dsl.types import type_utils
 from kfp.pipeline_spec import pipeline_spec_pb2
 import yaml
 
 # must be defined here to avoid circular imports
 group_type_to_dsl_class = {
     tasks_group.TasksGroupType.PIPELINE: pipeline_context.Pipeline,
     tasks_group.TasksGroupType.CONDITION: tasks_group.Condition,
@@ -1744,14 +1744,15 @@
         output_name = '' if len(dag_outputs) == 1 else f'{output_name!r} '
         error_message_prefix = f'Incompatible return type provided for output {output_name}of pipeline {structures_component_spec.name!r}. '
         type_utils.verify_type_compatibility(
             output_channel,
             output_spec,
             error_message_prefix,
             checks_input=False,
+            raise_on_error=kfp.TYPE_CHECK,
         )
 
 
 def convert_pipeline_outputs_to_dict(
     pipeline_outputs: Union[pipeline_channel.PipelineChannel, typing.NamedTuple,
                             None]
 ) -> Dict[str, pipeline_channel.PipelineChannel]:
@@ -1766,15 +1767,15 @@
         return dict(pipeline_outputs._asdict())
     else:
         raise ValueError(f'Got unknown pipeline output: {pipeline_outputs}')
 
 
 def write_pipeline_spec_to_file(
     pipeline_spec: pipeline_spec_pb2.PipelineSpec,
-    pipeline_description: str,
+    pipeline_description: Union[str, None],
     platform_spec: pipeline_spec_pb2.PlatformSpec,
     package_path: str,
 ) -> None:
     """Writes PipelineSpec into a YAML or JSON (deprecated) file.
 
     Args:
         pipeline_spec: The PipelineSpec.
```

### Comparing `kfp-2.0.1/kfp/compiler/pipeline_spec_builder_test.py` & `kfp-2.1.1/kfp/compiler/pipeline_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/compiler/read_write_test.py` & `kfp-2.1.1/kfp/compiler/read_write_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import tempfile
 from typing import Any, Callable, Dict, List, Union
 import unittest
 
 from absl.testing import parameterized
 from kfp import compiler
 from kfp import components
-from kfp.components import placeholders
-from kfp.components import python_component
-from kfp.components import structures
+from kfp.dsl import placeholders
+from kfp.dsl import python_component
+from kfp.dsl import structures
 import yaml
 
 _PROJECT_ROOT = os.path.abspath(os.path.join(__file__, *([os.path.pardir] * 5)))
 
 
 def create_test_cases() -> List[Dict[str, Any]]:
     parameters: List[Dict[str, Any]] = []
@@ -70,15 +70,16 @@
     pipeline_spec = spec.get('pipelineSpec', spec)
 
     if 'executors' in pipeline_spec['deploymentSpec']:
         for executor in pipeline_spec['deploymentSpec']['executors']:
             pipeline_spec['deploymentSpec']['executors'][
                 executor] = yaml.safe_load(
                     re.sub(
-                        r"'kfp==(\d+).(\d+).(\d+)(-[a-z]+.\d+)?'", 'kfp',
+                        r"'(kfp(-dsl)?)==(\d+).(\d+).(\d+)(-[a-z]+.\d+)?'",
+                        'kfp',
                         yaml.dump(
                             pipeline_spec['deploymentSpec']['executors']
                             [executor],
                             sort_keys=True)))
     return spec
```

### Comparing `kfp-2.0.1/kfp/components/__init__.py` & `kfp-2.1.1/kfp/components/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,14 @@
     'load_component_from_text',
     'PythonComponent',
     'BaseComponent',
     'ContainerComponent',
     'YamlComponent',
 ]
 
-from kfp.components.base_component import BaseComponent
-from kfp.components.container_component import ContainerComponent
-from kfp.components.python_component import PythonComponent
-from kfp.components.yaml_component import load_component_from_file
-from kfp.components.yaml_component import load_component_from_text
-from kfp.components.yaml_component import load_component_from_url
-from kfp.components.yaml_component import YamlComponent
+from kfp.components.load_yaml_utilities import load_component_from_file
+from kfp.components.load_yaml_utilities import load_component_from_text
+from kfp.components.load_yaml_utilities import load_component_from_url
+from kfp.dsl.base_component import BaseComponent
+from kfp.dsl.container_component_class import ContainerComponent
+from kfp.dsl.python_component import PythonComponent
+from kfp.dsl.yaml_component import YamlComponent
```

### Comparing `kfp-2.0.1/kfp/components/base_component.py` & `kfp-2.1.1/kfp/deprecated/dsl/_component.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,149 +1,167 @@
-# Copyright 2021 The Kubeflow Authors
+# Copyright 2018 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Base class for KFP components."""
 
-import abc
-from typing import List
-
-from kfp.components import pipeline_task
-from kfp.components import structures
-from kfp.components.types import type_utils
-from kfp.pipeline_spec import pipeline_spec_pb2
-
-
-class BaseComponent(abc.ABC):
-    """Base class for a component.
-
-    **Note:** ``BaseComponent`` is not intended to be used to construct components directly. Use ``@kfp.dsl.component`` or ``kfp.components.load_component_from_*()`` instead.
-
-    Attributes:
-      name: Name of the component.
-      component_spec: Component definition.
+import inspect
+from ._pipeline_param import PipelineParam
+from .types import check_types, InconsistentTypeException
+from ._ops_group import Graph
+import kfp.deprecated as kfp
+
+# @deprecated(
+#     version='0.2.6',
+#     reason='This decorator does not seem to be used, so we deprecate it. '
+#     'If you need this decorator, please create an issue at '
+#     'https://github.com/kubeflow/pipelines/issues',
+# )
+# def python_component(name,
+#                      description=None,
+#                      base_image=None,
+#                      target_component_file: str = None):
+#     """Decorator for Python component functions.
+
+#     This decorator adds the metadata to the function object itself.
+
+#     Args:
+#       name: Human-readable name of the component
+#       description: Optional. Description of the component
+#       base_image: Optional. Docker container image to use as the base of the
+#         component. Needs to have Python 3.5+ installed.
+#       target_component_file: Optional. Local file to store the component
+#         definition. The file can then be used for sharing.
+
+#     Returns:
+#       The same function (with some metadata fields set).
+
+#     Example:
+#       ::
+
+#         @dsl.python_component(
+#           name='my awesome component',
+#           description='Come, Let\'s play',
+#           base_image='tensorflow/tensorflow:1.11.0-py3',
+#         )
+#         def my_component(a: str, b: int) -> str:
+#           ...
+#     """
+
+#     def _python_component(func):
+#         func._component_human_name = name
+#         if description:
+#             func._component_description = description
+#         if base_image:
+#             func._component_base_image = base_image
+#         if target_component_file:
+#             func._component_target_component_file = target_component_file
+#         return func
+
+#     return _python_component
+
+
+def component(func):
+    """Decorator for component functions that returns a ContainerOp.
+
+    This is useful to enable type checking in the DSL compiler.
+
+    Example:
+      ::
+
+        @dsl.component
+        def foobar(model: TFModel(), step: MLStep()):
+          return dsl.ContainerOp()
     """
+    from functools import wraps
 
-    def __init__(self, component_spec: structures.ComponentSpec):
-        """Init function for BaseComponent.
-
-        Args:
-          component_spec: The component definition.
-        """
-        self.component_spec = component_spec
-        self.name = component_spec.name
-        self.description = component_spec.description or None
-
-        # Arguments typed as PipelineTaskFinalStatus are special arguments that
-        # do not count as user inputs. Instead, they are reserved to for the
-        # (backend) system to pass a value.
-        self._component_inputs = {
-            input_name for input_name, input_spec in (
-                self.component_spec.inputs or {}).items()
-            if not type_utils.is_task_final_status_type(input_spec.type)
-        }
-
-    def _prevent_using_output_lists_of_artifacts(self):
-        """This method should be called at the end of __init__ for
-        PythonComponent and ContainerComponent subclasses to temporarily block
-        outputting lists of artifacts from a component."""
-        # TODO: remove when output lists of artifacts from primitive components is supported
-        for output_name, output_spec in (self.component_spec.outputs or
-                                         {}).items():
-            if output_spec.is_artifact_list:
-                raise ValueError(
-                    f'Output lists of artifacts are only supported for pipelines. Got output list of artifacts for output parameter {output_name!r} of component {self.name!r}.'
-                )
-
-    def __call__(self, *args, **kwargs) -> pipeline_task.PipelineTask:
-        """Creates a PipelineTask object.
-
-        The arguments are generated on the fly based on component input
-        definitions.
-        """
-        task_inputs = {}
-
-        if args:
-            raise TypeError(
-                'Components must be instantiated using keyword arguments. Positional '
-                f'parameters are not allowed (found {len(args)} such parameters for '
-                f'component "{self.name}").')
-
-        for k, v in kwargs.items():
-            if k not in self._component_inputs:
-                raise TypeError(
-                    f'{self.name}() got an unexpected keyword argument "{k}".')
-            task_inputs[k] = v
-
-        # Skip optional inputs and arguments typed as PipelineTaskFinalStatus.
-        missing_arguments = [
-            arg for arg in self.required_inputs if arg not in kwargs
-        ]
-        if missing_arguments:
-            argument_or_arguments = 'argument' if len(
-                missing_arguments) == 1 else 'arguments'
-            arguments = ', '.join(
-                arg_name.replace('-', '_') for arg_name in missing_arguments)
-
-            raise TypeError(
-                f'{self.name}() missing {len(missing_arguments)} required '
-                f'{argument_or_arguments}: {arguments}.')
-
-        return pipeline_task.PipelineTask(
-            component_spec=self.component_spec,
-            args=task_inputs,
-        )
-
-    @property
-    def pipeline_spec(self) -> pipeline_spec_pb2.PipelineSpec:
-        """Returns the pipeline spec of the component."""
-        with BlockPipelineTaskRegistration():
-            return self.component_spec.to_pipeline_spec()
-
-    @property
-    def platform_spec(self) -> pipeline_spec_pb2.PlatformSpec:
-        """Returns the PlatformSpec of the component.
-
-        Useful when the component is a GraphComponent, else will be
-        empty per component_spec.platform_spec default.
-        """
-        return self.component_spec.platform_spec
-
-    @abc.abstractmethod
-    def execute(self, **kwargs):
-        """Executes the component locally if implemented by the inheriting
-        subclass."""
-
-    @property
-    def required_inputs(self) -> List[str]:
-        return [
-            input_name for input_name, input_spec in (
-                self.component_spec.inputs or {}).items()
-            if not input_spec.optional
-        ]
-
-
-class BlockPipelineTaskRegistration:
-    """Temporarily stop registering tasks to the default pipeline.
-
-    Handles special, uncommon functions that decorate and mutate a
-    component, possibly by using the component's .pipeline_spec
-    attribute. This is exhibited in the version of
-    google_cloud_pipeline_components compatible with KFP SDK v2.
+    @wraps(func)
+    def _component(*args, **kargs):
+        from ..components._python_op import _extract_component_interface
+        component_meta = _extract_component_interface(func)
+        if kfp.TYPE_CHECK:
+            arg_index = 0
+            for arg in args:
+                if isinstance(arg, PipelineParam) and not check_types(
+                        arg.param_type, component_meta.inputs[arg_index].type):
+                    raise InconsistentTypeException(
+                        'Component "' + component_meta.name +
+                        '" is expecting ' +
+                        component_meta.inputs[arg_index].name + ' to be type(' +
+                        str(component_meta.inputs[arg_index].type) +
+                        '), but the passed argument is type(' +
+                        str(arg.param_type) + ')')
+                arg_index += 1
+            if kargs is not None:
+                for key in kargs:
+                    if isinstance(kargs[key], PipelineParam):
+                        for input_spec in component_meta.inputs:
+                            if input_spec.name == key and not check_types(
+                                    kargs[key].param_type, input_spec.type):
+                                raise InconsistentTypeException(
+                                    'Component "' + component_meta.name +
+                                    '" is expecting ' + input_spec.name +
+                                    ' to be type(' + str(input_spec.type) +
+                                    '), but the passed argument is type(' +
+                                    str(kargs[key].param_type) + ')')
+
+        container_op = func(*args, **kargs)
+        container_op._set_metadata(component_meta)
+        return container_op
+
+    return _component
+
+
+#TODO: combine the component and graph_component decorators into one
+def graph_component(func):
+    """Decorator for graph component functions.
+
+    This decorator returns an ops_group.
+
+    Example:
+      ::
+
+        # Warning: caching is tricky when recursion is involved. Please be careful
+        # and set proper max_cache_staleness in case of infinite loop.
+        import kfp.dsl as dsl
+        @dsl.graph_component
+        def flip_component(flip_result):
+          print_flip = PrintOp(flip_result)
+          flipA = FlipCoinOp().after(print_flip)
+          flipA.execution_options.caching_strategy.max_cache_staleness = "P0D"
+          with dsl.Condition(flipA.output == 'heads'):
+            flip_component(flipA.output)
+          return {'flip_result': flipA.output}
     """
+    from functools import wraps
 
-    # TODO: this handles the special case of a compiled component (when compiled inside a pipeline), which should not have any concept of a default pipeline. Perhaps there is a way to unify component/pipeline compilation concepts to remove this workaround?
+    @wraps(func)
+    def _graph_component(*args, **kargs):
+        # We need to make sure that the arguments are correctly mapped to inputs
+        # regardless of the passing order
+        signature = inspect.signature(func)
+        bound_arguments = signature.bind(*args, **kargs)
+        graph_ops_group = Graph(func.__name__)
+        graph_ops_group.inputs = list(bound_arguments.arguments.values())
+        graph_ops_group.arguments = bound_arguments.arguments
+        for input in graph_ops_group.inputs:
+            if not isinstance(input, PipelineParam):
+                raise ValueError('arguments to ' + func.__name__ +
+                                 ' should be PipelineParams.')
+
+        # Entering the Graph Context
+        with graph_ops_group:
+            # Call the function
+            if not graph_ops_group.recursive_ref:
+                func(*args, **kargs)
 
-    def __enter__(self):
-        self.task_handler, pipeline_task.PipelineTask._register_task_handler = pipeline_task.PipelineTask._register_task_handler, pipeline_task._register_task_handler
+        return graph_ops_group
 
-    def __exit__(self, *args):
-        pipeline_task.PipelineTask._register_task_handler = self.task_handler
+    return _graph_component
```

### Comparing `kfp-2.0.1/kfp/components/component_decorator_test.py` & `kfp-2.1.1/kfp/components/load_yaml_utilities_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,171 @@
-# Copyright 2022 The Kubeflow Authors
+# Copyright 2021 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Tests for kfp.dsl.yaml_component."""
 
 import os
 import tempfile
-from typing import Dict, List, NamedTuple
+import textwrap
 import unittest
 
-from kfp.components import python_component
-from kfp.components import structures
-from kfp.components.component_decorator import component
+from kfp import components
+from kfp.components import load_yaml_utilities
+from kfp.dsl import structures
+
+SAMPLE_YAML = textwrap.dedent("""\
+components:
+  comp-component-1:
+    executorLabel: exec-component-1
+    inputDefinitions:
+      parameters:
+        input1:
+          parameterType: STRING
+    outputDefinitions:
+      parameters:
+        output1:
+          parameterType: STRING
+deploymentSpec:
+  executors:
+    exec-component-1:
+      container:
+        command:
+        - sh
+        - -c
+        - 'set -ex
+
+          echo "$0" > "$1"'
+        - '{{$.inputs.parameters[''input1'']}}'
+        - '{{$.outputs.parameters[''output1''].output_file}}'
+        image: alpine
+pipelineInfo:
+  name: component-1
+root:
+  dag:
+    tasks:
+      component-1:
+        cachingOptions:
+          enableCache: true
+        componentRef:
+          name: comp-component-1
+        inputs:
+          parameters:
+            input1:
+              componentInputParameter: input1
+        taskInfo:
+          name: component-1
+  inputDefinitions:
+    parameters:
+      input1:
+        parameterType: STRING
+schemaVersion: 2.1.0
+sdkVersion: kfp-2.0.0-alpha.3
+        """)
+
+V1_COMPONENTS_TEST_DATA_DIR = os.path.join(
+    os.path.dirname(os.path.dirname(__file__)), 'compiler', 'test_data',
+    'v1_component_yaml')
+
+V1_COMPONENT_YAML_TEST_CASES = [
+    'concat_placeholder_component.yaml',
+    'ingestion_component.yaml',
+    'serving_component.yaml',
+    'if_placeholder_component.yaml',
+    'trainer_component.yaml',
+    'add_component.yaml',
+]
+
+
+class LoadYamlTests(unittest.TestCase):
+
+    def test_load_component_from_text(self):
+        component = components.load_component_from_text(SAMPLE_YAML)
+        self.assertEqual(component.component_spec.name, 'component-1')
+        self.assertEqual(component.component_spec.outputs,
+                         {'output1': structures.OutputSpec(type='String')})
+        self.assertEqual(component._component_inputs, {'input1'})
+        self.assertEqual(component.name, 'component-1')
+        self.assertEqual(
+            component.component_spec.implementation.container.image, 'alpine')
 
+    def test_load_component_from_file(self):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            path = os.path.join(tmpdir, 'sample_yaml.yaml')
+            with open(path, 'w') as f:
+                f.write(SAMPLE_YAML)
+            component = components.load_component_from_file(path)
+        self.assertEqual(component.component_spec.name, 'component-1')
+        self.assertEqual(component.component_spec.outputs,
+                         {'output1': structures.OutputSpec(type='String')})
+        self.assertEqual(component._component_inputs, {'input1'})
+        self.assertEqual(component.name, 'component-1')
+        self.assertEqual(
+            component.component_spec.implementation.container.image, 'alpine')
+
+    def test_load_component_from_url(self):
+        component_url = 'https://raw.githubusercontent.com/kubeflow/pipelines/7b49eadf621a9054e1f1315c86f95fb8cf8c17c3/sdk/python/kfp/compiler/test_data/components/identity.yaml'
+        component = components.load_component_from_url(component_url)
+
+        self.assertEqual(component.component_spec.name, 'identity')
+        self.assertEqual(component.component_spec.outputs,
+                         {'Output': structures.OutputSpec(type='String')})
+        self.assertEqual(component._component_inputs, {'value'})
+        self.assertEqual(component.name, 'identity')
+        self.assertEqual(
+            component.component_spec.implementation.container.image,
+            'python:3.7')
+
+
+class TestLoadDocumentsFromYAML(unittest.TestCase):
+
+    def test_no_documents(self):
+        with self.assertRaisesRegex(
+                ValueError,
+                r'Expected one or two YAML documents in the IR YAML file\. Got\: 0\.'
+        ):
+            load_yaml_utilities._load_documents_from_yaml('')
+
+    def test_one_document(self):
+        doc1, doc2 = load_yaml_utilities._load_documents_from_yaml(
+            textwrap.dedent("""\
+            key1: value1
+            """))
+        self.assertEqual(doc1, {'key1': 'value1'})
+        self.assertEqual(doc2, {})
+
+    def test_two_documents(self):
+        doc1, doc2 = load_yaml_utilities._load_documents_from_yaml(
+            textwrap.dedent("""\
+            key1: value1
+            ---
+            key2: value2
+            """))
+        self.assertEqual(doc1, {'key1': 'value1'})
+        self.assertEqual(doc2, {'key2': 'value2'})
+
+    def test_three_documents(self):
+        with self.assertRaisesRegex(
+                ValueError,
+                r'Expected one or two YAML documents in the IR YAML file\. Got\: 3\.'
+        ):
+            load_yaml_utilities._load_documents_from_yaml(
+                textwrap.dedent("""\
+                key3: value3
+                ---
+                key3: value3
+                ---
+                key3: value3
+                """))
 
-class TestComponentDecorator(unittest.TestCase):
-
-    def test_as_decorator_syntactic_sugar_no_args(self):
-
-        @component
-        def hello_world(text: str) -> str:
-            """Hello world component."""
-            return text
-
-        self.assertIsInstance(hello_world, python_component.PythonComponent)
-
-    def test_as_decorator_syntactic_sugar_some_args(self):
-
-        @component(base_image='python:3.9')
-        def hello_world(text: str) -> str:
-            """Hello world component."""
-            return text
-
-        self.assertIsInstance(hello_world, python_component.PythonComponent)
-
-    def test_no_args(self):
-
-        @component
-        def comp(text: str) -> str:
-            return text
-
-        self.assertIsInstance(comp, python_component.PythonComponent)
-
-    def test_some_args(self):
-
-        @component(base_image='python:3.9')
-        def comp(text: str) -> str:
-            return text
-
-        self.assertIsInstance(comp, python_component.PythonComponent)
-
-    def test_packages_to_install(self):
-
-        @component(packages_to_install=['numpy', 'tensorflow'])
-        def comp(text: str) -> str:
-            return text
-
-        self.assertIsInstance(comp, python_component.PythonComponent)
-
-        concat_command = ' '.join(
-            comp.component_spec.implementation.container.command)
-        self.assertTrue('numpy' in concat_command and
-                        'tensorflow' in concat_command)
-
-    def test_packages_to_install_with_custom_index_url(self):
-
-        @component(
-            packages_to_install=['numpy', 'tensorflow'],
-            pip_index_urls=['https://pypi.org/simple'])
-        def comp(text: str) -> str:
-            return text
-
-        self.assertIsInstance(comp, python_component.PythonComponent)
-
-        concat_command = ' '.join(
-            comp.component_spec.implementation.container.command)
-        self.assertTrue('numpy' in concat_command and
-                        'tensorflow' in concat_command)
-        self.assertTrue('https://pypi.org/simple' in concat_command)
 
-    def test_output_component_file_parameter(self):
-        with tempfile.TemporaryDirectory() as tmpdir:
-            filepath = os.path.join(tmpdir, 'my_component.yaml')
-            with self.assertWarnsRegex(
-                    DeprecationWarning,
-                    r'output_component_file parameter is deprecated and will eventually be removed\.'
-            ):
-
-                @component(output_component_file=filepath)
-                def comp(text: str) -> str:
-                    return text
-
-            self.assertIsInstance(comp, python_component.PythonComponent)
-            self.assertTrue(os.path.exists(filepath))
-            with open(filepath, 'r') as f:
-                yaml_text = f.read()
-
-        component_spec = structures.ComponentSpec.from_yaml_documents(yaml_text)
-        self.assertEqual(component_spec.name, comp.component_spec.name)
-
-    def test_output_named_tuple_with_dict(self):
-
-        @component
-        def comp(
-                text: str) -> NamedTuple('outputs', [('data', Dict[str, str])]):
-            outputs = NamedTuple('outputs', [('data', Dict[str, str])])
-            return outputs(data={text: text})
-
-        # TODO: ideally should be the canonical type string, rather than the specific annotation as string, but both work
-        self.assertEqual(comp.component_spec.outputs['data'].type,
-                         'typing.Dict[str, str]')
-
-    def test_output_dict(self):
-
-        @component
-        def comp(text: str) -> Dict[str, str]:
-            return {text: text}
-
-        # TODO: ideally should be the canonical type string, rather than the specific annotation as string, but both work
-        self.assertEqual(comp.component_spec.outputs['Output'].type,
-                         'typing.Dict[str, str]')
-
-    def test_output_named_tuple_with_list(self):
-
-        @component
-        def comp(text: str) -> NamedTuple('outputs', [('data', List[str])]):
-            outputs = NamedTuple('outputs', [('data', List[str])])
-            return outputs(data={text: text})
-
-        # TODO: ideally should be the canonical type string, rather than the specific annotation as string, but both work
-        self.assertEqual(comp.component_spec.outputs['data'].type,
-                         'typing.List[str]')
-
-    def test_output_list(self):
-
-        @component
-        def comp(text: str) -> List[str]:
-            return {text: text}
-
-        # TODO: ideally should be the canonical type string, rather than the specific annotation as string, but both work
-        self.assertEqual(comp.component_spec.outputs['Output'].type,
-                         'typing.List[str]')
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `kfp-2.0.1/kfp/components/constants.py` & `kfp-2.1.1/kfp/deprecated/dsl/serialization_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-# Copyright 2021 The Kubeflow Authors
+# Copyright 2020 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Constants."""
+"""Utilities for serialization/deserialization."""
+from typing import Any, Dict
+import yaml
 
-# Unit constants for k8s size string.
-_E = 10**18  # Exa
-_EI = 1 << 60  # Exa: power-of-two approximate
-_P = 10**15  # Peta
-_PI = 1 << 50  # Peta: power-of-two approximate
-# noinspection PyShadowingBuiltins
-_T = 10**12  # Tera
-_TI = 1 << 40  # Tera: power-of-two approximate
-_G = 10**9  # Giga
-_GI = 1 << 30  # Giga: power-of-two approximate
-_M = 10**6  # Mega
-_MI = 1 << 20  # Mega: power-of-two approximate
-_K = 10**3  # Kilo
-_KI = 1 << 10  # Kilo: power-of-two approximate
+
+# Serialize None as blank instead of 'null'.
+def _represent_none(self, _):
+    return self.represent_scalar('tag:yaml.org,2002:null', '')
+
+
+class _NoneAsBlankDumper(yaml.SafeDumper):
+    """Alternative dumper to print YAML literal.
+
+    The behavior is mostly identical to yaml.SafeDumper, except for this
+    dumper dumps None object as blank, instead of 'null'.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.add_representer(type(None), _represent_none)
+
+
+def yaml_dump(data: Dict[str, Any]) -> str:
+    """Dumps YAML string.
+
+    None will be represented as blank.
+    """
+    return yaml.dump(data, Dumper=_NoneAsBlankDumper)
```

### Comparing `kfp-2.0.1/kfp/components/for_loop.py` & `kfp-2.1.1/kfp/deprecated/dsl/_for_loop.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,309 +7,251 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Classes and methods that supports argument for ParallelFor."""
-
 import re
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-from kfp.components import pipeline_channel
+from kfp.deprecated import dsl
+from kfp.deprecated.dsl import _pipeline_param
 
 ItemList = List[Union[int, float, str, Dict[str, Any]]]
 
 
-def _get_loop_item_type(type_name: str) -> Optional[str]:
-    """Extracts the loop item type.
-
-    This method is used for extract the item type from a collection type.
-    For example:
-
-        List[str] -> str
-        typing.List[int] -> int
-        typing.Sequence[str] -> str
-        List -> None
-        str -> None
-
-    Args:
-        type_name: The collection type name, like `List`, Sequence`, etc.
-
-    Returns:
-        The collection item type or None if no match found.
-    """
-    match = re.match('(typing\.)?(?:\w+)(?:\[(?P<item_type>.+)\])', type_name)
-    return match['item_type'].lstrip().rstrip() if match else None
-
-
-def _get_subvar_type(type_name: str) -> Optional[str]:
-    """Extracts the subvar type.
-
-    This method is used for extract the value type from a dictionary type.
-    For example:
+class LoopArguments(dsl.PipelineParam):
+    """Class representing the arguments that are looped over in a ParallelFor
+    loop in the KFP DSL.
 
-        Dict[str, int] -> int
-        typing.Mapping[str, float] -> float
-
-    Args:
-        type_name: The dictionary type.
-
-    Returns:
-        The dictionary value type or None if no match found.
-    """
-    match = re.match(
-        '(typing\.)?(?:\w+)(?:\[\s*(?:\w+)\s*,\s*(?P<value_type>.+)\])',
-        type_name)
-    return match['value_type'].lstrip().rstrip() if match else None
-
-
-class LoopArgument(pipeline_channel.PipelineParameterChannel):
-    """Represents the argument that are looped over in a ParallelFor loop.
-
-    The class shouldn't be instantiated by the end user, rather it is
-    created automatically by a ParallelFor ops group.
-
-    To create a LoopArgument instance, use one of its factory methods::
-
-        LoopArgument.from_pipeline_channel(...)
-        LoopArgument.from_raw_items(...)
-
-
-    Attributes:
-        items_or_pipeline_channel: The raw items or the PipelineChannel object
-            this LoopArgument is associated to.
+    This doesn't need to be instantiated by the end user, rather it will
+    be automatically created by a ParallelFor ops group.
     """
     LOOP_ITEM_NAME_BASE = 'loop-item'
     LOOP_ITEM_PARAM_NAME_BASE = 'loop-item-param'
+    # number of characters in the code which is passed to the constructor
+    NUM_CODE_CHARS = 8
+    LEGAL_SUBVAR_NAME_REGEX = re.compile(r'^[a-zA-Z_][0-9a-zA-Z_]*$')
 
-    def __init__(
-        self,
-        items: Union[ItemList, pipeline_channel.PipelineChannel],
-        name_code: Optional[str] = None,
-        name_override: Optional[str] = None,
-        **kwargs,
-    ):
-        """Initializes a LoopArguments object.
+    @classmethod
+    def _subvar_name_is_legal(cls, proposed_variable_name: str):
+        return re.match(cls.LEGAL_SUBVAR_NAME_REGEX,
+                        proposed_variable_name) is not None
+
+    def __init__(self,
+                 items: Union[ItemList, dsl.PipelineParam],
+                 code: str,
+                 name_override: Optional[str] = None,
+                 op_name: Optional[str] = None,
+                 *args,
+                 **kwargs):
+        """LoopArguments represent the set of items to loop over in a
+        ParallelFor loop.
+
+        This class shouldn't be instantiated by the user but rather is created by
+        _ops_group.ParallelFor.
 
         Args:
-            items: List of items to loop over.  If a list of dicts then, all
-                dicts must have the same keys and every key must be a legal
-                Python variable name.
-            name_code: A unique code used to identify these loop arguments.
-                Should match the code for the ParallelFor ops_group which created
-                these LoopArguments. This prevents parameter name collisions.
-            name_override: The override name for PipelineChannel.
-            **kwargs: Any other keyword arguments passed down to PipelineChannel.
+          items: List of items to loop over.  If a list of dicts then, all
+            dicts must have the same keys and every key must be a legal Python
+            variable name.
+          code: A unique code used to identify these loop arguments.  Should
+            match the code for the ParallelFor ops_group which created these
+            LoopArguments.  This prevents parameter name collisions.
         """
-        if (name_code is None) == (name_override is None):
-            raise ValueError(
-                'Expect one and only one of `name_code` and `name_override` to '
-                'be specified.')
-
         if name_override is None:
-            super().__init__(name=self._make_name(name_code), **kwargs)
+            super().__init__(name=self._make_name(code), *args, **kwargs)
         else:
-            super().__init__(name=name_override, **kwargs)
+            super().__init__(
+                name=name_override, op_name=op_name, *args, **kwargs)
 
-        if not isinstance(items,
-                          (list, tuple, pipeline_channel.PipelineChannel)):
+        if not isinstance(items, (list, tuple, dsl.PipelineParam)):
             raise TypeError(
-                f'Expected list, tuple, or PipelineChannel, got {items}.')
+                'Expected list, tuple, or PipelineParam, got {}.'.format(
+                    type(items)))
 
         if isinstance(items, tuple):
             items = list(items)
 
-        self.items_or_pipeline_channel = items
-        self.is_with_items_loop_argument = not isinstance(
-            items, pipeline_channel.PipelineChannel)
-        self._referenced_subvars: Dict[str, LoopArgumentVariable] = {}
-
         if isinstance(items, list) and isinstance(items[0], dict):
             subvar_names = set(items[0].keys())
-            # then this block creates loop_arg.variable_a and loop_arg.variable_b
+            for item in items:
+                if not set(item.keys()) == subvar_names:
+                    raise ValueError(
+                        'If you input a list of dicts then all dicts should have the same keys. '
+                        'Got: {}.'.format(items))
+
+            # then this block creates loop_args.variable_a and loop_args.variable_b
             for subvar_name in subvar_names:
-                loop_arg_var = LoopArgumentVariable(
-                    loop_argument=self,
-                    subvar_name=subvar_name,
-                )
-                self._referenced_subvars[subvar_name] = loop_arg_var
-                setattr(self, subvar_name, loop_arg_var)
+                if not self._subvar_name_is_legal(subvar_name):
+                    raise ValueError(
+                        "Tried to create subvariable named {} but that's not a legal Python variable "
+                        'name.'.format(subvar_name))
+                setattr(
+                    self, subvar_name,
+                    LoopArgumentVariable(
+                        loop_args_name=self.name,
+                        this_variable_name=subvar_name,
+                        loop_args_op_name=self.op_name,
+                        loop_args=self,
+                    ))
 
-    def __getattr__(self, name: str):
-        # this is being overridden so that we can access subvariables of the
-        # LoopArgument (i.e.: item.a) without knowing the subvariable names ahead
-        # of time.
+        self.items_or_pipeline_param = items
+        self.referenced_subvar_names = []
 
-        return self._referenced_subvars.setdefault(
-            name, LoopArgumentVariable(
-                loop_argument=self,
-                subvar_name=name,
-            ))
-
-    def _make_name(self, code: str):
-        """Makes a name for this loop argument from a unique code."""
-        return f'{self.LOOP_ITEM_PARAM_NAME_BASE}-{code}'
-
-    @classmethod
-    def from_pipeline_channel(
-        cls,
-        channel: pipeline_channel.PipelineChannel,
-    ) -> 'LoopArgument':
-        """Creates a LoopArgument object from a PipelineChannel object."""
-        return LoopArgument(
-            items=channel,
-            name_override=channel.name + '-' + cls.LOOP_ITEM_NAME_BASE,
-            task_name=channel.task_name,
-            channel_type=_get_loop_item_type(channel.channel_type) or 'String',
+    @classmethod
+    def from_pipeline_param(cls, param: dsl.PipelineParam) -> 'LoopArguments':
+        return LoopArguments(
+            items=param,
+            code=None,
+            name_override=param.name + '-' + cls.LOOP_ITEM_NAME_BASE,
+            op_name=param.op_name,
+            value=param.value,
         )
 
-    @classmethod
-    def from_raw_items(
-        cls,
-        raw_items: ItemList,
-        name_code: str,
-    ) -> 'LoopArgument':
-        """Creates a LoopArgument object from raw item list."""
-        if len(raw_items) == 0:
-            raise ValueError('Got an empty item list for loop argument.')
-
-        return LoopArgument(
-            items=raw_items,
-            name_code=name_code,
-            channel_type=type(raw_items[0]).__name__,
+    def __getattr__(self, item):
+        # this is being overridden so that we can access subvariables of the
+        # LoopArguments (i.e.: item.a) without knowing the subvariable names ahead
+        # of time
+        self.referenced_subvar_names.append(item)
+        return LoopArgumentVariable(
+            loop_args_name=self.name,
+            this_variable_name=item,
+            loop_args_op_name=self.op_name,
+            loop_args=self,
         )
 
+    def to_list_for_task_yaml(self):
+        if isinstance(self.items_or_pipeline_param, (list, tuple)):
+            return self.items_or_pipeline_param
+        else:
+            raise ValueError(
+                'You should only call this method on loop args which have list items, '
+                'not pipeline param items.')
+
+    @classmethod
+    def _make_name(cls, code: str):
+        """Make a name for this parameter.
+
+        Code is a
+        """
+        return '{}-{}'.format(cls.LOOP_ITEM_PARAM_NAME_BASE, code)
+
     @classmethod
-    def name_is_loop_argument(cls, name: str) -> bool:
-        """Returns True if the given channel name looks like a loop argument.
+    def name_is_loop_argument(cls, param_name: str) -> bool:
+        """Return True if the given parameter name looks like a loop argument.
 
         Either it came from a withItems loop item or withParams loop
         item.
         """
-        return  ('-' + cls.LOOP_ITEM_NAME_BASE) in name \
-          or (cls.LOOP_ITEM_PARAM_NAME_BASE + '-') in name
+        return cls.name_is_withitems_loop_argument(param_name) \
+          or cls.name_is_withparams_loop_argument(param_name)
 
+    @classmethod
+    def name_is_withitems_loop_argument(cls, param_name: str) -> bool:
+        """Return True if the given parameter name looks like it came from a
+        loop arguments parameter."""
+        return (cls.LOOP_ITEM_PARAM_NAME_BASE + '-') in param_name
 
-class LoopArgumentVariable(pipeline_channel.PipelineChannel):
-    """Represents a subvariable for a loop argument.
+    @classmethod
+    def name_is_withparams_loop_argument(cls, param_name: str) -> bool:
+        """Return True if the given parameter name looks like it came from a
+        withParams loop item."""
+        return ('-' + cls.LOOP_ITEM_NAME_BASE) in param_name
 
-    This is used for cases where we're looping over maps, each of which contains
-    several variables. If the user ran:
+    @classmethod
+    def remove_loop_item_base_name(cls, param_name: str) -> str:
+        """Removes the last LOOP_ITEM_NAME_BASE from the end of param name."""
+        if ('-' + cls.LOOP_ITEM_NAME_BASE) in param_name:
+            # Split from the right, so that it handles multi-level nested args.
+            return param_name.rsplit('-' + cls.LOOP_ITEM_NAME_BASE, 1)[0]
+        return param_name
 
-        with dsl.ParallelFor([{'a': 1, 'b': 2}, {'a': 3, 'b': 4}]) as item:
-            ...
 
-    Then there's one LoopArgumentVariable for 'a' and another for 'b'.
+class LoopArgumentVariable(dsl.PipelineParam):
+    """Represents a subvariable for loop arguments.
 
-    Attributes:
-        loop_argument: The original LoopArgument object this subvariable is
-          attached to.
-        subvar_name: The subvariable name.
+    This is used for cases where we're looping over maps,   each of
+    which contains several variables.
     """
     SUBVAR_NAME_DELIMITER = '-subvar-'
-    LEGAL_SUBVAR_NAME_REGEX = re.compile(r'^[a-zA-Z_][0-9a-zA-Z_]*$')
 
     def __init__(
         self,
-        loop_argument: LoopArgument,
-        subvar_name: str,
+        loop_args_name: str,
+        this_variable_name: str,
+        loop_args_op_name: Optional[str],
+        # For backward compatible, add loop_args as an optional argument.
+        # Ideally, this should replace loop_args_name and loop_args_op_name.
+        loop_args: Optional[LoopArguments] = None,
     ):
-        """Initializes a LoopArgumentVariable instance.
-
-        Args:
-            loop_argument: The LoopArgument object this subvariable is based on
-                a subvariable to.
-            subvar_name: The name of this subvariable, which is the name of the
-                dict key that spawned this subvariable.
-
-        Raises:
-            ValueError is subvar name is illegal.
         """
-        if not self._subvar_name_is_legal(subvar_name):
-            raise ValueError(
-                f'Tried to create subvariable named {subvar_name}, but that is '
-                'not a legal Python variable name.')
-
-        self.subvar_name = subvar_name
-        self.loop_argument = loop_argument
+    If the user ran:
+        with dsl.ParallelFor([{'a': 1, 'b': 2}, {'a': 3, 'b': 4}]) as item:
+            ...
+    Then there's be one LoopArgumentsVariable for 'a' and another for 'b'.
 
+    Args:
+      loop_args_name:  The name of the LoopArguments object that this is
+        a subvariable to.
+      this_variable_name: The name of this subvariable, which is the name
+        of the dict key that spawned this subvariable.
+      loop_args_op_name: The name of the op that produced the loop arguments.
+      loop_args: Optional; The LoopArguments object this subvariable is based on.
+    """
         super().__init__(
-            name=self._get_name_override(
-                loop_arg_name=loop_argument.name,
-                subvar_name=subvar_name,
-            ),
-            task_name=loop_argument.task_name,
-            channel_type=_get_subvar_type(loop_argument.channel_type) or
-            'String',
+            name=self.get_name(
+                loop_args_name=loop_args_name,
+                this_variable_name=this_variable_name),
+            op_name=loop_args_op_name,
         )
+        self.loop_args = loop_args
 
     @property
-    def items_or_pipeline_channel(
-            self) -> Union[ItemList, pipeline_channel.PipelineChannel]:
-        """Returns the loop argument items."""
-        return self.loop_argument.items_or_pipeline_chanenl
+    def items_or_pipeline_param(
+            self) -> Union[ItemList, _pipeline_param.PipelineParam]:
+        return self.loop_args.items_or_pipeline_param
 
-    @property
-    def is_with_items_loop_argument(self) -> bool:
-        """Whether the loop argument is originated from raw items."""
-        return self.loop_argument.is_with_items_loop_argument
-
-    def _subvar_name_is_legal(self, proposed_variable_name: str) -> bool:
-        """Returns True if the subvar name is legal."""
-        return re.match(self.LEGAL_SUBVAR_NAME_REGEX,
-                        proposed_variable_name) is not None
-
-    def _get_name_override(self, loop_arg_name: str, subvar_name: str) -> str:
-        """Gets the name.
+    @classmethod
+    def get_name(cls, loop_args_name: str, this_variable_name: str) -> str:
+        """Get the name.
 
         Args:
-            loop_arg_name: the name of the loop argument parameter that this
-              LoopArgumentVariable is attached to.
-            subvar_name: The name of this subvariable.
+          loop_args_name: the name of the loop args parameter that this
+            LoopArgsVariable is attached to.
+          this_variable_name: the name of this LoopArgumentsVariable subvar.
 
         Returns:
-            The name of this loop arg variable.
+          The name of this loop args variable.
         """
-        return f'{loop_arg_name}{self.SUBVAR_NAME_DELIMITER}{subvar_name}'
-
-
-class Collected(pipeline_channel.PipelineChannel):
-    """For collecting into a list the output from a task in dsl.ParallelFor
-    loops.
-
-    Args:
-        output: The output of an upstream task within a dsl.ParallelFor loop.
-
-    Example:
-      ::
+        return '{}{}{}'.format(loop_args_name, cls.SUBVAR_NAME_DELIMITER,
+                               this_variable_name)
 
-        @dsl.pipeline
-        def math_pipeline() -> int:
-            with dsl.ParallelFor([1, 2, 3]) as x:
-                t = double(num=x)
-
-        return add(nums=dsl.Collected(t.output)).output
-    """
+    @classmethod
+    def name_is_loop_arguments_variable(cls, param_name: str) -> bool:
+        """Return True if the given parameter name looks like it came from a
+        LoopArgumentsVariable."""
+        return re.match('.+%s.+' % cls.SUBVAR_NAME_DELIMITER,
+                        param_name) is not None
 
-    def __init__(
-        self,
-        output: pipeline_channel.PipelineChannel,
-    ) -> None:
-        self.output = output
-        if isinstance(output, pipeline_channel.PipelineArtifactChannel):
-            channel_type = output.channel_type
-            self.is_artifact_channel = True
-            # we know all dsl.Collected instances are lists, so set to true
-            # for type checking, which occurs before dsl.Collected is updated to
-            # it's "correct" channel during compilation
-            self.is_artifact_list = True
+    @classmethod
+    def parse_loop_args_name_and_this_var_name(cls, t: str) -> Tuple[str, str]:
+        """Get the loop arguments param name and this subvariable name from the
+        given parameter name."""
+        m = re.match(
+            '(?P<loop_args_name>.*){}(?P<this_var_name>.*)'.format(
+                cls.SUBVAR_NAME_DELIMITER), t)
+        if m is None:
+            return None
         else:
-            channel_type = 'LIST'
-            self.is_artifact_channel = False
+            return m.groupdict()['loop_args_name'], m.groupdict(
+            )['this_var_name']
 
-        super().__init__(
-            output.name,
-            channel_type=channel_type,
-            task_name=output.task_name,
-        )
+    @classmethod
+    def get_subvar_name(cls, t: str) -> str:
+        """Get the subvariable name from a given LoopArgumentsVariable
+        parameter name."""
+        out = cls.parse_loop_args_name_and_this_var_name(t)
+        if out is None:
+            raise ValueError("Couldn't parse variable name: {}".format(t))
+        return out[1]
```

### Comparing `kfp-2.0.1/kfp/components/tasks_group.py` & `kfp-2.1.1/kfp/deprecated/dsl/_ops_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,230 +1,235 @@
-# Copyright 2021 The Kubeflow Authors
+# Copyright 2018-2019 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Definition for TasksGroup."""
+from typing import Union
 
-import enum
-from typing import Optional, Union
+from kfp.deprecated.dsl import _for_loop, _pipeline_param
 
-from kfp.components import for_loop
-from kfp.components import pipeline_channel
-from kfp.components import pipeline_context
-from kfp.components import pipeline_task
+from . import _container_op
+from . import _pipeline
 
 
-class TasksGroupType(str, enum.Enum):
-    """Types of TasksGroup."""
-    PIPELINE = 'pipeline'
-    CONDITION = 'condition'
-    FOR_LOOP = 'for-loop'
-    EXIT_HANDLER = 'exit-handler'
+class OpsGroup(object):
+    """Represents a logical group of ops and group of OpsGroups.
 
-
-class TasksGroup:
-    """Represents a logical group of tasks and groups of TasksGroups.
-
-    This class is the base class for groups of tasks, such as tasks
-    sharing an exit handler, a condition branch, or a loop. This class
-    is not supposed to be used by pipeline authors. It is useful for
+    This class is the base class for groups of ops, such as ops sharing
+    an exit handler, a condition branch, or a loop. This class is not
+    supposed to be used by pipeline authors. It is useful for
     implementing a compiler.
-
-    Attributes:
-        group_type: The type of the TasksGroup.
-        tasks: A list of all PipelineTasks in this group.
-        groups: A list of TasksGroups in this group.
-        display_name: The optional user given name of the group.
-        dependencies: A list of tasks or groups this group depends on.
-        is_root: If TasksGroup is root group.
     """
 
-    def __init__(
-        self,
-        group_type: TasksGroupType,
-        name: Optional[str] = None,
-        is_root: bool = False,
-    ):
-        """Create a new instance of TasksGroup.
+    def __init__(self,
+                 group_type: str,
+                 name: str = None,
+                 parallelism: int = None):
+        """Create a new instance of OpsGroup.
 
         Args:
-          group_type: The type of the group.
-          name: The name of the group. Used as display name in UI.
+          group_type (str): one of 'pipeline', 'exit_handler', 'condition',
+            'for_loop', and 'graph'.
+          name (str): name of the opsgroup
+          parallelism (int): parallelism for the sub-DAG:s
         """
-        self.group_type = group_type
-        self.tasks = []
-        self.groups = []
-        self.display_name = name
+        #TODO: declare the group_type to be strongly typed
+        self.type = group_type
+        self.ops = list()
+        self.groups = list()
+        self.name = name
         self.dependencies = []
-        self.is_root = is_root
+        self.parallelism = parallelism
+        # recursive_ref points to the opsgroups with the same name if exists.
+        self.recursive_ref = None
 
-    def __enter__(self):
-        if not pipeline_context.Pipeline.get_default_pipeline():
-            raise ValueError('Default pipeline not defined.')
+        self.loop_args = None
 
-        self._make_name_unique()
+    @staticmethod
+    def _get_matching_opsgroup_already_in_pipeline(group_type, name):
+        """Retrieves the opsgroup when the pipeline already contains it.
 
-        pipeline_context.Pipeline.get_default_pipeline().push_tasks_group(self)
-        return self
+        the opsgroup might be already in the pipeline in case of recursive calls.
 
-    def __exit__(self, *unused_args):
-        pipeline_context.Pipeline.get_default_pipeline().pop_tasks_group()
+        Args:
+          group_type (str): one of 'pipeline', 'exit_handler', 'condition', and
+            'graph'.
+          name (str): the name before conversion.
+        """
+        if not _pipeline.Pipeline.get_default_pipeline():
+            raise ValueError('Default pipeline not defined.')
+        if name is None:
+            return None
+        name_pattern = '^' + (group_type + '-' + name + '-').replace(
+            '_', '-') + '[\d]+$'
+        for ops_group_already_in_pipeline in _pipeline.Pipeline.get_default_pipeline(
+        ).groups:
+            import re
+            if ops_group_already_in_pipeline.type == group_type \
+                    and re.match(name_pattern ,ops_group_already_in_pipeline.name):
+                return ops_group_already_in_pipeline
+        return None
 
     def _make_name_unique(self):
-        """Generates a unique TasksGroup name in the pipeline."""
-        if not pipeline_context.Pipeline.get_default_pipeline():
+        """Generate a unique opsgroup name in the pipeline."""
+        if not _pipeline.Pipeline.get_default_pipeline():
             raise ValueError('Default pipeline not defined.')
 
-        group_id = pipeline_context.Pipeline.get_default_pipeline(
-        ).get_next_group_id()
-        self.name = f'{self.group_type.value}-{group_id}'
+        self.name = (
+            self.type + '-' + ('' if self.name is None else self.name + '-') +
+            str(_pipeline.Pipeline.get_default_pipeline().get_next_group_id()))
         self.name = self.name.replace('_', '-')
 
-    def remove_task_recursive(self, task: pipeline_task.PipelineTask):
-        """Removes a task from the group recursively."""
-        if self.tasks and task in self.tasks:
-            self.tasks.remove(task)
-        for group in self.groups or []:
-            group.remove_task_recursive(task)
+    def __enter__(self):
+        if not _pipeline.Pipeline.get_default_pipeline():
+            raise ValueError('Default pipeline not defined.')
+
+        self.recursive_ref = self._get_matching_opsgroup_already_in_pipeline(
+            self.type, self.name)
+        if not self.recursive_ref:
+            self._make_name_unique()
+
+        _pipeline.Pipeline.get_default_pipeline().push_ops_group(self)
+        return self
+
+    def __exit__(self, *args):
+        _pipeline.Pipeline.get_default_pipeline().pop_ops_group()
+
+    def after(self, *ops):
+        """Specify explicit dependency on other ops."""
+        for op in ops:
+            self.dependencies.append(op)
+        return self
+
+    def remove_op_recursive(self, op):
+        if self.ops and op in self.ops:
+            self.ops.remove(op)
+        for sub_group in self.groups or []:
+            sub_group.remove_op_recursive(op)
 
 
-class ExitHandler(TasksGroup):
-    """A class for setting an exit handler task that is invoked upon exiting a
-    group of other tasks.
+class SubGraph(OpsGroup):
+    TYPE_NAME = 'subgraph'
+
+    def __init__(self, parallelism: int):
+        if parallelism < 1:
+            raise ValueError(
+                'SubGraph parallism set to < 1, allowed values are > 0')
+        super(SubGraph, self).__init__(self.TYPE_NAME, parallelism=parallelism)
+
+
+class ExitHandler(OpsGroup):
+    """Represents an exit handler that is invoked upon exiting a group of ops.
 
     Args:
-        exit_task: The task that is invoked after exiting a group of other tasks.
-        name: The name of the exit handler group.
+      exit_op: An operator invoked at exiting a group of ops.
+
+    Raises:
+      ValueError: Raised if the exit_op is invalid.
 
     Example:
       ::
 
-        exit_task = ExitComponent(...)
-        with ExitHandler(exit_task):
-            task1 = my_component1(...)
-            task2 = my_component2(...)
+        exit_op = ContainerOp(...)
+        with ExitHandler(exit_op):
+          op1 = ContainerOp(...)
+          op2 = ContainerOp(...)
     """
 
-    def __init__(
-        self,
-        exit_task: pipeline_task.PipelineTask,
-        name: Optional[str] = None,
-    ):
-        """Initializes a Condition task group."""
-        super().__init__(
-            group_type=TasksGroupType.EXIT_HANDLER,
-            name=name,
-            is_root=False,
-        )
-
-        if exit_task.dependent_tasks:
-            raise ValueError('exit_task cannot depend on any other tasks.')
-
-        # Removing exit_task form any group
-        pipeline_context.Pipeline.get_default_pipeline(
-        ).remove_task_from_groups(exit_task)
-
-        # Set is_exit_handler since the compiler might be using this attribute.
-        exit_task.is_exit_handler = True
-
-        self.exit_task = exit_task
-
-
-class Condition(TasksGroup):
-    """A class for creating conditional control flow within a pipeline
-    definition.
+    def __init__(self, exit_op: _container_op.ContainerOp):
+        super(ExitHandler, self).__init__('exit_handler')
+        if exit_op.dependent_names:
+            raise ValueError('exit_op cannot depend on any other ops.')
 
-    Args:
-        condition: A comparative expression that evaluates to True or False. At least one of the operands must be an output from an upstream task or a pipeline parameter.
-        name: The name of the condition group.
+        # Removing exit_op form any group
+        _pipeline.Pipeline.get_default_pipeline().remove_op_from_groups(exit_op)
+
+        # Setting is_exit_handler since the compiler might be using this attribute.
+        # TODO: Check that it's needed
+        exit_op.is_exit_handler = True
+
+        self.exit_op = exit_op
 
-    Example:
-      ::
 
-        task1 = my_component1(...)
-        with Condition(task1.output=='pizza', 'pizza-condition'):
-            task2 = my_component2(...)
+class Condition(OpsGroup):
+    """Represents an condition group with a condition.
+
+    Args:
+      condition (ConditionOperator): the condition.
+      name (str): name of the condition
+    Example: ::
+        with Condition(param1=='pizza', '[param1 is pizza]'): op1 =
+          ContainerOp(...) op2 = ContainerOp(...)
     """
 
-    def __init__(
-        self,
-        condition: pipeline_channel.ConditionOperator,
-        name: Optional[str] = None,
-    ):
-        """Initializes a conditional task group."""
-        super().__init__(
-            group_type=TasksGroupType.CONDITION,
-            name=name,
-            is_root=False,
-        )
+    def __init__(self, condition, name=None):
+        super(Condition, self).__init__('condition', name)
         self.condition = condition
 
 
-class ParallelFor(TasksGroup):
-    """A class for creating parallelized for loop control flow over a static
-    set of items within a pipeline definition.
+class Graph(OpsGroup):
+    """Graph DAG with inputs, recursive_inputs, and outputs.
+
+    This is not used directly by the users but auto generated when the
+    graph_component decoration exists
 
     Args:
-        items: The items to loop over. It can be either a constant Python list or a list output from an upstream task.
-        name: The name of the for loop group.
-        parallelism: The maximum number of concurrent iterations that can be scheduled for execution. A value of 0 represents unconstrained parallelism (default is unconstrained).
+      name: Name of the graph.
+    """
+
+    def __init__(self, name):
+        super(Graph, self).__init__(group_type='graph', name=name)
+        self.inputs = []
+        self.outputs = {}
+        self.dependencies = []
+
+
+class ParallelFor(OpsGroup):
+    """Represents a parallel for loop over a static set of items.
 
     Example:
-      ::
+      In this case :code:`op1` would be executed twice, once with case
+      :code:`args=['echo 1']` and once with case :code:`args=['echo 2']`::
 
-        with dsl.ParallelFor(
-          items=[{'a': 1, 'b': 10}, {'a': 2, 'b': 20}],
-          parallelism=1
-        ) as item:
-            task1 = my_component(..., number=item.a)
-            task2 = my_component(..., number=item.b)
-
-    In the example, the group of tasks containing ``task1`` and ``task2`` would
-    be executed twice, once with case ``args=[{'a': 1, 'b': 10}]`` and once with
-    case ``args=[{'a': 2, 'b': 20}]``. The ``parallelism=1`` setting causes only
-    1 execution to be scheduled at a time.
+        with dsl.ParallelFor([{'a': 1, 'b': 10}, {'a': 2, 'b': 20}]) as item:
+          op1 = ContainerOp(..., args=['echo {}'.format(item.a)])
+          op2 = ContainerOp(..., args=['echo {}'.format(item.b])
     """
+    TYPE_NAME = 'for_loop'
 
-    def __init__(
-        self,
-        items: Union[for_loop.ItemList, pipeline_channel.PipelineChannel],
-        name: Optional[str] = None,
-        parallelism: Optional[int] = None,
-    ):
-        """Initializes a for loop task group."""
-        parallelism = parallelism or 0
-        if parallelism < 0:
+    def __init__(self,
+                 loop_args: Union[_for_loop.ItemList,
+                                  _pipeline_param.PipelineParam],
+                 parallelism: int = None):
+        if parallelism and parallelism < 1:
             raise ValueError(
-                f'ParallelFor parallelism must be >= 0. Got: {parallelism}.')
+                'ParallelFor parallism set to < 1, allowed values are > 0')
+
+        self.items_is_pipeline_param = isinstance(loop_args,
+                                                  _pipeline_param.PipelineParam)
+
+        super().__init__(self.TYPE_NAME, parallelism=parallelism)
 
-        super().__init__(
-            group_type=TasksGroupType.FOR_LOOP,
-            name=name,
-            is_root=False,
-        )
-
-        if isinstance(items, pipeline_channel.PipelineChannel):
-            self.loop_argument = for_loop.LoopArgument.from_pipeline_channel(
-                items)
-            self.items_is_pipeline_channel = True
-        else:
-            self.loop_argument = for_loop.LoopArgument.from_raw_items(
-                raw_items=items,
-                name_code=pipeline_context.Pipeline.get_default_pipeline()
-                .get_next_group_id(),
+        if self.items_is_pipeline_param:
+            loop_args = _for_loop.LoopArguments.from_pipeline_param(loop_args)
+        elif not self.items_is_pipeline_param and not isinstance(
+                loop_args, _for_loop.LoopArguments):
+            # we were passed a raw list, wrap it in loop args
+            loop_args = _for_loop.LoopArguments(
+                loop_args,
+                code=str(_pipeline.Pipeline.get_default_pipeline()
+                         .get_next_group_id()),
             )
-            self.items_is_pipeline_channel = False
 
-        self.parallelism_limit = parallelism
+        self.loop_args = loop_args
 
-    def __enter__(self) -> for_loop.LoopArgument:
-        super().__enter__()
-        return self.loop_argument
+    def __enter__(self) -> _for_loop.LoopArguments:
+        _ = super().__enter__()
+        return self.loop_args
```

### Comparing `kfp-2.0.1/kfp/components/types/__init__.py` & `kfp-2.1.1/kfp/registry/context/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 The Kubeflow Authors
+# Copyright 2022 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kfp-2.0.1/kfp/components/v1_modelbase.py` & `kfp-2.1.1/kfp/deprecated/components/modelbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-# Copyright 2018-2022 The Kubeflow Authors
+# Copyright 2018 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections import abc
-from collections import OrderedDict
+__all__ = [
+    'ModelBase',
+]
+
 import inspect
-from typing import (Any, cast, Dict, get_type_hints, List, Mapping,
-                    MutableMapping, MutableSequence, Sequence, Type, TypeVar,
-                    Union)
+from collections import abc, OrderedDict
+from typing import Any, Dict, List, Mapping, MutableMapping, MutableSequence, Sequence, Type, TypeVar, Union, cast, get_type_hints
 
 T = TypeVar('T')
 
 
 def verify_object_against_type(x: Any, typ: Type[T]) -> T:
     """Verifies that the object is compatible to the specified type (types from
     the typing package can be used)."""
     #TODO: Merge with parse_object_from_struct_based_on_type which has almost the same code
     if typ is type(None):
         if x is None:
             return x
         else:
-            raise TypeError(f'Error: Object "{x}" is not None.')
+            raise TypeError('Error: Object "{}" is not None.'.format(x))
 
     if typ is Any or type(typ) is TypeVar:
         return x
 
     try:  #isinstance can fail for generics
         if isinstance(x, typ):
             return cast(typ, x)
-    except Exception:
+    except:
         pass
 
     if hasattr(typ, '__origin__'):  #Handling generic types
         if typ.__origin__ is Union:  #Optional == Union
             exception_map = {}
             possible_types = typ.__args__
             if type(
@@ -54,77 +55,84 @@
                     verify_object_against_type(x, possible_type)
                     return x
                 except Exception as ex:
                     exception_map[possible_type] = ex
             #exception_lines = ['Exception for type {}: {}.'.format(t, e) for t, e in exception_map.items()]
             exception_lines = [str(e) for t, e in exception_map.items()]
             exception_lines.append(
-                f'Error: Object "{x}" is incompatible with type "{typ}".')
+                'Error: Object "{}" is incompatible with type "{}".'.format(
+                    x, typ))
             raise TypeError('\n'.join(exception_lines))
 
         #not Union => not None
         if x is None:
             raise TypeError(
-                f'Error: None object is incompatible with type {typ}')
+                'Error: None object is incompatible with type {}'.format(typ))
 
-        generic_type = typ.__origin__
+        #assert isinstance(x, typ.__origin__)
+        generic_type = typ.__origin__ or getattr(
+            typ, '__extra__', None
+        )  #In python <3.7 typing.List.__origin__ == None; Python 3.7 has working __origin__, but no __extra__  TODO: Remove the __extra__ once we move to Python 3.7
         if generic_type in [
                 list, List, abc.Sequence, abc.MutableSequence, Sequence,
                 MutableSequence
         ] and type(x) is not str:  #! str is also Sequence
             if not isinstance(x, generic_type):
                 raise TypeError(
-                    f'Error: Object "{x}" is incompatible with type "{typ}"')
-
+                    'Error: Object "{}" is incompatible with type "{}"'.format(
+                        x, typ))
+            # In Python <3.7 Mapping.__args__ is None.
             # In Python 3.9 typ.__args__ does not exist when the generic type does not have subscripts
             type_args = typ.__args__ if getattr(
                 typ, '__args__', None) is not None else (Any, Any)
             inner_type = type_args[0]
             for item in x:
                 verify_object_against_type(item, inner_type)
             return x
 
         elif generic_type in [
                 dict, Dict, abc.Mapping, abc.MutableMapping, Mapping,
                 MutableMapping, OrderedDict
         ]:
             if not isinstance(x, generic_type):
                 raise TypeError(
-                    f'Error: Object "{x}" is incompatible with type "{typ}"')
-
+                    'Error: Object "{}" is incompatible with type "{}"'.format(
+                        x, typ))
+            # In Python <3.7 Mapping.__args__ is None.
             # In Python 3.9 typ.__args__ does not exist when the generic type does not have subscripts
             type_args = typ.__args__ if getattr(
                 typ, '__args__', None) is not None else (Any, Any)
             inner_key_type = type_args[0]
             inner_value_type = type_args[1]
             for k, v in x.items():
                 verify_object_against_type(k, inner_key_type)
                 verify_object_against_type(v, inner_value_type)
             return x
 
         else:
             raise TypeError(
-                f'Error: Unsupported generic type "{typ}". type.__origin__ or type.__extra__ == "{generic_type}"'
-            )
+                'Error: Unsupported generic type "{}". type.__origin__ or type.__extra__ == "{}"'
+                .format(typ, generic_type))
 
-    raise TypeError(f'Error: Object "{x}" is incompatible with type "{typ}"')
+    raise TypeError('Error: Object "{}" is incompatible with type "{}"'.format(
+        x, typ))
 
 
 def parse_object_from_struct_based_on_type(struct: Any, typ: Type[T]) -> T:
     """Constructs an object from structure (usually dict) based on type.
 
     Supports list and dict types from the typing package plus Optional[]
     and Union[] types. If some type is a class that has .from_dict class
     method, that method is used for object construction.
     """
     if typ is type(None):
         if struct is None:
             return None
         else:
-            raise TypeError(f'Error: Structure "{struct}" is not None.')
+            raise TypeError('Error: Structure "{}" is not None.'.format(struct))
 
     if typ is Any or type(typ) is TypeVar:
         return struct
 
     try:  #isinstance can fail for generics
         #if (isinstance(struct, typ)
         #    and not (typ is Sequence and type(struct) is str) #! str is also Sequence
@@ -135,104 +143,111 @@
     except:
         pass
     if hasattr(typ, 'from_dict'):
         try:  #More informative errors
             return typ.from_dict(struct)
         except Exception as ex:
             raise TypeError(
-                f'Error: {typ.__name__}.from_dict(struct={struct}) failed with exception:\n{str(ex)}'
-            )
+                'Error: {}.from_dict(struct={}) failed with exception:\n{}'
+                .format(typ.__name__, struct, str(ex)))
     if hasattr(typ, '__origin__'):  #Handling generic types
         if typ.__origin__ is Union:  #Optional == Union
             results = {}
             exception_map = {}
             # In Python 3.9 typ.__args__ does not exist when the generic type does not have subscripts
             # Union without subscripts seems useless, but semantically it should be the same as Any.
             possible_types = list(getattr(typ, '__args__', [Any]))
             #if type(None) in possible_types and struct is None: #Shortcut for Optional[] tests. Can be removed, but the exceptions will be more noisy.
             #    return None
-
+            #Hack for Python <3.7 which for some reason "simplifies" Union[bool, int, ...] to just Union[int, ...]
+            if int in possible_types:
+                possible_types = possible_types + [bool]
             for possible_type in possible_types:
                 try:
                     obj = parse_object_from_struct_based_on_type(
                         struct, possible_type)
                     results[possible_type] = obj
                 except Exception as ex:
                     if isinstance(ex, TypeError):
                         exception_map[possible_type] = ex
                     else:
                         exception_map[
-                            possible_type] = f'Unexpected exception when trying to convert structure "{struct}" to type "{typ}": {type(ex)}: {ex}'
+                            possible_type] = 'Unexpected exception when trying to convert structure "{}" to type "{}": {}: {}'.format(
+                                struct, typ, type(ex), ex)
 
             #Single successful parsing.
             if len(results) == 1:
                 return list(results.values())[0]
 
             if len(results) > 1:
                 raise TypeError(
-                    f'Error: Structure "{struct}" is ambiguous. It can be parsed to multiple types: {list(results.keys())}.'
-                )
+                    'Error: Structure "{}" is ambiguous. It can be parsed to multiple types: {}.'
+                    .format(struct, list(results.keys())))
 
             exception_lines = [str(e) for t, e in exception_map.items()]
             exception_lines.append(
-                f'Error: Structure "{struct}" is incompatible with type "{typ}" - none of the types in Union are compatible.'
-            )
+                'Error: Structure "{}" is incompatible with type "{}" - none of the types in Union are compatible.'
+                .format(struct, typ))
             raise TypeError('\n'.join(exception_lines))
         #not Union => not None
         if struct is None:
             raise TypeError(
-                f'Error: None structure is incompatible with type {typ}')
+                'Error: None structure is incompatible with type {}'.format(
+                    typ))
 
-        generic_type = typ.__origin__
+        #assert isinstance(x, typ.__origin__)
+        generic_type = typ.__origin__ or getattr(
+            typ, '__extra__', None
+        )  #In python <3.7 typing.List.__origin__ == None; Python 3.7 has working __origin__, but no __extra__  TODO: Remove the __extra__ once we move to Python 3.7
         if generic_type in [
                 list, List, abc.Sequence, abc.MutableSequence, Sequence,
                 MutableSequence
         ] and type(struct) is not str:  #! str is also Sequence
             if not isinstance(struct, generic_type):
                 raise TypeError(
-                    f'Error: Structure "{struct}" is incompatible with type "{typ}" - it does not have list type.'
-                )
-
+                    'Error: Structure "{}" is incompatible with type "{}" - it does not have list type.'
+                    .format(struct, typ))
+            # In Python <3.7 Mapping.__args__ is None.
             # In Python 3.9 typ.__args__ does not exist when the generic type does not have subscripts
             type_args = typ.__args__ if getattr(
                 typ, '__args__', None) is not None else (Any, Any)
             inner_type = type_args[0]
             return [
                 parse_object_from_struct_based_on_type(item, inner_type)
                 for item in struct
             ]
 
         elif generic_type in [
                 dict, Dict, abc.Mapping, abc.MutableMapping, Mapping,
                 MutableMapping, OrderedDict
-        ]:
+        ]:  #in Python <3.7 there is a difference between abc.Mapping and typing.Mapping
             if not isinstance(struct, generic_type):
                 raise TypeError(
-                    f'Error: Structure "{struct}" is incompatible with type "{typ}" - it does not have dict type.'
-                )
-
+                    'Error: Structure "{}" is incompatible with type "{}" - it does not have dict type.'
+                    .format(struct, typ))
+            # In Python <3.7 Mapping.__args__ is None.
             # In Python 3.9 typ.__args__ does not exist when the generic type does not have subscripts
             type_args = typ.__args__ if getattr(
                 typ, '__args__', None) is not None else (Any, Any)
             inner_key_type = type_args[0]
             inner_value_type = type_args[1]
             return {
                 parse_object_from_struct_based_on_type(k, inner_key_type):
                 parse_object_from_struct_based_on_type(v, inner_value_type)
                 for k, v in struct.items()
             }
 
         else:
             raise TypeError(
-                f'Error: Unsupported generic type "{typ}". type.__origin__ or type.__extra__ == "{generic_type}"'
-            )
+                'Error: Unsupported generic type "{}". type.__origin__ or type.__extra__ == "{}"'
+                .format(typ, generic_type))
 
     raise TypeError(
-        f'Error: Structure "{struct}" is incompatible with type "{typ}". Structure is not the instance of the type, the type does not have .from_dict method and is not generic.'
-    )
+        'Error: Structure "{}" is incompatible with type "{}". Structure is not the instance of the type, the type does not have .from_dict method and is not generic.'
+        .format(struct, typ))
 
 
 def convert_object_to_struct(obj, serialized_names: Mapping[str, str] = {}):
     """Converts an object to structure (usually a dict).
 
     Serializes all properties that do not start with underscores. If the
     type of some property is a class that has .to_dict class method,
@@ -241,15 +256,15 @@
     signature = inspect.signature(obj.__init__)  #Needed for default values
     result = {}
     for python_name in signature.parameters:  #TODO: Make it possible to specify the field ordering regardless of the presence of default values
         value = getattr(obj, python_name)
         if python_name.startswith('_'):
             continue
         attr_name = serialized_names.get(python_name, python_name)
-        if hasattr(value, 'to_dict'):
+        if hasattr(value, "to_dict"):
             result[attr_name] = value.to_dict()
         elif isinstance(value, list):
             result[attr_name] = [
                 (x.to_dict() if hasattr(x, 'to_dict') else x) for x in value
             ]
         elif isinstance(value, dict):
             result[attr_name] = {
@@ -285,16 +300,16 @@
     forbidden_struct_keys = set(
         serialized_names_to_pythonic.values()).difference(
             serialized_names_to_pythonic.keys())
     args = {}
     for original_name, value in struct.items():
         if original_name in forbidden_struct_keys:
             raise ValueError(
-                f'Use "{serialized_names[original_name]}" key instead of pythonic key "{original_name}" in the structure: {struct}.'
-            )
+                'Use "{}" key instead of pythonic key "{}" in the structure: {}.'
+                .format(serialized_names[original_name], original_name, struct))
         python_name = serialized_names_to_pythonic.get(original_name,
                                                        original_name)
         param_type = parameter_types.get(python_name, None)
         if param_type is not None:
             args[python_name] = parse_object_from_struct_based_on_type(
                 value, param_type)
         else:
@@ -342,24 +357,24 @@
         for k, v in field_values.items():
             parameter_type = parameter_types.get(k, None)
             if parameter_type is not None:
                 try:
                     verify_object_against_type(v, parameter_type)
                 except Exception as e:
                     raise TypeError(
-                        f'Argument for {k} is not compatible with type "{parameter_type}". Exception: {e}'
-                    )
+                        'Argument for {} is not compatible with type "{}". Exception: {}'
+                        .format(k, parameter_type, e))
         self.__dict__.update(field_values)
 
     @classmethod
     def from_dict(cls: Type[T], struct: Mapping) -> T:
         return parse_object_from_struct_based_on_class_init(
             cls, struct, serialized_names=cls._serialized_names)
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> Mapping:
         return convert_object_to_struct(
             self, serialized_names=self._serialized_names)
 
     def _get_field_names(self):
         return list(inspect.signature(self.__init__).parameters)
 
     def __repr__(self):
```

### Comparing `kfp-2.0.1/kfp/components/v1_structures.py` & `kfp-2.1.1/kfp/deprecated/components/_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,68 @@
-# Copyright 2018-2022 The Kubeflow Authors
+# Copyright 2018 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+__all__ = [
+    'InputSpec',
+    'OutputSpec',
+    'InputValuePlaceholder',
+    'InputPathPlaceholder',
+    'OutputPathPlaceholder',
+    'InputUriPlaceholder',
+    'OutputUriPlaceholder',
+    'InputMetadataPlaceholder',
+    'InputOutputPortNamePlaceholder',
+    'OutputMetadataPlaceholder',
+    'ExecutorInputPlaceholder',
+    'ConcatPlaceholder',
+    'IsPresentPlaceholder',
+    'IfPlaceholderStructure',
+    'IfPlaceholder',
+    'ContainerSpec',
+    'ContainerImplementation',
+    'ComponentSpec',
+    'ComponentReference',
+    'GraphInputReference',
+    'GraphInputArgument',
+    'TaskOutputReference',
+    'TaskOutputArgument',
+    'EqualsPredicate',
+    'NotEqualsPredicate',
+    'GreaterThanPredicate',
+    'GreaterThanOrEqualPredicate',
+    'LessThenPredicate',
+    'LessThenOrEqualPredicate',
+    'NotPredicate',
+    'AndPredicate',
+    'OrPredicate',
+    'RetryStrategySpec',
+    'CachingStrategySpec',
+    'ExecutionOptionsSpec',
+    'TaskSpec',
+    'GraphSpec',
+    'GraphImplementation',
+    'PipelineRunSpec',
+]
+
 from collections import OrderedDict
-from typing import Any, Dict, List, Mapping, Optional, Union
 
-import yaml
+from typing import Any, Dict, List, Mapping, Optional, Union
 
-from .v1_modelbase import ModelBase
+from .modelbase import ModelBase
 
 PrimitiveTypes = Union[str, int, float, bool]
 PrimitiveTypesIncludingNone = Optional[PrimitiveTypes]
 
 TypeSpecType = Union[str, Dict, List]
 
 
@@ -198,16 +239,16 @@
     _serialized_names = {
         'executor_input': 'executorInput',
     }
 
     def __init__(self, executor_input: type(None) = None):
         if executor_input:
             raise RuntimeError(
-                f'Executor input placeholder cannot be associated with input key. Got {executor_input}'
-            )
+                'Executor input placeholder cannot be associated with input key'
+                '. Got %s' % executor_input)
         super().__init__(locals())
 
     def to_dict(self) -> Mapping[str, Any]:
         # Override parent implementation. Otherwise it always returns {}.
         return {'executorInput': None}
 
 
@@ -356,23 +397,25 @@
 
     def _post_init(self):
         #Checking input names for uniqueness
         self._inputs_dict = {}
         if self.inputs:
             for input in self.inputs:
                 if input.name in self._inputs_dict:
-                    raise ValueError(f'Non-unique input name "{input.name}"')
+                    raise ValueError('Non-unique input name "{}"'.format(
+                        input.name))
                 self._inputs_dict[input.name] = input
 
         #Checking output names for uniqueness
         self._outputs_dict = {}
         if self.outputs:
             for output in self.outputs:
                 if output.name in self._outputs_dict:
-                    raise ValueError(f'Non-unique output name "{output.name}"')
+                    raise ValueError('Non-unique output name "{}"'.format(
+                        output.name))
                 self._outputs_dict[output.name] = output
 
         if isinstance(self.implementation, ContainerImplementation):
             container = self.implementation.container
 
             if container.file_outputs:
                 for output_name, path in container.file_outputs.items():
@@ -394,29 +437,31 @@
                 elif isinstance(
                         arg,
                     (InputUriPlaceholder, InputValuePlaceholder,
                      InputPathPlaceholder, IsPresentPlaceholder,
                      InputMetadataPlaceholder, InputOutputPortNamePlaceholder)):
                     if arg.input_name not in self._inputs_dict:
                         raise TypeError(
-                            f'Argument "{arg}" references non-existing input.')
+                            'Argument "{}" references non-existing input.'
+                            .format(arg))
                 elif isinstance(arg,
                                 (OutputUriPlaceholder, OutputPathPlaceholder)):
                     if arg.output_name not in self._outputs_dict:
                         raise TypeError(
-                            f'Argument "{arg}" references non-existing output.')
+                            'Argument "{}" references non-existing output.'
+                            .format(arg))
                 elif isinstance(arg, ConcatPlaceholder):
                     for arg2 in arg.items:
                         verify_arg(arg2)
                 elif isinstance(arg, IfPlaceholder):
                     verify_arg(arg.if_structure.condition)
                     verify_arg(arg.if_structure.then_value)
                     verify_arg(arg.if_structure.else_value)
                 else:
-                    raise TypeError(f'Unexpected argument "{arg}"')
+                    raise TypeError('Unexpected argument "{}"'.format(arg))
 
             verify_arg(container.command)
             verify_arg(container.args)
 
         if isinstance(self.implementation, GraphImplementation):
             graph = self.implementation.graph
 
@@ -431,25 +476,25 @@
                 for task in graph.tasks.values():
                     if task.arguments is not None:
                         for argument in task.arguments.values():
                             if isinstance(
                                     argument, GraphInputArgument
                             ) and argument.graph_input.input_name not in self._inputs_dict:
                                 raise TypeError(
-                                    f'Argument "{argument}" references non-existing input.'
-                                )
+                                    'Argument "{}" references non-existing input.'
+                                    .format(argument))
 
     def save(self, file_path: str):
         """Saves the component definition to file.
 
         It can be shared online and later loaded using the
         load_component function.
         """
-
-        component_yaml = yaml.dump(self.to_dict(), sort_keys=True)
+        from ._yaml_utils import dump_yaml
+        component_yaml = dump_yaml(self.to_dict())
         with open(file_path, 'w') as f:
             f.write(component_yaml)
 
 
 class ComponentReference(ModelBase):
     """Component reference.
 
@@ -781,16 +826,16 @@
             task_dependencies[task_id] = dependencies
             if task.arguments is not None:
                 for argument in task.arguments.values():
                     if isinstance(argument, TaskOutputArgument):
                         dependencies.add(argument.task_output.task_id)
                         if argument.task_output.task_id not in self.tasks:
                             raise TypeError(
-                                f'Argument "{argument}" references non-existing task.'
-                            )
+                                'Argument "{}" references non-existing task.'
+                                .format(argument))
 
         #Topologically sorting tasks to detect cycles
         task_dependents = {k: set() for k in task_dependencies.keys()}
         for task_id, dependencies in task_dependencies.items():
             for dependency in dependencies:
                 task_dependents[dependency].add(task_id)
         task_number_of_remaining_dependencies = {
@@ -816,17 +861,16 @@
                 for k, v in task_number_of_remaining_dependencies.items()
                 if v > 0
             }
             task_wth_minimal_number_of_unsatisfied_dependencies = min(
                 tasks_with_unsatisfied_dependencies.keys(),
                 key=lambda task_id: tasks_with_unsatisfied_dependencies[task_id]
             )
-            raise ValueError(
-                f'Task "{task_wth_minimal_number_of_unsatisfied_dependencies}" has cyclical dependency.'
-            )
+            raise ValueError('Task "{}" has cyclical dependency.'.format(
+                task_wth_minimal_number_of_unsatisfied_dependencies))
 
         self._toposorted_tasks = sorted_tasks
 
 
 class GraphImplementation(ModelBase):
     """Represents the graph component implementation."""
```

### Comparing `kfp-2.0.1/kfp/deprecated/__init__.py` & `kfp-2.1.1/kfp/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/__main__.py` & `kfp-2.1.1/kfp/deprecated/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/_auth.py` & `kfp-2.1.1/kfp/deprecated/_auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/_client.py` & `kfp-2.1.1/kfp/deprecated/_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/_config.py` & `kfp-2.1.1/kfp/deprecated/_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/_local_client.py` & `kfp-2.1.1/kfp/deprecated/_local_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/_runners.py` & `kfp-2.1.1/kfp/deprecated/_runners.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/auth/__init__.py` & `kfp-2.1.1/kfp/deprecated/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/auth/_satvolumecredentials.py` & `kfp-2.1.1/kfp/deprecated/auth/_satvolumecredentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/auth/_tokencredentialsbase.py` & `kfp-2.1.1/kfp/deprecated/auth/_tokencredentialsbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/aws.py` & `kfp-2.1.1/kfp/deprecated/aws.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/azure.py` & `kfp-2.1.1/kfp/deprecated/azure.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/__init__.py` & `kfp-2.1.1/kfp/deprecated/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/cli.py` & `kfp-2.1.1/kfp/deprecated/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/components.py` & `kfp-2.1.1/kfp/deprecated/cli/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/components_test.py` & `kfp-2.1.1/kfp/deprecated/cli/components_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/__init__.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/dev_env.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/gcp.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/gcp_test.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/utility.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me/utility_test.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/diagnose_me_cli.py` & `kfp-2.1.1/kfp/deprecated/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/experiment.py` & `kfp-2.1.1/kfp/deprecated/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/output.py` & `kfp-2.1.1/kfp/deprecated/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/pipeline.py` & `kfp-2.1.1/kfp/deprecated/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/recurring_run.py` & `kfp-2.1.1/kfp/deprecated/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/cli/run.py` & `kfp-2.1.1/kfp/deprecated/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/__init__.py` & `kfp-2.1.1/kfp/deprecated/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/_data_passing_rewriter.py` & `kfp-2.1.1/kfp/deprecated/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/_data_passing_using_volume.py` & `kfp-2.1.1/kfp/deprecated/compiler/_data_passing_using_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/_default_transformers.py` & `kfp-2.1.1/kfp/deprecated/compiler/_default_transformers.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/_k8s_helper.py` & `kfp-2.1.1/kfp/deprecated/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/_op_to_template.py` & `kfp-2.1.1/kfp/deprecated/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/compiler.py` & `kfp-2.1.1/kfp/deprecated/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/main.py` & `kfp-2.1.1/kfp/deprecated/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/v2_compat.py` & `kfp-2.1.1/kfp/deprecated/compiler/v2_compat.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py` & `kfp-2.1.1/kfp/deprecated/compiler/v2_compatible_compiler_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/__init__.py` & `kfp-2.1.1/kfp/deprecated/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_airflow_op.py` & `kfp-2.1.1/kfp/deprecated/components/_airflow_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_component_store.py` & `kfp-2.1.1/kfp/deprecated/components/_component_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_components.py` & `kfp-2.1.1/kfp/deprecated/components/_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_data_passing.py` & `kfp-2.1.1/kfp/deprecated/components/_data_passing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_dynamic.py` & `kfp-2.1.1/kfp/deprecated/components/_dynamic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_key_value_store.py` & `kfp-2.1.1/kfp/deprecated/components/_key_value_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_naming.py` & `kfp-2.1.1/kfp/deprecated/components/_naming.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_python_op.py` & `kfp-2.1.1/kfp/deprecated/components/_python_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_python_to_graph_component.py` & `kfp-2.1.1/kfp/deprecated/components/_python_to_graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/_yaml_utils.py` & `kfp-2.1.1/kfp/deprecated/components/_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/type_annotation_utils.py` & `kfp-2.1.1/kfp/deprecated/components/type_annotation_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/components/type_annotation_utils_test.py` & `kfp-2.1.1/kfp/deprecated/components/type_annotation_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/__init__.py` & `kfp-2.1.1/kfp/deprecated/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_build_image_api.py` & `kfp-2.1.1/kfp/deprecated/containers/_build_image_api.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_cache.py` & `kfp-2.1.1/kfp/deprecated/containers/_cache.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_component_builder.py` & `kfp-2.1.1/kfp/deprecated/containers/_component_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_container_builder.py` & `kfp-2.1.1/kfp/deprecated/containers/_container_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_gcs_helper.py` & `kfp-2.1.1/kfp/deprecated/containers/_gcs_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/_k8s_job_helper.py` & `kfp-2.1.1/kfp/deprecated/containers/_k8s_job_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/entrypoint.py` & `kfp-2.1.1/kfp/deprecated/containers/entrypoint.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/containers/entrypoint_utils.py` & `kfp-2.1.1/kfp/deprecated/containers/entrypoint_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/__init__.py` & `kfp-2.1.1/kfp/deprecated/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_component_bridge.py` & `kfp-2.1.1/kfp/deprecated/dsl/_component_bridge.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_container_op.py` & `kfp-2.1.1/kfp/deprecated/dsl/_container_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_container_op_test.py` & `kfp-2.1.1/kfp/deprecated/dsl/_container_op_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_for_loop.py` & `kfp-2.1.1/kfp/deprecated/dsl/_pipeline_param.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,257 +1,253 @@
-# Copyright 2021 The Kubeflow Authors
+# Copyright 2018 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
-from typing import Any, Dict, List, Optional, Tuple, Union
+from collections import namedtuple
+from typing import Dict, List, Optional, Union
 
-from kfp.deprecated import dsl
-from kfp.deprecated.dsl import _pipeline_param
+# TODO: Move this to a separate class
+# For now, this identifies a condition with only "==" operator supported.
+ConditionOperator = namedtuple('ConditionOperator',
+                               'operator operand1 operand2')
+PipelineParamTuple = namedtuple('PipelineParamTuple', 'name op pattern')
 
-ItemList = List[Union[int, float, str, Dict[str, Any]]]
 
+def sanitize_k8s_name(name, allow_capital_underscore=False):
+    """Cleans and converts the names in the workflow.
 
-class LoopArguments(dsl.PipelineParam):
-    """Class representing the arguments that are looped over in a ParallelFor
-    loop in the KFP DSL.
+    Args:
+      name: original name,
+      allow_capital_underscore: whether to allow capital letter and underscore in
+        this name.
 
-    This doesn't need to be instantiated by the end user, rather it will
-    be automatically created by a ParallelFor ops group.
+    Returns:
+      A sanitized name.
     """
-    LOOP_ITEM_NAME_BASE = 'loop-item'
-    LOOP_ITEM_PARAM_NAME_BASE = 'loop-item-param'
-    # number of characters in the code which is passed to the constructor
-    NUM_CODE_CHARS = 8
-    LEGAL_SUBVAR_NAME_REGEX = re.compile(r'^[a-zA-Z_][0-9a-zA-Z_]*$')
-
-    @classmethod
-    def _subvar_name_is_legal(cls, proposed_variable_name: str):
-        return re.match(cls.LEGAL_SUBVAR_NAME_REGEX,
-                        proposed_variable_name) is not None
+    if allow_capital_underscore:
+        return re.sub('-+', '-', re.sub('[^-_0-9A-Za-z]+', '-',
+                                        name)).lstrip('-').rstrip('-')
+    else:
+        return re.sub('-+', '-', re.sub('[^-0-9a-z]+', '-',
+                                        name.lower())).lstrip('-').rstrip('-')
 
-    def __init__(self,
-                 items: Union[ItemList, dsl.PipelineParam],
-                 code: str,
-                 name_override: Optional[str] = None,
-                 op_name: Optional[str] = None,
-                 *args,
-                 **kwargs):
-        """LoopArguments represent the set of items to loop over in a
-        ParallelFor loop.
-
-        This class shouldn't be instantiated by the user but rather is created by
-        _ops_group.ParallelFor.
-
-        Args:
-          items: List of items to loop over.  If a list of dicts then, all
-            dicts must have the same keys and every key must be a legal Python
-            variable name.
-          code: A unique code used to identify these loop arguments.  Should
-            match the code for the ParallelFor ops_group which created these
-            LoopArguments.  This prevents parameter name collisions.
-        """
-        if name_override is None:
-            super().__init__(name=self._make_name(code), *args, **kwargs)
-        else:
-            super().__init__(
-                name=name_override, op_name=op_name, *args, **kwargs)
-
-        if not isinstance(items, (list, tuple, dsl.PipelineParam)):
-            raise TypeError(
-                'Expected list, tuple, or PipelineParam, got {}.'.format(
-                    type(items)))
-
-        if isinstance(items, tuple):
-            items = list(items)
-
-        if isinstance(items, list) and isinstance(items[0], dict):
-            subvar_names = set(items[0].keys())
-            for item in items:
-                if not set(item.keys()) == subvar_names:
-                    raise ValueError(
-                        'If you input a list of dicts then all dicts should have the same keys. '
-                        'Got: {}.'.format(items))
-
-            # then this block creates loop_args.variable_a and loop_args.variable_b
-            for subvar_name in subvar_names:
-                if not self._subvar_name_is_legal(subvar_name):
-                    raise ValueError(
-                        "Tried to create subvariable named {} but that's not a legal Python variable "
-                        'name.'.format(subvar_name))
-                setattr(
-                    self, subvar_name,
-                    LoopArgumentVariable(
-                        loop_args_name=self.name,
-                        this_variable_name=subvar_name,
-                        loop_args_op_name=self.op_name,
-                        loop_args=self,
-                    ))
-
-        self.items_or_pipeline_param = items
-        self.referenced_subvar_names = []
-
-    @classmethod
-    def from_pipeline_param(cls, param: dsl.PipelineParam) -> 'LoopArguments':
-        return LoopArguments(
-            items=param,
-            code=None,
-            name_override=param.name + '-' + cls.LOOP_ITEM_NAME_BASE,
-            op_name=param.op_name,
-            value=param.value,
-        )
-
-    def __getattr__(self, item):
-        # this is being overridden so that we can access subvariables of the
-        # LoopArguments (i.e.: item.a) without knowing the subvariable names ahead
-        # of time
-        self.referenced_subvar_names.append(item)
-        return LoopArgumentVariable(
-            loop_args_name=self.name,
-            this_variable_name=item,
-            loop_args_op_name=self.op_name,
-            loop_args=self,
-        )
-
-    def to_list_for_task_yaml(self):
-        if isinstance(self.items_or_pipeline_param, (list, tuple)):
-            return self.items_or_pipeline_param
-        else:
-            raise ValueError(
-                'You should only call this method on loop args which have list items, '
-                'not pipeline param items.')
 
-    @classmethod
-    def _make_name(cls, code: str):
-        """Make a name for this parameter.
+def match_serialized_pipelineparam(payload: str) -> List[PipelineParamTuple]:
+    """Matches the supplied serialized pipelineparam.
 
-        Code is a
-        """
-        return '{}-{}'.format(cls.LOOP_ITEM_PARAM_NAME_BASE, code)
+    Args:
+      payloads: The search space for the serialized pipelineparams.
 
-    @classmethod
-    def name_is_loop_argument(cls, param_name: str) -> bool:
-        """Return True if the given parameter name looks like a loop argument.
+    Returns:
+      The matched pipeline params we found in the supplied payload.
+    """
+    matches = re.findall(r'{{pipelineparam:op=([\w\s_-]*);name=([\w\s_-]+)}}',
+                         payload)
+    param_tuples = []
+    for match in matches:
+        pattern = '{{pipelineparam:op=%s;name=%s}}' % (match[0], match[1])
+        param_tuples.append(
+            PipelineParamTuple(
+                name=sanitize_k8s_name(match[1], True),
+                op=sanitize_k8s_name(match[0]),
+                pattern=pattern))
+    return param_tuples
+
+
+def _extract_pipelineparams(
+        payloads: Union[str, List[str]]) -> List['PipelineParam']:
+    """Extracts a list of PipelineParam instances from the payload string.
 
-        Either it came from a withItems loop item or withParams loop
-        item.
-        """
-        return cls.name_is_withitems_loop_argument(param_name) \
-          or cls.name_is_withparams_loop_argument(param_name)
+    Note: this function removes all duplicate matches.
 
-    @classmethod
-    def name_is_withitems_loop_argument(cls, param_name: str) -> bool:
-        """Return True if the given parameter name looks like it came from a
-        loop arguments parameter."""
-        return (cls.LOOP_ITEM_PARAM_NAME_BASE + '-') in param_name
-
-    @classmethod
-    def name_is_withparams_loop_argument(cls, param_name: str) -> bool:
-        """Return True if the given parameter name looks like it came from a
-        withParams loop item."""
-        return ('-' + cls.LOOP_ITEM_NAME_BASE) in param_name
-
-    @classmethod
-    def remove_loop_item_base_name(cls, param_name: str) -> str:
-        """Removes the last LOOP_ITEM_NAME_BASE from the end of param name."""
-        if ('-' + cls.LOOP_ITEM_NAME_BASE) in param_name:
-            # Split from the right, so that it handles multi-level nested args.
-            return param_name.rsplit('-' + cls.LOOP_ITEM_NAME_BASE, 1)[0]
-        return param_name
+    Args:
+      payload: a string/a list of strings that contains serialized pipelineparams
 
+    Return: List[]
+    """
+    if isinstance(payloads, str):
+        payloads = [payloads]
+    param_tuples = []
+    for payload in payloads:
+        param_tuples += match_serialized_pipelineparam(payload)
+    pipeline_params = []
+    for param_tuple in list(set(param_tuples)):
+        pipeline_params.append(
+            PipelineParam(
+                param_tuple.name, param_tuple.op, pattern=param_tuple.pattern))
+    return pipeline_params
+
+
+def extract_pipelineparams_from_any(
+    payload: Union['PipelineParam', str, list, tuple, dict]
+) -> List['PipelineParam']:
+    """Recursively extract PipelineParam instances or serialized string from
+    any object or list of objects.
 
-class LoopArgumentVariable(dsl.PipelineParam):
-    """Represents a subvariable for loop arguments.
+    Args:
+      payload (str or k8_obj or list[str or k8_obj]): a string/a list of strings
+        that contains serialized pipelineparams or a k8 definition object.
 
-    This is used for cases where we're looping over maps,   each of
-    which contains several variables.
+    Return: List[PipelineParam]
     """
-    SUBVAR_NAME_DELIMITER = '-subvar-'
+    if not payload:
+        return []
 
-    def __init__(
-        self,
-        loop_args_name: str,
-        this_variable_name: str,
-        loop_args_op_name: Optional[str],
-        # For backward compatible, add loop_args as an optional argument.
-        # Ideally, this should replace loop_args_name and loop_args_op_name.
-        loop_args: Optional[LoopArguments] = None,
-    ):
-        """
-    If the user ran:
-        with dsl.ParallelFor([{'a': 1, 'b': 2}, {'a': 3, 'b': 4}]) as item:
-            ...
-    Then there's be one LoopArgumentsVariable for 'a' and another for 'b'.
+    # PipelineParam
+    if isinstance(payload, PipelineParam):
+        return [payload]
+
+    # str
+    if isinstance(payload, str):
+        return list(set(_extract_pipelineparams(payload)))
+
+    # list or tuple
+    if isinstance(payload, list) or isinstance(payload, tuple):
+        pipeline_params = []
+        for item in payload:
+            pipeline_params += extract_pipelineparams_from_any(item)
+        return list(set(pipeline_params))
+
+    # dict
+    if isinstance(payload, dict):
+        pipeline_params = []
+        for key, value in payload.items():
+            pipeline_params += extract_pipelineparams_from_any(key)
+            pipeline_params += extract_pipelineparams_from_any(value)
+        return list(set(pipeline_params))
+
+    # k8s OpenAPI object
+    if hasattr(payload, 'attribute_map') and isinstance(payload.attribute_map,
+                                                        dict):
+        pipeline_params = []
+        for key in payload.attribute_map:
+            pipeline_params += extract_pipelineparams_from_any(
+                getattr(payload, key))
+
+        return list(set(pipeline_params))
+
+    # return empty list
+    return []
+
+
+class PipelineParam(object):
+    """Representing a future value that is passed between pipeline components.
+
+    A PipelineParam object can be used as a pipeline function argument so that it
+    will be a pipeline parameter that shows up in ML Pipelines system UI. It can
+    also represent an intermediate value passed between components.
 
     Args:
-      loop_args_name:  The name of the LoopArguments object that this is
-        a subvariable to.
-      this_variable_name: The name of this subvariable, which is the name
-        of the dict key that spawned this subvariable.
-      loop_args_op_name: The name of the op that produced the loop arguments.
-      loop_args: Optional; The LoopArguments object this subvariable is based on.
+      name: name of the pipeline parameter.
+      op_name: the name of the operation that produces the PipelineParam. None
+        means it is not produced by any operator, so if None, either user
+        constructs it directly (for providing an immediate value), or it is a
+        pipeline function argument.
+      value: The actual value of the PipelineParam. If provided, the PipelineParam
+        is "resolved" immediately. For now, we support string only.
+      param_type: the type of the PipelineParam.
+      pattern: the serialized string regex pattern this pipeline parameter created
+        from.
+
+    Raises: ValueError in name or op_name contains invalid characters, or both
+      op_name and value are set.
     """
-        super().__init__(
-            name=self.get_name(
-                loop_args_name=loop_args_name,
-                this_variable_name=this_variable_name),
-            op_name=loop_args_op_name,
-        )
-        self.loop_args = loop_args
 
-    @property
-    def items_or_pipeline_param(
-            self) -> Union[ItemList, _pipeline_param.PipelineParam]:
-        return self.loop_args.items_or_pipeline_param
-
-    @classmethod
-    def get_name(cls, loop_args_name: str, this_variable_name: str) -> str:
-        """Get the name.
-
-        Args:
-          loop_args_name: the name of the loop args parameter that this
-            LoopArgsVariable is attached to.
-          this_variable_name: the name of this LoopArgumentsVariable subvar.
+    def __init__(self,
+                 name: str,
+                 op_name: Optional[str] = None,
+                 value: Optional[str] = None,
+                 param_type: Optional[Union[str, Dict]] = None,
+                 pattern: Optional[str] = None):
+        valid_name_regex = r'^[A-Za-z][A-Za-z0-9\s_-]*$'
+        if not re.match(valid_name_regex, name):
+            raise ValueError(
+                'Only letters, numbers, spaces, "_", and "-" are allowed in name. '
+                'Must begin with a letter. Got name: {}'.format(name))
+
+        if op_name and value:
+            raise ValueError('op_name and value cannot be both set.')
 
-        Returns:
-          The name of this loop args variable.
+        self.name = name
+        # ensure value is None even if empty string or empty list
+        # so that serialization and unserialization remain consistent
+        # (i.e. None => '' => None)
+        self.op_name = op_name if op_name else None
+        self.value = value
+        self.param_type = param_type
+        self.pattern = pattern or str(self)
+
+    @property
+    def full_name(self):
+        """Unique name in the argo yaml for the PipelineParam."""
+        if self.op_name:
+            return self.op_name + '-' + self.name
+        return self.name
+
+    def __str__(self):
+        """String representation.
+
+        The string representation is a string identifier so we can mix
+        the PipelineParam inline with other strings such as arguments.
+        For example, we can support: ['echo %s' % param] as the
+        container command and later a compiler can replace the
+        placeholder "{{pipelineparam:op=%s;name=%s}}" with its own
+        parameter identifier.
         """
-        return '{}{}{}'.format(loop_args_name, cls.SUBVAR_NAME_DELIMITER,
-                               this_variable_name)
 
-    @classmethod
-    def name_is_loop_arguments_variable(cls, param_name: str) -> bool:
-        """Return True if the given parameter name looks like it came from a
-        LoopArgumentsVariable."""
-        return re.match('.+%s.+' % cls.SUBVAR_NAME_DELIMITER,
-                        param_name) is not None
-
-    @classmethod
-    def parse_loop_args_name_and_this_var_name(cls, t: str) -> Tuple[str, str]:
-        """Get the loop arguments param name and this subvariable name from the
-        given parameter name."""
-        m = re.match(
-            '(?P<loop_args_name>.*){}(?P<this_var_name>.*)'.format(
-                cls.SUBVAR_NAME_DELIMITER), t)
-        if m is None:
-            return None
-        else:
-            return m.groupdict()['loop_args_name'], m.groupdict(
-            )['this_var_name']
-
-    @classmethod
-    def get_subvar_name(cls, t: str) -> str:
-        """Get the subvariable name from a given LoopArgumentsVariable
-        parameter name."""
-        out = cls.parse_loop_args_name_and_this_var_name(t)
-        if out is None:
-            raise ValueError("Couldn't parse variable name: {}".format(t))
-        return out[1]
+        #This is deleted because if users specify default values to PipelineParam,
+        # The compiler can not detect it as the value is not NULL.
+        #if self.value:
+        #  return str(self.value)
+
+        op_name = self.op_name if self.op_name else ''
+        return '{{pipelineparam:op=%s;name=%s}}' % (op_name, self.name)
+
+    def __repr__(self):
+        # return str({self.__class__.__name__: self.__dict__})
+        # We make repr return the placeholder string so that if someone uses
+        # str()-based serialization of complex objects containing `PipelineParam`,
+        # it works properly.
+        # (e.g. str([1, 2, 3, kfp.dsl.PipelineParam("aaa"), 4, 5, 6,]))
+        return str(self)
+
+    def to_struct(self):
+        # Used by the json serializer. Outputs a JSON-serializable representation of
+        # the object
+        return str(self)
+
+    def __eq__(self, other):
+        return ConditionOperator('==', self, other)
+
+    def __ne__(self, other):
+        return ConditionOperator('!=', self, other)
+
+    def __lt__(self, other):
+        return ConditionOperator('<', self, other)
+
+    def __le__(self, other):
+        return ConditionOperator('<=', self, other)
+
+    def __gt__(self, other):
+        return ConditionOperator('>', self, other)
+
+    def __ge__(self, other):
+        return ConditionOperator('>=', self, other)
+
+    def __hash__(self):
+        return hash((self.op_name, self.name))
+
+    def ignore_type(self):
+        """ignore_type ignores the type information such that type checking
+        would also pass."""
+        self.param_type = None
+        return self
```

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_metadata.py` & `kfp-2.1.1/kfp/deprecated/dsl/_metadata.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_pipeline.py` & `kfp-2.1.1/kfp/deprecated/dsl/_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_pipeline_volume.py` & `kfp-2.1.1/kfp/deprecated/dsl/_pipeline_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_resource_op.py` & `kfp-2.1.1/kfp/deprecated/dsl/_resource_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_volume_op.py` & `kfp-2.1.1/kfp/deprecated/dsl/_volume_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/_volume_snapshot_op.py` & `kfp-2.1.1/kfp/deprecated/dsl/_volume_snapshot_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/artifact.py` & `kfp-2.1.1/kfp/deprecated/dsl/artifact.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/artifact_utils.py` & `kfp-2.1.1/kfp/deprecated/dsl/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/component_spec.py` & `kfp-2.1.1/kfp/deprecated/dsl/component_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/component_spec_test.py` & `kfp-2.1.1/kfp/deprecated/dsl/component_spec_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/data_passing_methods.py` & `kfp-2.1.1/kfp/deprecated/dsl/data_passing_methods.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/dsl_utils.py` & `kfp-2.1.1/kfp/deprecated/dsl/dsl_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/dsl_utils_test.py` & `kfp-2.1.1/kfp/deprecated/dsl/dsl_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/extensions/kubernetes.py` & `kfp-2.1.1/kfp/deprecated/dsl/extensions/kubernetes.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/io_types.py` & `kfp-2.1.1/kfp/deprecated/dsl/io_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/metrics_utils.py` & `kfp-2.1.1/kfp/deprecated/dsl/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/metrics_utils_test.py` & `kfp-2.1.1/kfp/deprecated/dsl/metrics_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/serialization_utils_test.py` & `kfp-2.1.1/kfp/deprecated/dsl/serialization_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/type_utils.py` & `kfp-2.1.1/kfp/deprecated/dsl/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/dsl/types.py` & `kfp-2.1.1/kfp/deprecated/dsl/types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/gcp.py` & `kfp-2.1.1/kfp/deprecated/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/notebook/__init__.py` & `kfp-2.1.1/kfp/deprecated/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/notebook/_magic.py` & `kfp-2.1.1/kfp/deprecated/notebook/_magic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/deprecated/onprem.py` & `kfp-2.1.1/kfp/deprecated/onprem.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/registry/__init__.py` & `kfp-2.1.1/kfp/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/registry/context/__init__.py` & `kfp-2.1.1/kfp/v2/components.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from kfp.components import *  # noqa
```

### Comparing `kfp-2.0.1/kfp/registry/context/default_pkg_dev.json` & `kfp-2.1.1/kfp/registry/context/default_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/registry/context/kfp_pkg_dev.json` & `kfp-2.1.1/kfp/registry/context/kfp_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/registry/registry_client.py` & `kfp-2.1.1/kfp/registry/registry_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/registry/registry_client_test.py` & `kfp-2.1.1/kfp/registry/registry_client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/v2/__init__.py` & `kfp-2.1.1/kfp/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/v2/compiler.py` & `kfp-2.1.1/kfp/v2/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.1/kfp/v2/components.py` & `kfp-2.1.1/kfp/v2/dsl.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from kfp.components import *  # noqa
+from kfp.dsl import *  # noqa
```

### Comparing `kfp-2.0.1/kfp.egg-info/PKG-INFO` & `kfp-2.1.1/kfp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.1
+Version: 2.1.1
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.0.1/requirements.in` & `kfp-2.1.1/requirements.in`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 docstring-parser>=0.7.3,<1
 # Pin google-api-core version for the bug fixing in 1.31.5
 # https://github.com/googleapis/python-api-core/releases/tag/v1.31.5
 google-api-core>=1.31.5,<3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0
 google-auth>=1.6.1,<3
 # https://github.com/googleapis/python-storage/blob/main/CHANGELOG.md#221-2022-03-15
 google-cloud-storage>=2.2.1,<3
+kfp-dsl==2.1.1
 # pin kfp-pipeline-spec to an exact version, since this is the contract between a given KFP SDK version and the BE. we don't want old version of the SDK to write new fields and to have the BE reject the new unsupported field (even if the new field backward compatible from a proto perspective)
 kfp-pipeline-spec==0.2.2
 # Update the upper version whenever a new major version of the
 # kfp-server-api package is released.
 # Update the lower version when kfp sdk depends on new apis/fields in
 # kfp-server-api.
 kfp-server-api>=2.0.0,<2.1.0
```

### Comparing `kfp-2.0.1/setup.py` & `kfp-2.1.1/setup.py`

 * *Files identical despite different names*

