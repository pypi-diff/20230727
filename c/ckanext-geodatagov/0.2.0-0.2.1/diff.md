# Comparing `tmp/ckanext-geodatagov-0.2.0.tar.gz` & `tmp/ckanext-geodatagov-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-geodatagov-0.2.0.tar", last modified: Thu Jul 13 19:10:28 2023, max compression
+gzip compressed data, was "ckanext-geodatagov-0.2.1.tar", last modified: Thu Jul 27 19:41:02 2023, max compression
```

## Comparing `ckanext-geodatagov-0.2.0.tar` & `ckanext-geodatagov-0.2.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24050 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    36767 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   262469 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/waf_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/z3950.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/read.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/organization_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/snippets/related_collection.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/geodatagov_source_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection1/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection2/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-fgdc/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-gmi/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    50490 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    35634 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.355781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    31779 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   101010 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20687 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    22569 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    27195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    35720 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.487636 ckanext-geodatagov-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-27 19:41:02.487636 ckanext-geodatagov-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.467636 ckanext-geodatagov-0.2.1/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.467636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36767 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262469 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/waf_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/z3950.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/pkitestcrt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.463636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/organization/read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/organization/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/organization/snippets/organization_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/package/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/snippets/related_collection.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/source/geodatagov_source_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.463636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.463636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-collection1/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-collection2/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-fgdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-gmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.471636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.475636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf1/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.475636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.463636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.475636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    50490 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    35634 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.479636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    31779 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.483636 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   101010 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20687 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22569 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    27195 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    35720 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:41:02.487636 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 19:41:02.487636 ckanext-geodatagov-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-27 19:41:02.000000 ckanext-geodatagov-0.2.1/setup.py
```

### Comparing `ckanext-geodatagov-0.2.0/LICENSE.md` & `ckanext-geodatagov-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/PKG-INFO` & `ckanext-geodatagov-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ckanext-geodatagov-0.2.0/README.md` & `ckanext-geodatagov-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/blueprint.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/blueprint.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/cli.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,35 +42,43 @@
 
 @click.group()
 def datagovs3():
     pass
 
 
 class Sitemap:
-    """Sitemap object
-
-    Accepts file_num, start, page_size
-    """
 
     def __init__(self, file_num: str, start: int, page_size: int) -> None:
         self.file_num = file_num
-        self.filename_s3 = f"sitemap/sitemap-{file_num}.xml"
         self.start = start
         self.page_size = page_size
         self.xml = ""
 
     def write_xml(self, some_xml, add_newline=True) -> None:
         if add_newline:
             self.xml += f"{some_xml}\n"
         else:
             self.xml += some_xml
 
-    def write_sitemap_header(self) -> None:
+    def to_json(self) -> str:
+        return json.dumps(self, default=lambda o: o.__dict__)
+
+    def write_sitemap_header(self, index=False) -> None:
         self.write_xml('<?xml version="1.0" encoding="UTF-8"?>')
