# Comparing `tmp/cumulus_library-0.4.0.dev1.tar.gz` & `tmp/cumulus_library-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.4.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.4.0.dev1.tar` & `cumulus_library-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,68 @@
-lrwxr-xr-x   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      587 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/README.md
--rw-r--r--   0        0        0      963 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       51 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11182 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli.py
--rw-r--r--   0        0        0     5249 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      272 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6030 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2549 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2688 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql
--rw-r--r--   0        0        0     3493 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0     4550 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.sql
--rw-r--r--   0        0        0     4176 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/denormalizer.py
--rw-r--r--   0        0        0     2857 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     1505 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     2001 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter_type.sql
--rw-r--r--   0        0        0     4330 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      782 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1231 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2874 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1222 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     6521 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql
--rw-r--r--   0        0        0     1426 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      824 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2023-07-06 16:36:22.124354 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2023-07-06 16:36:22.236356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      394 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4643 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16059 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py
--rw-r--r--   0        0        0     1430 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0      577 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1798 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     7462 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2664 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/upload.py
--rw-r--r--   0        0        0     1588 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 cumulus_library-0.4.0.dev1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      587 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/README.md
+-rw-r--r--   0        0        0     1359 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       45 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0     2875 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/base_table_builder.py
+-rwxr-xr-x   0        0        0    12441 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5504 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6030 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     1188 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_condition_codeableconcept.py
+-rw-r--r--   0        0        0     4538 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_core_medication.py
+-rw-r--r--   0        0        0     4171 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_core_medication.sql
+-rw-r--r--   0        0        0     5143 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_encounter_coding.py
+-rw-r--r--   0        0        0     9897 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_encounter_coding.sql
+-rw-r--r--   0        0        0     1368 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/builder_patient_extension.py
+-rw-r--r--   0        0        0     2876 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2711 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/condition_codeable_concept.sql
+-rw-r--r--   0        0        0     3612 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0     4481 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/count_core.sql
+-rw-r--r--   0        0        0     2863 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     1505 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     1281 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/encounter_type.sql
+-rw-r--r--   0        0        0     4330 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      915 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1213 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1225 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     6521 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/patient_extensions.sql
+-rw-r--r--   0        0        0     1426 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1481 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1416 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-07-27 19:05:18.566308 cumulus_library-1.0.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2023-07-27 19:05:18.602309 cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2023-07-27 19:05:18.698309 cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      394 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      145 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     3346 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    17320 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0     1692 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0      176 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/column_datatype.sql.jinja
+-rw-r--r--   0        0        0     6119 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/core_medication.sql.jinja
+-rw-r--r--   0        0        0      577 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0      484 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/ctas_empty.sql.jinja
+-rw-r--r--   0        0        0       61 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1791 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0      439 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
+-rw-r--r--   0        0        0       52 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0    10606 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     3747 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/template_sql/utils.py
+-rw-r--r--   0        0        0     2664 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1459 2023-07-27 19:05:18.706309 cumulus_library-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 cumulus_library-1.0.0/PKG-INFO
```

### Comparing `cumulus_library-0.4.0.dev1/README.md` & `cumulus_library-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff` & `cumulus_library-1.0.0/cumulus_library/.sqlfluff`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 [sqlfluff]
 templater = jinja
 dialect = athena
 sql_file_exts = .sql,.sql.jinja
 # this rule overfires on athena nested arrays
-exclude_rules=references.from,structure.column_order
+exclude_rules=references.from,structure.column_order,aliasing.unused
 max_line_length = 88
 
 [sqlfluff:indentation]
 template_blocks_indent = false
 
 [sqlfluff:rules:layout.long_lines]
 ignore_comment_lines = true
 
 [sqlfluff:rules:capitalisation.keywords]
 capitalisation_policy = upper
 
 [sqlfluff:templater:jinja:context]
+code_systems = ["http://snomed.info/sct", "http://hl7.org/fhir/sid/icd-10-cm"]
+col_type_list = ["a string","b string"]
+cc_columns = [{"name": "baz", "is_array": True}, {"name": "foobar", "is_array": False}]
+cc_column = 'code'
+
+column_name = 'bar'
+conditions = ["1 > 0", "1 < 2"]
+dataset = [["foo","foo"],["bar","bar"]]
+ext_systems = ["omb", "text"]
+field = 'column_name'
+fhir_extension = fhir_extension
+id = 'id'
+medication_datasources = {"by_contained_ref" : True, "by_external_ref" : True}
+prefix = Test
 schema_name = test_schema
+source_table = source_table
+source_id = source_id
+table_cols = ["a","b"]
 table_name = test_table
+target_col_prefix = prefix
+target_table = target_table
+unnests = [{"source col": "g", "table_alias": "i", "row_alias":"j"}, {"source col": "k", "table_alias": "l", "row_alias":"m"},]
+view_cols = ["c","d"]
 view_name = test_view
 view_or_table_name = test_view_or_table
 view_or_table = TABLE
-prefix = Test
-dataset = [["foo","foo"],["bar","bar"]]
-table_cols = ["a","b"]
-view_cols = ["c","d"]
-col_type_list = ["a string","b string"]
-source_table = source_table
-source_id = source_id
-target_table = target_table
-target_col_prefix = prefix
-fhir_extension = fhir_extension
-ext_systems = ["omb", "text"]
-code_systems = ["http://snomed.info/sct", "http://hl7.org/fhir/sid/icd-10-cm"]
-cc_column = 'code'
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/cli.py` & `cumulus_library-1.0.0/cumulus_library/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from pathlib import Path, PosixPath
 from typing import Dict, List, Optional
 
 import pyathena
 
 from pyathena.pandas.cursor import PandasCursor
+from rich.console import Console
+from rich.table import Table
 
 from cumulus_library import __version__
 from cumulus_library.cli_parser import get_parser
 from cumulus_library.study_parser import StudyManifestParser
 from cumulus_library.upload import upload_files
 
 
@@ -108,17 +110,29 @@
     def clean_and_build_study(self, target: PosixPath) -> None:
         """Recreates study views/tables
 
         :param target: A PosixPath to the study directory
         """
         studyparser = StudyManifestParser(target)
         studyparser.clean_study(self.cursor, self.schema_name, self.verbose)
-        studyparser.run_python_builder(self.cursor, self.schema_name, self.verbose)
+        studyparser.run_table_builder(self.cursor, self.schema_name, self.verbose)
         studyparser.build_study(self.cursor, self.verbose)
 
+    def run_single_table_builder(
+        self, target: PosixPath, table_builder_name: str
+    ) -> None:
+        """Runs a single table builder
+
+        :param target: A PosixPath to the study directory
+        """
+        studyparser = StudyManifestParser(target)
+        studyparser.run_single_table_builder(
+            self.cursor, self.schema_name, table_builder_name, self.verbose
+        )
+
     def clean_and_build_all(self, study_dict: Dict) -> None:
         """Builds views for all studies.
 
         NOTE: By design, this method will always exclude the `template` study dir,
         since 99% of the time you don't need a live copy in the database.
 
         :param study_dict: A dict of PosixPaths
@@ -222,15 +236,15 @@
             args["workgroup"],
             args["profile"],
             args["schema_name"],
         )
         if args["verbose"]:
             builder.verbose = True
         print("Testing connection to athena...")
-        builder.cursor.execute("show tables")
+        builder.cursor.execute("SHOW DATABASES")
 
         if args["action"] == "clean":
             builder.clean_study(args["target"])
 
         else:
             study_dict = get_study_dict(args["study_dir"])
             if args["target"]:
@@ -244,15 +258,20 @@
                         )
 
             if args["action"] == "build":
                 if "all" in args["target"]:
                     builder.clean_and_build_all(study_dict)
                 else:
                     for target in args["target"]:
-                        builder.clean_and_build_study(study_dict[target])
+                        if args["table_builder"]:
+                            builder.run_single_table_builder(
+                                study_dict[target], args["table_builder"]
+                            )
+                        else:
+                            builder.clean_and_build_study(study_dict[target])
 
             elif args["action"] == "export":
                 if "all" in args["target"]:
                     builder.export_all(study_dict, args["data_path"])
                 else:
                     for target in args["target"]:
                         builder.export_study(study_dict[target], args["data_path"])
@@ -285,17 +304,31 @@
         ("region", "CUMULUS_LIBRARY_REGION"),
         ("study_dir", "CUMULUS_LIBRARY_STUDY_DIR"),
         ("data_path", "CUMULUS_LIBRARY_DATA_PATH"),
         ("user", "CUMULUS_AGGREGATOR_USER"),
         ("id", "CUMULUS_AGGREGATOR_ID"),
         ("url", "CUMULUS_AGGREGATOR_URL"),
     )
+    read_env_vars = []
     for pair in arg_env_pairs:
         if env_val := os.environ.get(pair[1]):
             args[pair[0]] = env_val
+            read_env_vars.append([pair[1], env_val])
+
+    if len(read_env_vars) > 0:
+        table = Table(title="Values read from environment variables")
+        table.add_column("Environment Variable", style="green")
+        table.add_column("Value", style="cyan")
+        for row in read_env_vars:
+            if row[0] == "CUMULUS_AGGREGATOR_ID":
+                table.add_row(row[0], "#########")
+            else:
+                table.add_row(row[0], row[1])
+        console = Console()
+        console.print(table)
 
     if args.get("study_dir"):
         posix_paths = []
         for path in args["study_dir"]:
             posix_paths.append(get_abs_posix_path(path))
         args["study_dir"] = posix_paths
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py` & `cumulus_library-1.0.0/cumulus_library/cli_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,22 @@
         help=(
             "Specify one or more studies to perform actions against. "
             "Default is to use all studies."
         ),
     )
 
 
+def add_table_builder_argument(parser: argparse.ArgumentParser) -> None:
+    """Adds --table_builder arg to a subparser"""
+    parser.add_argument(
+        "--table-builder",
+        help=(argparse.SUPPRESS),
+    )
+
+
 def add_study_dir_argument(parser: argparse.ArgumentParser) -> None:
     """Adds --study_dir arg to a subparser"""
     parser.add_argument(
         "-s",
         "--study-dir",
         action="append",
         help=(
@@ -120,14 +128,15 @@
     add_aws_config(clean)
 
     build = actions.add_parser(
         "build",
         help="Removes and recreates Athena tables & views for specified studies",
     )
     add_target_argument(build)
+    add_table_builder_argument(build)
     add_study_dir_argument(build)
     add_verbose_argument(build)
     add_aws_config(build)
 
     export = actions.add_parser(
         "export", help="Generates files on disk from Athena views"
     )
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/helper.py` & `cumulus_library-1.0.0/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-1.0.0/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py` & `cumulus_library-1.0.0/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py` & `cumulus_library-1.0.0/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py` & `cumulus_library-1.0.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py` & `cumulus_library-1.0.0/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/condition.sql`

 * *Files 12% similar despite different names*

