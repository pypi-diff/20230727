# Comparing `tmp/nodestream-0.4.0.tar.gz` & `tmp/nodestream-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream-0.4.0.tar", max compression
+gzip compressed data, was "nodestream-0.5.0.tar", max compression
```

## Comparing `nodestream-0.4.0.tar` & `nodestream-0.5.0.tar`

### file list

```diff
@@ -1,124 +1,123 @@
--rw-r--r--   0        0        0    32335 2023-05-18 13:51:44.150322 nodestream-0.4.0/LICENSE
--rw-r--r--   0        0        0     1774 2023-07-09 02:30:41.172288 nodestream-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-18 13:51:44.151306 nodestream-0.4.0/nodestream/__init__.py
--rw-r--r--   0        0        0      109 2023-07-09 02:30:17.242799 nodestream-0.4.0/nodestream/cli/__init__.py
--rw-r--r--   0        0        0     1006 2023-07-09 02:30:17.243252 nodestream-0.4.0/nodestream/cli/application.py
--rw-r--r--   0        0        0      250 2023-07-09 02:30:17.243680 nodestream-0.4.0/nodestream/cli/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-07-09 02:30:41.176375 nodestream-0.4.0/nodestream/cli/commands/audit_command.py
--rw-r--r--   0        0        0      276 2023-07-09 02:30:41.176781 nodestream-0.4.0/nodestream/cli/commands/audit_refs.py
--rw-r--r--   0        0        0      212 2023-07-09 02:30:41.177101 nodestream-0.4.0/nodestream/cli/commands/audit_ttls.py
--rw-r--r--   0        0        0     1165 2023-07-09 02:30:17.245002 nodestream-0.4.0/nodestream/cli/commands/new.py
--rw-r--r--   0        0        0     1113 2023-07-09 02:30:17.245557 nodestream-0.4.0/nodestream/cli/commands/nodestream_command.py
--rw-r--r--   0        0        0     1213 2023-06-07 19:09:40.099387 nodestream-0.4.0/nodestream/cli/commands/print_schema.py
--rw-r--r--   0        0        0      893 2023-06-05 20:55:40.270803 nodestream-0.4.0/nodestream/cli/commands/remove.py
--rw-r--r--   0        0        0     1087 2023-06-06 14:48:12.780185 nodestream-0.4.0/nodestream/cli/commands/run.py
--rw-r--r--   0        0        0     1426 2023-07-09 00:52:53.455422 nodestream-0.4.0/nodestream/cli/commands/scaffold.py
--rw-r--r--   0        0        0      508 2023-06-06 14:48:12.780577 nodestream-0.4.0/nodestream/cli/commands/shared_options.py
--rw-r--r--   0        0        0      596 2023-06-05 20:55:40.271384 nodestream-0.4.0/nodestream/cli/commands/show.py
--rw-r--r--   0        0        0      986 2023-07-09 02:30:17.246161 nodestream-0.4.0/nodestream/cli/operations/__init__.py
--rw-r--r--   0        0        0      988 2023-06-05 20:55:40.271830 nodestream-0.4.0/nodestream/cli/operations/add_pipeline_to_project.py
--rw-r--r--   0        0        0      438 2023-07-09 02:52:37.857528 nodestream-0.4.0/nodestream/cli/operations/commit_project_to_disk.py
--rw-r--r--   0        0        0     2276 2023-07-09 02:30:41.177496 nodestream-0.4.0/nodestream/cli/operations/generate_pipeline_scaffold.py
--rw-r--r--   0        0        0     1434 2023-07-09 02:30:17.246752 nodestream-0.4.0/nodestream/cli/operations/generate_project.py
--rw-r--r--   0        0        0     2344 2023-07-09 02:30:41.177975 nodestream-0.4.0/nodestream/cli/operations/generate_python_scaffold.py
--rw-r--r--   0        0        0      796 2023-07-09 02:30:41.178237 nodestream-0.4.0/nodestream/cli/operations/initialize_logger.py
--rw-r--r--   0        0        0      339 2023-07-09 02:30:17.247745 nodestream-0.4.0/nodestream/cli/operations/initialize_project.py
--rw-r--r--   0        0        0      384 2023-06-05 20:55:40.273394 nodestream-0.4.0/nodestream/cli/operations/operation.py
--rw-r--r--   0        0        0     1209 2023-07-09 02:30:41.178628 nodestream-0.4.0/nodestream/cli/operations/print_project_schema.py
--rw-r--r--   0        0        0      533 2023-06-05 20:55:40.273559 nodestream-0.4.0/nodestream/cli/operations/remove_pipeline_from_project.py
--rw-r--r--   0        0        0     1145 2023-07-09 02:30:41.178958 nodestream-0.4.0/nodestream/cli/operations/run_audit.py
--rw-r--r--   0        0        0     2625 2023-06-12 14:46:03.281447 nodestream-0.4.0/nodestream/cli/operations/run_pipeline.py
--rw-r--r--   0        0        0     2371 2023-06-20 22:13:09.786648 nodestream-0.4.0/nodestream/cli/operations/show_pipelines.py
--rw-r--r--   0        0        0      165 2023-05-19 19:07:54.211393 nodestream-0.4.0/nodestream/databases/__init__.py
--rw-r--r--   0        0        0     3383 2023-07-09 02:30:41.179306 nodestream-0.4.0/nodestream/databases/debounced_ingest_strategy.py
--rw-r--r--   0        0        0     2628 2023-07-09 02:30:41.179490 nodestream-0.4.0/nodestream/databases/ingest_strategy.py
--rw-r--r--   0        0        0      166 2023-06-16 15:12:04.656280 nodestream-0.4.0/nodestream/databases/neo4j/__init__.py
--rw-r--r--   0        0        0     2710 2023-07-09 02:30:41.179959 nodestream-0.4.0/nodestream/databases/neo4j/index_query_builder.py
--rw-r--r--   0        0        0     8855 2023-07-09 02:30:41.180288 nodestream-0.4.0/nodestream/databases/neo4j/ingest_query_builder.py
--rw-r--r--   0        0        0     1060 2023-06-16 15:12:00.243062 nodestream-0.4.0/nodestream/databases/neo4j/query.py
--rw-r--r--   0        0        0     3984 2023-07-09 02:30:41.180709 nodestream-0.4.0/nodestream/databases/neo4j/query_executor.py
--rw-r--r--   0        0        0     3344 2023-06-12 14:46:03.284282 nodestream-0.4.0/nodestream/databases/operation_debouncer.py
--rw-r--r--   0        0        0     2045 2023-07-09 02:30:41.181099 nodestream-0.4.0/nodestream/databases/query_executor.py
--rw-r--r--   0        0        0     2044 2023-07-09 02:30:41.181398 nodestream-0.4.0/nodestream/databases/query_executor_with_statistics.py
--rw-r--r--   0        0        0     1890 2023-07-09 02:30:41.181685 nodestream-0.4.0/nodestream/databases/writer.py
--rw-r--r--   0        0        0     3566 2023-06-20 22:13:09.788231 nodestream-0.4.0/nodestream/file_io.py
--rw-r--r--   0        0        0      137 2023-07-09 02:30:41.182284 nodestream-0.4.0/nodestream/interpreting/__init__.py
--rw-r--r--   0        0        0      574 2023-07-09 02:30:41.182462 nodestream-0.4.0/nodestream/interpreting/interpretations/__init__.py
--rw-r--r--   0        0        0     1369 2023-07-09 02:30:41.182627 nodestream-0.4.0/nodestream/interpreting/interpretations/extract_variables_interpretation.py
--rw-r--r--   0        0        0      861 2023-07-09 02:30:41.182754 nodestream-0.4.0/nodestream/interpreting/interpretations/interpretation.py
--rw-r--r--   0        0        0     1262 2023-07-09 02:30:41.182941 nodestream-0.4.0/nodestream/interpreting/interpretations/properties_interpretation.py
--rw-r--r--   0        0        0    10264 2023-07-09 02:30:41.183161 nodestream-0.4.0/nodestream/interpreting/interpretations/relationship_interpretation.py
--rw-r--r--   0        0        0     4469 2023-07-09 02:30:41.183340 nodestream-0.4.0/nodestream/interpreting/interpretations/source_node_interpretation.py
--rw-r--r--   0        0        0     2181 2023-07-09 02:30:41.183590 nodestream-0.4.0/nodestream/interpreting/interpretations/switch_interpretation.py
--rw-r--r--   0        0        0     4662 2023-07-09 02:30:41.183926 nodestream-0.4.0/nodestream/interpreting/interpreter.py
--rw-r--r--   0        0        0     1744 2023-07-09 02:30:41.184285 nodestream-0.4.0/nodestream/interpreting/record_decomposers.py
--rw-r--r--   0        0        0      723 2023-07-09 02:30:41.184711 nodestream-0.4.0/nodestream/model/__init__.py
--rw-r--r--   0        0        0     3350 2023-07-09 02:30:41.184889 nodestream-0.4.0/nodestream/model/desired_ingestion.py
--rw-r--r--   0        0        0     6924 2023-07-09 02:30:41.185249 nodestream-0.4.0/nodestream/model/graph_objects.py
--rw-r--r--   0        0        0      873 2023-05-18 13:51:44.156142 nodestream-0.4.0/nodestream/model/ingestion_hooks.py
--rw-r--r--   0        0        0      282 2023-06-23 16:46:33.306823 nodestream-0.4.0/nodestream/model/match_strategy.py
--rw-r--r--   0        0        0      851 2023-07-09 02:30:41.185603 nodestream-0.4.0/nodestream/model/ttl.py
--rw-r--r--   0        0        0      875 2023-06-13 14:00:17.870064 nodestream-0.4.0/nodestream/pipeline/__init__.py
--rw-r--r--   0        0        0      321 2023-07-09 02:30:41.185809 nodestream-0.4.0/nodestream/pipeline/argument_resolvers/__init__.py
--rw-r--r--   0        0        0      441 2023-07-09 02:30:41.185999 nodestream-0.4.0/nodestream/pipeline/argument_resolvers/argument_resolver.py
--rw-r--r--   0        0        0      600 2023-07-09 02:30:41.186163 nodestream-0.4.0/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py
--rw-r--r--   0        0        0      689 2023-07-09 02:30:41.186305 nodestream-0.4.0/nodestream/pipeline/argument_resolvers/include_file_resolver.py
--rw-r--r--   0        0        0     2085 2023-07-09 02:30:41.186634 nodestream-0.4.0/nodestream/pipeline/class_loader.py
--rw-r--r--   0        0        0      275 2023-07-09 02:30:41.186850 nodestream-0.4.0/nodestream/pipeline/extractors/__init__.py
--rw-r--r--   0        0        0      678 2023-07-09 02:30:41.187009 nodestream-0.4.0/nodestream/pipeline/extractors/extractor.py
--rw-r--r--   0        0        0     2636 2023-07-09 02:30:41.187214 nodestream-0.4.0/nodestream/pipeline/extractors/files.py
--rw-r--r--   0        0        0      546 2023-07-09 02:30:41.187372 nodestream-0.4.0/nodestream/pipeline/extractors/iterable.py
--rw-r--r--   0        0        0        0 2023-07-09 02:30:41.187471 nodestream-0.4.0/nodestream/pipeline/extractors/stores/__init__.py
--rw-r--r--   0        0        0      130 2023-07-09 02:30:41.187838 nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/__init__.py
--rw-r--r--   0        0        0     4562 2023-07-09 02:30:41.188049 nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/athena_extractor.py
--rw-r--r--   0        0        0     2498 2023-07-09 02:30:41.188297 nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/credential_utils.py
--rw-r--r--   0        0        0     2156 2023-07-09 02:30:41.188507 nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/s3_extractor.py
--rw-r--r--   0        0        0      231 2023-07-09 02:30:41.188694 nodestream-0.4.0/nodestream/pipeline/extractors/streams/__init__.py
--rw-r--r--   0        0        0     2866 2023-07-09 02:30:41.188876 nodestream-0.4.0/nodestream/pipeline/extractors/streams/extractor.py
--rw-r--r--   0        0        0     1550 2023-07-09 02:30:41.189051 nodestream-0.4.0/nodestream/pipeline/extractors/streams/kafka.py
--rw-r--r--   0        0        0      646 2023-07-09 02:30:41.189199 nodestream-0.4.0/nodestream/pipeline/extractors/ttls.py
--rw-r--r--   0        0        0     3150 2023-07-09 02:30:41.189623 nodestream-0.4.0/nodestream/pipeline/filters.py
--rw-r--r--   0        0        0       22 2023-05-19 19:07:54.216776 nodestream-0.4.0/nodestream/pipeline/flush.py
--rw-r--r--   0        0        0      869 2023-06-12 14:46:03.288804 nodestream-0.4.0/nodestream/pipeline/meta.py
--rw-r--r--   0        0        0      327 2023-07-09 02:30:41.189776 nodestream-0.4.0/nodestream/pipeline/normalizers/__init__.py
--rw-r--r--   0        0        0      240 2023-07-09 02:30:41.190001 nodestream-0.4.0/nodestream/pipeline/normalizers/lowercase_strings.py
--rw-r--r--   0        0        0     1711 2023-07-09 02:30:41.190181 nodestream-0.4.0/nodestream/pipeline/normalizers/normalizer.py
--rw-r--r--   0        0        0      249 2023-07-09 02:30:41.190411 nodestream-0.4.0/nodestream/pipeline/normalizers/remove_trailing_dots.py
--rw-r--r--   0        0        0      236 2023-07-09 02:30:41.190719 nodestream-0.4.0/nodestream/pipeline/normalizers/trim_whitespace.py
--rw-r--r--   0        0        0     1252 2023-07-09 02:51:32.187156 nodestream-0.4.0/nodestream/pipeline/pipeline.py
--rw-r--r--   0        0        0     2968 2023-07-09 02:30:41.191800 nodestream-0.4.0/nodestream/pipeline/pipeline_file_loader.py
--rw-r--r--   0        0        0      742 2023-06-15 02:17:55.638831 nodestream-0.4.0/nodestream/pipeline/step.py
--rw-r--r--   0        0        0      195 2023-07-09 02:51:32.187730 nodestream-0.4.0/nodestream/pipeline/transformers/__init__.py
--rw-r--r--   0        0        0      686 2023-07-09 02:51:32.188072 nodestream-0.4.0/nodestream/pipeline/transformers/expand_json_field.py
--rw-r--r--   0        0        0     1038 2023-07-09 02:30:41.192402 nodestream-0.4.0/nodestream/pipeline/transformers/transformer.py
--rw-r--r--   0        0        0      451 2023-07-09 02:30:41.192561 nodestream-0.4.0/nodestream/pipeline/transformers/value_projection.py
--rw-r--r--   0        0        0      794 2023-07-09 02:30:41.192751 nodestream-0.4.0/nodestream/pipeline/value_providers/__init__.py
--rw-r--r--   0        0        0     1171 2023-07-09 02:30:41.192897 nodestream-0.4.0/nodestream/pipeline/value_providers/context.py
--rw-r--r--   0        0        0     1755 2023-07-09 02:30:41.193087 nodestream-0.4.0/nodestream/pipeline/value_providers/jmespath_value_provider.py
--rw-r--r--   0        0        0     1121 2023-07-09 02:30:41.193249 nodestream-0.4.0/nodestream/pipeline/value_providers/jq_value_provder.py
--rw-r--r--   0        0        0     1283 2023-07-09 02:30:41.193407 nodestream-0.4.0/nodestream/pipeline/value_providers/mapping_value_provider.py
--rw-r--r--   0        0        0      611 2023-07-09 02:30:41.193585 nodestream-0.4.0/nodestream/pipeline/value_providers/static_value_provider.py
--rw-r--r--   0        0        0     1287 2023-07-09 02:30:41.193756 nodestream-0.4.0/nodestream/pipeline/value_providers/string_format_value_provider.py
--rw-r--r--   0        0        0     2192 2023-07-09 02:30:41.193920 nodestream-0.4.0/nodestream/pipeline/value_providers/value_provider.py
--rw-r--r--   0        0        0      963 2023-07-09 02:30:41.194113 nodestream-0.4.0/nodestream/pipeline/value_providers/variable_value_provider.py
--rw-r--r--   0        0        0     1726 2023-06-12 14:46:03.290482 nodestream-0.4.0/nodestream/pipeline/writers.py
--rw-r--r--   0        0        0      351 2023-07-09 02:30:17.263877 nodestream-0.4.0/nodestream/project/__init__.py
--rw-r--r--   0        0        0      262 2023-07-09 02:30:41.194428 nodestream-0.4.0/nodestream/project/audits/__init__.py
--rw-r--r--   0        0        0      695 2023-07-09 02:30:41.194712 nodestream-0.4.0/nodestream/project/audits/audit.py
--rw-r--r--   0        0        0      375 2023-07-09 02:30:41.194955 nodestream-0.4.0/nodestream/project/audits/audit_printer.py
--rw-r--r--   0        0        0     1647 2023-07-09 02:30:41.195097 nodestream-0.4.0/nodestream/project/audits/audit_referencial_integrity.py
--rw-r--r--   0        0        0     1546 2023-07-09 02:30:41.195262 nodestream-0.4.0/nodestream/project/audits/audit_ttls.py
--rw-r--r--   0        0        0     2706 2023-07-09 02:30:41.195594 nodestream-0.4.0/nodestream/project/pipeline_definition.py
--rw-r--r--   0        0        0     1557 2023-07-09 02:30:41.195888 nodestream-0.4.0/nodestream/project/pipeline_progress_reporter.py
--rw-r--r--   0        0        0     3025 2023-07-09 02:30:41.196198 nodestream-0.4.0/nodestream/project/pipeline_scope.py
--rw-r--r--   0        0        0     3790 2023-07-09 02:30:41.196529 nodestream-0.4.0/nodestream/project/project.py
--rw-r--r--   0        0        0      755 2023-07-09 02:30:17.265791 nodestream-0.4.0/nodestream/project/run_request.py
--rw-r--r--   0        0        0     1408 2023-07-09 02:30:41.196704 nodestream-0.4.0/nodestream/schema/indexes.py
--rw-r--r--   0        0        0      329 2023-07-09 02:30:41.196926 nodestream-0.4.0/nodestream/schema/printers/__init__.py
--rw-r--r--   0        0        0     5710 2023-07-09 02:30:41.197121 nodestream-0.4.0/nodestream/schema/printers/graphql_schema_printer.py
--rw-r--r--   0        0        0      272 2023-07-09 02:30:41.197356 nodestream-0.4.0/nodestream/schema/printers/plain_text_schema_printer.py
--rw-r--r--   0        0        0      634 2023-07-09 02:30:41.200726 nodestream-0.4.0/nodestream/schema/printers/schema_printer.py
--rw-r--r--   0        0        0    13845 2023-07-09 02:30:41.200971 nodestream-0.4.0/nodestream/schema/schema.py
--rw-r--r--   0        0        0     1879 2023-07-09 02:30:41.201282 nodestream-0.4.0/nodestream/subclass_registry.py
--rw-r--r--   0        0        0     1976 2023-07-09 02:51:32.188776 nodestream-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 nodestream-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    32335 2023-05-18 13:51:44.150322 nodestream-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1774 2023-07-09 02:30:41.172288 nodestream-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 13:51:44.151306 nodestream-0.5.0/nodestream/__init__.py
+-rw-r--r--   0        0        0      120 2023-07-27 19:40:21.423892 nodestream-0.5.0/nodestream/cli/__init__.py
+-rw-r--r--   0        0        0      683 2023-07-27 19:40:21.424596 nodestream-0.5.0/nodestream/cli/application.py
+-rw-r--r--   0        0        0      394 2023-07-27 19:40:21.425214 nodestream-0.5.0/nodestream/cli/commands/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-27 19:40:21.425679 nodestream-0.5.0/nodestream/cli/commands/audit_command.py
+-rw-r--r--   0        0        0      879 2023-07-27 19:40:21.426195 nodestream-0.5.0/nodestream/cli/commands/new.py
+-rw-r--r--   0        0        0     1285 2023-07-27 19:40:21.426441 nodestream-0.5.0/nodestream/cli/commands/nodestream_command.py
+-rw-r--r--   0        0        0     1213 2023-06-07 19:09:40.099387 nodestream-0.5.0/nodestream/cli/commands/print_schema.py
+-rw-r--r--   0        0        0      893 2023-06-05 20:55:40.270803 nodestream-0.5.0/nodestream/cli/commands/remove.py
+-rw-r--r--   0        0        0     1087 2023-06-06 14:48:12.780185 nodestream-0.5.0/nodestream/cli/commands/run.py
+-rw-r--r--   0        0        0     1426 2023-07-09 00:52:53.455422 nodestream-0.5.0/nodestream/cli/commands/scaffold.py
+-rw-r--r--   0        0        0      508 2023-06-06 14:48:12.780577 nodestream-0.5.0/nodestream/cli/commands/shared_options.py
+-rw-r--r--   0        0        0      596 2023-06-05 20:55:40.271384 nodestream-0.5.0/nodestream/cli/commands/show.py
+-rw-r--r--   0        0        0      917 2023-07-27 19:40:21.427093 nodestream-0.5.0/nodestream/cli/operations/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-05 20:55:40.271830 nodestream-0.5.0/nodestream/cli/operations/add_pipeline_to_project.py
+-rw-r--r--   0        0        0      438 2023-07-09 03:19:15.369967 nodestream-0.5.0/nodestream/cli/operations/commit_project_to_disk.py
+-rw-r--r--   0        0        0     2276 2023-07-09 02:30:41.177496 nodestream-0.5.0/nodestream/cli/operations/generate_pipeline_scaffold.py
+-rw-r--r--   0        0        0      796 2023-07-09 02:30:41.178237 nodestream-0.5.0/nodestream/cli/operations/initialize_logger.py
+-rw-r--r--   0        0        0      267 2023-07-27 19:40:21.427657 nodestream-0.5.0/nodestream/cli/operations/initialize_project.py
+-rw-r--r--   0        0        0      384 2023-06-05 20:55:40.273394 nodestream-0.5.0/nodestream/cli/operations/operation.py
+-rw-r--r--   0        0        0     1333 2023-07-27 19:40:21.428254 nodestream-0.5.0/nodestream/cli/operations/print_project_schema.py
+-rw-r--r--   0        0        0      533 2023-06-05 20:55:40.273559 nodestream-0.5.0/nodestream/cli/operations/remove_pipeline_from_project.py
+-rw-r--r--   0        0        0     1145 2023-07-09 02:30:41.178958 nodestream-0.5.0/nodestream/cli/operations/run_audit.py
+-rw-r--r--   0        0        0     2625 2023-06-12 14:46:03.281447 nodestream-0.5.0/nodestream/cli/operations/run_pipeline.py
+-rw-r--r--   0        0        0      866 2023-07-27 19:40:21.428669 nodestream-0.5.0/nodestream/cli/operations/run_project_cookiecutter.py
+-rw-r--r--   0        0        0     2436 2023-07-27 19:40:21.429248 nodestream-0.5.0/nodestream/cli/operations/show_pipelines.py
+-rw-r--r--   0        0        0      165 2023-07-27 19:40:16.908918 nodestream-0.5.0/nodestream/databases/__init__.py
+-rw-r--r--   0        0        0     3383 2023-07-27 19:40:16.909569 nodestream-0.5.0/nodestream/databases/debounced_ingest_strategy.py
+-rw-r--r--   0        0        0     2628 2023-07-27 19:40:16.910303 nodestream-0.5.0/nodestream/databases/ingest_strategy.py
+-rw-r--r--   0        0        0      166 2023-06-16 15:12:04.656280 nodestream-0.5.0/nodestream/databases/neo4j/__init__.py
+-rw-r--r--   0        0        0     2710 2023-07-09 02:30:41.179959 nodestream-0.5.0/nodestream/databases/neo4j/index_query_builder.py
+-rw-r--r--   0        0        0     8855 2023-07-27 19:40:16.910986 nodestream-0.5.0/nodestream/databases/neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0     1060 2023-06-16 15:12:00.243062 nodestream-0.5.0/nodestream/databases/neo4j/query.py
+-rw-r--r--   0        0        0     3984 2023-07-27 19:40:16.911542 nodestream-0.5.0/nodestream/databases/neo4j/query_executor.py
+-rw-r--r--   0        0        0     3344 2023-07-27 19:40:16.912576 nodestream-0.5.0/nodestream/databases/operation_debouncer.py
+-rw-r--r--   0        0        0     2125 2023-07-27 19:40:21.430003 nodestream-0.5.0/nodestream/databases/query_executor.py
+-rw-r--r--   0        0        0     2044 2023-07-27 19:40:16.913862 nodestream-0.5.0/nodestream/databases/query_executor_with_statistics.py
+-rw-r--r--   0        0        0     2015 2023-07-27 19:40:21.430803 nodestream-0.5.0/nodestream/databases/writer.py
+-rw-r--r--   0        0        0     3566 2023-06-20 22:13:09.788231 nodestream-0.5.0/nodestream/file_io.py
+-rw-r--r--   0        0        0      137 2023-07-27 19:40:16.914384 nodestream-0.5.0/nodestream/interpreting/__init__.py
+-rw-r--r--   0        0        0      574 2023-07-09 02:30:41.182462 nodestream-0.5.0/nodestream/interpreting/interpretations/__init__.py
+-rw-r--r--   0        0        0     1369 2023-07-27 19:40:16.914960 nodestream-0.5.0/nodestream/interpreting/interpretations/extract_variables_interpretation.py
+-rw-r--r--   0        0        0      948 2023-07-27 19:40:21.431920 nodestream-0.5.0/nodestream/interpreting/interpretations/interpretation.py
+-rw-r--r--   0        0        0     1262 2023-07-27 19:40:16.915955 nodestream-0.5.0/nodestream/interpreting/interpretations/properties_interpretation.py
+-rw-r--r--   0        0        0    10264 2023-07-27 19:40:16.916516 nodestream-0.5.0/nodestream/interpreting/interpretations/relationship_interpretation.py
+-rw-r--r--   0        0        0     4469 2023-07-27 19:40:16.917070 nodestream-0.5.0/nodestream/interpreting/interpretations/source_node_interpretation.py
+-rw-r--r--   0        0        0     2181 2023-07-27 19:40:16.917579 nodestream-0.5.0/nodestream/interpreting/interpretations/switch_interpretation.py
+-rw-r--r--   0        0        0     4786 2023-07-27 19:40:21.432602 nodestream-0.5.0/nodestream/interpreting/interpreter.py
+-rw-r--r--   0        0        0     1744 2023-07-09 02:30:41.184285 nodestream-0.5.0/nodestream/interpreting/record_decomposers.py
+-rw-r--r--   0        0        0      723 2023-07-27 19:40:16.918936 nodestream-0.5.0/nodestream/model/__init__.py
+-rw-r--r--   0        0        0     3350 2023-07-27 19:40:16.919178 nodestream-0.5.0/nodestream/model/desired_ingestion.py
+-rw-r--r--   0        0        0     6924 2023-07-27 19:40:16.919398 nodestream-0.5.0/nodestream/model/graph_objects.py
+-rw-r--r--   0        0        0      873 2023-07-27 19:40:16.919738 nodestream-0.5.0/nodestream/model/ingestion_hooks.py
+-rw-r--r--   0        0        0      282 2023-07-27 19:40:16.920211 nodestream-0.5.0/nodestream/model/match_strategy.py
+-rw-r--r--   0        0        0      851 2023-07-27 19:40:16.920507 nodestream-0.5.0/nodestream/model/ttl.py
+-rw-r--r--   0        0        0      875 2023-07-27 19:40:16.921973 nodestream-0.5.0/nodestream/pipeline/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-09 02:30:41.185809 nodestream-0.5.0/nodestream/pipeline/argument_resolvers/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-27 19:40:21.433264 nodestream-0.5.0/nodestream/pipeline/argument_resolvers/argument_resolver.py
+-rw-r--r--   0        0        0      600 2023-07-09 02:30:41.186163 nodestream-0.5.0/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py
+-rw-r--r--   0        0        0      680 2023-07-27 19:40:21.433692 nodestream-0.5.0/nodestream/pipeline/argument_resolvers/include_file_resolver.py
+-rw-r--r--   0        0        0     2085 2023-07-09 02:30:41.186634 nodestream-0.5.0/nodestream/pipeline/class_loader.py
+-rw-r--r--   0        0        0      275 2023-07-09 02:30:41.186850 nodestream-0.5.0/nodestream/pipeline/extractors/__init__.py
+-rw-r--r--   0        0        0      678 2023-07-09 02:30:41.187009 nodestream-0.5.0/nodestream/pipeline/extractors/extractor.py
+-rw-r--r--   0        0        0     2855 2023-07-27 19:40:21.434003 nodestream-0.5.0/nodestream/pipeline/extractors/files.py
+-rw-r--r--   0        0        0      546 2023-07-09 02:30:41.187372 nodestream-0.5.0/nodestream/pipeline/extractors/iterable.py
+-rw-r--r--   0        0        0        0 2023-07-09 02:30:41.187471 nodestream-0.5.0/nodestream/pipeline/extractors/stores/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-09 02:30:41.187838 nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/__init__.py
+-rw-r--r--   0        0        0     4562 2023-07-09 02:30:41.188049 nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/athena_extractor.py
+-rw-r--r--   0        0        0     2498 2023-07-09 02:30:41.188297 nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/credential_utils.py
+-rw-r--r--   0        0        0     2156 2023-07-09 02:30:41.188507 nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/s3_extractor.py
+-rw-r--r--   0        0        0      231 2023-07-09 02:30:41.188694 nodestream-0.5.0/nodestream/pipeline/extractors/streams/__init__.py
+-rw-r--r--   0        0        0     3151 2023-07-27 19:40:21.434564 nodestream-0.5.0/nodestream/pipeline/extractors/streams/extractor.py
+-rw-r--r--   0        0        0     1550 2023-07-09 02:30:41.189051 nodestream-0.5.0/nodestream/pipeline/extractors/streams/kafka.py
+-rw-r--r--   0        0        0      646 2023-07-27 19:40:16.923284 nodestream-0.5.0/nodestream/pipeline/extractors/ttls.py
+-rw-r--r--   0        0        0     3150 2023-07-09 02:30:41.189623 nodestream-0.5.0/nodestream/pipeline/filters.py
+-rw-r--r--   0        0        0       22 2023-05-19 19:07:54.216776 nodestream-0.5.0/nodestream/pipeline/flush.py
+-rw-r--r--   0        0        0      869 2023-06-12 14:46:03.288804 nodestream-0.5.0/nodestream/pipeline/meta.py
+-rw-r--r--   0        0        0      327 2023-07-09 02:30:41.189776 nodestream-0.5.0/nodestream/pipeline/normalizers/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-09 02:30:41.190001 nodestream-0.5.0/nodestream/pipeline/normalizers/lowercase_strings.py
+-rw-r--r--   0        0        0     1845 2023-07-27 19:40:21.435113 nodestream-0.5.0/nodestream/pipeline/normalizers/normalizer.py
+-rw-r--r--   0        0        0      249 2023-07-09 02:30:41.190411 nodestream-0.5.0/nodestream/pipeline/normalizers/remove_trailing_dots.py
+-rw-r--r--   0        0        0      236 2023-07-09 02:30:41.190719 nodestream-0.5.0/nodestream/pipeline/normalizers/trim_whitespace.py
+-rw-r--r--   0        0        0     1252 2023-07-09 03:19:15.370764 nodestream-0.5.0/nodestream/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3021 2023-07-27 19:40:21.435508 nodestream-0.5.0/nodestream/pipeline/pipeline_file_loader.py
+-rw-r--r--   0        0        0      742 2023-06-15 02:17:55.638831 nodestream-0.5.0/nodestream/pipeline/step.py
+-rw-r--r--   0        0        0      195 2023-07-09 03:19:15.371440 nodestream-0.5.0/nodestream/pipeline/transformers/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-27 19:40:16.924367 nodestream-0.5.0/nodestream/pipeline/transformers/expand_json_field.py
+-rw-r--r--   0        0        0     1038 2023-07-09 02:30:41.192402 nodestream-0.5.0/nodestream/pipeline/transformers/transformer.py
+-rw-r--r--   0        0        0      451 2023-07-09 02:30:41.192561 nodestream-0.5.0/nodestream/pipeline/transformers/value_projection.py
+-rw-r--r--   0        0        0      794 2023-07-09 02:30:41.192751 nodestream-0.5.0/nodestream/pipeline/value_providers/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-27 19:40:16.924906 nodestream-0.5.0/nodestream/pipeline/value_providers/context.py
+-rw-r--r--   0        0        0     1755 2023-07-09 02:30:41.193087 nodestream-0.5.0/nodestream/pipeline/value_providers/jmespath_value_provider.py
+-rw-r--r--   0        0        0     1121 2023-07-09 02:30:41.193249 nodestream-0.5.0/nodestream/pipeline/value_providers/jq_value_provder.py
+-rw-r--r--   0        0        0     1283 2023-07-09 02:30:41.193407 nodestream-0.5.0/nodestream/pipeline/value_providers/mapping_value_provider.py
+-rw-r--r--   0        0        0      611 2023-07-09 02:30:41.193585 nodestream-0.5.0/nodestream/pipeline/value_providers/static_value_provider.py
+-rw-r--r--   0        0        0     1287 2023-07-09 02:30:41.193756 nodestream-0.5.0/nodestream/pipeline/value_providers/string_format_value_provider.py
+-rw-r--r--   0        0        0     2279 2023-07-27 19:40:21.436021 nodestream-0.5.0/nodestream/pipeline/value_providers/value_provider.py
+-rw-r--r--   0        0        0      963 2023-07-09 02:30:41.194113 nodestream-0.5.0/nodestream/pipeline/value_providers/variable_value_provider.py
+-rw-r--r--   0        0        0     1726 2023-06-12 14:46:03.290482 nodestream-0.5.0/nodestream/pipeline/writers.py
+-rw-r--r--   0        0        0      807 2023-07-27 19:40:21.436390 nodestream-0.5.0/nodestream/pluggable.py
+-rw-r--r--   0        0        0      387 2023-07-27 19:40:21.436939 nodestream-0.5.0/nodestream/project/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-27 19:40:21.437397 nodestream-0.5.0/nodestream/project/audits/__init__.py
+-rw-r--r--   0        0        0     1623 2023-07-27 19:40:21.438103 nodestream-0.5.0/nodestream/project/audits/audit.py
+-rw-r--r--   0        0        0      375 2023-07-09 02:30:41.194955 nodestream-0.5.0/nodestream/project/audits/audit_printer.py
+-rw-r--r--   0        0        0     1751 2023-07-27 19:40:21.438543 nodestream-0.5.0/nodestream/project/audits/audit_referencial_integrity.py
+-rw-r--r--   0        0        0     1641 2023-07-27 19:40:21.438960 nodestream-0.5.0/nodestream/project/audits/audit_ttls.py
+-rw-r--r--   0        0        0     4009 2023-07-27 19:40:21.439291 nodestream-0.5.0/nodestream/project/pipeline_definition.py
+-rw-r--r--   0        0        0     2650 2023-07-27 19:40:21.439883 nodestream-0.5.0/nodestream/project/pipeline_progress_reporter.py
+-rw-r--r--   0        0        0     5037 2023-07-27 19:40:21.440206 nodestream-0.5.0/nodestream/project/pipeline_scope.py
+-rw-r--r--   0        0        0     7792 2023-07-27 19:40:21.440555 nodestream-0.5.0/nodestream/project/project.py
+-rw-r--r--   0        0        0     1561 2023-07-27 19:40:21.441013 nodestream-0.5.0/nodestream/project/run_request.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:40:21.441120 nodestream-0.5.0/nodestream/schema/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-09 02:30:41.196704 nodestream-0.5.0/nodestream/schema/indexes.py
+-rw-r--r--   0        0        0      329 2023-07-09 02:30:41.196926 nodestream-0.5.0/nodestream/schema/printers/__init__.py
+-rw-r--r--   0        0        0     5710 2023-07-09 02:30:41.197121 nodestream-0.5.0/nodestream/schema/printers/graphql_schema_printer.py
+-rw-r--r--   0        0        0      272 2023-07-09 02:30:41.197356 nodestream-0.5.0/nodestream/schema/printers/plain_text_schema_printer.py
+-rw-r--r--   0        0        0      721 2023-07-27 19:40:21.441565 nodestream-0.5.0/nodestream/schema/printers/schema_printer.py
+-rw-r--r--   0        0        0    13845 2023-07-09 02:30:41.200971 nodestream-0.5.0/nodestream/schema/schema.py
+-rw-r--r--   0        0        0     1879 2023-07-09 02:30:41.201282 nodestream-0.5.0/nodestream/subclass_registry.py
+-rw-r--r--   0        0        0     2818 2023-07-27 20:02:55.948300 nodestream-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 nodestream-0.5.0/PKG-INFO
```

### Comparing `nodestream-0.4.0/LICENSE` & `nodestream-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/README.md` & `nodestream-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/commands/new.py` & `nodestream-0.5.0/nodestream/cli/commands/scaffold.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from pathlib import Path
-
-from cleo.helpers import argument
-
 from ..operations import (
+    AddPipelineToProject,
     CommitProjectToDisk,
     GeneratePipelineScaffold,
-    GenerateProject,
-    GeneratePythonScaffold,
+    InitializeProject,
 )
 from .nodestream_command import NodestreamCommand
