# Comparing `tmp/forestadmin_datasource_toolkit-1.0.0b2.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b2.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b3.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-1.0.0b2.tar` & `forestadmin_datasource_toolkit-1.0.0b3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/README.md
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     2276 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      678 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      658 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     6971 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0     4741 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
--rw-r--r--   0        0        0     1608 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
--rw-r--r--   0        0        0     1536 2023-07-26 13:23:14.557402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     5188 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     2039 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      664 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      907 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     2167 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    14435 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/__init__.py
--rw-r--r--   0        0        0     1941 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
--rw-r--r--   0        0        0     2133 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
--rw-r--r--   0        0        0     1549 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
--rw-r--r--   0        0        0     3484 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
--rw-r--r--   0        0        0      557 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/types.py
--rw-r--r--   0        0        0     4906 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/collection_decorator.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      154 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     3886 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      651 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2812 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0      902 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
--rw-r--r--   0        0        0     4074 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/decorator_stack.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/__init__.py
--rw-r--r--   0        0        0     4495 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/collection.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
--rw-r--r--   0        0        0     6398 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
--rw-r--r--   0        0        0      320 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
--rw-r--r--   0        0        0     3855 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
--rw-r--r--   0        0        0     3015 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
--rw-r--r--   0        0        0     9761 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/__init__.py
--rw-r--r--   0        0        0      671 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/collection.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2651 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/__init__.py
--rw-r--r--   0        0        0     4142 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/collection.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
--rw-r--r--   0        0        0     5102 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
--rw-r--r--   0        0        0     4845 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
--rw-r--r--   0        0        0     1020 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
--rw-r--r--   0        0        0      258 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
--rw-r--r--   0        0        0     1045 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
--rw-r--r--   0        0        0     6327 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
--rw-r--r--   0        0        0      281 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0      954 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/chart.py
--rw-r--r--   0        0        0     2534 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5323 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1420 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7775 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4506 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5377 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2572 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4647 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9798 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3941 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1688 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7660 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     6832 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2877 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3213 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      875 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4511 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      902 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2619 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      595 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0       73 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     7235 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     1169 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1658 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0        0 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4788 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     3581 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4536 2023-07-26 13:23:14.561402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4352 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2023-07-26 13:23:14.565402 forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1758 2023-07-26 13:23:41.857538 forestadmin_datasource_toolkit-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.193229 forestadmin_datasource_toolkit-1.0.0b3/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.193229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-27 12:27:46.193229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     7105 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0     4741 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     1608 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0     1536 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5369 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2127 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      664 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      907 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     2167 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    14435 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     1941 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2133 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1549 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     3484 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      557 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     4972 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3886 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      651 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2812 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0      902 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     4074 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
+-rw-r--r--   0        0        0     6398 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
+-rw-r--r--   0        0        0      320 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
+-rw-r--r--   0        0        0     3015 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0     9761 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2651 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4142 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     5102 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0     1045 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6327 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0      281 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0      954 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2591 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5323 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1420 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7775 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4506 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5377 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2572 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4647 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9798 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2023-07-27 12:27:46.197229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1688 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7660 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2877 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3213 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      875 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4511 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2619 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0       73 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     7235 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     1169 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1658 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4788 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     3581 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4536 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4352 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2023-07-27 12:27:46.201229 forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1758 2023-07-27 12:28:10.717546 forestadmin_datasource_toolkit-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b3/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.datasources import DatasourceException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
 from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.models.collections import Datasource
@@ -68,54 +68,54 @@
     @property
     def schema(self):
         return self.collection.schema
 
     async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         return await self.collection.create(caller, data)
 
-    def _build_filter(self, filter: Optional[Union[Filter, PlainFilter]]) -> Optional[Filter]:
-        if not filter:
+    def _build_filter(self, filter_: Optional[Union[Filter, PlainFilter]]) -> Optional[Filter]:
+        if not filter_:
             return None
-        elif is_filter(filter):
-            return filter
+        elif is_filter(filter_):
+            return filter_
         else:
-            plain_filter = cast(PlainFilter, filter)
+            plain_filter = cast(PlainFilter, filter_)
             condition_tree = None
             if plain_filter.get("condition_tree"):
                 condition_tree = ConditionTreeFactory.from_plain_object(plain_filter.get("condition_tree"))
             component = cast(
                 FilterComponent,
                 {
                     **plain_filter,
                     "condition_tree": condition_tree,
                 },
             )
             return Filter(component)
 
-    def _build_paginated_filter(self, filter: Union[PaginatedFilter, PlainPaginatedFilter]):
-        if is_paginated_filter(filter):
-            return filter
+    def _build_paginated_filter(self, filter_: Union[PaginatedFilter, PlainPaginatedFilter]):
+        if is_paginated_filter(filter_):
+            return filter_
 
-        filter = cast(PlainPaginatedFilter, filter)
+        filter_ = cast(PlainPaginatedFilter, filter_)
         filter_component: PaginatedFilterComponent = {
-            "search": filter.get("search"),
-            "search_extended": filter.get("search_extended", False),
-            "segment": filter.get("segment"),
-            "timezone": filter.get("timezone"),  # type: ignore
+            "search": filter_.get("search"),
+            "search_extended": filter_.get("search_extended", False),
+            "segment": filter_.get("segment"),
+            "timezone": filter_.get("timezone"),  # type: ignore
         }
 
-        if filter.get("condition_tree"):
-            filter_component["condition_tree"] = ConditionTreeFactory.from_plain_object(filter.get("condition_tree"))
+        if filter_.get("condition_tree"):
+            filter_component["condition_tree"] = ConditionTreeFactory.from_plain_object(filter_.get("condition_tree"))
 
-        if filter.get("sort"):
-            sort_clauses = cast(List[PlainSortClause], filter.get("sort"))
+        if filter_.get("sort"):
+            sort_clauses = cast(List[PlainSortClause], filter_.get("sort"))
             filter_component["sort"] = Sort(sort_clauses)
 
-        if filter.get("page"):
-            plain_page = cast(PlainPage, filter.get("page"))
+        if filter_.get("page"):
+            plain_page = cast(PlainPage, filter_.get("page"))
             filter_component["page"] = Page(plain_page["skip"], plain_page["limit"])
 
         return PaginatedFilter(PaginatedFilterComponent(**filter_component))
 
     def _build_projection(self, projection: Union[Projection, List[str]]) -> Projection:
         if is_projection(projection):
             return projection
@@ -124,44 +124,51 @@
     def _build_aggregation(self, aggregation: Union[Aggregation, PlainAggregation]) -> Aggregation:
         if is_aggregation(aggregation):
             return aggregation
         aggregation = cast(PlainAggregation, aggregation)
         return Aggregation(aggregation)
 
     async def list(
-        self, caller: User, filter: Union[PaginatedFilter, PlainPaginatedFilter], projection: Projection
+        self, caller: User, filter_: Union[PaginatedFilter, PlainPaginatedFilter], projection: Projection
     ) -> List[RecordsDataAlias]:
-        filter_instance = self._build_paginated_filter(filter)
+        filter_instance = self._build_paginated_filter(filter_)
         projection_instance = self._build_projection(projection)
 
         return await self.collection.list(caller, filter_instance, projection_instance)
 
-    async def update(self, caller: User, filter: Optional[Union[Filter, PlainFilter]], patch: RecordsDataAlias) -> None:
-        filter_instance = self._build_filter(filter)
+    async def update(
+        self, caller: User, filter_: Optional[Union[Filter, PlainFilter]], patch: RecordsDataAlias
+    ) -> None:
+        filter_instance = self._build_filter(filter_)
         return await self.collection.update(caller, filter_instance, patch)
 
     async def delete(self, caller: User, filter: Optional[Union[Filter, PlainFilter]]) -> None:
         filter_instance = self._build_filter(filter)
         return await self.collection.delete(caller, filter_instance)
 
     async def aggregate(
-        self, caller: User, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+        self, caller: User, filter_: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
     ) -> List[AggregateResult]:
-        filter_instance = self._build_filter(filter)
+        filter_instance = self._build_filter(filter_)
         aggregation_instance = self._build_aggregation(aggregation)
 
         return await self.collection.aggregate(caller, filter_instance, aggregation_instance, limit)
 
     async def execute(
-        self, caller: User, name: str, data: RecordsDataAlias, filter: Optional[Union[Filter, PlainFilter]]
+        self, caller: User, name: str, data: RecordsDataAlias, filter_: Optional[Union[Filter, PlainFilter]]
     ) -> ActionResult:
-        filter_instance = self._build_filter(filter)
+        filter_instance = self._build_filter(filter_)
         return await self.collection.execute(caller, name, data, filter_instance)
 
     async def get_form(
-        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
+        self,
+        caller: User,
+        name: str,
+        data: Optional[RecordsDataAlias],
+        filter_: Optional[Filter],
+        meta: Optional[Dict[str, Any]],
     ) -> List[ActionField]:
-        filter_instance = self._build_filter(filter)
-        return await super().get_form(caller, name, data, filter_instance)
+        filter_instance = self._build_filter(filter_)
+        return await super().get_form(caller, name, data, filter_instance, meta)
 
     async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
         return await super().render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,33 +36,38 @@
         data: RecordsDataAlias,
         filter_: Optional[Filter] = None,
     ) -> ActionResult:
         action = self._actions.get(name)
         if not action:
             return await super().execute(caller, name, data, filter_)  # type: ignore
 
-        context = self._get_context(caller, action, data, filter_)
+        context = self._get_context(caller, action, data, filter_, None)
         response_builder = ResultBuilder()
         result = action.execute(context, response_builder)  # type: ignore
         if isinstance(result, Awaitable):
             result = await result
         return result or {"type": "Success", "invalidated": set(), "format": "text", "message": "Success"}
 
     async def get_form(
-        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter_: Optional[Filter] = None
+        self,
+        caller: User,
+        name: str,
+        data: Optional[RecordsDataAlias],
+        filter_: Optional[Filter] = None,
+        meta: Optional[Dict[str, Any]] = dict(),
     ) -> List[ActionField]:
         action = self._actions.get(name)
         if not action:
-            return await super().get_form(caller, name, data, filter_)  # type: ignore
+            return await super().get_form(caller, name, data, filter_, meta)  # type: ignore
         elif not action.form:
             return []
 
         form_values = data or {}
         used: Set[str] = set()
-        context = self._get_context(caller, action, form_values, filter_, used)
+        context = self._get_context(caller, action, form_values, filter_, used, meta.get("changed_field"))
         form_fields: List[DynamicField[ActionContext]] = cast(
             List[DynamicField[ActionContext]], [field for field in action.form]
         )
 
         form_values = await self._build_form_values(context, form_fields, form_values)
         action_fields = await self._build_fields(context, form_fields, form_values)
         for field in action_fields:
@@ -83,21 +88,22 @@
     def _get_context(
         self,
         caller: User,
         action: Union[ActionSingle, ActionBulk, ActionGlobal],
         form_values: RecordsDataAlias,
         filter_: Optional[Filter] = None,
         used: Optional[Set[str]] = None,
+        changed_field: Optional[str] = None,
     ) -> ActionContext:
         return {
             ActionSingle.SCOPE: ActionContextSingle,
             ActionBulk.SCOPE: ActionContextBulk,
             ActionGlobal.SCOPE: ActionContext,
         }[action.SCOPE](
-            cast(Collection, self), caller, form_values, filter_, used  # type: ignore
+            cast(Collection, self), caller, form_values, filter_, used, changed_field  # type: ignore
         )
 
     async def _build_form_values(
         self, context: ActionContext, fields: List[DynamicField[ActionContext]], data: Optional[Dict[str, Any]]
     ):
         if data is None:
             form_values: Dict[str, Any] = {}
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,18 +32,20 @@
     def __init__(
         self,
         collection: Collection,
         caller: User,
         form_value: RecordsDataAlias,
         filter: Filter,
         used: Optional[Set[str]] = set(),
+        changed_field: Optional[str] = None,
     ):
         super(ActionContext, self).__init__(collection, caller)
         self.form_values = FormValueObserver(**form_value)
         self.filter = filter