```diff
@@ -43,31 +43,42 @@
     date_trunc('year', date(tc.recordeddate)) AS recorded_year
 FROM temp_condition AS tc,
     unnest(category) AS t_category (category_coding), --noqa
     unnest(category_coding.coding) AS t_category_coding (category_row), --noqa
     unnest(code.coding) AS t_coding (code_row) --noqa
 WHERE tc.recordeddate BETWEEN date('2016-01-01') AND current_date;
 
-CREATE TABLE core__count_condition_month AS
-WITH powerset AS (
+-- ###########################################################################
+-- Encounter.diagnosis may also join, we can't rely on link to encounter!
+-- cond_month is a similar enough proxy for encounter month
+
+CREATE TABLE core__count_condition_month AS WITH
+concept_map AS (
+    SELECT
+        c.recorded_month AS cond_month,
+        c.subject_ref,
+        coalesce(c.encounter_ref, 'None') AS encounter_ref,
+        coalesce(mapping.display, 'None') AS cond_code_display,
+        c.category.code AS cond_category_code
+    FROM core__condition AS c
+    LEFT JOIN core__condition_codable_concepts AS mapping
+        ON c.condition_id = mapping.id
+),
+
+powerset AS (
     SELECT
-        count(DISTINCT cc.subject_ref) AS cnt_subject,
-        count(DISTINCT cc.encounter_ref) AS cnt_encounter,
-        cccc.display AS display,
-        cc.recorded_month,
-        ce.enc_class
-    FROM core__condition AS cc
-    INNER JOIN core__encounter AS ce
-        ON cc.encounter_ref = ce.encounter_ref
-    LEFT JOIN core__condition_codable_concepts AS cccc
-        ON cc.condition_id = cccc.id
-    GROUP BY cube(display, cc.recorded_month, ce.enc_class)
+        count(DISTINCT subject_ref) AS cnt_subject,
+        count(DISTINCT encounter_ref) AS cnt_encounter,
+        cond_category_code,
+        cond_month,
+        cond_code_display
+    FROM concept_map
+    GROUP BY cube(cond_category_code, cond_month, cond_code_display)
 )
 
-SELECT
+SELECT DISTINCT
     powerset.cnt_subject AS cnt,
-    powerset.recorded_month AS cond_month,
-    powerset.display AS cond_code_display,
-    enc_class.code AS enc_class_code
+    powerset.cond_category_code,
+    powerset.cond_month,
+    powerset.cond_code_display
 FROM powerset
-WHERE powerset.cnt_subject >= 10
-ORDER BY powerset.cnt_subject DESC, powerset.cnt_encounter DESC;
+WHERE powerset.cnt_subject >= 10;
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/condition_codeable_concept.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 -- noqa: disable=all
 /*
-This is a reference output of the SQL generated by denormalizer.py that is
+This is a reference output of the SQL generated by 
+builder_condition_condeableconcept.py that is
 used by the core__condition table. It is not invoked directly. We may
 in the future change the priority order of concept systems, or add
 additional systems to support other implementations if we run into
 unusual data in the wild.
 */
 CREATE TABLE core__condition_codable_concepts AS (
     WITH
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.py` & `cumulus_library-1.0.0/cumulus_library/studies/core/count_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,18 @@
 
 
 def write_view_sql(view_list_sql: List[str], filename="count_core.sql") -> None:
     """
     :param view_list_sql: SQL prepared statements
     :param filename: path to output file, default 'count_core.sql' in PWD
     """
-    sql_optimizer = concat_view_sql(view_list_sql).replace("ORDER BY cnt desc", "")
+    sql_optimizer = concat_view_sql(view_list_sql)
+    sql_optimizer = sql_optimizer.replace("ORDER BY cnt desc", "")
+    sql_optimizer = sql_optimizer.replace("CREATE or replace VIEW", "CREATE TABLE")
+
     with open(filename, "w") as fout:
         fout.write(sql_optimizer)
 
 
 if __name__ == "__main__":
     write_view_sql(
         [
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/count_core.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_patient AS
+CREATE TABLE core__count_patient AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
 
         age,
         gender,
         race_display,
@@ -18,15 +18,15 @@
     gender,
     race_display,
     ethnicity_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_month AS
+CREATE TABLE core__count_encounter_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         start_month,
         enc_class_display,
         age_at_visit,
@@ -53,15 +53,15 @@
     gender,
     race_display,
     ethnicity_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_type AS
+CREATE TABLE core__count_encounter_type AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         enc_service_display,
@@ -82,15 +82,15 @@
     enc_type_display,
     enc_service_display,
     enc_priority_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_type_month AS
+CREATE TABLE core__count_encounter_type_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         enc_service_display,
@@ -113,16 +113,17 @@
     enc_type_display,
     enc_service_display,
     enc_priority_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
+
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_enc_type_month AS
+CREATE TABLE core__count_encounter_enc_type_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         start_month
@@ -135,15 +136,15 @@
     enc_class_display,
     enc_type_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_service_month AS
+CREATE TABLE core__count_encounter_service_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_service_display,
         start_month
@@ -156,15 +157,15 @@
     enc_class_display,
     enc_service_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE OR REPLACE VIEW core__count_encounter_priority_month AS
+CREATE TABLE core__count_encounter_priority_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_priority_display,
         start_month
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/documentreference.sql`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         ) AS author_date,
         concat('DocumentReference/', dr.id) AS doc_ref
     FROM documentreference AS dr
 )
 
 SELECT DISTINCT
     type_coding.type_row AS doc_type,