-from .shared_options import DATABASE_NAME_OPTION
+from .shared_options import (
+    DATABASE_NAME_OPTION,
+    PIPELINE_ARGUMENT,
+    PROJECT_FILE_OPTION,
+    SCOPE_NAME_OPTION,
+)
 
 
-class New(NodestreamCommand):
-    name = "new"
-    description = "Generate a New Nodestream"
-    arguments = [
-        argument("project", "the name of the project to create"),
-    ]
-    options = [DATABASE_NAME_OPTION]
+class Scaffold(NodestreamCommand):
+    name = "scaffold"
+    description = "Generate a New Nodestream Pipeline"
+    arguments = [PIPELINE_ARGUMENT]
+    options = [DATABASE_NAME_OPTION, SCOPE_NAME_OPTION, PROJECT_FILE_OPTION]
 
     async def handle_async(self):
-        project_root = Path(self.argument("project"))
-        db = self.option("database")
-        python_files = await self.run_operation(GeneratePythonScaffold(project_root))
-        pipelines = await self.run_operation(GeneratePipelineScaffold(project_root, db))
-        gen_project = GenerateProject(project_root, pipelines, python_files, db)
-        project = await self.run_operation(gen_project)
-        commit_to_disk = CommitProjectToDisk(project, project_root / "nodestream.yaml")
-        await self.run_operation(commit_to_disk)
-        self.line(f"<info>Created new project at '{project_root}'</info>")
+        pipeline_name = self.argument("pipeline")
+        desired_scope = self.option("scope")
+        database_name = self.option("database")
+        project = await self.run_operation(InitializeProject())
+        generated_pipelines = await self.run_operation(
+            GeneratePipelineScaffold(
+                project_root=self.get_project_path().parent,
+                database_name=database_name,
+                pipeline_file_name=pipeline_name + ".yaml",
+            )
+        )
+        for generated_pipeline in generated_pipelines:
+            self.line(f"<info>Generated pipeline at '{generated_pipeline}'</info>")
+            await self.run_operation(
+                AddPipelineToProject(project, generated_pipeline, desired_scope)
+            )
+
+        await self.run_operation(CommitProjectToDisk(project, self.get_project_path()))
```

### Comparing `nodestream-0.4.0/nodestream/cli/commands/nodestream_command.py` & `nodestream-0.5.0/nodestream/cli/commands/nodestream_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import asyncio
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from cleo.commands.command import Command
 from cleo.io.outputs.output import Verbosity
 