-        self.write_xml('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
+        if index:
+            self.write_xml('<sitemapindex xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
+        else:
+            self.write_xml('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
+
+
+class SitemapData(Sitemap):
+
+    def __init__(self, file_num: str, start: int, page_size: int) -> None:
+        super().__init__(file_num, start, page_size)
+        self.filename_s3 = f"sitemap/sitemap-{file_num}.xml"
 
     def write_pkgs(self, package_query: GeoPackageSearchQuery) -> None:
 
         pkgs = package_query.get_paginated_entity_name_modtime(
             max_results=self.page_size, start=self.start
         )
         for pkg in pkgs:
@@ -82,16 +90,34 @@
                 f"<lastmod>{pkg.get('metadata_modified').strftime('%Y-%m-%d')}</lastmod>"
             )
             self.write_xml("</url>")
 
     def write_sitemap_footer(self) -> None:
         self.write_xml("</urlset>")
 
-    def to_json(self) -> str:
-        return json.dumps(self, default=lambda o: o.__dict__)
+
+class SitemapIndex(Sitemap):
+
+    def __init__(self, file_num: str, start: int, page_size: int) -> None:
+        super().__init__(file_num, start, page_size)
+        self.filename_s3 = "sitemap.xml"
+
+    def write_table_of_contents(self, number_of_sitemaps):
+        current_time = datetime.datetime.now().strftime("%Y-%m-%d")
+
+        log.info("Creating sitemap index...")
+
+        for file_num in range(number_of_sitemaps):
+            # add sitemaps to sitemap index file
+            self.write_xml("<sitemap>")
+            loc = f"{config.get('ckan.site_url')}/sitemap/sitemap-{file_num}.xml"
+            self.write_xml(f"<loc>{loc}</loc>")
+            self.write_xml(f"<lastmod>{current_time}</lastmod>")
+            self.write_xml("</sitemap>")
+        self.write_xml("</sitemapindex>")
 
 
 def get_s3() -> None:
     """Sets global CKAN_SITE_URL, S3 object, checks access to bucket BUCKET_NAME, creates if needed.
 
     Refer to values in .env file in ckanext_geodatagov and
     .profile file in catalog repo for s3 config.
@@ -170,57 +196,28 @@
             log.info(
                 f"File {filename_on_s3} upload complete to: \
                 {S3_ENDPOINT_URL}/{BUCKET_NAME}/{filename_on_s3}"
             )
         else:
             log.error(f"File {filename_on_s3} upload failed. Error: {resp_metadata}")
 
+    del temp_file
 
-def upload_sitemap_index(sitemaps: list) -> None:
-    """Creates and uploads sitemap index xml file"""
-
-    current_time = datetime.datetime.now().strftime("%Y-%m-%d")
-    sitemap_index = Sitemap("index", 0, 0)
-    sitemap_index.filename_s3 = "sitemap.xml"
-
-    log.info("Creating sitemap index...")
-    # write sitemap index
-    sitemap_index.write_xml('<?xml version="1.0" encoding="UTF-8"?>')
-    sitemap_index.write_xml(
-        '<sitemapindex xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">'
-    )
 
-    for sitemap in sitemaps:
-        # add sitemaps to sitemap index file
-        sitemap_index.write_xml("<sitemap>")
-        loc = f"{CKAN_SITE_URL}/{sitemap.filename_s3}"
-        sitemap_index.write_xml(f"<loc>{loc}</loc>")
-        sitemap_index.write_xml(f"<lastmod>{current_time}</lastmod>")
-        sitemap_index.write_xml("</sitemap>")
-    sitemap_index.write_xml("</sitemapindex>")
+def upload_sitemap_file(sitemap: list) -> None:
+    """Handles uploading sitemap files to s3"""
 
-    upload_to_key(sitemap_index.xml, sitemap_index.filename_s3)
+    log.info("Uploading sitemap file...")
+    upload_to_key(sitemap.xml, sitemap.filename_s3)
     log.info(
-        f"Sitemap index upload complete to: \
-        {S3_ENDPOINT_URL}/{BUCKET_NAME}/{sitemap_index.filename_s3}"
+        f"Sitemap file {sitemap.filename_s3} upload complete to: \
+        {S3_ENDPOINT_URL}/{BUCKET_NAME}/{sitemap.filename_s3}"
     )
 
 
-def upload_sitemap_files(sitemaps: list) -> None:
-    """Handles uploading sitemap files to s3"""
-
-    log.info(f"Uploading {len(sitemaps)} sitemap files...")
-    for sitemap in sitemaps:
-        upload_to_key(sitemap.xml, sitemap.filename_s3)
-        log.info(
-            f"Sitemap file {sitemap.filename_s3} upload complete to: \
-            {S3_ENDPOINT_URL}/{BUCKET_NAME}/{sitemap.filename_s3}"
-        )
-
-
 @geodatagov.command()
 @click.option("--upload_to_s3", default=UPLOAD_TO_S3, type=click.BOOL)
 @click.option("--page_size", default=PAGE_SIZE, type=click.INT)
 @click.option("--max_per_page", default=MAX_PER_PAGE, type=click.INT)
 def sitemap_to_s3(upload_to_s3: bool, page_size: int, max_per_page: int):
     """Generates sitemap and uploads to s3"""
     log.info("Sitemap is being generated...")
@@ -229,50 +226,58 @@
     count = package_query.get_count()
     log.info(f"{count} records found")
     if not count:
         log.info("Nothing to process, exiting.")
         return
 
     start = 0
-    file_num = 1
-    sitemaps = []
 
-    paginations = (count // page_size) + 1
-    for _ in range(paginations):
-        sitemap = Sitemap(str(file_num), start, page_size)
+    num_of_pages = (count // page_size) + 1
+
+    # Create + Upload Sitemap Index File
+    sitemap_index = SitemapIndex("index", 0, 0)
+    sitemap_index.write_sitemap_header(index=True)
+    sitemap_index.write_table_of_contents(num_of_pages)
+
+    if upload_to_s3:
+        # set global S3 object and vars
+        get_s3()
+        upload_to_key(sitemap_index.xml, sitemap_index.filename_s3)
+        log.info(
+            f"Sitemap index upload complete to: \
+            {S3_ENDPOINT_URL}/{BUCKET_NAME}/{sitemap_index.filename_s3}"
+        )
+
+    for file_num in range(1, num_of_pages + 1):
+        sitemap = SitemapData(str(file_num), start, page_size)
         sitemap.write_sitemap_header()
         sitemap.write_pkgs(package_query)
         sitemap.write_sitemap_footer()
 
         log.info(
             f"{start+1} to {min(start + page_size, count)} of {count} records done."
         )
 
         # large block removed here, I'm not convinced that it was ever hit
         # if issues arise around max_per_page, re-add here
         # see https://github.com/GSA/ckanext-geodatagov/blob/
         # 597610699434bde9415a48ed0b1085bfa0e9720f/ckanext/geodatagov/cli.py#L183
 
         log.info(f"done with {sitemap.filename_s3}.")
-        sitemaps.append(sitemap)
 
         start += page_size
-        file_num += 1
 
-    if upload_to_s3:
-        log.info("Starting S3 uploads...")
-        # set global S3 object and vars
-        get_s3()
+        if upload_to_s3:
+            log.info(f"Uploading {sitemap.filename_s3}...")
+            upload_sitemap_file(sitemap)
+        else:
+            log.info(f"Skip upload and return local copy of sitemap {file_num}.")
+            print(json.dumps(sitemap.to_json(), indent=4))
 
-        upload_sitemap_index(sitemaps)
-        upload_sitemap_files(sitemaps)
-    else:
-        log.info("Skip upload and finish.")
-        dump = [sitemap.to_json() for sitemap in sitemaps]
-        print(f"Done locally: Sitemap list\n{json.dumps(dump, indent=4)}")
+        del sitemap
 
 
 def _normalize_type(_type):
     if isinstance(_type, model.domain_object.DomainObject):
         _type = _type.__class__
     if isinstance(_type, type):
         _type = _type.__name__
```

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/commands.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/commands.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/__init__.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/arcgis.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/arcgis.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/base.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/waf_collection.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/waf_collection.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/z3950.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/harvesters/z3950.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/helpers.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/logic.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/logic.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/model.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/model.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/plugin.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/search.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/organization_form.html` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/organization/snippets/organization_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/read.html` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/geodatagov_source_form.html` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/templates/source/geodatagov_source_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/index.html` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/tests/data-samples/waf1/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/__init__.py` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd` & `ckanext-geodatagov-0.2.1/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/PKG-INFO` & `ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/SOURCES.txt` & `ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/entry_points.txt` & `ckanext-geodatagov-0.2.1/ckanext_geodatagov.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.2.0/requirements.txt` & `ckanext-geodatagov-0.2.1/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # redis==2.10.6 # included in ckan core
 # requests>=2.11.1 # included in ckan core
 
 # ckanext-spatial
 # ckantoolkit # included as dep of ckanext-harvest
 GeoAlchemy2==0.5.0
 Shapely>=1.2.13
-pyproj==3.4.1
 OWSLib==0.28.1
 lxml>=2.3
 argparse
 pyparsing>=2.1.10
 # requests>=1.1.0 # included in ckan-core
 six
 geojson==3.0.1
```

### Comparing `ckanext-geodatagov-0.2.0/setup.py` & `ckanext-geodatagov-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ckanext-geodatagov",
-    version="0.2.0",
+    version="0.2.1",
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