-    coalesce(type_coding.type_row.code, '?') AS doc_type_code,
+    coalesce(type_coding.type_row.code, 'None') AS doc_type_code,
     CASE
         WHEN
             type_coding.type_row.display IS NOT NULL
             THEN replace(type_coding.type_row.display, ',')
         ELSE type_row.code
     END AS doc_type_display,
     tdr.status,
@@ -61,15 +61,15 @@
 WITH powerset AS (
     SELECT
         count(DISTINCT d.subject_ref) AS cnt_subject,
         count(DISTINCT d.encounter_ref) AS cnt_encounter,
         count(DISTINCT d.doc_id) AS cnt_document,
         d.doc_type_display,
         d.author_month,
-        e.enc_class.code AS enc_class_code
+        e.enc_class.display AS enc_class_code
     FROM core__documentreference AS d, core__encounter AS e
     WHERE d.encounter_ref = e.encounter_ref
     GROUP BY cube(d.doc_type_display, d.author_month, e.enc_class)
 )
 
 SELECT DISTINCT
     cnt_document AS cnt,
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/patient.sql`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     tp.gender,
     tp.birthdate,
     date_diff('year', tp.birthdate, current_date) AS age,
     CASE
         WHEN
             t_address.addr_row.postalcode IS NOT NULL
             THEN substr(t_address.addr_row.postalcode, 1, 3)
-        ELSE '?'
+        ELSE 'None'
     END AS postalcode3,
     tp.subject_id,
     tp.subject_ref,
     coalesce(tp.race_display, ARRAY['unknown']) AS race_display,
     coalesce(tp.ethnicity_display, ARRAY['unknown']) AS ethnicity_display
 FROM
     temp_patient AS tp,
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/patient_extensions.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql` & `cumulus_library-1.0.0/cumulus_library/studies/core/study_period.sql`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         cp.gender,
         cp.race_display,
         cp.ethnicity_display,
         cp.subject_ref,
         ce.encounter_ref,
         cd.doc_ref,
         date_diff('day', ce.start_date, cd.author_date) AS diff_enc_note_days,