+from ...pluggable import Pluggable
 from ...project import Project
 
 if TYPE_CHECKING:
     from ..operations import Operation
 
 DEFAULT_PROJECT_FILE = Path("nodestream.yaml")
 
 
-class NodestreamCommand(Command):
+class NodestreamCommand(Command, Pluggable):
+    entrypoint_name = "commands"
+
     def handle(self):
         return asyncio.run(self.handle_async())
 
     async def handle_async(self):
         raise NotImplementedError
 
     async def run_operation(self, operation: "Operation"):
@@ -36,7 +39,11 @@
     @property
     def has_json_logging_set(self) -> bool:
         return self.option("json")
 
     @property
     def scope(self) -> str:
         return self.option("scope")
+
+    @property
+    def is_verbose(self) -> bool:
+        return self.io.output.is_verbose()
```

### Comparing `nodestream-0.4.0/nodestream/cli/commands/print_schema.py` & `nodestream-0.5.0/nodestream/cli/commands/print_schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/commands/remove.py` & `nodestream-0.5.0/nodestream/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/commands/run.py` & `nodestream-0.5.0/nodestream/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/commands/show.py` & `nodestream-0.5.0/nodestream/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/add_pipeline_to_project.py` & `nodestream-0.5.0/nodestream/cli/operations/add_pipeline_to_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/generate_pipeline_scaffold.py` & `nodestream-0.5.0/nodestream/cli/operations/generate_pipeline_scaffold.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/generate_project.py` & `nodestream-0.5.0/nodestream/cli/operations/show_pipelines.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,72 @@
-from pathlib import Path
-from typing import List
+import json
+from abc import ABC, abstractmethod
+from typing import Iterable, List, Optional, Tuple
 
