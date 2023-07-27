# Comparing `tmp/xmlschema-2.3.1.tar.gz` & `tmp/xmlschema-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-2.3.1.tar", last modified: Wed Jun 14 07:04:26 2023, max compression
+gzip compressed data, was "xmlschema-2.4.0.tar", last modified: Thu Jul 27 20:04:16 2023, max compression
```

## Comparing `xmlschema-2.3.1.tar` & `xmlschema-2.4.0.tar`

### file list

```diff
@@ -1,496 +1,518 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.663356 xmlschema-2.3.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.3.1/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    25333 2023-06-14 07:04:00.000000 xmlschema-2.3.1/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.3.1/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.3.1/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-06-14 07:04:26.663356 xmlschema-2.3.1/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.3.1/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.628356 xmlschema-2.3.1/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.3.1/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.3.1/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.3.1/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-06-14 07:04:00.000000 xmlschema-2.3.1/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/extras.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.3.1/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.3.1/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.3.1/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.3.1/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.3.1/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.3.1/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-05-18 20:18:16.000000 xmlschema-2.3.1/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-06-14 07:04:26.663356 xmlschema-2.3.1/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-06-14 07:04:00.000000 xmlschema-2.3.1/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.630356 xmlschema-2.3.1/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.3.1/tests/__init__.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.621356 xmlschema-2.3.1/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.630356 xmlschema-2.3.1/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.631356 xmlschema-2.3.1/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.3.1/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.3.1/tests/templates/filters/wrong-template.jinja
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.631356 xmlschema-2.3.1/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.622356 xmlschema-2.3.1/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.632356 xmlschema-2.3.1/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection-default.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-06-14 06:39:51.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.632356 xmlschema-2.3.1/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.622356 xmlschema-2.3.1/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.634356 xmlschema-2.3.1/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.635356 xmlschema-2.3.1/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.635356 xmlschema-2.3.1/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.636356 xmlschema-2.3.1/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.637356 xmlschema-2.3.1/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.3.1/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.3.1/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.639356 xmlschema-2.3.1/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/namespaces/included6-invalid.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.640356 xmlschema-2.3.1/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.640356 xmlschema-2.3.1/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.641356 xmlschema-2.3.1/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.642356 xmlschema-2.3.1/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.643356 xmlschema-2.3.1/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.644356 xmlschema-2.3.1/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.645356 xmlschema-2.3.1/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.646356 xmlschema-2.3.1/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.624356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.647356 xmlschema-2.3.1/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.648356 xmlschema-2.3.1/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.649356 xmlschema-2.3.1/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.650356 xmlschema-2.3.1/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.650356 xmlschema-2.3.1/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.651356 xmlschema-2.3.1/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/issues/issue_349/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_349/issue_349.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/issues/issue_349/issue_349.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.652356 xmlschema-2.3.1/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.3.1/tests/test_cases/mypy/extra_validator.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-2.3.1/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.3.1/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.653356 xmlschema-2.3.1/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/dummy file #2.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.3.1/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.3.1/tests/test_cases/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6534 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_cases/testfiles
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.3.1/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.3.1/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.3.1/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24557 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.3.1/tests/test_files.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/test_helpers.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.3.1/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.3.1/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    70653 2023-02-06 06:20:42.000000 xmlschema-2.3.1/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3600 2022-05-20 20:00:14.000000 xmlschema-2.3.1/tests/test_translations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2101 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.3.1/tests/test_validation.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    27317 2023-06-12 10:20:33.000000 xmlschema-2.3.1/tests/test_w3c_suite.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.3.1/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.653356 xmlschema-2.3.1/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.1/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66088 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/validation/test_decoding.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17401 2023-06-14 07:04:00.000000 xmlschema-2.3.1/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.655356 xmlschema-2.3.1/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.3.1/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.3.1/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.3.1/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.3.1/tests/validators/test_elements.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_exceptions.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.3.1/tests/validators/test_global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13500 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.3.1/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.3.1/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41506 2022-10-01 13:42:01.000000 xmlschema-2.3.1/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_wildcards.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.3.1/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1569 2023-05-18 20:18:16.000000 xmlschema-2.3.1/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.656356 xmlschema-2.3.1/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5515 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/aliases.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11669 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/converters/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.3.1/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35730 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.3.1/xmlschema/exceptions.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.3.1/xmlschema/extras/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.3.1/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.3.1/xmlschema/extras/templates/python/sample.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24454 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11097 2022-08-26 15:33:28.000000 xmlschema-2.3.1/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.3.1/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.658356 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.625356 xmlschema-2.3.1/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8827 2020-12-23 12:38:37.000000 xmlschema-2.3.1/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.3.1/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.3.1/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    55658 2023-04-14 13:49:05.000000 xmlschema-2.3.1/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.626356 xmlschema-2.3.1/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.659356 xmlschema-2.3.1/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.660356 xmlschema-2.3.1/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.3.1/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.661356 xmlschema-2.3.1/xmlschema/testing/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2116 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30214 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/testing/_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_case_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.3.1/xmlschema/testing/_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.3.1/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.663356 xmlschema-2.3.1/xmlschema/validators/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.3.1/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-05-07 06:35:13.000000 xmlschema-2.3.1/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.3.1/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.3.1/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-05-07 06:33:55.000000 xmlschema-2.3.1/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64310 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14970 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-06-10 06:00:33.000000 xmlschema-2.3.1/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    63815 2023-06-14 07:04:00.000000 xmlschema-2.3.1/xmlschema/validators/groups.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.3.1/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.3.1/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.3.1/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6684 2023-05-18 20:18:16.000000 xmlschema-2.3.1/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   103598 2023-06-09 17:48:42.000000 xmlschema-2.3.1/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61468 2023-05-08 10:45:15.000000 xmlschema-2.3.1/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.3.1/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.3.1/xmlschema/validators/xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.3.1/xmlschema/xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-14 07:04:26.657356 xmlschema-2.3.1/xmlschema.egg-info/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    17217 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-06-14 07:04:26.000000 xmlschema-2.3.1/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.450284 xmlschema-2.4.0/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-2.4.0/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    25577 2023-07-27 19:52:28.000000 xmlschema-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2022-09-26 10:47:27.000000 xmlschema-2.4.0/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-2.4.0/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7377 2023-07-27 20:04:16.450284 xmlschema-2.4.0/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6045 2022-08-26 15:33:28.000000 xmlschema-2.4.0/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.412284 xmlschema-2.4.0/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-2.4.0/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11613 2022-10-01 13:42:01.000000 xmlschema-2.4.0/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-2.4.0/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5474 2023-07-27 19:52:28.000000 xmlschema-2.4.0/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-2.4.0/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-2.4.0/doc/extras.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7488 2022-06-24 14:13:22.000000 xmlschema-2.4.0/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-2.4.0/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-2.4.0/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-2.4.0/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27730 2022-10-01 13:42:01.000000 xmlschema-2.4.0/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-2.4.0/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2023-07-27 19:52:28.000000 xmlschema-2.4.0/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-07-27 20:04:16.450284 xmlschema-2.4.0/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2764 2023-07-27 19:52:28.000000 xmlschema-2.4.0/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.414284 xmlschema-2.4.0/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-2.4.0/tests/__init__.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     4934 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.406284 xmlschema-2.4.0/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.414284 xmlschema-2.4.0/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.415284 xmlschema-2.4.0/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-2.4.0/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-2.4.0/tests/templates/filters/wrong-template.jinja
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3484 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.415284 xmlschema-2.4.0/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.406284 xmlschema-2.4.0/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.417284 xmlschema-2.4.0/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection-default.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2023-07-27 19:59:04.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-2.4.0/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.417284 xmlschema-2.4.0/tests/test_cases/examples/menù/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù-ascii.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù-ascii.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù-cp1252.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù-cp1252.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/examples/menù/menù.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.418284 xmlschema-2.4.0/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.419284 xmlschema-2.4.0/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.407284 xmlschema-2.4.0/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.419284 xmlschema-2.4.0/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.419284 xmlschema-2.4.0/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.420284 xmlschema-2.4.0/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-2.4.0/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.421284 xmlschema-2.4.0/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.421284 xmlschema-2.4.0/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.422284 xmlschema-2.4.0/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-2.4.0/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-2.4.0/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.424284 xmlschema-2.4.0/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/namespaces/included6-invalid.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.425284 xmlschema-2.4.0/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-2.4.0/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.425284 xmlschema-2.4.0/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.409284 xmlschema-2.4.0/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.426284 xmlschema-2.4.0/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.426284 xmlschema-2.4.0/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.426284 xmlschema-2.4.0/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.426284 xmlschema-2.4.0/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.426284 xmlschema-2.4.0/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.427284 xmlschema-2.4.0/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.427284 xmlschema-2.4.0/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.427284 xmlschema-2.4.0/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.428284 xmlschema-2.4.0/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.428284 xmlschema-2.4.0/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.428284 xmlschema-2.4.0/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.428284 xmlschema-2.4.0/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.428284 xmlschema-2.4.0/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.429284 xmlschema-2.4.0/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.430284 xmlschema-2.4.0/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.430284 xmlschema-2.4.0/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.430284 xmlschema-2.4.0/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.430284 xmlschema-2.4.0/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.431284 xmlschema-2.4.0/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.431284 xmlschema-2.4.0/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.431284 xmlschema-2.4.0/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.431284 xmlschema-2.4.0/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.431284 xmlschema-2.4.0/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.408284 xmlschema-2.4.0/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.432284 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.432284 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.432284 xmlschema-2.4.0/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.432284 xmlschema-2.4.0/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.433284 xmlschema-2.4.0/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.433284 xmlschema-2.4.0/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.434284 xmlschema-2.4.0/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.434284 xmlschema-2.4.0/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.434284 xmlschema-2.4.0/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.434284 xmlschema-2.4.0/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.435284 xmlschema-2.4.0/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.435284 xmlschema-2.4.0/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.435284 xmlschema-2.4.0/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.436284 xmlschema-2.4.0/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.436284 xmlschema-2.4.0/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.436284 xmlschema-2.4.0/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.437284 xmlschema-2.4.0/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.437284 xmlschema-2.4.0/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.437284 xmlschema-2.4.0/tests/test_cases/issues/issue_349/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_349/issue_349.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-2.4.0/tests/test_cases/issues/issue_349/issue_349.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.437284 xmlschema-2.4.0/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-2.4.0/tests/test_cases/mypy/extra_validator.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-2.4.0/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-2.4.0/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.438284 xmlschema-2.4.0/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/dummy file #2.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-2.4.0/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-2.4.0/tests/test_cases/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6534 2023-06-14 07:04:00.000000 xmlschema-2.4.0/tests/test_cases/testfiles
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.409284 xmlschema-2.4.0/tests/test_cases/translations/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.438284 xmlschema-2.4.0/tests/test_cases/translations/pl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11973 2021-03-04 20:38:45.000000 xmlschema-2.4.0/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-2.4.0/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28857 2022-08-26 15:33:28.000000 xmlschema-2.4.0/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26556 2023-02-06 08:55:27.000000 xmlschema-2.4.0/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24557 2023-06-14 07:04:00.000000 xmlschema-2.4.0/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-2.4.0/tests/test_files.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    26065 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/test_helpers.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5745 2021-12-08 22:11:41.000000 xmlschema-2.4.0/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9099 2023-02-11 10:41:50.000000 xmlschema-2.4.0/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-03-05 21:16:57.000000 xmlschema-2.4.0/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    70655 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-2.4.0/tests/test_schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5416 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2101 2023-06-14 07:04:00.000000 xmlschema-2.4.0/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-2.4.0/tests/test_validation.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27317 2023-07-11 14:51:58.000000 xmlschema-2.4.0/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2023-02-11 10:41:50.000000 xmlschema-2.4.0/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.439284 xmlschema-2.4.0/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.4.0/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67570 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/validation/test_decoding.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33339 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    18819 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.441284 xmlschema-2.4.0/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-2.4.0/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-2.4.0/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33116 2023-03-05 20:30:24.000000 xmlschema-2.4.0/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-2.4.0/tests/validators/test_elements.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     9464 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_exceptions.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60271 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2022-03-07 13:26:41.000000 xmlschema-2.4.0/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13500 2023-05-18 20:18:16.000000 xmlschema-2.4.0/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19187 2023-02-06 06:20:42.000000 xmlschema-2.4.0/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-2.4.0/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44192 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_simple_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_wildcards.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    33897 2022-07-18 14:19:15.000000 xmlschema-2.4.0/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1553 2023-07-27 19:52:28.000000 xmlschema-2.4.0/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.442284 xmlschema-2.4.0/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2857 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5641 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11669 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.443284 xmlschema-2.4.0/xmlschema/converters/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      813 2022-07-18 14:19:15.000000 xmlschema-2.4.0/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5977 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7228 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19819 2023-07-11 15:21:12.000000 xmlschema-2.4.0/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4769 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5840 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5711 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23717 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35730 2023-07-11 14:51:58.000000 xmlschema-2.4.0/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-2.4.0/xmlschema/exceptions.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.443284 xmlschema-2.4.0/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-2.4.0/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.409284 xmlschema-2.4.0/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.444284 xmlschema-2.4.0/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-2.4.0/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-2.4.0/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24454 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11595 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-2.4.0/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.410284 xmlschema-2.4.0/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.409284 xmlschema-2.4.0/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.444284 xmlschema-2.4.0/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-2.4.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-2.4.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.409284 xmlschema-2.4.0/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.444284 xmlschema-2.4.0/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-2.4.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-2.4.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.410284 xmlschema-2.4.0/xmlschema/locale/pl/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.444284 xmlschema-2.4.0/xmlschema/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.410284 xmlschema-2.4.0/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.445284 xmlschema-2.4.0/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-2.4.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-2.4.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9432 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9907 2023-02-04 20:00:06.000000 xmlschema-2.4.0/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-2.4.0/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    54945 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.410284 xmlschema-2.4.0/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.445284 xmlschema-2.4.0/xmlschema/schemas/DSIG/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.445284 xmlschema-2.4.0/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.445284 xmlschema-2.4.0/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.445284 xmlschema-2.4.0/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.446284 xmlschema-2.4.0/xmlschema/schemas/XENC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/schemas/XENC/xenc-schema-11.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/schemas/XENC/xenc-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.446284 xmlschema-2.4.0/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.446284 xmlschema-2.4.0/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.446284 xmlschema-2.4.0/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.446284 xmlschema-2.4.0/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-2.4.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.447284 xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.447284 xmlschema-2.4.0/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-2.4.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.447284 xmlschema-2.4.0/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30214 2023-06-14 07:04:00.000000 xmlschema-2.4.0/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6911 2022-09-08 10:16:11.000000 xmlschema-2.4.0/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-2.4.0/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.450284 xmlschema-2.4.0/xmlschema/validators/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3557 2021-11-11 15:30:24.000000 xmlschema-2.4.0/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6619 2023-05-07 06:35:13.000000 xmlschema-2.4.0/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34132 2022-09-24 15:52:22.000000 xmlschema-2.4.0/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-2.4.0/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2023-05-07 06:33:55.000000 xmlschema-2.4.0/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64310 2023-06-14 07:04:00.000000 xmlschema-2.4.0/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14973 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31723 2023-07-25 09:47:22.000000 xmlschema-2.4.0/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33050 2023-06-10 06:00:33.000000 xmlschema-2.4.0/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63815 2023-06-14 07:04:00.000000 xmlschema-2.4.0/xmlschema/validators/groups.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     6655 2022-05-20 16:16:20.000000 xmlschema-2.4.0/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    18740 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23474 2023-04-14 13:49:05.000000 xmlschema-2.4.0/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-2.4.0/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6684 2023-05-18 20:18:16.000000 xmlschema-2.4.0/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   104421 2023-07-27 19:52:28.000000 xmlschema-2.4.0/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    61812 2023-07-27 19:52:29.000000 xmlschema-2.4.0/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38290 2022-09-25 07:58:42.000000 xmlschema-2.4.0/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41151 2023-03-05 21:16:57.000000 xmlschema-2.4.0/xmlschema/validators/xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13135 2023-02-11 10:41:50.000000 xmlschema-2.4.0/xmlschema/xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-07-27 20:04:16.442284 xmlschema-2.4.0/xmlschema.egg-info/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7377 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    17913 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2023-07-27 20:04:16.000000 xmlschema-2.4.0/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-2.3.1/CHANGELOG.rst` & `xmlschema-2.4.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v2.4.0`_ (2023-07-27)
+======================
+* Improve schema export using XSD source encoding
+* Add XML signature and encryption to local fallback schemas (issue #357)
+
 `v2.3.1`_ (2023-06-14)
 ======================
 * Meta-schema elements and groups ignore xsi:type attributes (issue #350)
 * Use the meta-schemas only for validating XSD sources otherwise create dummy schemas
 
 `v2.3.0`_ (2023-05-18)
 ======================
@@ -624,7 +629,8 @@
 .. _v2.1.1: https://github.com/brunato/xmlschema/compare/v2.1.0...v2.1.1
 .. _v2.2.0: https://github.com/brunato/xmlschema/compare/v2.1.1...v2.2.0
 .. _v2.2.1: https://github.com/brunato/xmlschema/compare/v2.2.0...v2.2.1
 .. _v2.2.2: https://github.com/brunato/xmlschema/compare/v2.2.1...v2.2.2
 .. _v2.2.3: https://github.com/brunato/xmlschema/compare/v2.2.2...v2.2.3
 .. _v2.3.0: https://github.com/brunato/xmlschema/compare/v2.2.3...v2.3.0
 .. _v2.3.1: https://github.com/brunato/xmlschema/compare/v2.3.0...v2.3.1
+.. _v2.4.0: https://github.com/brunato/xmlschema/compare/v2.3.1...v2.4.0
```