-        coalesce(ce.enc_class.code, '?') AS enc_class_code,
-        coalesce(cd.doc_type.code, '?') AS doc_type_code,
+        coalesce(ce.enc_class.display, 'None') AS enc_class_code,
+        coalesce(cd.doc_type.code, 'None') AS doc_type_code,
         coalesce(cd.doc_type.display, cd.doc_type.code) AS doc_type_display
     FROM
         core__patient AS cp,
         core__encounter AS ce,
         core__documentreference AS cd
     WHERE
         (cp.subject_ref = ce.subject_ref)
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql` & `cumulus_library-1.0.0/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-1.0.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml` & `cumulus_library-1.0.0/cumulus_library/studies/template/manifest.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 # The following tables will be output to disk when an export is run. In most cases,
 # only count tables should be output in this way.
 export_list = [
     "template__count_influenza_test_month",
 ]
 
 
-# For most use cases, this should not be required, but if you need to run code, you
-# can point to a python module. The vocab study provides an example of this. 
-# Python code will always be run before any SQL queries are executed.
-# [python_config]
+# For most use cases, this should not be required, but if you need to programmatically
+# build tables, you can provide a list of files implementing BaseTableBuilder.
+# See vocab and core studies for examples of this pattern
+# [table_builder_config]
 # file_names = [
-#     "my_script.py",
+#     "my_table_builder.py",
 # ]
-
-# If you'd like another language available, please reach out - we can likely 
-# accomadate, but we'd need to understand the use cases a little better.
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql` & `cumulus_library-1.0.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-1.0.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-1.0.0/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,46 @@
 """ Module for directly loading ICD bsvs into athena tables """
 import csv
 
 from pathlib import Path
 