-from ...project import PipelineDefinition, PipelineScope, Project
+from ...project import PipelineDefinition, Project
 from ..commands.nodestream_command import NodestreamCommand
 from .operation import Operation
 
 
-class GenerateProject(Operation):
-    def __init__(
-        self,
-        project_root: Path,
-        pipelines: List[Path],
-        source_modules: List[Path],
-        database: str,
-    ) -> None:
-        self.pipelines = pipelines
-        self.source_modules = source_modules
-        self.project_root = project_root
-        self.database = database
-
-    async def perform(self, _: NodestreamCommand):
-        imports = self.generate_import_directives()
-        scope = self.generate_pipeline_scope()
-        return Project([scope], imports)
-
-    def generate_import_directives(self) -> List[str]:
-        project_imports = [
-            str(path.relative_to(self.project_root).with_suffix(""))
-            .replace("/", ".")
-            .replace("\\", ".")
-            for path in self.source_modules
-            if "__init__" not in path.name
+class OutputFormat(ABC):
+    def __init__(self, command: NodestreamCommand) -> None:
+        self.command = command
+
+    @abstractmethod
+    def output(self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]):
+        raise NotImplementedError
+
+
+class TableOutputFormat(OutputFormat):
+    HEADERS = ["scope", "name", "file", "annotations"]
+
+    def get_data_rows(
+        self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]
+    ) -> List[list]:
+        return [
+            [
+                scope,
+                definition.name,
+                str(definition.file_path),
+                "".join(definition.annotations.keys()),
+            ]
+            for scope, definition in matching_pipelines
         ]