+        self.changed_field = changed_field
 
     async def get_records(self, fields: Projection) -> List[RecordsDataAlias]:
         ProjectionValidator.validate(self.collection, fields)
         projection = Projection(*fields)
         return await self._run_query(projection)
 
     async def _run_query(self, projection: Projection) -> List[RecordsDataAlias]:
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/chart/types.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/chart/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import CollectionException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
 from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.collections import Collection
 from forestadmin.datasource_toolkit.interfaces.models.collections import BoundCollection, CollectionSchema, Datasource
@@ -96,13 +96,14 @@
 
     async def get_form(
         self,
         caller: User,
         name: str,
         data: Optional[RecordsDataAlias],
         _filter: Optional[Filter] = None,
+        meta: Optional[Dict[str, Any]] = dict(),
     ) -> List[ActionField]:
         refined_filter = cast(Optional[Filter], await self._refine_filter(caller, _filter))
-        return await self.child_collection.get_form(caller, name, data, refined_filter)
+        return await self.child_collection.get_form(caller, name, data, refined_filter, meta)
 
     async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
         return await self.child_collection.render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/decorator_stack.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/decorator_stack.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/empty/collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/empty/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/publication_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/publication_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/schema/collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/schema/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/validation/collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/validation/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/chart.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/chart.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.exceptions import ForestException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
 from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.models.collections import Collection as CollectionModel
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import AggregateResult, Aggregation
@@ -16,49 +16,50 @@
 class Collection(CollectionModel, abc.ABC):
     @abc.abstractmethod
     async def execute(
         self,
         caller: User,
         name: str,
         data: RecordsDataAlias,
-        filter: Optional[Filter],
+        filter_: Optional[Filter],
     ) -> ActionResult:
         """to execute an action"""
         raise ForestException(f"Action {name} is not implemented")
 
     @abc.abstractmethod
     async def get_form(
         self,
         caller: User,
         name: str,
         data: Optional[RecordsDataAlias],
-        filter: Optional[Filter],
+        filter_: Optional[Filter],
+        meta: Optional[Dict[str, Any]],
     ) -> List[ActionField]:
         """to get the form of an action"""
         return []
 
     @abc.abstractmethod
     async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
         """to render a chart"""
         raise ForestException(f"Chart {name} is not implemented")
 
     @abc.abstractmethod
     async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         """to create records"""
 
     @abc.abstractmethod
-    async def list(self, caller: User, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+    async def list(self, caller: User, filter_: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         """to list records"""
 
     @abc.abstractmethod
-    async def update(self, caller: User, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
+    async def update(self, caller: User, filter_: Optional[Filter], patch: RecordsDataAlias) -> None:
         """to update records"""
 
     @abc.abstractmethod
-    async def delete(self, caller: User, filter: Optional[Filter]) -> None:
+    async def delete(self, caller: User, filter_: Optional[Filter]) -> None:
         """to delete records"""
 
     @abc.abstractmethod
     async def aggregate(
-        self, caller: User, filter: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
+        self, caller: User, filter_: Optional[Filter], aggregation: Aggregation, limit: Optional[int] = None
     ) -> List[AggregateResult]:
         """to make aggregate request"""
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.0.0b3/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/pyproject.toml` & `forestadmin_datasource_toolkit-1.0.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
-version = "1.0.0-beta.2"
+version = "1.0.0-beta.3"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b2/PKG-INFO` & `forestadmin_datasource_toolkit-1.0.0b3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