-from cumulus_library.base_runner import BaseRunner
+from cumulus_library.base_table_builder import BaseTableBuilder
 from cumulus_library.helper import query_console_output, get_progress_bar
 from cumulus_library.template_sql.templates import (
     get_ctas_query,
     get_insert_into_query,
 )
 
 
-class VocabIcdRunner(BaseRunner):
-    def run_executor(self, cursor: object, schema: str, verbose: bool):
-        self.create_icd_legend(self, cursor, schema, verbose)
+class VocabIcdRunner(BaseTableBuilder):
+    display_text = "Creating ICD vocab..."
+    partition_size = 1200
 
     @staticmethod
     def clean_row(row, filename):
         """Removes non-SQL safe charatcers from the input row."""
         for i in range(len(row)):
             cell = str(row[i]).replace("'", "").replace(";", ",")
             row[i] = cell
         return row
 
-    def create_icd_legend(
-        self, cursor: object, schema: str, verbose: bool, partition_size: int = 1200
-    ):
-        """input point from make.execute_sql_template.
+    def prepare_queries(self, cursor: object, schema: str):
+        """Creates queries for populating ICD vocab
+
+        TODO: this would be a lot faster if we converted the bsv to parquet,
+        uploaded that, and then created the table from an external datasource
 
         :param cursor: A database cursor object
         :param schema: the schema/db name, matching the cursor