-        project_imports.append(f"nodestream.databases.{self.database}")
-        return project_imports
 
-    def generate_pipeline_scope(self):
-        pipeline_definitions = [
-            PipelineDefinition.from_path(path.relative_to(self.project_root))
-            for path in self.pipelines
+    def output(self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]):
+        table = self.command.table(self.HEADERS, self.get_data_rows(matching_pipelines))
+        table.render()
+
+
+class JsonOutputFormat(OutputFormat):
+    def output(self, matching_pipelines: Iterable[Tuple[str, PipelineDefinition]]):
+        json_data = [
+            pipeline.to_file_data(verbose=self.command.is_verbose)
+            for _, pipeline in matching_pipelines
         ]
-        return PipelineScope("default", pipeline_definitions)
+        self.command.write(json.dumps(json_data))
+
+
+class ShowPipelines(Operation):
+    def __init__(
+        self, project: Project, scope_name: Optional[str], use_json: bool = False
+    ) -> None:
+        self.project = project
+        self.scope_name = scope_name
+        self.use_json = use_json
+
+    async def perform(self, command: NodestreamCommand):
+        self.get_output_format(command).output(self.get_matching_pipelines())
+
+    def get_output_format(self, command: NodestreamCommand):
+        cls = JsonOutputFormat if self.use_json else TableOutputFormat
+        return cls(command)
+
+    def get_matching_pipelines(self) -> Iterable[Tuple[str, PipelineDefinition]]:
+        if self.scope_name:
+            scopes = [self.project.scopes_by_name[self.scope_name]]
+        else:
+            scopes = self.project.scopes_by_name.values()
+
+        for scope in scopes:
+            for pipeline in scope.pipelines_by_name.values():
+                yield scope.name, pipeline
```

### Comparing `nodestream-0.4.0/nodestream/cli/operations/initialize_logger.py` & `nodestream-0.5.0/nodestream/cli/operations/initialize_logger.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/print_project_schema.py` & `nodestream-0.5.0/nodestream/cli/operations/print_project_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Optional
 
 from ...project import Project