### Comparing `xmlschema-2.3.1/LICENSE` & `xmlschema-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/PKG-INFO` & `xmlschema-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.3.1
+Version: 2.4.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.3.1/README.rst` & `xmlschema-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/Makefile` & `xmlschema-2.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/api.rst` & `xmlschema-2.4.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/components.rst` & `xmlschema-2.4.0/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/conf.py` & `xmlschema-2.4.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 author = 'Davide Brunato'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2.3'
+version = '2.4'
 # The full version, including alpha/beta/rc tags.
-release = '2.3.1'
+release = '2.4.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-2.3.1/doc/converters.rst` & `xmlschema-2.4.0/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/extras.rst` & `xmlschema-2.4.0/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/features.rst` & `xmlschema-2.4.0/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/testing.rst` & `xmlschema-2.4.0/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/doc/usage.rst` & `xmlschema-2.4.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/setup.py` & `xmlschema-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='2.3.1',
+    version='2.4.0',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
             'xmlschema-validate=xmlschema.cli:validate',
             'xmlschema-xml2json=xmlschema.cli:xml2json',
             'xmlschema-json2xml=xmlschema.cli:json2xml',
         ]
     },
     python_requires='>=3.7',
-    install_requires=['elementpath>=4.1.2, <5.0.0'],
+    install_requires=['elementpath>=4.1.5, <5.0.0'],
     extras_require={
-        'codegen': ['elementpath>=4.1.2, <5.0.0', 'jinja2'],
-        'dev': ['tox', 'coverage', 'lxml', 'elementpath>=4.1.2, <5.0.0',
+        'codegen': ['elementpath>=4.1.5, <5.0.0', 'jinja2'],
+        'dev': ['tox', 'coverage', 'lxml', 'elementpath>=4.1.5, <5.0.0',
                 'memory_profiler', 'Sphinx', 'sphinx_rtd_theme', 'jinja2',
                 'flake8', 'mypy', 'lxml-stubs'],
-        'docs': ['elementpath>=4.1.2, <5.0.0', 'Sphinx', 'sphinx_rtd_theme', 'jinja2']
+        'docs': ['elementpath>=4.1.5, <5.0.0', 'Sphinx', 'sphinx_rtd_theme', 'jinja2']
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
     url='https://github.com/sissaschool/xmlschema',
     license='MIT',
     license_file='LICENSE',
     description='An XML Schema validator and decoder',
```

### Comparing `xmlschema-2.3.1/tests/check_memory.py` & `xmlschema-2.4.0/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_all.py` & `xmlschema-2.4.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.py` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-2.4.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-2.4.0/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-2.4.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-2.4.0/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-2.4.0/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-2.4.0/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/data.xml` & `xmlschema-2.4.0/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/data2.xml` & `xmlschema-2.4.0/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/data3.xml` & `xmlschema-2.4.0/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-2.4.0/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-2.4.0/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-2.4.0/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/complex11-restrictions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-2.4.0/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-2.4.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-2.4.0/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/models.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-2.4.0/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-2.4.0/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-2.4.0/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-2.4.0/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-2.4.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_022/README.md` & `xmlschema-2.4.0/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-2.4.0/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-2.4.0/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/issues/issue_349/issue_349.xsd` & `xmlschema-2.4.0/tests/test_cases/issues/issue_349/issue_349.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/mypy/extra_validator.py` & `xmlschema-2.4.0/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/mypy/schema_source.py` & `xmlschema-2.4.0/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/mypy/simple_types.py` & `xmlschema-2.4.0/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cases/testfiles` & `xmlschema-2.4.0/tests/test_cases/testfiles`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_cli.py` & `xmlschema-2.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_codegen.py` & `xmlschema-2.4.0/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_converters.py` & `xmlschema-2.4.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_dataobjects.py` & `xmlschema-2.4.0/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_documents.py` & `xmlschema-2.4.0/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_files.py` & `xmlschema-2.4.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_helpers.py` & `xmlschema-2.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_memory.py` & `xmlschema-2.4.0/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_namespaces.py` & `xmlschema-2.4.0/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_package.py` & `xmlschema-2.4.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_resources.py` & `xmlschema-2.4.0/tests/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from xmlschema.resources import is_url, is_local_url, is_remote_url, \
     url_path_is_file, normalize_locations
 from xmlschema.testing import SKIP_REMOTE_TESTS
 
 
 TEST_CASES_DIR = str(pathlib.Path(__file__).absolute().parent.joinpath('test_cases'))
 
-DRIVE_REGEX = '/[a-zA-Z]:' if platform.system() == 'Windows' else ''
+DRIVE_REGEX = '(/[a-zA-Z]:|/)' if platform.system() == 'Windows' else ''
 
 XML_WITH_NAMESPACES = '<pfa:root xmlns:pfa="http://xmlschema.test/nsa">\n' \
                       '  <pfb:elem xmlns:pfb="http://xmlschema.test/nsb"/>\n' \
                       '</pfa:root>'
 
 
 def casepath(relative_path):
@@ -403,15 +403,15 @@
         )
         self.assertListEqual(locations, [('tns0', 'file:alpha'),
                                          ('tns1', 'http://example.com/beta')])
 
     def test_fetch_resource_function(self):
         with self.assertRaises(ValueError) as ctx:
             fetch_resource('')
-        self.assertIn('argument should contain a not empty string', str(ctx.exception))
+        self.assertIn('argument must contain a not empty string', str(ctx.exception))
 
         wrong_path = casepath('resources/dummy_file.txt')
         self.assertRaises(XMLResourceError, fetch_resource, wrong_path)
 
         wrong_path = casepath('/home/dummy_file.txt')
         self.assertRaises(XMLResourceError, fetch_resource, wrong_path)
 
@@ -1335,15 +1335,15 @@
             </root>""", lazy=False)
         self.assertEqual(set(resource.get_namespaces(root_only=False).keys()),
                          {'default', 'tns', 'tns0'})
 
         resource = XMLResource('<root/>')
         with self.assertRaises(ValueError) as ctx:
             resource.get_namespaces(namespaces={'xml': "http://example.com/ne"})
-        self.assertIn("reserved prefix (xml)", str(ctx.exception))
+        self.assertIn("reserved prefix 'xml'", str(ctx.exception))
 
     def test_xml_resource_get_locations(self):
         resource = XMLResource(self.col_xml_file)
         self.check_url(resource.url, normalize_url(self.col_xml_file))
 
         locations = resource.get_locations([('ns', 'other.xsd')])
         self.assertEqual(len(locations), 2)
```

### Comparing `xmlschema-2.3.1/tests/test_schemas.py` & `xmlschema-2.4.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_translations.py` & `xmlschema-2.4.0/tests/test_translations.py`

 * *Files 20% similar despite different names*

```diff
@@ -85,14 +85,54 @@
             translation.activate(languages=['en', 'it'])
             self.assertIsInstance(translation._translation, gettext.GNUTranslations)
             result = translation.gettext("not a redefinition!")
             self.assertEqual(result, "not a redefinition!")
         finally:
             translation._translation = None
 
+    def test_pl_translation(self):
+        self.assertIsNone(translation._translation)
+        try:
+            translation.activate(languages=['pl'])
+            self.assertIsInstance(translation._translation, gettext.GNUTranslations)
+            result = translation.gettext("The content of element %r is not complete.")
+            self.assertEqual(result, "Zawartość elementu %r nie jest kompletna.")
+        finally:
+            translation._translation = None
+
+        try:
+            translation.activate(languages=['pl', 'en'])
+            self.assertIsInstance(translation._translation, gettext.GNUTranslations)
+            result = translation.gettext("The content of element %r is not complete.")
+            self.assertEqual(result, "Zawartość elementu %r nie jest kompletna.")
+        finally:
+            translation._translation = None
+
+    def test_pl_validation_translation(self):
+        xml_path = "tests//test_cases//translations//pl//tytul_wykonawczy_niekompletny.xml"
+        xsd_path = "tests//test_cases//translations//pl//tw-1(5)8e.xsd"
+        expected_errors = [
+            "Zawartość elementu 'com:Opisowy' nie jest kompletna. "
+            "Oczekiwany znacznik 'com:Miejscowosc'.",
+            "atrybut rodzaj='8': wartość musi być jedną z [1, 2]",
+            "Zawartość elementu 'com:Beneficjent' nie jest kompletna. "
+            "Oczekiwany znacznik 'com:NrRachunkuPL'.",
+        ]
+        try:
+            translation.activate(languages=['pl'])
+            schema = XMLSchema(
+                xsd_path,
+                defuse="never",
+                validation="lax",
+            )
+            errors = [error.reason for error in schema.iter_errors(xml_path)]
+            assert errors == expected_errors
+        finally:
+            translation._translation = None
+
 
 if __name__ == '__main__':
     import platform
 
     header_template = "Test xmlschema translations with Python {} on {}"
     header = header_template.format(platform.python_version(), platform.platform())
     print('{0}\n{1}\n{0}'.format("*" * len(header), header))
```

### Comparing `xmlschema-2.3.1/tests/test_typing.py` & `xmlschema-2.4.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_validation.py` & `xmlschema-2.4.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_w3c_suite.py` & `xmlschema-2.4.0/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_wsdl.py` & `xmlschema-2.4.0/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/test_xpath.py` & `xmlschema-2.4.0/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validation/test_decoding.py` & `xmlschema-2.4.0/tests/validation/test_decoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,23 @@
             },
             'position': 2,
             'title': None,
             'year': '1925'
     }]
 }
 
+MENU_DICT = {
+    '@xmlns:xsi': 'http://www.w3.org/2001/XMLSchema-instance',
+    '@xsi:noNamespaceSchemaLocation': 'menù.xsd',
+    'antipasto': ['Affettati misti', 'Bruschetta', 'Polenta e funghi'],
+    'primo': ['Lasagne', 'Gnocchi al ragù', 'Risotto allo zafferano'],
+    'secondo': ['Tagliata di pollo', 'Cotoletta alla milanese', 'Caprese'],
+    'dolce': ['Crostata ai mirtilli', 'Tiramisù']
+}
+
 COLLECTION_PARKER = {
     'object': [{'author': {'born': '1841-02-25',
                            'dead': '1919-12-03',
                            'name': 'Pierre-Auguste Renoir',
                            'qualification': 'painter'},
                 'estimation': 10000.0,
                 'position': 1,
@@ -1459,14 +1468,39 @@
                  'choice_elem1': None,
                  'choice_elem2': None,  # this is wrong (at most one element for a choice)
              }}
         ]}
         xml_dict = schema.decode(xml_file, element_hook=fill_missing_content, fill_missing=True)
         self.assertDictEqual(xml_dict, expected)
 
+    def test_decoding_non_unicode_files(self):
+        # Using cp1252 encoded XSD
+        schema_file = self.casepath('examples/menù/menù-cp1252.xsd')
+        schema = self.schema_class(schema_file)
+
+        xml_file = self.casepath('examples/menù/menù-cp1252.xml')
+        self.assertDictEqual(schema.decode(xml_file), MENU_DICT)
+
+        xml_file = self.casepath('examples/menù/menù-ascii.xml')
+        with self.assertRaises(ElementTree.ParseError):
+            schema.decode(xml_file)  # Invalid XML file (entity in a tag name)
+
+        xml_file = self.casepath('examples/menù/menù.xml')
+        self.assertDictEqual(schema.decode(xml_file), MENU_DICT)
+
+        # Using ASCII encoded XSD
+        schema_file = self.casepath('examples/menù/menù-ascii.xsd')
+        schema = self.schema_class(schema_file)
+
+        xml_file = self.casepath('examples/menù/menù-cp1252.xml')
+        self.assertDictEqual(schema.decode(xml_file), MENU_DICT)
+
+        xml_file = self.casepath('examples/menù/menù.xml')
+        self.assertDictEqual(schema.decode(xml_file), MENU_DICT)
+
 
 class TestDecoding11(TestDecoding):
     schema_class = XMLSchema11
 
     def test_datetime_types(self):
         xs = self.get_schema('<xs:element name="dt" type="xs:dateTime"/>')
         self.assertEqual(xs.decode('<dt>2019-01-01T13:40:00</dt>'), '2019-01-01T13:40:00')
```

### Comparing `xmlschema-2.3.1/tests/validation/test_encoding.py` & `xmlschema-2.4.0/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validation/test_validation.py` & `xmlschema-2.4.0/tests/validation/test_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -351,14 +351,49 @@
             'xsi:type="non-empty-string"></root>'
         ))
         self.assertTrue(schema.is_valid(
             '<root xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
             'xsi:type="non-empty-string">foo</root>'
         ))
 
+    def test_issue_356__validate_empty_simple_elements(self):
+        schema = xmlschema.XMLSchema(dedent("""\
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+
+                <xs:element name="root1" type="emptyString" />
+                <xs:element name="root2" type="emptyList" />
+                <xs:element name="root3" type="emptiableUnion" />
+
+                <xs:simpleType name="emptyString">
+                    <xs:restriction base='xs:string'>
+                      <xs:length value="0"/>
+                    </xs:restriction>
+                </xs:simpleType>
+
+                <xs:simpleType name="emptyList">
+                    <xs:list itemType="emptyString"/>
+                </xs:simpleType>
+
+                <xs:simpleType name="emptiableUnion">
+                    <xs:union memberTypes="xs:int emptyString"/>
+                </xs:simpleType>
+
+            </xs:schema>"""))
+
+        self.assertTrue(schema.is_valid('<root1></root1>'))
+        self.assertFalse(schema.is_valid('<root1>foo</root1>'))
+
+        self.assertTrue(schema.is_valid('<root2></root2>'))
+        self.assertFalse(schema.is_valid('<root2>foo</root2>'))
+        self.assertFalse(schema.is_valid('<root2>foo bar</root2>'))
+
+        self.assertTrue(schema.is_valid('<root3>1</root3>'))
+        self.assertTrue(schema.is_valid('<root3></root3>'))
+        self.assertFalse(schema.is_valid('<root3>foo</root3>'))
+
 
 class TestValidation11(TestValidation):
     schema_class = XMLSchema11
 
     def test_default_attributes(self):
         xs = self.schema_class(self.casepath('features/attributes/default_attributes.xsd'))
         self.assertTrue(xs.is_valid("<tree xmlns='ns'>\n"
```

### Comparing `xmlschema-2.3.1/tests/validators/test_attributes.py` & `xmlschema-2.4.0/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_builtins.py` & `xmlschema-2.4.0/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_complex_types.py` & `xmlschema-2.4.0/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_elements.py` & `xmlschema-2.4.0/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_exceptions.py` & `xmlschema-2.4.0/tests/validators/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_facets.py` & `xmlschema-2.4.0/tests/validators/test_facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_global_maps.py` & `xmlschema-2.4.0/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_groups.py` & `xmlschema-2.4.0/tests/validators/test_groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_identities.py` & `xmlschema-2.4.0/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_models.py` & `xmlschema-2.4.0/tests/validators/test_models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_notations.py` & `xmlschema-2.4.0/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_particles.py` & `xmlschema-2.4.0/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_schemas.py` & `xmlschema-2.4.0/tests/validators/test_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import unittest
+import filecmp
 import logging
 import tempfile
 import warnings
 import pathlib
 import pickle
 import platform
 import glob
@@ -802,14 +803,44 @@
                 exported_schema,
                 original_schema.replace('https://raw.githubusercontent.com',
                                         dirname.replace('\\', '/') + '/raw.githubusercontent.com')
             )
 
         self.assertFalse(os.path.isdir(dirname))
 
+    @unittest.skipIf(platform.system() == 'Windows', 'skip, Windows systems save with <CR><LF>')
+    def test_export_other_encoding(self):
+        schema_file = self.casepath('examples/menù/menù.xsd')
+        schema_ascii_file = self.casepath('examples/menù/menù-ascii.xsd')
+        schema_cp1252_file = self.casepath('examples/menù/menù-cp1252.xsd')
+
+        schema = self.schema_class(schema_file)
+        with tempfile.TemporaryDirectory() as dirname:
+            schema.export(target=dirname)
+            exported_schema = pathlib.Path(dirname).joinpath('menù.xsd')
+            self.assertTrue(filecmp.cmp(schema_file, exported_schema))
+            self.assertFalse(filecmp.cmp(schema_ascii_file, exported_schema))
+            self.assertFalse(filecmp.cmp(schema_cp1252_file, exported_schema))
+
+        schema = self.schema_class(schema_ascii_file)
+        with tempfile.TemporaryDirectory() as dirname:
+            schema.export(target=dirname)
+            exported_schema = pathlib.Path(dirname).joinpath('menù-ascii.xsd')
+            self.assertFalse(filecmp.cmp(schema_file, exported_schema))
+            self.assertTrue(filecmp.cmp(schema_ascii_file, exported_schema))
+            self.assertFalse(filecmp.cmp(schema_cp1252_file, exported_schema))
+
+        schema = self.schema_class(schema_cp1252_file)
+        with tempfile.TemporaryDirectory() as dirname:
+            schema.export(target=dirname)
+            exported_schema = pathlib.Path(dirname).joinpath('menù-cp1252.xsd')
+            self.assertFalse(filecmp.cmp(schema_file, exported_schema))
+            self.assertFalse(filecmp.cmp(schema_ascii_file, exported_schema))
+            self.assertTrue(filecmp.cmp(schema_cp1252_file, exported_schema))
+
     def test_pickling_subclassed_schema__issue_263(self):
         cases_dir = pathlib.Path(__file__).parent.parent
         schema_file = cases_dir.joinpath('test_cases/examples/vehicles/vehicles.xsd')
         xml_file = cases_dir.joinpath('test_cases/examples/vehicles/vehicles.xml')
 
         schema = self.CustomXMLSchema(str(schema_file))
         self.assertTrue(schema.is_valid(str(xml_file)))
@@ -850,14 +881,32 @@
         with self.assertRaises(XMLSchemaParseError) as ec:
             self.schema_class(schema_file)
 
         error_message = str(ec.exception)
         self.assertIn("the QName 'testAttribute3' is mapped to no namespace", error_message)
         self.assertIn("requires that there is an xs:import statement", error_message)
 
+    @unittest.skipIf(SKIP_REMOTE_TESTS, "Remote networks are not accessible.")
+    def test_import_dsig_namespace__issue_357(self):
+        location = 'https://www.w3.org/TR/2008/REC-xmldsig-core-20080610/xmldsig-core-schema.xsd'
+        dsig_namespace = 'http://www.w3.org/2000/09/xmldsig#'
+
+        schema = self.schema_class(dedent(f"""<?xml version="1.0" encoding="UTF-8"?>
+            <!-- Test import of defused data from remote with a fallback.-->
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+                <xs:import namespace="{dsig_namespace}"
+                    schemaLocation="{location}"/>
+                <xs:element name="root"/>
+            </xs:schema>"""))
+
+        self.assertIn(dsig_namespace, schema.maps.namespaces)
+        url = schema.maps.namespaces[dsig_namespace][0].url
+        self.assertIsInstance(url, str)
+        self.assertTrue(url.endswith('schemas/DSIG/xmldsig-core-schema.xsd'))
+
 
 class TestXMLSchema11(TestXMLSchema10):
 
     schema_class = XMLSchema11
 
     class CustomXMLSchema(XMLSchema11):
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmlschema-2.3.1/tests/validators/test_simple_types.py` & `xmlschema-2.4.0/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_wildcards.py` & `xmlschema-2.4.0/tests/validators/test_wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tests/validators/test_xsdbase.py` & `xmlschema-2.4.0/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/tox.ini` & `xmlschema-2.4.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tox]
-envlist = py{37,38,39,310,311,312,py3}, docs,
-    flake8, mypy-py{37,38,39,310,311,312,py3}, coverage, pytest
+envlist = flake8, py{37,38,39,310,311,312,py3}, docs,
+    mypy-py{37,38,39,310,311,312,py3}, coverage, pytest
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/xmlschema
 
 [testenv]
 deps =
-    elementpath>=4.1.2, <5.0.0
+    elementpath>=4.1.5, <5.0.0
     lxml
     jinja2
     py{310,311}: memory_profiler
     docs: Sphinx
     docs: sphinx_rtd_theme
     coverage: coverage
 commands =
     python -m unittest
 
 [testenv:py312]
 deps =
-    elementpath>=4.1.2, <5.0.0
-    # lxml: skip for now
+    elementpath>=4.1.5, <5.0.0
+    lxml
     jinja2
 
 [testenv:docs]
 commands =
     make -C doc html SPHINXOPTS="-W -n"
     make -C doc latexpdf SPHINXOPTS="-W -n"
     make -C doc doctest SPHINXOPTS="-W -n"
@@ -38,25 +38,25 @@
     flake8
 commands =
     flake8 xmlschema
     flake8 tests
 
 [testenv:mypy-py37]
 deps =
-    mypy==1.3.0
-    elementpath==4.1.2
+    mypy==1.4.1
+    elementpath==4.1.5
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
 
 [testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.3.0
-    elementpath==4.1.2
+    mypy==1.4.1
+    elementpath==4.1.5
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
     python tests/test_typing.py
 
 [testenv:coverage]
@@ -65,18 +65,18 @@
     coverage run -a -m unittest
     coverage report -m
 
 [testenv:pytest]
 deps =
     pytest
     pytest-randomly
-    elementpath>=4.1.2, <5.0.0
+    elementpath>=4.1.5, <5.0.0
     lxml
     jinja2
-    mypy==1.3.0
+    mypy==1.4.1
     lxml-stubs
 commands =
     pytest tests -ra
 
 [testenv:build]
 deps =
     setuptools
```

### Comparing `xmlschema-2.3.1/xmlschema/__init__.py` & `xmlschema-2.4.0/xmlschema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaIncludeWarning, XMLSchemaImportWarning, XMLSchemaTypeTableWarning,
     XsdGlobals, XMLSchemaBase, XMLSchema, XMLSchema10, XMLSchema11,
     XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '2.3.1'
+__version__ = '2.4.0'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-2.3.1/xmlschema/aliases.py` & `xmlschema-2.4.0/xmlschema/aliases.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,17 @@
     XPathElementType = Union[XsdElement, XsdAnyElement, XsdAssert]
 
     C = TypeVar('C')
     GlobalMapType = Dict[str, Union[C, Tuple[ElementType, SchemaType]]]
 
     ##
     # Type aliases for datatypes
-    AtomicValueType = Union[str, int, float, Decimal, bool, Integer, Float10, NormalizedString,
-                            AnyURI, HexBinary, Base64Binary, QName, Duration, OrderedDateTime, Time]
+    AtomicValueType = Union[str, bytes, int, float, Decimal, bool, Integer,
+                            Float10, NormalizedString, AnyURI, HexBinary,
+                            Base64Binary, QName, Duration, OrderedDateTime, Time]
     NumericValueType = Union[str, bytes, int, float, Decimal]
     DateTimeType = Union[OrderedDateTime, Time]
 
     ##
     # Type aliases for validation/decoding/encoding
     ConverterType = Union[Type[XMLSchemaConverter], XMLSchemaConverter]
     ExtraValidatorType = Callable[[ElementType, XsdElement],
@@ -96,16 +97,17 @@
     E = TypeVar('E')
     EncodeType = Union[E, Tuple[E, List[XMLSchemaValidationError]]]
     IterEncodeType = Iterator[Union[E, XMLSchemaValidationError]]
 
     JsonDecodeType = Union[str, None, Tuple[XMLSchemaValidationError, ...],
                            Tuple[Union[str, None], Tuple[XMLSchemaValidationError, ...]]]
 
-    DecodedValueType = Union[None, AtomicValueType, List[AtomicValueType]]
-    EncodedValueType = Union[None, str, List[str]]
+    DecodedValueType = Union[None, AtomicValueType, List[Optional[AtomicValueType]],
+                             XMLSchemaValidationError]
+    EncodedValueType = Union[None, str, List[str], XMLSchemaValidationError]
 
     FillerType = Callable[[Union[XsdElement, XsdAttribute]], Any]
     DepthFillerType = Callable[[XsdElement], Any]
     ValueHookType = Callable[[AtomicValueType, BaseXsdType], Any]
     ElementHookType = Callable[
         [ElementData, Optional[XsdElement], Optional[BaseXsdType]], ElementData
     ]
```

### Comparing `xmlschema-2.3.1/xmlschema/cli.py` & `xmlschema-2.4.0/xmlschema/cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/__init__.py` & `xmlschema-2.4.0/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/abdera.py` & `xmlschema-2.4.0/xmlschema/converters/abdera.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/badgerfish.py` & `xmlschema-2.4.0/xmlschema/converters/badgerfish.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/columnar.py` & `xmlschema-2.4.0/xmlschema/converters/columnar.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/default.py` & `xmlschema-2.4.0/xmlschema/converters/default.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/jsonml.py` & `xmlschema-2.4.0/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/parker.py` & `xmlschema-2.4.0/xmlschema/converters/parker.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/converters/unordered.py` & `xmlschema-2.4.0/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/dataobjects.py` & `xmlschema-2.4.0/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/documents.py` & `xmlschema-2.4.0/xmlschema/documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/exceptions.py` & `xmlschema-2.4.0/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/extras/codegen.py` & `xmlschema-2.4.0/xmlschema/extras/codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-2.4.0/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-2.4.0/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/extras/wsdl.py` & `xmlschema-2.4.0/xmlschema/extras/wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/helpers.py` & `xmlschema-2.4.0/xmlschema/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # @author Davide Brunato <brunato@sissa.it>
 #
 import re
 from collections import Counter
 from decimal import Decimal
 from typing import Any, Callable, Iterator, List, MutableMapping, \
     Optional, Tuple, Union
+from xml.etree.ElementTree import ParseError
+
 from .exceptions import XMLSchemaValueError, XMLSchemaTypeError
 from .names import XSI_SCHEMA_LOCATION, XSI_NONS_SCHEMA_LOCATION
 from .aliases import ElementType, NamespacesType, AtomicValueType, NumericValueType
 
 ###
 # Helper functions for QNames
 
@@ -317,7 +319,21 @@
     """Encodes a simple value to XML."""
     if isinstance(value, bool):
         return 'true' if value else 'false'
     elif isinstance(value, (list, tuple)):
         return ' '.join(str(e) for e in value)
     else:
         return str(value) if value is not None else None
+
+
+def is_defuse_error(err: Exception) -> bool:
+    """
+    Returns `True` if the error is related to defuse of XML data in the DTD
+    of the source (forbid entities or external references), `False` otherwise.
+    """
+    if not isinstance(err, ParseError):
+        return False
+
+    msg = str(err)
+    return "Entities are forbidden" in msg or \
+        "Unparsed entities are forbidden" in msg or \
+        "External references are forbidden" in msg
```

### Comparing `xmlschema-2.3.1/xmlschema/limits.py` & `xmlschema-2.4.0/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.4.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-2.4.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.4.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-2.4.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-2.4.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-2.4.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/names.py` & `xmlschema-2.4.0/xmlschema/names.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,40 +36,54 @@
 HFP_NAMESPACE = 'http://www.w3.org/2001/XMLSchema-hasFacetAndProperty'
 "URI of the XML Schema has Facet and Property namespace (hfp)"
 
 VC_NAMESPACE = 'http://www.w3.org/2007/XMLSchema-versioning'
 "URI of the XML Schema Versioning namespace (vc)"
 
 ###
-# Namespace URIs for XML documents
+# Namespaces for WSDL documents
 WSDL_NAMESPACE = 'http://schemas.xmlsoap.org/wsdl/'
 SOAP_NAMESPACE = 'http://schemas.xmlsoap.org/wsdl/soap/'
 SOAP_ENVELOPE_NAMESPACE = 'http://schemas.xmlsoap.org/soap/envelope/'
 SOAP_ENCODING_NAMESPACE = 'http://schemas.xmlsoap.org/soap/encoding/'
 
+###
+# Namespaces for XML Signature Syntax and Processing
+DSIG_NAMESPACE = 'http://www.w3.org/2000/09/xmldsig#'
+DSIG11_NAMESPACE = 'http://www.w3.org/2009/xmldsig11#'
+
+###
+# Namespaces for XML Encryption Syntax and Processing
+XENC_NAMESPACE = 'http://www.w3.org/2001/04/xmlenc#'
+XENC11_NAMESPACE = 'http://www.w3.org/2009/xmlenc11#'
+
 
 ###
 # Schema location hints
 
 SCHEMAS_DIR = os.path.join(os.path.dirname(__file__), 'schemas/')
 
 LOCATION_HINTS = {
     # Locally saved schemas
-    # HFP_NAMESPACE: os.path.join(SCHEMAS_DIR, 'HFP/XMLSchema-hasFacetAndProperty_minimal.xsd'),
+    HFP_NAMESPACE: os.path.join(SCHEMAS_DIR, 'HFP/XMLSchema-hasFacetAndProperty_minimal.xsd'),
     VC_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XSI/XMLSchema-versioning.xsd'),
     XLINK_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XLINK/xlink.xsd'),
     XHTML_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XHTML/xhtml1-strict.xsd'),
     WSDL_NAMESPACE: os.path.join(SCHEMAS_DIR, 'WSDL/wsdl.xsd'),
     SOAP_NAMESPACE: os.path.join(SCHEMAS_DIR, 'WSDL/wsdl-soap.xsd'),
     SOAP_ENVELOPE_NAMESPACE: os.path.join(SCHEMAS_DIR, 'WSDL/soap-envelope.xsd'),
     SOAP_ENCODING_NAMESPACE: os.path.join(SCHEMAS_DIR, 'WSDL/soap-encoding.xsd'),
+    DSIG_NAMESPACE: os.path.join(SCHEMAS_DIR, 'DSIG/xmldsig-core-schema.xsd'),
+    DSIG11_NAMESPACE: os.path.join(SCHEMAS_DIR, 'DSIG/xmldsig11-schema.xsd'),
+    XENC_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XENC/xenc-schema.xsd'),
+    XENC11_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XENC/xenc-schema-11.xsd'),
 
     # Remote locations: contributors can propose additional official locations
     # for other namespaces for extending this list.
-    XSLT_NAMESPACE: os.path.join(SCHEMAS_DIR, 'http://www.w3.org/2007/schema-for-xslt20.xsd'),
+    XSLT_NAMESPACE: 'http://www.w3.org/2007/schema-for-xslt20.xsd',
 }
 
 
 ###
 # Elements and attributes names
 
 _VC_TEMPLATE = '{http://www.w3.org/2007/XMLSchema-versioning}%s'
```

### Comparing `xmlschema-2.3.1/xmlschema/namespaces.py` & `xmlschema-2.4.0/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/resources.py` & `xmlschema-2.4.0/xmlschema/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,70 +187,63 @@
 
 
 def is_url(obj: object) -> bool:
     """Returns `True` if the provided object is a URL, `False` otherwise."""
     if isinstance(obj, str):
         if '\n' in obj or obj.lstrip().startswith('<'):
             return False
-        try:
-            urlsplit(obj.strip())
-        except ValueError:
-            return False
     elif isinstance(obj, bytes):
         if b'\n' in obj or obj.lstrip().startswith(b'<'):
             return False
-        try:
-            urlsplit(obj.strip())
-        except ValueError:  # pragma: no cover
-            return False
     else:
         return isinstance(obj, Path)
 
-    return True
+    try:
+        urlsplit(obj.strip())  # type: ignore
+    except ValueError:  # pragma: no cover
+        return False
+    else:
+        return True
 
 
 def is_remote_url(obj: object) -> bool:
     if isinstance(obj, str):
         if '\n' in obj or obj.lstrip().startswith('<'):
             return False
-        try:
-            return not is_local_scheme(urlsplit(obj.strip()).scheme)
-        except ValueError:  # pragma: no cover
-            return False
-
+        url = obj.strip()
     elif isinstance(obj, bytes):
         if b'\n' in obj or obj.lstrip().startswith(b'<'):
             return False
-        try:
-            return not is_local_scheme(urlsplit(obj.strip().decode('utf-8')).scheme)
-        except ValueError:  # pragma: no cover
-            return False
+        url = obj.strip().decode('utf-8')
     else:
         return False
 
+    try:
+        return not is_local_scheme(urlsplit(url).scheme)
+    except ValueError:  # pragma: no cover
+        return False
+
 
 def is_local_url(obj: object) -> bool:
     if isinstance(obj, str):
         if '\n' in obj or obj.lstrip().startswith('<'):
             return False
-        try:
-            return is_local_scheme(urlsplit(obj.strip()).scheme)
-        except ValueError:  # pragma: no cover
-            return False
-
+        url = obj.strip()
     elif isinstance(obj, bytes):
         if b'\n' in obj or obj.lstrip().startswith(b'<'):
             return False
-        try:
-            return is_local_scheme(urlsplit(obj.strip().decode('utf-8')).scheme)
-        except ValueError:  # pragma: no cover
-            return False
+        url = obj.strip().decode('utf-8')
     else:
         return isinstance(obj, Path)
 
+    try:
+        return is_local_scheme(urlsplit(url).scheme)
+    except ValueError:  # pragma: no cover
+        return False
+
 
 def url_path_is_file(url: str) -> bool:
     if not is_local_url(url):
         return False
     if os.path.isfile(url):
         return True
     path = unquote(urlsplit(normalize_url(url)).path)
@@ -298,15 +291,15 @@
 
     :param location: a URL or a file path.
     :param base_url: reference base URL for normalizing local and relative URLs.
     :param timeout: the timeout in seconds for the connection attempt in case of remote data.
     :return: a normalized URL.
     """
     if not location:
-        raise XMLSchemaValueError("'location' argument should contain a not empty string")
+        raise XMLSchemaValueError("the 'location' argument must contain a not empty string")
 
     url = normalize_url(location, base_url)
     try:
         with urlopen(url, timeout=timeout):
             return url
     except URLError as err:
         # fallback joining the path without a base URL
@@ -351,23 +344,23 @@
         resource = source
 
     base_url = resource.base_url
     namespace = resource.namespace
     locations = resource.get_locations(locations, root_only=False)
     if not locations:
         msg = "%r does not contain any schema location hint"
-        raise XMLSchemaValueError(msg % source)
+        raise XMLSchemaValueError(msg % resource)
 
     for ns, url in sorted(locations, key=lambda x: x[0] != namespace):
         try:
             return fetch_resource(url, base_url, timeout), locations
         except XMLResourceError:
             pass
 
-    raise XMLSchemaValueError("not found a schema for XML data resource %r" % source)
+    raise XMLSchemaValueError("not found a schema for %r" % resource)
 
 
 def fetch_schema(source: Union['XMLResource', XMLSourceType],
                  locations: Optional[LocationsType] = None,
                  base_url: Optional[str] = None,
                  allow: str = 'all',
                  defuse: str = 'remote',
@@ -434,24 +427,20 @@
     def __init__(self, source: XMLSourceType,
                  base_url: Union[None, str, Path, bytes] = None,
                  allow: str = 'all',
                  defuse: str = 'remote',
                  timeout: int = 300,
                  lazy: Union[bool, int] = False) -> None:
 
-        if isinstance(base_url, str):
+        if isinstance(base_url, (str, bytes)):
             if not is_url(base_url):
                 raise XMLSchemaValueError("'base_url' argument is not an URL")
-            self._base_url = base_url
+            self._base_url = base_url if isinstance(base_url, str) else base_url.decode()
         elif isinstance(base_url, Path):
             self._base_url = str(base_url)
-        elif isinstance(base_url, bytes):
-            if not is_url(base_url):
-                raise XMLSchemaValueError("'base_url' argument is not an URL")
-            self._base_url = base_url.decode()
         elif base_url is not None:
             msg = "invalid type %r for argument 'base_url'"
             raise XMLSchemaTypeError(msg % type(base_url))
 
         if not isinstance(allow, str):
             msg = "invalid type %r for argument 'allow'"
             raise XMLSchemaTypeError(msg % type(allow))
@@ -578,15 +567,15 @@
 
     def _update_nsmap(self, nsmap: MutableMapping[str, str], prefix: str, uri: str) -> None:
         if not prefix:
             if not uri:
                 return
             elif '' not in nsmap:
                 if self.namespace:
-                    nsmap[prefix] = uri
+                    nsmap[''] = uri
                     return
             elif nsmap[''] == uri:
                 return
             prefix = 'default'
 
         while prefix in nsmap:
             if nsmap[prefix] == uri:
@@ -633,17 +622,17 @@
                 if event == 'start':
                     if not root_started:
                         self._root = node
                         self._xpath_root = LazyElementNode(
                             self._root, nsmap={k: v for k, v in _nsmap}
                         )
                         root_started = True
-                    if nsmap_update and isinstance(nsmap, dict):
+                    if nsmap_update:
                         for prefix, uri in _nsmap:
-                            self._update_nsmap(nsmap, prefix, uri)
+                            self._update_nsmap(nsmap, prefix, uri)  # type: ignore[arg-type]
                         nsmap_update = False
                     yield event, node
 
                 elif event == 'end':
                     yield event, node
                 elif nsmap is not None:
                     if event == 'start-ns':
@@ -795,15 +784,15 @@
                     url = None
 
             self._parse_resource(cast(IO[str], source), url, lazy)
             self._text = None
             self._lazy = lazy
 
         else:
-            # Source is already an Element or an ElementTree.
+            # source is an Element or an ElementTree
             if hasattr(source, 'tag') and hasattr(source, 'attrib'):
                 # Source is already an Element --> nothing to parse
                 self._root = cast(ElementType, source)
             elif is_etree_document(source):
                 # Could be only an ElementTree object at last
                 self._root = source.getroot()
             else:
@@ -830,57 +819,52 @@
 
         self._parent_map = None
         self._source = source
 
     @property
     def namespace(self) -> str:
         """The namespace of the XML resource."""
-        return '' if self._root is None else get_namespace(self._root.tag)
+        return get_namespace(self._root.tag)
 
     @property
     def parent_map(self) -> Dict[ElementType, Optional[ElementType]]:
         if self._lazy:
             raise XMLResourceError("cannot create the parent map of a lazy XML resource")
         if self._parent_map is None:
-            assert self._root is not None
             self._parent_map = {child: elem for elem in self._root.iter() for child in elem}
             self._parent_map[self._root] = None
         return self._parent_map
 
-    def _build_node_tree(self, namespaces: Optional[NamespacesType] = None) \
-            -> Union[DocumentNode, ElementNode]:
-        """Build a node tree for non-lazy resources."""
-        if hasattr(self._root, 'xpath'):
-            return build_lxml_node_tree(cast(LxmlElementProtocol, self._root))
-        else:
-            try:
-                _nsmap = self._nsmap[self._root]
-            except KeyError:
-                # A resource based on an ElementTree structure (no namespace maps)
-                return build_node_tree(self._root, namespaces)
-            else:
-                _namespaces: Any = {pfx: uri for pfx, uri in _nsmap}
-                node_tree = build_node_tree(self._root, _namespaces)
-
-                # Update namespace maps
-                for node in node_tree.iter_descendants(with_self=False):
-                    if isinstance(node, ElementNode):
-                        elem_nsmap = self._nsmap[cast(ElementType, node.elem)]
-                        if _nsmap is not elem_nsmap:
-                            _nsmap = elem_nsmap
-                            _namespaces = {pfx: uri for pfx, uri in _nsmap}
-                        node.nsmap = _namespaces
-
-                return node_tree
-
     @property
     def xpath_root(self) -> Union[ElementNode, DocumentNode]:
         """The XPath root node."""
         if self._xpath_root is None:
-            self._xpath_root = self._build_node_tree()
+            if hasattr(self._root, 'xpath'):
+                self._xpath_root = build_lxml_node_tree(cast(LxmlElementProtocol, self._root))
+            else:
+                try:
+                    _nsmap = self._nsmap[self._root]
+                except KeyError:
+                    # A resource based on an ElementTree structure (no namespace maps)
+                    self._xpath_root = build_node_tree(self._root)
+                else:
+                    _namespaces: Any = {pfx: uri for pfx, uri in _nsmap}
+                    node_tree = build_node_tree(self._root, _namespaces)
+
+                    # Update namespace maps
+                    for node in node_tree.iter_descendants(with_self=False):
+                        if isinstance(node, ElementNode):
+                            elem_nsmap = self._nsmap[cast(ElementType, node.elem)]
+                            if _nsmap is not elem_nsmap:
+                                _nsmap = elem_nsmap
+                                _namespaces = {pfx: uri for pfx, uri in _nsmap}
+                            node.nsmap = _namespaces
+
+                    self._xpath_root = node_tree
+
         return self._xpath_root
 
     def get_xpath_node(self, elem: ElementType) -> ElementNode:
         """
         Returns an XPath node for the element, fetching it from the XPath root node.
         Returns a new lazy element node if the matching element node is not found.
         """
@@ -1337,15 +1321,15 @@
         :param root_only: if `True`, or `None` and the resource is lazy, extracts \
         only the namespaces declared in the root element.
         :return: a dictionary for mapping namespace prefixes to full URI.
         """
         if namespaces is None:
             namespaces = {}
         elif namespaces.get('xml', XML_NAMESPACE) != XML_NAMESPACE:
-            msg = "reserved prefix (xml) must not be bound to another namespace name"
+            msg = "reserved prefix 'xml' can't be used for another namespace name"
             raise XMLSchemaValueError(msg)
         else:
             namespaces = copy.copy(namespaces)
 
         try:
             if root_only or root_only is None and self._lazy:
                 for _elem in self.iter(nsmap=namespaces):
```

### Comparing `xmlschema-2.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-2.4.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-2.4.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-2.4.0/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-2.4.0/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-2.4.0/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-2.4.0/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-2.4.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/testing/__init__.py` & `xmlschema-2.4.0/xmlschema/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,23 @@
     get_test_program_args_parser, get_test_line_args_parser, factory_tests
 from ._observers import SchemaObserver, ObservedXMLSchema10, ObservedXMLSchema11
 
 
 def has_network_access(*locations):
     for url in locations:
         try:
-            urlopen(url, timeout=5)
+            urlopen(url, timeout=10)
         except (URLError, OSError):
             pass
         else:
             return True
     return False
 
 
-SKIP_REMOTE_TESTS = not has_network_access(
-    'https://github.com/', 'https://www.w3.org/', 'https://www.sissa.it/'
-)
+SKIP_REMOTE_TESTS = not has_network_access('https://github.com/')
 
 
 __all__ = [
     'XsdValidatorTestCase', 'make_schema_test_class', 'make_validation_test_class',
     'get_test_args', 'xsd_version_number', 'defuse_data', 'get_test_program_args_parser',
     'get_test_line_args_parser', 'factory_tests', 'SchemaObserver', 'ObservedXMLSchema10',
     'ObservedXMLSchema11', 'has_network_access', 'iter_nested_items',
```

### Comparing `xmlschema-2.3.1/xmlschema/testing/_builders.py` & `xmlschema-2.4.0/xmlschema/testing/_builders.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/testing/_case_class.py` & `xmlschema-2.4.0/xmlschema/testing/_case_class.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/testing/_factory.py` & `xmlschema-2.4.0/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/testing/_helpers.py` & `xmlschema-2.4.0/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/testing/_observers.py` & `xmlschema-2.4.0/xmlschema/testing/_observers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/translation.py` & `xmlschema-2.4.0/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/__init__.py` & `xmlschema-2.4.0/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/assertions.py` & `xmlschema-2.4.0/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/attributes.py` & `xmlschema-2.4.0/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/builtins.py` & `xmlschema-2.4.0/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/complex_types.py` & `xmlschema-2.4.0/xmlschema/validators/complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/elements.py` & `xmlschema-2.4.0/xmlschema/validators/elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/exceptions.py` & `xmlschema-2.4.0/xmlschema/validators/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         self.index = index
         self.particle = particle
         self.occurs = occurs
         self.expected = expected
 
         tag = get_prefixed_qname(elem.tag, validator.namespaces, use_empty=False)
         if index >= len(elem):
-            reason = "The content of element %r is not complete." % tag
+            reason = _("The content of element %r is not complete.") % tag
         else:
             child_tag = get_prefixed_qname(elem[index].tag, validator.namespaces, use_empty=False)
             reason = _("Unexpected child with tag %r at position %d.") % (child_tag, index + 1)
 
         if occurs and particle.is_missing(occurs):
             reason += " The particle %r occurs %d times but the minimum is %d." % (
                 particle, occurs, particle.min_occurs
```

### Comparing `xmlschema-2.3.1/xmlschema/validators/facets.py` & `xmlschema-2.4.0/xmlschema/validators/facets.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/global_maps.py` & `xmlschema-2.4.0/xmlschema/validators/global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/groups.py` & `xmlschema-2.4.0/xmlschema/validators/groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/helpers.py` & `xmlschema-2.4.0/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/identities.py` & `xmlschema-2.4.0/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/models.py` & `xmlschema-2.4.0/xmlschema/validators/models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/notations.py` & `xmlschema-2.4.0/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/particles.py` & `xmlschema-2.4.0/xmlschema/validators/particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/schemas.py` & `xmlschema-2.4.0/xmlschema/validators/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import re
 import sys
 from copy import copy as _copy
 from itertools import chain
 from operator import attrgetter
 from typing import cast, Callable, ItemsView, List, Optional, Dict, Any, \
     Set, Union, Tuple, Type, Iterator, Counter
+from urllib.parse import unquote
 from xml.etree.ElementTree import Element, ParseError
 
 from elementpath import XPathToken, SchemaElementNode, build_schema_node_tree
 
 from ..exceptions import XMLSchemaTypeError, XMLSchemaKeyError, XMLSchemaRuntimeError, \
     XMLSchemaValueError, XMLSchemaNamespaceError
 from ..names import VC_MIN_VERSION, VC_MAX_VERSION, VC_TYPE_AVAILABLE, \
@@ -41,15 +42,15 @@
     XSD_IMPORT, XSD_REDEFINE, XSD_OVERRIDE, XSD_DEFAULT_OPEN_CONTENT, \
     XSD_ANY_SIMPLE_TYPE, XSD_UNION, XSD_LIST, XSD_RESTRICTION
 from ..aliases import ElementType, XMLSourceType, NamespacesType, LocationsType, \
     SchemaType, SchemaSourceType, ConverterType, ComponentClassType, DecodeType, \
     EncodeType, BaseXsdType, ExtraValidatorType, SchemaGlobalType, \
     FillerType, DepthFillerType, ValueHookType, ElementHookType
 from ..translation import gettext as _
-from ..helpers import prune_etree, get_namespace, get_qname
+from ..helpers import prune_etree, get_namespace, get_qname, is_defuse_error
 from ..namespaces import NamespaceResourcesMap, NamespaceView
 from ..resources import is_local_url, is_remote_url, url_path_is_file, \
     normalize_locations, fetch_resource, normalize_url, XMLResource
 from ..converters import XMLSchemaConverter
 from ..xpath import XsdSchemaProtocol, XMLSchemaProxy, ElementPathMixin
 from .. import dataobjects
 
@@ -1308,34 +1309,40 @@
 
             if namespace in self.fallback_locations:
                 locations.append(self.fallback_locations[namespace])
 
             self._import_namespace(namespace, locations)
 
     def _import_namespace(self, namespace: str, locations: List[str]) -> None:
-        import_error = None
+        import_error: Optional[Exception] = None
         for url in locations:
             try:
                 logger.debug("Import namespace %r from %r", namespace, url)
                 self.import_schema(namespace, url, self.base_url)
             except (OSError, IOError) as err:
                 # It's not an error if the location access fails (ref. section 4.2.6.2):
                 #   https://www.w3.org/TR/2012/REC-xmlschema11-1-20120405/#composition-schemaImport
                 logger.debug('%s', err)
                 if import_error is None:
                     import_error = err
             except (XMLSchemaParseError, XMLSchemaTypeError, ParseError) as err:
-                if namespace:
-                    msg = _("cannot import namespace {0!r}: {1}").format(namespace, err)
+                if is_defuse_error(err):
+                    # Consider defuse of XML data as a location access fail
+                    logger.debug('%s', err)
+                    if import_error is None:
+                        import_error = err
                 else:
-                    msg = _("cannot import chameleon schema: %s") % err
-                if isinstance(err, (XMLSchemaParseError, ParseError)):
-                    self.parse_error(msg)
-                else:
-                    raise type(err)(msg)
+                    if namespace:
+                        msg = _("cannot import namespace {0!r}: {1}").format(namespace, err)
+                    else:
+                        msg = _("cannot import chameleon schema: %s") % err
+                    if isinstance(err, (XMLSchemaParseError, ParseError)):
+                        self.parse_error(msg)
+                    else:
+                        raise type(err)(msg)
 
             except XMLSchemaValueError as err:
                 self.parse_error(err)
             else:
                 logger.info("Namespace %r imported from %r", namespace, url)
                 break
         else:
@@ -1447,15 +1454,15 @@
             msg = _("target parent directory {} does not exist")
             raise XMLSchemaValueError(msg.format(target_path.parent))
         elif not target_path.parent.is_dir():
             msg = _("target parent {} is not a directory")
             raise XMLSchemaValueError(msg.format(target_path.parent))
 
         url = self.url or 'schema.xsd'
-        basename = pathlib.Path(urlsplit(url).path).name
+        basename = pathlib.Path(unquote(urlsplit(url).path)).name
         exports: Any = {self: [target_path.joinpath(basename), self.get_text()]}
         path: Any
 
         while True:
             current_length = len(exports)
 
             for schema in list(exports):
@@ -1506,29 +1513,38 @@
                         for strip_path in ('/', '\\', '..'):
                             while True:
                                 try:
                                     path = path.relative_to(strip_path)
                                 except ValueError:
                                     break
 
-                    path = target_path.joinpath(path)
+                    path = target_path.joinpath(unquote(str(path)))
                     repl = 'schemaLocation="{}"'.format(path.as_posix())
                     schema_text = exports[schema][1]
                     pattern = r'\bschemaLocation\s*=\s*[\'\"].*%s.*[\'"]' % re.escape(location)
                     exports[schema][1] = re.sub(pattern, repl, schema_text)
                     exports[ref_schema] = [path, ref_schema.get_text()]
 
             if current_length == len(exports):
                 break
 
         for schema, (path, text) in exports.items():
             if not path.parent.exists():
                 path.parent.mkdir(parents=True)
 
-            with path.open(mode='w') as fp:
+            encoding = 'utf-8'  # default encoding for XML 1.0
+
+            if text.startswith('<?'):
+                # Get the encoding from XML declaration
+                xml_declaration = text.split('\n', maxsplit=1)[0]
+                re_match = re.search('(?<=encoding=["\'])[^"\']+', xml_declaration)
+                if re_match is not None:
+                    encoding = re_match.group(0).lower()
+
+            with path.open(mode='w', encoding=encoding) as fp:
                 fp.write(text)
 
     def version_check(self, elem: ElementType) -> bool:
         """
         Checks if the element is compatible with the version of the validator and XSD
         types/facets availability. Invalid vc attributes are not detected in XSD 1.0.
```

### Comparing `xmlschema-2.3.1/xmlschema/validators/simple_types.py` & `xmlschema-2.4.0/xmlschema/validators/simple_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,23 +919,25 @@
     def iter_components(self, xsd_classes: ComponentClassType = None) \
             -> Iterator[XsdComponent]:
         if xsd_classes is None or isinstance(self, xsd_classes):
             yield self
         if self.base_type.parent is not None:
             yield from self.base_type.iter_components(xsd_classes)
 
-    def iter_decode(self, obj: Union[str, bytes],  # type: ignore[override]
+    def iter_decode(self, obj: Union[str, bytes],
                     validation: str = 'lax', **kwargs: Any) \
-            -> IterDecodeType[List[DecodedValueType]]:
+            -> IterDecodeType[Union[XMLSchemaValidationError,
+                              List[Optional[AtomicValueType]]]]:
         items = []
         for chunk in self.normalize(obj).split():
             for result in self.base_type.iter_decode(chunk, validation, **kwargs):
                 if isinstance(result, XMLSchemaValidationError):
                     yield result
                 else:
+                    assert not isinstance(result, list)
                     items.append(result)
         else:
             yield items
 
     def iter_encode(self, obj: Any, validation: str = 'lax', **kwargs: Any) \
             -> IterEncodeType[EncodedValueType]:
         if not hasattr(obj, '__iter__') or isinstance(obj, (str, bytes)):
@@ -1080,36 +1082,39 @@
     def iter_components(self, xsd_classes: ComponentClassType = None) \
             -> Iterator[XsdComponent]:
         if xsd_classes is None or isinstance(self, xsd_classes):
             yield self
         for mt in filter(lambda x: x.parent is not None, self.member_types):
             yield from mt.iter_components(xsd_classes)
 
-    def iter_decode(self, obj: Any, validation: str = 'lax',
+    def iter_decode(self, obj: AtomicValueType, validation: str = 'lax',
                     patterns: Optional[XsdPatternFacets] = None,
                     **kwargs: Any) -> IterDecodeType[DecodedValueType]:
 
-        # Try decoding the whole text
+        # Try decoding the whole text (or validate the decoded atomic value)
         for member_type in self.member_types:
             for result in member_type.iter_decode(obj, validation='lax', **kwargs):
                 if not isinstance(result, XMLSchemaValidationError):
-                    if patterns:
-                        obj = member_type.normalize(obj)
+                    if patterns and isinstance(obj, (str, bytes)):
                         try:
-                            patterns(obj)
+                            patterns(member_type.normalize(obj))
                         except XMLSchemaValidationError as err:
                             yield err
 
                     yield result
                     return
                 break
 
-        if ' ' not in obj.strip():
+        if isinstance(obj, bytes):
+            obj = obj.decode('utf-8')
+
+        if not isinstance(obj, str) or ' ' not in obj.strip():
             reason = _("invalid value {!r}").format(obj)
             yield XMLSchemaDecodeError(self, obj, self.member_types, reason)
+            return
 
         items = []
         not_decodable = []
         for chunk in obj.split():
             for member_type in self.member_types:
                 for result in member_type.iter_decode(chunk, validation='lax', **kwargs):
                     if isinstance(result, XMLSchemaValidationError):
@@ -1360,41 +1365,41 @@
                         yield from facet
                     elif isinstance(facet, XsdFacet):
                         yield facet
 
         if self.base_type.parent is not None:
             yield from self.base_type.iter_components(xsd_classes)
 
-    def iter_decode(self, obj: Union[str, bytes], validation: str = 'lax', **kwargs: Any) \
+    def iter_decode(self, obj: AtomicValueType, validation: str = 'lax', **kwargs: Any) \
             -> IterDecodeType[DecodedValueType]:
         if isinstance(obj, (str, bytes)):
             obj = self.normalize(obj)
 
+            if self.patterns:
+                if not isinstance(self.primitive_type, XsdUnion):
+                    try:
+                        self.patterns(obj)
+                    except XMLSchemaValidationError as err:
+                        yield err
+                elif 'patterns' not in kwargs:
+                    kwargs['patterns'] = self.patterns
+
         base_type: Any
         if isinstance(self.base_type, XsdSimpleType):
             base_type = self.base_type
         elif self.base_type.has_simple_content():
             base_type = self.base_type.content
         elif self.base_type.mixed:
             yield obj
             return
-        else:
+        else:  # pragma: no cover
             msg = _("wrong base type %r: a simpleType or a complexType "
                     "with simple or mixed content required")
             raise XMLSchemaValueError(msg % self.base_type)
 
-        if self.patterns:
-            if not isinstance(self.primitive_type, XsdUnion):
-                try:
-                    self.patterns(obj)
-                except XMLSchemaValidationError as err:
-                    yield err
-            elif 'patterns' not in kwargs:
-                kwargs['patterns'] = self.patterns
-
         for result in base_type.iter_decode(obj, validation, **kwargs):
             if isinstance(result, XMLSchemaValidationError):
                 yield result
             else:
                 if result is not None:
                     for validator in self.validators:
                         try:
@@ -1420,15 +1425,15 @@
             if isinstance(self.base_type, XsdSimpleType):
                 base_type = self.base_type
             elif self.base_type.has_simple_content():
                 base_type = self.base_type.content
             elif self.base_type.mixed:
                 yield str(obj)
                 return
-            else:
+            else:  # pragma: no cover
                 msg = _("wrong base type %r: a simpleType or a complexType "
                         "with simple or mixed content required")
                 raise XMLSchemaValueError(msg % self.base_type)
 
         result: Any
         for result in base_type.iter_encode(obj, validation):
             if isinstance(result, XMLSchemaValidationError):
```

### Comparing `xmlschema-2.3.1/xmlschema/validators/wildcards.py` & `xmlschema-2.4.0/xmlschema/validators/wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/validators/xsdbase.py` & `xmlschema-2.4.0/xmlschema/validators/xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema/xpath.py` & `xmlschema-2.4.0/xmlschema/xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-2.3.1/xmlschema.egg-info/PKG-INFO` & `xmlschema-2.4.0/xmlschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 2.3.1
+Version: 2.4.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-2.3.1/xmlschema.egg-info/SOURCES.txt` & `xmlschema-2.4.0/xmlschema.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,21 @@
 tests/test_cases/examples/collection/collection3.xml
 tests/test_cases/examples/collection/collection3.xsd
 tests/test_cases/examples/collection/collection3bis.xml
 tests/test_cases/examples/collection/collection3bis.xsd
 tests/test_cases/examples/collection/collection4.xml
 tests/test_cases/examples/collection/collection4.xsd
 tests/test_cases/examples/collection/collection5.xsd
+tests/test_cases/examples/menù/menù-ascii.xml
+tests/test_cases/examples/menù/menù-ascii.xsd
+tests/test_cases/examples/menù/menù-cp1252.xml
+tests/test_cases/examples/menù/menù-cp1252.xsd
+tests/test_cases/examples/menù/menù.txt
+tests/test_cases/examples/menù/menù.xml
+tests/test_cases/examples/menù/menù.xsd
 tests/test_cases/examples/stockquote/stockquote.wsdl
 tests/test_cases/examples/stockquote/stockquote.xsd
 tests/test_cases/examples/stockquote/stockquoteservice.wsdl
 tests/test_cases/examples/vehicles/bikes.xsd
 tests/test_cases/examples/vehicles/cars.xsd
 tests/test_cases/examples/vehicles/invalid.xsd
 tests/test_cases/examples/vehicles/types.xsd
@@ -289,14 +296,16 @@
 tests/test_cases/resources/dummy file.txt
 tests/test_cases/resources/external_entity.xml
 tests/test_cases/resources/malformed.xml
 tests/test_cases/resources/unparsed_entity.xml
 tests/test_cases/resources/unused_external_entity.xml
 tests/test_cases/resources/unused_unparsed_entity.xml
 tests/test_cases/resources/with_entity.xml
+tests/test_cases/translations/pl/tw-1(5)8e.xsd
+tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
 tests/validation/__init__.py
 tests/validation/test_decoding.py
 tests/validation/test_encoding.py
 tests/validation/test_validation.py
 tests/validators/__init__.py
 tests/validators/test_attributes.py
 tests/validators/test_builtins.py
@@ -347,22 +356,28 @@
 xmlschema/extras/wsdl.py
 xmlschema/extras/templates/python/bindings.py.jinja
 xmlschema/extras/templates/python/sample.py.jinja
 xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
 xmlschema/locale/en/LC_MESSAGES/xmlschema.po
 xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
 xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
+xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
 xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
 xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
+xmlschema/schemas/DSIG/xmldsig11-schema.xsd
 xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
 xmlschema/schemas/VC/XMLSchema-versioning.xsd
 xmlschema/schemas/WSDL/soap-encoding.xsd
 xmlschema/schemas/WSDL/soap-envelope.xsd
 xmlschema/schemas/WSDL/wsdl-soap.xsd
 xmlschema/schemas/WSDL/wsdl.xsd
+xmlschema/schemas/XENC/xenc-schema-11.xsd
+xmlschema/schemas/XENC/xenc-schema.xsd
 xmlschema/schemas/XHTML/xhtml1-strict.xsd
 xmlschema/schemas/XLINK/xlink.xsd
 xmlschema/schemas/XML/xml_minimal.xsd
 xmlschema/schemas/XSD_1.0/XMLSchema.xsd
 xmlschema/schemas/XSD_1.0/datatypes.xsd
 xmlschema/schemas/XSD_1.1/XMLSchema.xsd
 xmlschema/schemas/XSD_1.1/datatypes.xsd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