-        :param verbose: if true, outputs raw query, else displays progress bar
-        :partition_size: number of lines to read. Athena queries have a char limit.
         """
+
         table_name = "vocab__icd"
         icd_files = ["ICD10CM_2023AA", "ICD10PCS_2023AA", "ICD9CM_2023AA"]
         path = Path(__file__).parent
-        query_count = 1  # accounts for static CTAS query
-        for filename in icd_files:
-            query_count += (
-                sum(1 for i in open(f"{path}/{filename}.bsv", "rb")) / partition_size
-            )
-
-        with get_progress_bar(disable=verbose) as progress:
-            task = progress.add_task(
-                f"Uploading {table_name} data...",
-                total=query_count,
-                visible=not verbose,
-            )
-            self.build_vocab_icd(
-                self,
-                cursor,
-                schema,
-                verbose,
-                partition_size,
-                table_name,
-                path,
-                icd_files,
-                progress,
-                task,
-            )
 
-    @staticmethod
-    def build_vocab_icd(
-        self,
-        cursor,
-        schema,
-        verbose,
-        partition_size,
-        table_name,
-        path,
-        icd_files,
-        progress,
-        task,
-    ):
-        """Constructs queries and posts to athena."""
         headers = ["CUI", "TTY", "CODE", "SAB", "STR"]
         header_types = [f"{x} string" for x in headers]
         rows_processed = 0
         dataset = []
         created = False
         for filename in icd_files:
             with open(f"{path}/{filename}.bsv", "r") as file:
@@ -86,34 +48,36 @@
                 # varchar(len(item)) athena default to to an unrestricted varchar, so
                 # we'll create a table with one row - this make the recast faster, and
                 # lets us set the partition_size a little higher by limiting the
                 # character bloat to keep queries under athena's limit of 262144.
                 reader = csv.reader(file, delimiter="|")
                 if not created:
                     row = self.clean_row(next(reader), filename)
-                    ctas_query = get_ctas_query(
-                        schema_name=schema,
-                        table_name=table_name,
-                        dataset=[row],
-                        table_cols=headers,
+                    self.queries.append(
+                        get_ctas_query(
+                            schema_name=schema,
+                            table_name=table_name,
+                            dataset=[row],
+                            table_cols=headers,
+                        )
                     )
-                    cursor.execute(ctas_query)
-                    query_console_output(verbose, ctas_query, progress, task)
                     created = True
                 for row in reader:
                     row = self.clean_row(row, filename)
                     dataset.append(row)
                     rows_processed += 1
-                    if rows_processed == partition_size:
-                        insert_into_query = get_insert_into_query(
-                            table_name=table_name, table_cols=headers, dataset=dataset
+                    if rows_processed == self.partition_size:
+                        self.queries.append(
+                            get_insert_into_query(
+                                table_name=table_name,
+                                table_cols=headers,
+                                dataset=dataset,
+                            )
                         )
-                        query_console_output(verbose, insert_into_query, progress, task)
-                        cursor.execute(insert_into_query)
                         dataset = []
                         rows_processed = 0
                 if rows_processed > 0:
-                    insert_into_query = get_insert_into_query(
-                        table_name=table_name, table_cols=headers, dataset=dataset
+                    self.queries.append(
+                        get_insert_into_query(
+                            table_name=table_name, table_cols=headers, dataset=dataset
+                        )
                     )
-                    cursor.execute(insert_into_query)
-                    query_console_output(verbose, insert_into_query, progress, task)
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py` & `cumulus_library-1.0.0/cumulus_library/study_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """ Contains classes for loading study data based on manifest.toml files """
 import inspect
+import importlib.util
 import sys
 
-from importlib.machinery import SourceFileLoader
 from pathlib import Path, PosixPath
 from typing import List, Optional
 
 import toml
 
 from rich.progress import Progress, TaskID, track
 
-from cumulus_library.base_runner import BaseRunner
+from cumulus_library.base_table_builder import BaseTableBuilder
 from cumulus_library.errors import StudyManifestParsingError
 from cumulus_library.helper import (
     query_console_output,
     load_text,
     parse_sql,
     get_progress_bar,
 )
@@ -90,20 +90,20 @@
         """Reads the contents of the sql_config array from the manifest
 
         :returns: An array of sql files from the manifest, or None if not found.
         """
         sql_config = self._study_config.get("sql_config", {})
         return sql_config.get("file_names", [])
 
-    def get_python_file_list(self) -> Optional[StrList]:
+    def get_table_builder_file_list(self) -> Optional[StrList]:
         """Reads the contents of the python_config array from the manifest
 
         :returns: An array of sql files from the manifest, or None if not found.
         """
-        sql_config = self._study_config.get("python_config", {})
+        sql_config = self._study_config.get("table_builder_config", {})
         return sql_config.get("file_names", [])
 
     def get_export_table_list(self) -> Optional[StrList]:
         """Reads the contents of the export_list array from the manifest
 
         :returns: An array of tables to export from the manifest, or None if not found.
         """
@@ -206,51 +206,82 @@
         for view_table in view_table_list:
             drop_view_table = get_drop_view_table(
                 name=view_table[0], view_or_table=view_table[1]
             )
             cursor.execute(drop_view_table)
             query_console_output(verbose, drop_view_table, progress, task)
 
-    def run_python_builder(
+    def _load_and_execute_builder(
+        self, filename, cursor, schema, verbose, drop_table=False
+    ) -> None:
+        """Loads a table builder from a file.
+
+        Since we have to support arbitrary user-defined python files here, we
+        jump through some importlib hoops to import the module directly from
+        a source file defined in the manifest.
+
+        As with eating an ortolan, you may wish to cover your head with a cloth.
+        Per an article on the subject: "Tradition dictates that this is to shield
+        – from God’s eyes – the shame of such a decadent and disgraceful act."
+
+        """
+        spec = importlib.util.spec_from_file_location(
+            "table_builder", f"{self._study_path}/{filename}"
+        )
+        table_builder_module = importlib.util.module_from_spec(spec)
+        sys.modules["table_builder"] = table_builder_module
+        spec.loader.exec_module(table_builder_module)
+
+        # We're going to find all subclasses of BaseTableBuild in this file.
+        # Since BaseTableBuilder itself is a valid subclass of BaseTableBuilder,
+        # we'll detect and skip it. If we don't find exactly one subclass,
+        # we'll punt.
+        table_builder_subclasses = []
+        for _, cls_obj in inspect.getmembers(table_builder_module, inspect.isclass):
+            if issubclass(cls_obj, BaseTableBuilder) and cls_obj != BaseTableBuilder:
+                table_builder_subclasses.append(cls_obj)
+        if len(table_builder_subclasses) != 1:
+            raise StudyManifestParsingError(
+                f"Error loading {self._study_path}{filename}\n"
+                "Custom builders must extend the BaseTableBuilder "
+                "class exactly once per module."
+            )
+
+        # We'll get the subclass, initialize it, run the executor code, and then
+        # remove it so it doesn't interfere with the next python module to
+        # execute, since the subclass would otherwise hang around.
+        table_builder_class = table_builder_subclasses[0]
+        table_builder = table_builder_class()
+        table_builder.execute_queries(cursor, schema, verbose, drop_table)
+
+        # After runnning the executor code, we'll remove
+        # remove it so it doesn't interfere with the next python module to
+        # execute, since the subclass would otherwise hang around.
+        del sys.modules[table_builder_module.__name__]
+        del table_builder_module
+
+    def run_table_builder(
         self, cursor: object, schema: str, verbose: bool = False
     ) -> None:
-        """Loads arbitrary modules from a manifest and executes code via BaseRunners
+        """Loads modules from a manifest and executes code via BaseTableBuilder
 
         :param cursor: A PEP-249 compatible cursor object
         :param schema: The name of the schema to write tables to
         :param verbose: toggle from progress bar to query output
         """
-        for file in self.get_python_file_list():
-            # Grab the baserunner class from the manifest-defined module
-            # TODO: if we need to support python 3.12, cutover to exec_modules
-            # (warning: it sounds like this is non-trivial)
-            runner_module = SourceFileLoader(  # pylint: disable=deprecated-method, no-value-for-parameter
-                "BaseRunner", f"{self._study_path}/{file}"
-            ).load_module()
-
-            # We're going to find all subclasses of BaseRunner in this file.
-            # Since BaseRunner itself is a valid subclass of BaseRunner, we'll
-            # detect and skip it. If we don't find exactly one subclass, we'll punt.
-            runner_subclasses = []
-            for _, cls_obj in inspect.getmembers(runner_module, inspect.isclass):
-                if issubclass(cls_obj, BaseRunner) and cls_obj != BaseRunner:
-                    runner_subclasses.append(cls_obj)
-            if len(runner_subclasses) != 1:
-                raise StudyManifestParsingError(
-                    f"Error loading {self._study_path}/{file}\n"
-                    "Custom runners must extend the BaseRunner class exactly once per module."
-                )
+        for file in self.get_table_builder_file_list():
+            self._load_and_execute_builder(file, cursor, schema, verbose)
 