-from ...schema.printers import SCHEMA_PRINTER_SUBCLASS_REGISTRY
+from ...schema.printers import SCHEMA_PRINTER_SUBCLASS_REGISTRY, SchemaPrinter
 from ..commands.nodestream_command import NodestreamCommand
 from .operation import Operation
 
 
 class PrintProjectSchema(Operation):
     def __init__(
         self,
@@ -21,13 +21,15 @@
         self.type_overrides_file = type_overrides_file
 
     async def perform(self, command: NodestreamCommand):
         type_overrides_file = (
             Path(self.type_overrides_file) if self.type_overrides_file else None
         )
         schema = self.project.get_schema(type_overrides_file=type_overrides_file)
+        # Import all schema printers so that they can register themselves
+        SchemaPrinter.import_all()
         printer_cls = SCHEMA_PRINTER_SUBCLASS_REGISTRY.get(self.format_string)
         printer = printer_cls()
         if self.output_file:
             printer.print_schema_to_file(schema, Path(self.output_file))
         else:
             printer.print_schema_to_stdout(schema, print_fn=command.write)
```

### Comparing `nodestream-0.4.0/nodestream/cli/operations/remove_pipeline_from_project.py` & `nodestream-0.5.0/nodestream/cli/operations/remove_pipeline_from_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/run_audit.py` & `nodestream-0.5.0/nodestream/cli/operations/run_audit.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/cli/operations/run_pipeline.py` & `nodestream-0.5.0/nodestream/cli/operations/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/debounced_ingest_strategy.py` & `nodestream-0.5.0/nodestream/databases/debounced_ingest_strategy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/ingest_strategy.py` & `nodestream-0.5.0/nodestream/databases/ingest_strategy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/neo4j/index_query_builder.py` & `nodestream-0.5.0/nodestream/databases/neo4j/index_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/neo4j/ingest_query_builder.py` & `nodestream-0.5.0/nodestream/databases/neo4j/ingest_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/neo4j/query.py` & `nodestream-0.5.0/nodestream/databases/neo4j/query.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/neo4j/query_executor.py` & `nodestream-0.5.0/nodestream/databases/neo4j/query_executor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/operation_debouncer.py` & `nodestream-0.5.0/nodestream/databases/operation_debouncer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/query_executor.py` & `nodestream-0.5.0/nodestream/databases/query_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     MatchStrategy,
     Node,
     NodeIdentityShape,
     RelationshipIdentityShape,
     RelationshipWithNodes,
     TimeToLiveConfiguration,
 )
+from ..pluggable import Pluggable
 from ..schema.indexes import FieldIndex, KeyIndex
 from ..subclass_registry import SubclassRegistry
 
 QUERY_EXECUTOR_SUBCLASS_REGISTRY = SubclassRegistry()
 
 
 @dataclass(slots=True, frozen=True)
@@ -27,15 +28,17 @@
 class OperationOnRelationshipIdentity:
     from_node: OperationOnNodeIdentity
     to_node: OperationOnNodeIdentity
     relationship_identity: RelationshipIdentityShape
 
 
 @QUERY_EXECUTOR_SUBCLASS_REGISTRY.connect_baseclass
-class QueryExecutor(ABC):
+class QueryExecutor(ABC, Pluggable):
+    entrypoint_name = "databases"
+
     @classmethod
     def from_database_args(cls, database: str = "neo4j", **database_args):
         return QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database).from_file_data(
             **database_args
         )
 
     @classmethod
```

### Comparing `nodestream-0.4.0/nodestream/databases/query_executor_with_statistics.py` & `nodestream-0.5.0/nodestream/databases/query_executor_with_statistics.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/databases/writer.py` & `nodestream-0.5.0/nodestream/databases/writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import Optional
 
 from ..pipeline import Flush, Writer
 from .debounced_ingest_strategy import DebouncedIngestStrategy
 from .ingest_strategy import INGESTION_STRATEGY_REGISTRY, IngestionStrategy
-from .query_executor import QUERY_EXECUTOR_SUBCLASS_REGISTRY
+from .query_executor import QUERY_EXECUTOR_SUBCLASS_REGISTRY, QueryExecutor
 from .query_executor_with_statistics import QueryExecutorWithStatistics
 
 
 class GraphDatabaseWriter(Writer):
     @classmethod
     def from_file_data(
         cls,
         batch_size: int,
         database: str,
         ingest_strategy_name: Optional[str] = None,
         collect_stats: bool = True,
         **database_args
     ):