-            # We'll get the subclass, run the executor code, and then remove it
-            # so it doesn't interfere with the next python module to execute, since
-            # the subclass would otherwise hang around.
-            runner = runner_subclasses[0]
-            runner.run_executor(runner, cursor, schema, verbose)
-            del sys.modules[runner_module.__name__]
-            del runner_module
+    def run_single_table_builder(
+        self, cursor: object, schema: str, name: str, verbose: bool = False
+    ):
+        """targets a single table builder to run"""
+        if not name.endswith(".py"):
+            name = f"{name}.py"
+        self._load_and_execute_builder(name, cursor, schema, verbose, drop_table=True)
 
     def build_study(self, cursor: object, verbose: bool = False) -> List:
         """Creates tables in the schema by iterating through the sql_config.file_names
 
         :param cursor: A PEP-249 compatible cursor object
         :param schema: The name of the schema to write tables to
         :param verbose: toggle from progress bar to query output, optional
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-1.0.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 CREATE TABLE {{ target_table }} AS (
     WITH
-    {%- for system in code_systems %}
-
-    system_{{ loop.index0 }} AS (
+    {%- for system in cc_column.code_systems %}
+    system_{{ cc_column.name }}_{{ loop.index0 }} AS (
         SELECT DISTINCT
-            s.id AS id,
+            s.{{ source_id }} AS id,
             '{{ loop.index0 }}' AS priority,
             u.codeable_concept.code AS code,
             u.codeable_concept.display AS display,
             u.codeable_concept.system AS code_system
         FROM
             {{ source_table }} AS s,
-            UNNEST(s.{{ cc_column }}.coding) AS u (codeable_concept) --noqa: AL05
+        {% if cc_column.is_array %}
+            UNNEST(s.{{ cc_column.name }}) AS cc (cc_row),
+            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+        {% else %}
+            UNNEST(s.{{ cc_column.name }}.coding) AS u (codeable_concept)
+        {%- endif %}
         WHERE
             u.codeable_concept.system = '{{ system }}'
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
-        {%- for system in code_systems %}
+        {%- for system in cc_column.code_systems %}
         SELECT
             id,
             priority,
             code_system,
             code,
             display
-        FROM system_{{ loop.index0 }}
+        FROM system_{{ cc_column.name }}_{{ loop.index0 }}
         {%- if not loop.last %}
         UNION 
         {%- endif -%}
         {%- endfor %}
     ),
 
     partitioned_table AS (
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-1.0.0/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-1.0.0/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-1.0.0/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 CREATE TABLE {{ target_table }} AS (
     WITH
     {%- for system in ext_systems %}
 
     system_{{ system }} AS (
         SELECT DISTINCT
-            s.id,
+            s.{{ source_id }} AS id,
             '{{ loop.index0 }}' AS priority,
             '{{ system }}' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS {{ target_col_prefix }}_code,
             ext_child.ext.valuecoding.display AS {{ target_col_prefix }}_display
         FROM
             {{ source_table }} AS s,
-            UNNEST(extension) AS ext_parent (ext), --noqa: AL05
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext) --noqa: AL05
+            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = '{{ fhir_extension }}'
             AND ext_child.ext.url = '{{ system }}'
             AND ext_child.ext.valuecoding.display != ''
     ), --noqa: LT07
     {%- endfor %}
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py` & `cumulus_library-1.0.0/cumulus_library/template_sql/templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Collection of jinja template getters for common SQL queries """
 from enum import Enum
 from pathlib import Path
-from typing import List
+from typing import Dict, List
 
 from jinja2 import Template
 
 
 class TableView(Enum):
     TABLE = "TABLE"
     VIEW = "VIEW"
@@ -74,14 +74,37 @@
             schema_name=schema_name,
             table_name=table_name,
             dataset=dataset,
             table_cols=table_cols,
         )
 
 