+        # Import all query executors so that they can register themselves
+        QueryExecutor.import_all()
+
         executor_class = QUERY_EXECUTOR_SUBCLASS_REGISTRY.get(database)
         executor = executor_class.from_file_data(**database_args)
         if collect_stats:
             executor = QueryExecutorWithStatistics(executor)
 
         ingest_strategy_name = (
             ingest_strategy_name
```

### Comparing `nodestream-0.4.0/nodestream/file_io.py` & `nodestream-0.5.0/nodestream/file_io.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/__init__.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/extract_variables_interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/extract_variables_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/interpretation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from abc import ABC, abstractmethod
 
 from ...pipeline.value_providers import ProviderContext
+from ...pluggable import Pluggable
 from ...schema.schema import IntrospectiveIngestionComponent
 from ...subclass_registry import SubclassRegistry
 
 INTERPRETATION_REGISTRY = SubclassRegistry()
 
 
 @INTERPRETATION_REGISTRY.connect_baseclass
-class Interpretation(IntrospectiveIngestionComponent, ABC):
+class Interpretation(IntrospectiveIngestionComponent, Pluggable, ABC):
+    entrypoint_name = "interpretations"
+
     @abstractmethod
     def interpret(self, context: ProviderContext):
         raise NotImplementedError
 
     @classmethod
     def from_file_data(cls, **arguments) -> "Interpretation":
         name = arguments.pop("type")
```

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/properties_interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/properties_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/relationship_interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/relationship_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/source_node_interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/source_node_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpretations/switch_interpretation.py` & `nodestream-0.5.0/nodestream/interpreting/interpretations/switch_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/interpreting/interpreter.py` & `nodestream-0.5.0/nodestream/interpreting/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
         "before_iteration",
         "interpretations",
         "decomposer",
     )
 
     @classmethod
     def from_file_data(cls, interpretations, before_iteration=None, iterate_on=None):
+        # Import all interpretation plugins before we try to load any interpretations.
+        Interpretation.import_all()
+
         return cls(
             before_iteration=InterpretationPass.from_file_data(before_iteration),
             interpretations=InterpretationPass.from_file_data(interpretations),
             decomposer=RecordDecomposer.from_iteration_arguments(iterate_on),
         )
 
     def __init__(
```

### Comparing `nodestream-0.4.0/nodestream/interpreting/record_decomposers.py` & `nodestream-0.5.0/nodestream/interpreting/record_decomposers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/model/__init__.py` & `nodestream-0.5.0/nodestream/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/model/desired_ingestion.py` & `nodestream-0.5.0/nodestream/model/desired_ingestion.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/model/graph_objects.py` & `nodestream-0.5.0/nodestream/model/graph_objects.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/model/ingestion_hooks.py` & `nodestream-0.5.0/nodestream/model/ingestion_hooks.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/model/ttl.py` & `nodestream-0.5.0/nodestream/model/ttl.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/__init__.py` & `nodestream-0.5.0/nodestream/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py` & `nodestream-0.5.0/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/argument_resolvers/include_file_resolver.py` & `nodestream-0.5.0/nodestream/pipeline/argument_resolvers/include_file_resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,10 +13,10 @@
         loader.add_constructor(
             "!include",
             lambda loader, node: cls.include_file(loader.construct_scalar(node)),
         )
 
     @staticmethod
     def resolve_argument(file_path: str):
-        from ..pipeline.pipeline_file_loader import PipelineFileSafeLoader
+        from ..pipeline_file_loader import PipelineFileSafeLoader
 
         return PipelineFileSafeLoader.load_file_by_path(file_path)
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/class_loader.py` & `nodestream-0.5.0/nodestream/pipeline/class_loader.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/extractor.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/files.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from csv import DictReader
 from glob import glob
 from io import StringIO
 from pathlib import Path
 from typing import Any, AsyncGenerator, Iterable, Union
 
 from ...model import JsonLikeDocument
+from ...pluggable import Pluggable
 from ...subclass_registry import SubclassRegistry
 from .extractor import Extractor
 
 SUPPORTED_FILE_FORMAT_REGISTRY = SubclassRegistry()
 
 
 @SUPPORTED_FILE_FORMAT_REGISTRY.connect_baseclass
-class SupportedFileFormat(ABC):
+class SupportedFileFormat(Pluggable, ABC):
     def __init__(self, file: Union[Path, StringIO]) -> None:
         self.file = file
 
     @contextmanager
     def read_handle(self) -> StringIO:
         if isinstance(self.file, Path):
             with open(self.file, "r") as fp:
@@ -28,21 +29,25 @@
             yield self.file
 
     def read_file(self) -> Iterable[JsonLikeDocument]:
         with self.read_handle() as fp:
             return self.read_file_from_handle(fp)
 
     @classmethod
+    @contextmanager
     def open(cls, file: Path) -> "SupportedFileFormat":
-        return cls.from_file_pointer_and_format(file, file.suffix)
+        with open(file, "r") as fp:
+            yield cls.from_file_pointer_and_format(fp, file.suffix)
 
     @classmethod
     def from_file_pointer_and_format(
         cls, fp: StringIO, file_format: str
     ) -> "SupportedFileFormat":
+        # Import all file formats so that they can register themselves
+        cls.import_all()
         file_format = SUPPORTED_FILE_FORMAT_REGISTRY.get(file_format)
         return file_format(fp)
 
     @abstractmethod
     def read_file_from_handle(self, fp: StringIO) -> Iterable[JsonLikeDocument]:
         ...
 
@@ -50,20 +55,20 @@
 class JsonFileFormat(SupportedFileFormat, alias=".json"):
     def read_file_from_handle(self, fp: StringIO) -> Iterable[JsonLikeDocument]:
         return [json.load(fp)]
 
 
 class TextFileFormat(SupportedFileFormat, alias=".txt"):
     def read_file_from_handle(self, fp: StringIO) -> Iterable[JsonLikeDocument]:
-        return [{"line": line} for line in fp.readlines()]
+        return ({"line": line} for line in fp)
 
 
 class CommaSeperatedValuesFileFormat(SupportedFileFormat, alias=".csv"):
     def read_file_from_handle(self, fp: StringIO) -> Iterable[JsonLikeDocument]:
-        return tuple(DictReader(fp))
+        return DictReader(fp)
 
 
 class FileExtractor(Extractor):
     @classmethod
     def from_file_data(cls, globs: Iterable[str]):
         all_matching_paths = (
             Path(file)
@@ -74,9 +79,10 @@
         return cls(final_paths)
 
     def __init__(self, paths: Iterable[Path]) -> None:
         self.paths = paths
 
     async def extract_records(self) -> AsyncGenerator[Any, Any]:
         for path in self.paths:
-            for record in SupportedFileFormat.open(path).read_file():
-                yield record
+            with SupportedFileFormat.open(path) as file:
+                for record in file.read_file():
+                    yield record
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/iterable.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/iterable.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/athena_extractor.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/athena_extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/credential_utils.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/credential_utils.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/stores/aws/s3_extractor.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/stores/aws/s3_extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/streams/extractor.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/streams/extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import json
 from abc import ABC, abstractmethod
 from typing import Any, Iterable
 
 from ....model import JsonLikeDocument
+from ....pluggable import Pluggable
 from ....subclass_registry import SubclassRegistry
 from ...flush import Flush
 from ..extractor import Extractor
 
 STREAM_CONNECTOR_SUBCLASS_REGISTRY = SubclassRegistry()
 STREAM_OBJECT_FORMAT_SUBCLASS_REGISTRY = SubclassRegistry()
 
 DEFAULT_TIMEOUT = 60
 DEFAULT_MAX_RECORDS = 100
 
 
 @STREAM_CONNECTOR_SUBCLASS_REGISTRY.connect_baseclass
-class StreamConnector(ABC):
+class StreamConnector(Pluggable, ABC):
+    entrypoint_name = "stream_connectors"
+
     @abstractmethod
     async def connect(self):
         raise NotImplementedError
 
     @abstractmethod
     async def disconnect(self):
         raise NotImplementedError
 
     @abstractmethod
     async def poll(self, timeout: int, max_records: int) -> Iterable[Any]:
         raise NotImplementedError
 
 
 @STREAM_OBJECT_FORMAT_SUBCLASS_REGISTRY.connect_baseclass
-class StreamRecordFormat(ABC):
+class StreamRecordFormat(Pluggable, ABC):
+    entrypoint_name = "record_formats"
+
     @abstractmethod
     def parse(self, record: Any) -> JsonLikeDocument:
         raise NotImplementedError
 
 
 class JsonStreamRecordFormat(StreamRecordFormat, alias="json"):
     def parse(self, record: Any) -> JsonLikeDocument:
@@ -53,14 +58,18 @@
         cls,
         connector: str,
         record_format: str,
         timeout: int = DEFAULT_TIMEOUT,
         max_records: int = DEFAULT_MAX_RECORDS,
         **connector_args
     ):
+        # Import all plugins so that they can register themselves
+        StreamRecordFormat.import_all()
+        StreamConnector.import_all()
+
         object_format_cls = STREAM_OBJECT_FORMAT_SUBCLASS_REGISTRY.get(record_format)
         connector_cls = STREAM_CONNECTOR_SUBCLASS_REGISTRY.get(connector)
         return cls(
             timeout=timeout,
             max_records=max_records,
             record_format=object_format_cls(),
             connector=connector_cls(**connector_args),
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/streams/kafka.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/streams/kafka.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/extractors/ttls.py` & `nodestream-0.5.0/nodestream/pipeline/extractors/ttls.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/filters.py` & `nodestream-0.5.0/nodestream/pipeline/filters.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/meta.py` & `nodestream-0.5.0/nodestream/pipeline/meta.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/normalizers/normalizer.py` & `nodestream-0.5.0/nodestream/pipeline/normalizers/normalizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from functools import cache
 from typing import Any
 
+from ...pluggable import Pluggable
 from ...subclass_registry import MissingFromRegistryError, SubclassRegistry
 
 NORMALIZER_REGISTRY = SubclassRegistry()
 
 
 class InvalidFlagError(ValueError):
     """Raised when a normalization flag is not valid."""
@@ -13,22 +14,28 @@
     def __init__(self, flag_name, *args: object) -> None:
         super().__init__(
             f"Normalization flag with name '{flag_name}' is not valid.`", *args
         )
 
 
 @NORMALIZER_REGISTRY.connect_baseclass
-class Normalizer(ABC):
+class Normalizer(Pluggable, ABC):
     """A `Normalizer` is responsible for turning objects into a consistent form.
 
     When data is extracted from pipeline records from a value provider, the `Normalizer`
     is responsible for "cleaning up" the raw data such that is consistent. Often this comes
     in with regard to strings.
     """
 
+    entrypoint_name = "normalizers"
+
+    @classmethod
+    def setup(cls):
+        pass
+
     @classmethod
     def normalize_by_args(cls, value: Any, **normalizer_args) -> Any:
         for flag_name, enabled in normalizer_args.items():
             if enabled:
                 value = cls.by_flag_name(flag_name).normalize_value(value)
 
         return value
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/pipeline.py` & `nodestream-0.5.0/nodestream/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/pipeline_file_loader.py` & `nodestream-0.5.0/nodestream/pipeline/pipeline_file_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 from yaml import SafeLoader, load
 
-from .argument_resolvers import ARGUMENT_RESOLVER_REGISTRY
+from .argument_resolvers import ArgumentResolver
 from .class_loader import ClassLoader
+from .normalizers import Normalizer
 from .pipeline import Pipeline
-from .value_providers import VALUE_PROVIDER_REGISTRY
+from .value_providers import ValueProvider
 
 
 class InvalidPipelineDefinitionError(ValueError):
     """Raised when a pipeline definition is invalid."""
 
     pass
 
@@ -22,17 +23,19 @@
     was_configured = False
 
     @classmethod
     def configure(cls):
         if cls.was_configured:
             return
 
-        for value_provider in VALUE_PROVIDER_REGISTRY.all_subclasses:
+        for normalizer in Normalizer.all():
+            normalizer.setup()
+        for value_provider in ValueProvider.all():
             value_provider.install_yaml_tag(cls)
-        for argument_resolver in ARGUMENT_RESOLVER_REGISTRY.all_subclasses:
+        for argument_resolver in ArgumentResolver.all():
             argument_resolver.install_yaml_tag(cls)
 
         cls.was_configured = True
 
     @classmethod
     def load_file_by_path(cls, file_path: str):
         PipelineFileSafeLoader.configure()
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/step.py` & `nodestream-0.5.0/nodestream/pipeline/step.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/transformers/expand_json_field.py` & `nodestream-0.5.0/nodestream/pipeline/transformers/expand_json_field.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/transformers/transformer.py` & `nodestream-0.5.0/nodestream/pipeline/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/__init__.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/context.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/context.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/jmespath_value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/jmespath_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/jq_value_provder.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/jq_value_provder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/mapping_value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/mapping_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/static_value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/static_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/string_format_value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/string_format_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/value_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Iterable, Type, Union
 
 from yaml import SafeLoader
 
+from ...pluggable import Pluggable
 from ...subclass_registry import SubclassRegistry
 from ..normalizers import Normalizer
 from .context import ProviderContext
 
 StaticValueOrValueProvider = Union[Any, "ValueProvider"]
 
 
 VALUE_PROVIDER_REGISTRY = SubclassRegistry()
 
 
 @VALUE_PROVIDER_REGISTRY.connect_baseclass
-class ValueProvider(ABC):
+class ValueProvider(Pluggable, ABC):
     """A `ValueProvider` is a class that can extract values from a document."""
 
+    entrypoint_name = "value_providers"
+
     @classmethod
     def guarantee_value_provider(
         cls, maybe_provider: StaticValueOrValueProvider
     ) -> "ValueProvider":
         from .static_value_provider import StaticValueProvider
 
         return (
```

### Comparing `nodestream-0.4.0/nodestream/pipeline/value_providers/variable_value_provider.py` & `nodestream-0.5.0/nodestream/pipeline/value_providers/variable_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/pipeline/writers.py` & `nodestream-0.5.0/nodestream/pipeline/writers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/project/audits/audit_referencial_integrity.py` & `nodestream-0.5.0/nodestream/project/audits/audit_referencial_integrity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from ...interpreting import Interpreter
 from ...schema.indexes import KeyIndex
 from ..project import Project
 from .audit import Audit
 
 
 class AuditReferentialIntegrity(Audit):
+    name = "refs"
+    description = "Audit the correctness of references between nodes of the project"
+
     async def run(self, project: Project):
         all_interpreters = project.dig_for_step_of_type(Interpreter)
         node_types_so_far = {}
 
         for definition, step_index, interpreter in all_interpreters:
             for index in interpreter.gather_used_indexes():
                 if not isinstance(index, KeyIndex):
```

### Comparing `nodestream-0.4.0/nodestream/project/audits/audit_ttls.py` & `nodestream-0.5.0/nodestream/project/audits/audit_ttls.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 from ...model import TimeToLiveConfiguration
 from ...pipeline.extractors.ttls import TimeToLiveConfigurationExtractor
 from ..project import Project
 from .audit import Audit
 
 
-class TTLAudit(Audit):
+class AuditTimeToLiveConfigurations(Audit):
+    name = "ttls"
+    description = "Audit the project for missing TTLs"
+
     async def get_all_ttl_configurations(
         self, project: Project
     ) -> List[TimeToLiveConfiguration]:
         ttl_extractors = project.dig_for_step_of_type(TimeToLiveConfigurationExtractor)
         return [
             ttl
             for _, _, extractor in ttl_extractors
```

### Comparing `nodestream-0.4.0/nodestream/schema/indexes.py` & `nodestream-0.5.0/nodestream/schema/indexes.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/schema/printers/graphql_schema_printer.py` & `nodestream-0.5.0/nodestream/schema/printers/graphql_schema_printer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/schema/printers/schema_printer.py` & `nodestream-0.5.0/nodestream/schema/printers/schema_printer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from pathlib import Path
 
+from ...pluggable import Pluggable
 from ...subclass_registry import SubclassRegistry
 from ..schema import GraphSchema
 
 SCHEMA_PRINTER_SUBCLASS_REGISTRY = SubclassRegistry()
 
 
 @SCHEMA_PRINTER_SUBCLASS_REGISTRY.connect_baseclass
-class SchemaPrinter:
+class SchemaPrinter(Pluggable):
+    entrypoint_name = "schema_printers"
+
     def print_schema_to_file(self, schema: GraphSchema, file_path: Path):
         with open(file_path, "w") as f:
             f.write(self.print_schema_to_string(schema))
 
     def print_schema_to_stdout(self, schema: GraphSchema, print_fn=print):
         print_fn(self.print_schema_to_string(schema))
```

### Comparing `nodestream-0.4.0/nodestream/schema/schema.py` & `nodestream-0.5.0/nodestream/schema/schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/nodestream/subclass_registry.py` & `nodestream-0.5.0/nodestream/subclass_registry.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.4.0/pyproject.toml` & `nodestream-0.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nodestream"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Fast, Declarative ETL for Graph Databases."
 license = "GPL-3.0-only"
 authors = [
     "Zach Probst <Zach_Probst@intuit.com>"
 ]
 readme = "README.md"
 
@@ -37,14 +37,15 @@
 python-json-logger = "^2.0.4"
 cymple = "0.8.1"
 boto3 = "^1.26.137"
 aiokafka = "^0.8.0"
 Jinja2 = "^3"
 pandas = "^2"
 schema = "^0.7.5"
+cookiecutter = "^2.1.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.8"
 mkdocs-gen-files = "^0.5.0"
 mkdocstrings = {version = "^0.22.0", extras = ["python"]}
 
@@ -68,11 +69,26 @@
 [tool.pytest.ini_options]
 markers = [
     "integration: marks the test as an integration test (deselect with '-m \"not integration\"')",
     "e2e: marks the test as an end-to-end test (deselect with '-m \"not e2e\"')",
 ]
 
 [tool.poetry.scripts]
-nodestream = 'nodestream.cli:run'
+nodestream = 'nodestream.cli.application:run'
+
+# To prevent the "builin" stuff being a special case of plugins,
+# nodestream just considers itself a plugin for all of the things that are pluggable.
+[tool.poetry.plugins."nodestream.plugins"]
+"argument_resolvers" = "nodestream.pipeline.argument_resolvers"
+"file_formats" = "nodestream.pipeline.extractor.files"
+"interpretations" = "nodestream.interpreting.interpretations"
+"normalizers" = "nodestream.pipeline.normalizers"
+"value_providers" = "nodestream.pipeline.value_providers"   
+"record_formats" = "nodestream.extractors.streams"
+"stream_connectors" = "nodestream.extractors.streams"
+"commands" = "nodestream.cli.commands"                      
+"audits" = "nodestream.project.audits"                      
+"schema_printers" = "nodestream.schema.printers"
+"databases" = "nodestream.databases.neo4j"
 
 [tool.ruff]
 ignore = ["E501"]
```

### Comparing `nodestream-0.4.0/PKG-INFO` & `nodestream-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodestream
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Fast, Declarative ETL for Graph Databases.
 Home-page: https://github.com/nodestream-proj/nodestream
 License: GPL-3.0-only
 Keywords: etl,neo4j,declarative,data,kafka,ingest
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Dist: Jinja2 (>=3,<4)
 Requires-Dist: aiokafka (>=0.8.0,<0.9.0)
 Requires-Dist: boto3 (>=1.26.137,<2.0.0)
 Requires-Dist: cleo (>=2.0.1,<3.0.0)
+Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: cymple (==0.8.1)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jq (>=1.4.1,<2.0.0)
 Requires-Dist: neo4j (>=5.8.0,<6.0.0)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