+def get_ctas_empty_query(
+    schema_name: str, table_name: str, table_cols: List[str]
+) -> str:
+    """Generates a create table as query for initializing an empty table
+
+    Note that unlike other queries, the nature of the CTAS implementation in athena
+    requires a schema name. This schema name should match the schema of your cursor,
+    or the other queries in this template will not function correctly. All columns
+    will be specified as varchar type.
+
+    :param schema_name: The athena schema to create the table in
+    :param table_name: The name of the athena table to create
+    :param table_cols: Comma deleniated column names, i.e. ['first,second']
+    """
+    path = Path(__file__).parent
+    with open(f"{path}/ctas_empty.sql.jinja") as ctas_empty:
+        return Template(ctas_empty.read()).render(
+            schema_name=schema_name,
+            table_name=table_name,
+            table_cols=table_cols,
+        )
+
+
 def get_create_view_query(
     view_name: str, dataset: List[List[str]], view_cols: List[str]
 ) -> str:
     """Generates a create view as query for inserting static data into athena
 
     :param view_name: The name of the athena table to create
     :param dataset: Array of data arrays to insert, i.e. [['1','3'],['2','4']]
@@ -162,29 +185,86 @@
             target_table=config.target_table,
             target_col_prefix=config.target_col_prefix,
             fhir_extension=config.fhir_extension,
             ext_systems=config.ext_systems,
         )
 
 
-def get_codeable_concept_denormalize_query(
-    source_table: str, cc_column: str, target_table: str, code_systems: List[str]
-) -> str:
-    """extracts codeable concepts from a specified table.
-
-    See http://hl7.org/fhir/datatypes-definitions.html#CodeableConcept for more info
+class CodeableConceptConfig:
+    """Convenience class for holding parameters for generating codableconcept tables.
 
     :param source_table: the table to extract extensions from
-    :param cc_column: the column containing the codeableConcept you want to extract
+    :param source_id: the id field to use in the new table
+    :param cc_columns: the column containing the codeableConcept you want to extract.
+        Format:
+            {'name':[column],
+            'is_array': [boolean],
+            'code_systems':[List of code system strings, in priority order]}
+        is_array relates to the FHIR spec - if the field is specified
+        as 0...*, set this to be true.
     :param target_table: the name of the table to create
-    :param code_systems: a list of coding systems, in preference order, to use to select data
+    :param code_systems: a list of systems, in preference order, for selecting data
+    """
+
+    def __init__(
+        self, source_table: str, source_id: str, cc_column: dict, target_table: str
+    ):
+        self.source_table = source_table
+        self.source_id = source_id
+        self.cc_column = cc_column
+        self.target_table = target_table
+
+
+def get_codeable_concept_denormalize_query(config: CodeableConceptConfig) -> str:
+    """extracts codeable concepts from a specified table.
+
+    This function is targeted at arbitrary codeableConcept elements - see
+    http://hl7.org/fhir/datatypes-definitions.html#CodeableConcept for more info.
+    This may be or may not be an array field depending on the context of use -
+    check the specification of the specific resource you're interested in.
+    See the CodeableConceptConfig for details on how to handle array vs non-
+    array use cases.
+
+    :param config: a CodableConeptConfig
     """
     path = Path(__file__).parent
-    with open(
-        f"{path}/codeable_concept_denormalize.sql.jinja"
-    ) as extension_denormalize:
-        return Template(extension_denormalize.read()).render(
+    with open(f"{path}/codeable_concept_denormalize.sql.jinja") as codable_concept:
+        return Template(codable_concept.read()).render(
+            source_table=config.source_table,
+            source_id=config.source_id,
+            cc_column=config.cc_column,
+            target_table=config.target_table,
+        )
+
+
+def get_is_table_not_empty_query(
+    source_table: str, field: str, unnests: list[dict] = [], conditions: list[str] = []
+):
+    path = Path(__file__).parent
+    with open(f"{path}/is_table_not_empty.sql.jinja") as is_table_not_empty:
+        return Template(is_table_not_empty.read()).render(
             source_table=source_table,
-            cc_column=cc_column,
-            target_table=target_table,
-            code_systems=code_systems,
+            field=field,
+            unnests=unnests,
+            conditions=conditions,
+        )
+
+
+def get_core_medication_query(
+    medication_datasources: dict, missing_userselected: bool = False
+):
+    path = Path(__file__).parent
+    with open(f"{path}/core_medication.sql.jinja") as core_medication:
+        return Template(core_medication.read()).render(
+            medication_datasources=medication_datasources,
+            missing_userselected=missing_userselected,
+        )
+
+
+def get_column_datatype_query(schema_name: str, table_name: str, column_name: str):
+    path = Path(__file__).parent
+    with open(f"{path}/column_datatype.sql.jinja") as column_datatype:
+        return Template(column_datatype.read()).render(
+            schema_name=schema_name,
+            table_name=table_name,
+            column_name=column_name,
         )
```

### Comparing `cumulus_library-0.4.0.dev1/cumulus_library/upload.py` & `cumulus_library-1.0.0/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0.dev1/pyproject.toml` & `cumulus_library-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 [project]
 name = "cumulus-library"
-# In order to support 3.12, we wil need to refactor out load_module, which is
-# targeted for deprecation in that version.
-requires-python = ">= 3.9, <3.12"
+requires-python = ">= 3.9"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
     "pandas <2, >=1.5.0",
     "pyarrow >= 11.0",
     "pyathena >= 2.23",
```

### Comparing `cumulus_library-0.4.0.dev1/PKG-INFO` & `cumulus_library-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.4.0.dev1
+Version: 1.0.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
-Requires-Python: >= 3.9, <3.12
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ctakesclient >= 1.3
 Requires-Dist: fhirclient >= 4.1
```

