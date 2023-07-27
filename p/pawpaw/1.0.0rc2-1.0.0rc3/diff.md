# Comparing `tmp/pawpaw-1.0.0rc2.tar.gz` & `tmp/pawpaw-1.0.0rc3.tar.gz`

## Comparing `pawpaw-1.0.0rc2.tar` & `pawpaw-1.0.0rc3.tar`

### file list

```diff
@@ -1,117 +1,128 @@
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/SECURITY.md
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tinker.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/.gitignore
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/modules.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/pawpaw.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/vcs.xml
--rw-r--r--   0        0        0    37655 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/0. Introduction.md
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/1. Segment and Span.md
--rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/2. In Text Object.md
--rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/3. Visualization.md
--rw-r--r--   0        0        0    22995 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/4. Arborform.md
--rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/5. Traversal & Query.md
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/6. Xml.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/7. NLP.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/8. Serialization.md
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/Pawpaw Cookbook.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/Using Pawpaw with nltk.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/Q&A/description.md
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/Q&A/solution.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/description.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/input.txt
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/parser_compact.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/parser_verbose.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/solution.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/gettysburg_address/gettysburg_address.txt
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/description.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.py
--rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.txt
--rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/images/pawpaw.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/__init__.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/_type_magic.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/_version.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/errors.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/infix.py
--rw-r--r--   0        0        0    53966 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/ito.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/span.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/util.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/__init__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/desc.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/extract.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/filter.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/itorator.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/reflect.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/split.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/value_func.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/postorator.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/stacked_reduce.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/windowed_join.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/__init__.py
--rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/nlp.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/table.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/query/__init__.py
--rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/query/_query.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/__init__.py
--rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/ascii_box.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/highlighter.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/pepo/__init__.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/pepo/pepo.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/__init__.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/sgr.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/palettes/__init__.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/palettes/palettes.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/descriptors.py
--rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/xml_helper.py
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/xml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_child_itos.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_invoke_func.py
--rw-r--r--   0        0        0    20727 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito.py
--rw-r--r--   0        0        0    20370 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_ctor.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_descend.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_regex_equivalence_methods.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_serialization.py
--rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_str_equivalence_methods.py
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_nlp.py
--rw-r--r--   0        0        0    41635 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_query_and_traversal.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_span.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_type_magic.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_util.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_version.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_xml_helper.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_xml_parser.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/util.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/__init__.py
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_connectors.py
--rw-r--r--   0        0        0    14065 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_desc.py
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_extract.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_filter.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_reflect.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_split.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_value_func.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_postorator.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_postorator_windowed_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/test_sgr.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/test_visualization_ascii_box.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/README.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/SECURITY.md
+-rw-r--r--   0        0        0    14724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tinker.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/.gitignore
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/modules.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/pawpaw.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/vcs.xml
+-rw-r--r--   0        0        0    38121 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/0. Introduction.md
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/1. Segment and Span.md
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/2. In Text Object.md
+-rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/3. Visualization.md
+-rw-r--r--   0        0        0    26926 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/4. Arborform.md
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/5. Traversal & Query.md
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/6. Xml.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/7. NLP.md
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/8. Serialization.md
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/Pawpaw Cookbook.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/Using Pawpaw with nltk.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/Q&A/description.md
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/Q&A/solution.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/class_grades/description.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/class_grades/input.txt
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/class_grades/parser_compact.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/class_grades/parser_verbose.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/class_grades/solution.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/compounds/compound_1.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/compounds/compound_2.txt
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/compounds/description.md
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/compounds/solution.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/gettysburg_address/gettysburg_address.txt
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/quack_language/description.md
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/quack_language/q_lexer.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/quack_language/q_parser.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/quack_language/quack.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/us_constitution/description.md
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/us_constitution/us_constitution.py
+-rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/docs/demos/us_constitution/us_constitution.txt
+-rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/images/pawpaw.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/__init__.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/_type_magic.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/_version.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/errors.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/infix.py
+-rw-r--r--   0        0        0    54479 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/ito.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/span.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/util.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/desc.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/extract.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/filter.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/gaps.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/itorator.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/reflect.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/split.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/itorator/value_func.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/postorator/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/postorator/postorator.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/postorator/stacked_reduce.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/arborform/postorator/windowed_join.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/nlp/__init__.py
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/nlp/nlp.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/nlp/table.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/ontology/__init__.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/ontology/ontology.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/query/__init__.py
+-rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/query/_query.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/__init__.py
+-rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/ascii_box.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/highlighter.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/pepo/__init__.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/pepo/pepo.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/sgr/__init__.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/sgr/sgr.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/sgr/palettes/__init__.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/visualization/sgr/palettes/palettes.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/xml/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/xml/descriptors.py
+-rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/xml/xml_helper.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pawpaw/xml/xml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_child_itos.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_invoke_func.py
+-rw-r--r--   0        0        0    20680 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito.py
+-rw-r--r--   0        0        0    20186 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito_ctor.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito_descend.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito_regex_equivalence_methods.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito_serialization.py
+-rw-r--r--   0        0        0    17981 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_ito_str_equivalence_methods.py
+-rw-r--r--   0        0        0    41635 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_query_and_traversal.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_span.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_type_magic.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_util.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_version.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_xml_helper.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/test_xml_parser.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/__init__.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_connectors.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_gaps.py
+-rw-r--r--   0        0        0    14065 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_desc.py
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_extract.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_filter.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_reflect.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_split.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_itorator_value_func.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_postorator.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/arborform/test_postorator_windowed_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/nlp/__init__.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/nlp/test_nlp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/ontology/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/ontology/test_ontology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/ontology/test_quack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/visualization/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/visualization/test_ito_utility_methods.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/visualization/test_sgr.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/tests/visualization/test_visualization_ascii_box.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/README.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    16383 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc3/PKG-INFO
```

### Comparing `pawpaw-1.0.0rc2/CODE_OF_CONDUCT.md` & `pawpaw-1.0.0rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/CONTRIBUTING.md` & `pawpaw-1.0.0rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/SECURITY.md` & `pawpaw-1.0.0rc3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tinker.py` & `pawpaw-1.0.0rc3/tinker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,28 @@
 
 # Force Python XML parser, not faster C accelerators because we can't hook the C implementation (3.x hack)
 sys.modules['_elementtree'] = None
 import xml.etree.ElementTree as ET
 from dataclasses import dataclass, field
 import typing
 
+
+from pawpaw import Ito
+s = 'Here\nare\nseveral\nlines of stuff'
+ito = Ito(s)
+print(ito.to_line_col('\n'))
+ito = next(Ito.from_substrings(s, '\nlines of stuff'))
+print(ito.to_line_col('\n'))
+ito = next(Ito.from_substrings(s, 'lines of stuff'))
+print(ito.to_line_col('\n'))
+ito = next(Ito.from_substrings(s, 'es of stuff'))
+print(ito.to_line_col('\n'))
+exit(0)
+
+
 import regex
 import pawpaw
 from pawpaw import Ito
 from pawpaw.visualization import sgr, Highlighter, pepo
 
 from pawpaw import Ito, arborform, visualization
```

### Comparing `pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `pawpaw-1.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `pawpaw-1.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/.idea/workspace.xml` & `pawpaw-1.0.0rc3/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `pawpaw-1.0.0rc2/.idea/workspace.xml` & `pawpaw-1.0.0rc3/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
+    <list default="true" id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/docs/4. Arborform.md" beforeDir="false" afterPath="$PROJECT_DIR$/docs/4. Arborform.md" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -26,171 +28,151 @@
   </component>
   <component name="ProjectId" id="2HYqL0C1amxRmfYJALzRD6Il7pD"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;ignore.virus.scanning.warn.message&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;C:/Users/rlaye/Documents/PycharmProjects/pawpaw/pawpaw/arborform/itorator&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;project.propVCSSupport.CommitDialog&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.OpenProjectViewOnStart": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "ignore.virus.scanning.warn.message": "true",
+    "last_opened_file_path": "C:/Users/rlaye/Documents/PycharmProjects/pawpaw/tests/visualization",
+    "settings.editor.selected.configurable": "project.propVCSSupport.CommitDialog"
   },
-  &quot;keyToStringList&quot;: {
-    &quot;com.intellij.ide.scratch.ScratchImplUtil$2/New Scratch File&quot;: [
-      &quot;TEXT&quot;
+  "keyToStringList": {
+    "com.intellij.ide.scratch.ScratchImplUtil$2/New Scratch File": [
+      "TEXT"
     ]
   }
-}</component>
+}]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
+      <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\visualization"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\arborform"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\visualization"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
   </component>
   <component name="RunManager" selected="Python tests. All Unittests">
-    <configuration name="parser_verbose" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/class_grades"/>
-      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/class_grades/parser_verbose.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="solution (1)" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="us_constitution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/class_grades"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/us_constitution"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/class_grades/solution.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="solution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name=" All Unittests" type="tests" factoryName="Unittests">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <envs>
-        <env name="PYTHONUNBUFFERED" value="1"/>
-      </envs>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/Q&amp;A"/>
-      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
+      <option name="WORKING_DIRECTORY" value=""/>
+      <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/Q&amp;A/solution.py"/>
-      <option name="PARAMETERS" value=""/>
-      <option name="SHOW_COMMAND_LINE" value="false"/>
-      <option name="EMULATE_TERMINAL" value="false"/>
-      <option name="MODULE_MODE" value="false"/>
-      <option name="REDIRECT_INPUT" value="false"/>
-      <option name="INPUT_FILE" value=""/>
+      <option name="_new_pattern" value="&quot;&quot;"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
+      <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
+    <configuration name="Python tests for test_ito.TestIto.test_repr" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <envs>
-        <env name="PYTHONUNBUFFERED" value="1"/>
-      </envs>
-      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
-      <option name="PARAMETERS" value=""/>
-      <option name="SHOW_COMMAND_LINE" value="false"/>
-      <option name="EMULATE_TERMINAL" value="false"/>
-      <option name="MODULE_MODE" value="false"/>
-      <option name="REDIRECT_INPUT" value="false"/>
-      <option name="INPUT_FILE" value=""/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_ito.TestIto.test_repr&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="us_constitution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_ito_utility_methods.TestItoUtilityMethods" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <envs>
-        <env name="PYTHONUNBUFFERED" value="1"/>
-      </envs>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/us_constitution"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/visualization"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py"/>
-      <option name="PARAMETERS" value=""/>
-      <option name="SHOW_COMMAND_LINE" value="false"/>
-      <option name="EMULATE_TERMINAL" value="false"/>
-      <option name="MODULE_MODE" value="false"/>
-      <option name="REDIRECT_INPUT" value="false"/>
-      <option name="INPUT_FILE" value=""/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_ito_utility_methods.TestItoUtilityMethods&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name=" All Unittests" type="tests" factoryName="Unittests">
+    <configuration name="Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_col_empty" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
-      <option name="WORKING_DIRECTORY" value=""/>
-      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/visualization"/>
+      <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="_new_pattern" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <option name="_new_target" value="&quot;test_ito_utility_methods.TestItoUtilityMethods.test_to_line_col_empty&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests in test_nlp.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_non_empty" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/visualization"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_nlp.py&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <option name="_new_target" value="&quot;test_ito_utility_methods.TestItoUtilityMethods.test_to_line_non_empty&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact" type="tests" factoryName="Unittests" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
@@ -202,83 +184,41 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_type_magic.TestTypeMagic.test_is_callable_exact&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.tinker"/>
-      <item itemvalue="Python.parser_verbose"/>
-      <item itemvalue="Python.solution"/>
-      <item itemvalue="Python.solution (1)"/>
       <item itemvalue="Python.us_constitution"/>
       <item itemvalue="Python tests.Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact"/>
       <item itemvalue="Python tests. All Unittests"/>
-      <item itemvalue="Python tests.Python tests in test_nlp.py"/>
+      <item itemvalue="Python tests.Python tests for test_ito.TestIto.test_repr"/>
+      <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods"/>
+      <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_col_empty"/>
+      <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_non_empty"/>
     </list>
     <recent_temporary>
       <list>
-        <item itemvalue="Python.solution (1)"/>
-        <item itemvalue="Python.parser_verbose"/>
         <item itemvalue="Python.us_constitution"/>
-        <item itemvalue="Python.solution"/>
-        <item itemvalue="Python tests.Python tests in test_nlp.py"/>
+        <item itemvalue="Python tests.Python tests for test_ito.TestIto.test_repr"/>
+        <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods"/>
+        <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_non_empty"/>
+        <item itemvalue="Python tests.Python tests for test_ito_utility_methods.TestItoUtilityMethods.test_to_line_col_empty"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
       <created>1668472305766</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1668472305766</updated>
     </task>
-    <task id="LOCAL-00036" summary="peduncle -&gt; pepo">
-      <created>1673395183314</created>
-      <option name="number" value="00036"/>
-      <option name="presentableId" value="LOCAL-00036"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673395183314</updated>
-    </task>
-    <task id="LOCAL-00037" summary="Documentation arborform stub">
-      <created>1673396989303</created>
-      <option name="number" value="00037"/>
-      <option name="presentableId" value="LOCAL-00037"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673396989303</updated>
-    </task>
-    <task id="LOCAL-00038" summary="arborform module structuring">
-      <created>1673575438880</created>
-      <option name="number" value="00038"/>
-      <option name="presentableId" value="LOCAL-00038"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673575438880</updated>
-    </task>
-    <task id="LOCAL-00039" summary="itorator import cleanup">
-      <created>1673575487447</created>
-      <option name="number" value="00039"/>
-      <option name="presentableId" value="LOCAL-00039"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673575487447</updated>
-    </task>
-    <task id="LOCAL-00040" summary="Pep whitespace cleanups">
-      <created>1673576886768</created>
-      <option name="number" value="00040"/>
-      <option name="presentableId" value="LOCAL-00040"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673576886768</updated>
-    </task>
-    <task id="LOCAL-00041" summary="regex expansion">
-      <created>1673577233691</created>
-      <option name="number" value="00041"/>
-      <option name="presentableId" value="LOCAL-00041"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673577233691</updated>
-    </task>
     <task id="LOCAL-00042" summary="Documentation spelling and typo fixes">
       <created>1673592455687</created>
       <option name="number" value="00042"/>
       <option name="presentableId" value="LOCAL-00042"/>
       <option name="project" value="LOCAL"/>
       <updated>1673592455687</updated>
     </task>
@@ -572,23 +512,60 @@
     <task id="LOCAL-00084" summary="import cleanup &amp; typehint corrections">
       <created>1683944502477</created>
       <option name="number" value="00084"/>
       <option name="presentableId" value="LOCAL-00084"/>
       <option name="project" value="LOCAL"/>
       <updated>1683944502477</updated>
     </task>
-    <option name="localTasksCounter" value="85"/>
+    <task id="LOCAL-00085" summary="Typos">
+      <created>1689646947585</created>
+      <option name="number" value="00085"/>
+      <option name="presentableId" value="LOCAL-00085"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689646947585</updated>
+    </task>
+    <task id="LOCAL-00086" summary="Refactor">
+      <created>1689855578994</created>
+      <option name="number" value="00086"/>
+      <option name="presentableId" value="LOCAL-00086"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689855578994</updated>
+    </task>
+    <task id="LOCAL-00087" summary="LIT_STR prefix capture">
+      <created>1689907095984</created>
+      <option name="number" value="00087"/>
+      <option name="presentableId" value="LOCAL-00087"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689907095984</updated>
+    </task>
+    <task id="LOCAL-00088" summary="Added Ito.to_line_col">
+      <created>1690081991793</created>
+      <option name="number" value="00088"/>
+      <option name="presentableId" value="LOCAL-00088"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690081991793</updated>
+    </task>
+    <task id="LOCAL-00089" summary="Added Ito.to_line_col">
+      <created>1690419893205</created>
+      <option name="number" value="00089"/>
+      <option name="presentableId" value="LOCAL-00089"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690419893205</updated>
+    </task>
+    <task id="LOCAL-00090" summary="Ito.__format__ refactor">
+      <created>1690421568853</created>
+      <option name="number" value="00090"/>
+      <option name="presentableId" value="LOCAL-00090"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690421568853</updated>
+    </task>
+    <option name="localTasksCounter" value="91"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Format string typo"/>
-    <MESSAGE value="Concrete Itorators all return new or clones"/>
-    <MESSAGE value="Cleanup + tags"/>
-    <MESSAGE value="Itorator refactor; postorator roll-back"/>
-    <MESSAGE value="Itorator function decorations"/>
     <MESSAGE value="Grammer, whitespace, and table-formatting"/>
     <MESSAGE value="import directive cleanups"/>
     <MESSAGE value="typehint corrections"/>
     <MESSAGE value="import cleanups"/>
     <MESSAGE value="Refactor typos &amp; bugfixes"/>
     <MESSAGE value="test_limit subtests expansion"/>
     <MESSAGE value="Typehint and PEP cleanups"/>
@@ -601,15 +578,20 @@
     <MESSAGE value="Example cleanups"/>
     <MESSAGE value="Whitespace and comment spelling fixes"/>
     <MESSAGE value="Minor PEP cleanups"/>
     <MESSAGE value="Unit test count update"/>
     <MESSAGE value="Visualization sample fixes; added outputs"/>
     <MESSAGE value="Bumped version"/>
     <MESSAGE value="import cleanup &amp; typehint corrections"/>
-    <option name="LAST_COMMIT_MESSAGE" value="import cleanup &amp; typehint corrections"/>
+    <MESSAGE value="Typos"/>
+    <MESSAGE value="Refactor"/>
+    <MESSAGE value="LIT_STR prefix capture"/>
+    <MESSAGE value="Added Ito.to_line_col"/>
+    <MESSAGE value="Ito.__format__ refactor"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Ito.__format__ refactor"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>15</line>
@@ -638,30 +620,25 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>130</line>
           <option name="timeStamp" value="82"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito.py</url>
-          <line>402</line>
+          <line>401</line>
           <option name="timeStamp" value="83"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_ito.py</url>
-          <line>375</line>
-          <option name="timeStamp" value="84"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/visualization/ascii_box.py</url>
-          <line>1262</line>
+          <line>1264</line>
           <option name="timeStamp" value="125"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/visualization/ascii_box.py</url>
-          <line>1301</line>
+          <line>1303</line>
           <option name="timeStamp" value="127"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
           <line>109</line>
           <option name="timeStamp" value="128"/>
         </line-breakpoint>
@@ -678,15 +655,15 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>97</line>
           <option name="timeStamp" value="134"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
-          <line>1420</line>
+          <line>1437</line>
           <option name="timeStamp" value="137"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
           <line>77</line>
           <option name="timeStamp" value="138"/>
         </line-breakpoint>
@@ -771,11 +748,26 @@
           <option name="timeStamp" value="175"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/filter.py</url>
           <line>17</line>
           <option name="timeStamp" value="180"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/docs/demos/quack_language/quack.py</url>
+          <line>24</line>
+          <option name="timeStamp" value="183"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" log-message="true" suspend="NONE" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/visualization/test_ito_utility_methods.py</url>
+          <line>7</line>
+          <option name="timeStamp" value="199"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
+    <watches-manager>
+      <configuration name="tests">
+        <watch expression="self.string.count(eol, 0, prior_eol_idx)" language="Python"/>
+      </configuration>
+    </watches-manager>
   </component>
 </project>
```

### Comparing `pawpaw-1.0.0rc2/docs/0. Introduction.md` & `pawpaw-1.0.0rc3/docs/0. Introduction.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 The class ``Ito``, short for *In Text Object*, is a high performance, indexed substring. Creating
 an ``Ito`` does *not* create a new string.  Rather, an ``Ito`` instance maintains a reference to its
 basis string, along with start and stop indexes:
 
 ```python
 >>> i
-Ito('x Hello, world! x', 2, 15, None)
+Ito(span=(2, 15), desc='', substr='Hello, world!')
 ```
 
 Because ``Ito`` only maintains a reference to its basis string, its memory requirements are low:
 
 ```python
 >>> import sys
 >>> sys.getsizeof(s), sys.getsizeof(i)
@@ -76,16 +76,16 @@
 ```
 
 ``Ito`` also supports custom format strings.  You can quickly develop custom outputs by combining and formatting ``Ito``
 attributes in various ways, and even perform truncations to facilitate visualizations:
 
 ```python
 >>> j = Ito('Here is\n a super\nduper, very long string!')
->>> f'{i:%span% : %substr!r:21…}'  # Show span and substr
-(0, 40) : 'Here is\n a super\n'…'
+>>> f'{j:%span% : %substr!r:21…\'}'  # Show span and substr
+"(0, 41): 'Here is\\n a super\\…'"
 ```
 
 #### ``len``
 
 You can access the length of an `Ito` using the keyword `len`:
 
 ```python
@@ -108,15 +108,15 @@
 world!
 ```
   
 Just as index access on a ``str`` returns another ``str``, index access on an ``Ito`` returns another ``Ito``:
 
 ```python
 >>> i[-6:]
-Ito(Hello, world!', 7, 13, None)
+Ito(span=(9, 15), desc='', substr='world!')
 ```
 
 Relative index access allows for clear, easy to use code:
 
 ```python
 >>> j = i[-6:]   # new Ito based on the last 6 characters of the previous Ito
 >>> str(j[0:3])  # print first three characters of the new Ito
```

### Comparing `pawpaw-1.0.0rc2/docs/1. Segment and Span.md` & `pawpaw-1.0.0rc3/docs/1. Segment and Span.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/2. In Text Object.md` & `pawpaw-1.0.0rc3/docs/2. In Text Object.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 #### Creating from a ``str``
 
 Instantiating an ``Ito`` against a reference ``str`` is straightforward:
 
 ```python
 >>> from pawpaw import Ito
 >>> s = 'Hello, World!'
-Ito('Hello, World!', 0, 13, None)
+>>> Ito(s)
+Ito(span=(0, 13), desc='', substr='Hello, World!')
 ```
 
 The ``str`` value supplied to the constructor is accessible via a ``.string`` property.  The constructor features optional ``start`` and ``stop`` parameters, which are *Python-style indices*.  The values for ``str``, ``start``, and ``stop`` are used to create a ``Span``, which is accessible via the ``.span`` property:
 
 ```python
 >>> i = Ito('abcd', 1, -1)
 >>> i.span
@@ -47,15 +48,15 @@
 Having separate ``start`` and ``stop`` parameters is more idiomatic with Python than using a single, ``Span`` parameter.  However, given a span you can easily supply these values via unpacking:
 
 ```python
 >>> from pawpaw import Span
 >>> span = Span(1, 3)
 >>> i = Ito('abcd', *span)
 >>> i
-Ito('abcd', 1, 3, None)
+Ito(span=(1, 3), desc='', substr='bc')
 ```
 
 The ``start`` and ``stop`` values for the span are accessible via ``.start`` and ``.stop`` properties on *both* the ``Ito`` and ``Span``:
 
 ```python
 >>> i = Ito('abc')
 >>> i.span == (i.start, i.stop)
@@ -101,15 +102,15 @@
 ```
 
 ### ``.from_match_group``
 
 The ``.from_match_group`` method allows you to create ``Ito`` instances from an ``re.Match`` object and group key.  The ``group`` parameter accepts a group key, whose type can be either an ``int`` or ``str``, and which defaults to 0 (the group key corresponding to the *entire* match):
 
 ```python
->>> s = 'John doe'
+>>> s = 'John Doe'
 >>> re = regex.compile(r'(?P<fn>.+)\s(?P<ln>.+)')
 >>> m = re.fullmatch(s)
 >>> str(Ito.from_match_group(m))  # group defaults to 0 (the entire match)
 'John Doe'
 >>> str(Ito.from_match_group(m, 2))  # group key 2
 'Doe'
 >>> str(Ito.from_match_group(m, 'fn'))  # group key 'fn'
@@ -129,17 +130,17 @@
 
 which returns a string corresponding to the supplied ``group`` parameter.
 
 Example:
 
 ```python
 >>> Ito.from_match_group(m, 'fn')  # desc defaults to group parameter ('fn')
-Ito('John Doe', 0, 4, 'fn')
+Ito(span=(0, 4), desc='fn', substr='John')
 >>> Ito.from_match_group(m, 'fn', lambda mm, gk: f'{len(mm)}: {gk}')
-Ito('John Doe', 0, 4, '3: fn')
+Ito(span=(0, 4), desc='3: fn', substr='John')
 ```
 
 ### ``.from_match``
 
 The ``.from_match`` method allows you to create a fully hierarchical ``Ito`` instance whoses nodes correspond to the captures of an ``re.Match`` object.  Like the ``.from_match_group`` method, a ``desc`` parameter can be supplied, and which defaults to the same lambda.  Group keys are dynamically passed to this lambda to yield descriptors.  For named captures, the ``str`` group key (i.e., the capture name) is supplied, otherwise, the ``int`` group key is used.
 
 ```python
@@ -198,33 +199,34 @@
 ...
 (0, 2) my_desc: "Jo"
 (3, 6) my_desc: "n d"
 ```
 
 ### ``.from_gaps``
 
-The ``.from_gaps`` method allows you to create a sequence of ``Ito`` instances by providing spans you want *excluded* from the result.  An optional ``desc`` parameter, if provided, is used as the descriptor for the generated objects:
+The ``.from_gaps`` method allows you to create a sequence of ``Ito`` instances by providing spans you want *excluded* from the result.  An optional ``desc`` parameter can be used as the descriptor for the generated objects, while the optional 
+``return_zero_widths`` parameter (defaulted to ``False``) indicates if you want zero-width itos included in the result.
 
 ```python
 >>> s = 'John doe'
->>> for i in Ito.from_gaps(s, pawpaw.Span(0, 2), pawpaw.Span(3, 6), desc='my_desc'):
+>>> for i in Ito.from_gaps(s, pawpaw.Span(0, 2), pawpaw.Span(3, 6), 'my_desc'):
 ...     print(f'{i:%span: %desc: "%substr"}')
 ...
 (2, 3) my_desc: "h"
 (6, 8) my_desc: "oe"
 ```
 
 ### ``.from_substrings``
 
 Given a sequence of substrings, you can create an ``Ito`` sequence using the static ``.from_substrings`` method.  When supplied with a ``src`` of type ``str`` or ``Ito`` and one or more non-overlapping substrings, this method generates a sequence of ``Ito`` objects:
 
 ```python
 >>> s = 'A B C'
 >>> [*Ito.from_substrings(s, *s.split())]
-[Ito('A B C', 0, 1, None), Ito('A B C', 2, 3, None), Ito('A B C', 4, 5, None)]
+[Ito(span=(0, 1), desc='', substr='A'), Ito(span=(2, 3), desc='', substr='B'), Ito(span=(4, 5), desc='', substr='C')]
 ```
 
 ### ``.clone``
 
 The ``Ito.clone`` method allows you to duplicate existing ``Ito`` instances.  Optional parameters ``start``, ``stop``, and ``desc`` allow you to supply alternate values for the resulting object.  However, unlike in the ``Ito`` constructor, in ``.clone`` the parameters ``start`` and ``stop`` are *relative to the underlying string*.
 
 Unlike ``.__init__``, the ``.clone`` preserves the:
@@ -418,15 +420,16 @@
 * have no effects on the ``Ito`` used to call them
 * are available for associated methods that are *non-modifying* or *return values that are themselves substrings for the basis string*.  For example, ``str.count``, ``str.endswith``, and ``str.islower`` have equivalence methods, while ``str.upper()`` does not.
  
 ### str equivalence methods
 
 | ``str`` method | ``Ito`` equivalence method |
 |:--------------:|:--------------------------:| 
-|     count      |         str_count          |
+|     count      |        str_count           |
+|     __eq__     |         str_eq             |
 |    endswith    |        str_endswith        |
 |   startswith   |       str_startswith       |
 |      find      |          str_find          |
 |     index      |         str_index          |
 |     rfind      |         str_rfind          |
 |     rindex     |         str_rindex         |
 |    isalnum     |        str_isalnum         |
```

### Comparing `pawpaw-1.0.0rc2/docs/3. Visualization.md` & `pawpaw-1.0.0rc3/docs/3. Visualization.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/4. Arborform.md` & `pawpaw-1.0.0rc3/docs/4. Arborform.md`

 * *Files 18% similar despite different names*

```diff
@@ -84,37 +84,38 @@
 Itorators are callable objects[^callable_object] are are invoked using simple function syntax.  The single input parameter is an ``Ito``, and the return type is a generator, which you can iterate over, unpack into a container, etc:
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> i  # Starting ito has no .desc
-Ito('Hello, world!', 0, 13, None)
+Ito(span=(0, 13), desc='', substr='Hello, world!')
 >>> itor_desc = arborform.Desc('changed')  # Desc itorator: changes .desc property
 >>> next(itor_desc(i))  # Invoke itorator and get first item from pipeline
-Ito('Hello, world!', 0, 13, 'changed')
+Ito(span=(0, 13), desc='changed', substr='Hello, world!')
 ```
 
 When invoked, an itorator clones the input Ito, which guarrantees that it is unaltered by the pipeline:
 
 ```python
 >>> i  # Original remains unmodified
-Ito('Hello, world!', 0, 13, None)
+Ito(span=(0, 13), desc='', substr='Hello, world!')
 ```
 
 Transformations are performed in the ``._transform`` method, which is abstract for the base class ``Itorator``.  The ``._transform`` method is not intended to be called directly, rather, it is available for you to override in derived classes.  Several concrete itorators with implementations for ``._transform`` are available:
 
 | Concrete Class | Description                                          |
 |:---------------|:-----------------------------------------------------|
 | ``Reflect``    | Returns an unaltered ito                             |
 | ``Filter``     | Conditionally reflects an ito                        |
 | ``Desc``       | Alters the ``.desc`` for an ito and returns it       |
 | ``ValueFunc``  | Alters the ``.value_func`` for an ito and returns it |
 | ``Split``      | Splits an ito and returns the result                 |
 | ``Extract``    | Extracts and return an ito hierarchy                 |
+| ``Gaps``       | Returns itos of a given itorator along with the gaps |
 
 The arborform module also supports dynamically defining ``._transform`` behavior via the ``Itorator.wrap`` method.  This method creates a *wrapped, concrete itorator* whose behavior is defined by a method parameter you pass to it: 
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
@@ -133,23 +134,23 @@
 Note that if you use a ``return`` statement with a single Ito, the *ito itself* will be treated as iterable return type.  This can be useful if you need to return a series of one character long itos.
 
 ```python
 >>> from pawpaw import Ito
 >>> from pawpaw.arborform import Itorator
 >>> i = Itorator.wrap(lambda i: [i.clone()])  # ok: returns a list with 1 ito
 >>> [*i(Ito('abc'))]
-[Ito('abc', 0, 3, None)]
+[Ito(span=(0, 3), desc='', substr='abc')]
 
 >>> i = Itorator.wrap(lambda i: (i.clone(),))  # ok: returns a tuple with 1 ito
 >>> [*i(Ito('abc'))]
-[Ito('abc', 0, 3, None)]
+[Ito(span=(0, 3), desc='', substr='abc')]
 
 >>> i = Itorator.wrap(lambda i: i.clone())  # warning: returns an Ito...
 >>> [*i(Ito('abc'))] # ...which is also a 3-Ito sequence
-[Ito('abc', 0, 1, None), Ito('abc', 1, 2, None), Ito('abc', 2, 3, None)]
+[Ito(span=(0, 1), desc='', substr='a'), Ito(span=(1, 2), desc='', substr='b'), Ito(span=(2, 3), desc='', substr='c')]
 ```
 
 ``Itorator`` also features a ``.tag`` property, which is a convenience field that allows you to assign arbitrary labels in order to assist in the development and testing of your pipelines.
 
 Itorator chaining is implemented via the ``.connections`` property.  For more details, refer to [The Pipeline](https://github.com/rlayers/pawpaw/blob/master/docs/4.%20Arborform.md#the-pipeline) below.
 
 ### Itorator Class Diagram
@@ -250,15 +251,32 @@
 >>> rv = next(ito_vf(ito))
 >>> print(rv.value() + 3)
 5
 ```
 
 ### Split
 
-***This documentation has not yet been written***
+The ``Split`` itorator applies a regular expression to an ito via ``.regex_finditer``, and returns an Ito sequence based on the splits. Given:
+
+**P–O–O–S**
+
+where ``P`` is prefix, ``—`` is boundary, ``O`` is/are middle segments(s), and ``S`` is suffix, the beahvior of ``Split`` is governed by a BoundaryRetention parameter:
+
+| BoundaryRetention | Segments | Description |
+| :--: | :--: | :-- |
+| ``NONE`` | **P O O S** | boundaries are discarded (this is an 'ordinary' split operation) |
+| ``LEADING`` | **–O –O –S** | boundaries kept as prefixes, leading P is discarded |
+| ``TRAILING`` | **P– O– O–** | boundaries kept as suffixes, trailing S is discarded |
+| ``DISTINCT`` | **P– O– O–** | all non-zero-length boundaries kept as distincts |
+
+Zero-length boundaries are allowable.
+
+Note: Using the ``Split`` itorator with ``BoundaryRetention.DISTINCT`` is useful if you want to extract itos and then process downstream *both* the boundaries and non-boundaries.
+
+*-Further documentation for Split coming soon-*
 
 ### Extract
 
 The ``Extract`` itorator applies a regular expression to an ito via ``.regex_finditer``.  Each match is returned back as a pawpaw tree:
 
 ```python
 import regex 
@@ -356,17 +374,105 @@
 >>> import regex
 >>> from pawpaw import Ito, arborform
 >>> s = 'AB'
 >>> re = regex.compile(r'(.)(?<foo>.)')
 >>> d = lambda ito, match, group: match.group(1)  # Used first (unnamed) group as descriptor for 'foo'
 >>> extract = arborform.Extract(re, desc_func=d)
 >>> next(extract(Ito(s)))
-Ito('AB', 1, 2, 'A')
+Ito(span=(1, 2), desc='A', substr='B')
+```
+
+### Gaps
+
+The ``Gaps`` itorator evaluates a given itorator and returns the conjugates (gaps) of the itorator's results.  The result can optionally include or exclude the given itorator's results:
+
+```python
+>>> import regex 
+>>> from pawpaw import arborform, Ito
+>>> ito = Ito('ab12de')
+>>> re = regex.compile(r'(?P<number>\d+)')
+>>> itor_extract = arborform.Extract(re)
+>>> itor_gaps = arborform.Gaps(itor_extract, 'non-number')  # include non-gaps
+>>> for i in itor_gaps(ito):
+...   print(f'{i:%span %desc!r% : %substr!r}')
+... 
+(0, 2) 'non-number': 'ab'
+(2, 4) 'number': '12'
+(4, 6) 'non-number': 'de'
+>>> 
+>>> itor_gaps = arborform.Gaps(itor_extract, 'non-number', False)  # exclude non-gaps
+>>> for i in itor_gaps(ito):
+...   print(f'{i:%span %desc!r% : %substr!r}')
+... 
+(0, 2) 'non-number': 'ab'
+(4, 6) 'non-number': 'de'
+```
+
+The ``Gaps`` itorator allows you to return an itorator's results as well as the the 'non-results', ***both*** of which can then be processed downstream.  For example:
+
+```mermaid
+flowchart TD
+  subgraph Start
+    i0ab12d[''a b12 d'']
+  end
+  subgraph Step1
+    i1ab[''a b'']
+    i112[''12'']
+    i1d['' d'']
+  end
+  subgraph Step2
+    i2a[''a'']
+    i2sp1['' '']
+    i2b[''b'']
+    i212[''12'']
+    i2sp2['' '']
+    i2d[''d'']
+  end
+  subgraph Step3
+    i3a[''a'']
+    i3sp1['' '']
+    i3b[''b'']
+    i312[''12'']
+    i3sp2['' '']
+    i3d[''d'']
+  end
+  Start--"Extract (digits) w/ Gaps"-->Step1  
+  Step1--"Extract (letters) w/ Gaps"-->Step2
+  Step2--"Extract (whitespace) w/ Gaps"-->Step3
 ```
 
+The code for this is as follows:
+
+```python
+>>> import regex 
+>>> from pawpaw import arborform, Ito
+>>> ito = Ito('a b12 d')
+>>> extractors = [
+...   arborform.Extract(regex.compile('(?P<digits>\d+)')),
+...   arborform.Extract(regex.compile('(?P<letters>[a-z]+)')),
+...   arborform.Extract(regex.compile('(?P<ws>\s+)'))
+... ]
+>>> itor = arborform.Reflect()
+>>> for e in extractors:
+...   g = arborform.Gaps(e)  
+...   con = arborform.Connectors.Recurse(g, lambda ito: ito.desc is None)
+...   itor.connections.append(con)
+... 
+>>> for i in itor(ito):
+...   print(f'{i:%span %desc!r% : %substr!r}')
+(0, 1) 'letters': 'a'
+(1, 2) 'ws': ' '
+(2, 3) 'letters': 'b'
+(3, 5) 'digits': '12'
+(5, 6) 'ws': ' '
+(6, 7) 'letters': 'd'
+```
+
+Note: more sophisticated gap-consolidation techniques can be achieved using a ``Posterator`` object.
+
 ## Connector
 
 Data flow between Itorators is indicated through ``Connector`` objects.  
 
 A connector object consists of a single ``Itorator`` and an optional predicate[^predicate]:
 
 ```mermaid
@@ -597,30 +703,32 @@
   B --> C_2
   Stub --> D_1
   D_1 --> D_2
 ```
 
 ## Postorator
 
-***This documentation has not yet been written***
+The ``Postorator`` class offers a way to perform post-itorator operations, such as aggregation and other combinatorics.  Unlike itorators, whose key ability is to transform a *single* ito, class ``Postorator`` operates on ito *sequences*.
 
 ### Postorator Class Diagram
 
 ```mermaid
 classDiagram
   class Postorator{
     +tag str | None
-    +_traverse(itos) C_IT_BITOS
-    +__call__(itos) C_IT_BITOS
+    +_transform(C_IT_ITOS) C_IT_ITOS
+    +__call__(C_IT_ITOS) C_IT_ITOS
   }
 
   Postorator <|-- stacked_reduce
   Postorator <|-- windowed_join
 ```
 
+*** Additional documentation still being written... ***
+
 [^python_iter_gen]: See [generator objects](https://docs.python.org/3/c-api/gen.html) and [iterator objects](https://docs.python.org/3/c-api/iterator.html) for more information.
 
 [^itorator_name]: The name "Itorator" comes from a portmanteau of "Ito" and "Iterator"
 
 [^predicate]: A function that returns a Boolean value.
 
 [^tautology]: A function that always returns True.
```

### Comparing `pawpaw-1.0.0rc2/docs/5. Traversal & Query.md` & `pawpaw-1.0.0rc3/docs/5. Traversal & Query.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Traversal & Query
 
 ## Introduction
 
-Pawpaw's ``Ito`` class features recursive storage of descendants to arbitrary depth, resulting in a fully hierarchical data store.  The resulting trees
+Pawpaw's ``Ito`` class features recursive storage of descendants to arbitrary depth, resulting in a fully hierarchical data store.  The resulting tree
 can be searched for relevant data using either manual traversal techniques, or a highly capable structured query syntax called *plumule*[^plumule].
 
 ## Manual Traversal
 
 Manually traversing Pawpaw trees is possible using either the ``.children`` property to access an ``Ito`` object's children, or the ``.parent`` property to access its parent:
 
 ```python
@@ -35,42 +35,55 @@
 >>> print('|'.join(str(d) for d in i.walk_descendants()))
 the|t|h|e|quick|q|u|i|c|k|brown|b|r|o|w|n|fox|f|o|x
 ```
 
 ## Plumule Queries
 
 Manually traversing Pawpaw trees is practical for small collections.  Larger collections,
-by contrast, can benefit from Pawpaw *plumule* queries.  Plumule is similar in syntax to
-`XPath <https://www.w3.org/TR/xpath/>` in syntax and usage.  For example:
+by contrast, can benefit from Pawpaw's *plumule* query language.  Plumule has similar syntax and usage to 
+[XPath](https://www.w3.org/TR/xpath/).  For example:
 
 ```python
->>> plumule_xpr = '*{*[s:o]}'  # words containing char 'o'
+>>> plumule_xpr = '*{*[s:o]}'  # words containing 'o'
 >>> print([str(w) for w in i.find_all(plumule_xpr)])
 ['brown', 'fox']
 ```
 
-Because Plumule queries are strings, they can be persisted and used against multiple trees.  Plumule
-queries are interpreted by the Pawpaw *radicle* query engine, which even allows you to pre-compile
-them for faster performance:
+Plumule queries are strings and offer several advantages:
+
+* Easy string construction
+* Persistence
+* Can be run against multiple, *arbitrary* trees
+ 
+Plumule queries are interpreted by Pawpaw's *radicle* query engine, which even allows pre-compilation to improve run-time
+performance:
 
 ```python
 >>> query = pawpaw.query.compile(plumule_xpr)
 >>> print([str(w) for w in query.find_all(i)])
 ['brown', 'fox']
 ```
 
-### Query
+## Plumule Syntax
 
-A Plumule query allows you to query for arbitrary nodes in an ``Ito`` Tree.  A query consists
-of one or more *phrases* separated by fore-slash characters:
+Plumule query sytax allows you to search for arbitrary nodes in an ``Ito`` Tree.  A Plumule query comprises a sequence of one or more *phrases* separated by fore-slash characters:
 
 ```
 query := phrase [/ phrase] [/ phrase] ...
 ```
 
+Phrases, in turn, consists of axes, filters, and subqueries:
+
+* Phrases
+  * Axes
+  * Filters
+  * Subqueries
+
+Each component is further discussed below.
+
 ### Phrase
 
 A phrase consists of an *axis* along with an optional *filters* and *subqueries* parts:
 
 ```
 phrase := axis [filters] [subqueries]
 ```
@@ -147,22 +160,14 @@
 
 ```
 filters := [not_operator] filter [ combining_operator [not_operator] filter ]...
 ````
 
 Parentheses can be used for grouping to override operator precedence as needed.
 
-
-, and grouped as needed with parentheses:
-
-defines nodes matching a given criteria to pass through,
-and conists of one or more *filter* expressions separated by logical operators.  Parentheses may be used
-to group filter expressions when you need to override the default operator precedence:
-
-
 #### Operators
 
 The *not operator* consists of the tilde character (``'~'``):
 
 ```
 not_operator := '~'
 ```
@@ -308,15 +313,15 @@
 '*{*}'  # children that themselves have at least one child
 '.{**[d:word]}'  # nodes having descendants with .desc == 'word'
 '.[d:digit]{**{[s:4,6] | ~[d:prime]} | !{..[d:sci]}'  # nodes with .desc == 'digit' and having a) descendants with substr in ['4', '6'] or b) ancestors with .desc = 'sci'
 ```
 
 ## Tips & Tricks
 
-Q: How can I 'OR' together the filters and subqueries components?
+Q: How can I 'OR' together filter and subquery components?
 
 A: Operators are not supported between the filters and subqueries components of a query phrase.  However, you can achieve the same result by moving the filter to a subquery::
 
 ```
 [my_filter]{my_subquery}  ->  {./[my_filter]} | {my_subquery}
 ```
```

### Comparing `pawpaw-1.0.0rc2/docs/6. Xml.md` & `pawpaw-1.0.0rc3/docs/6. Xml.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/7. NLP.md` & `pawpaw-1.0.0rc3/docs/7. NLP.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/8. Serialization.md` & `pawpaw-1.0.0rc3/docs/8. Serialization.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,12 +58,12 @@
 
 ```python
 >>> json_data = json.dumps(i, cls=Ito.JsonEncoderStringless)
 >>> s in json_data  # verify s not present in JSON
 False
 >>> j = Ito.json_decode_stringless(s, json_data)
 >>> j
-Ito('See Jack run.', 0, 13, 'my desc')
+Ito(span=(0, 13), desc='my desc', substr='See Jack run.')
 ```
 
 [^lambda_pickling]: The python pickle library supports neither lambdas nor methods not-defined at the top level of a module.  See `Python pickle docs
 <https://docs.python.org/3/library/pickle.html/>` for more info.
```

### Comparing `pawpaw-1.0.0rc2/docs/Pawpaw Cookbook.md` & `pawpaw-1.0.0rc3/docs/Pawpaw Cookbook.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 ### Extract all characters as ``Ito``
 
 ```python
 >>> s = ' abc '
 >>> i = Ito(s, 1, -1)
 >>> [*i]
-[Ito(' abc ', 1, 2, None), Ito(' abc ', 2, 3, None), Ito(' abc ', 3, 4, None)]
+[Ito(span=(1, 2), desc='', substr='a'), Ito(span=(2, 3), desc='', substr='b'), Ito(span=(3, 4), desc='', substr='c')]
+
 ```
 
 ### Extract all characters as ``str`` 
 
 ```python
 >>> from pawpaw import Ito
 >>> s = 'abc'
@@ -31,15 +32,15 @@
 
 ```python
 >>> from pawpaw import Ito
 >>> s = ' abc '
 >>> i = Ito(s, 1, -1)
 >>> i.children.add(*i)
 >>> [*i.children]
-[Ito(' abc ', 1, 2, None), Ito(' abc ', 2, 3, None), Ito(' abc ', 3, 4, None)]
+[Ito(span=(1, 2), desc='', substr='a'), Ito(span=(2, 3), desc='', substr='b'), Ito(span=(3, 4), desc='', substr='c')]
 ```
 
 ### Create a char-extracting ``Itorator``
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> char_itor = arborform.Itorator.wrap(lambda ito: iter(ito))  # 1. If you don't need a desc
@@ -69,15 +70,15 @@
    ├──(46, 52) 'Word' : 'Sleepy'
    ├──(53, 59) 'Word' : 'Hollow'
    ├──(61, 63) 'Word' : 'by'
    ├──(64, 74) 'Word' : 'Washington'
    └──(75, 81) 'Word' : 'Irving'
 ```
 
-### Extract children and then extract a second set of children based on the leftover space
+### Extract children and then extract a second set of children based on the leftover space without using ``Gaps``
 
 **Code:**
 
 ```python
 from pawpaw import Ito, arborform, visualization
 import regex
```

### Comparing `pawpaw-1.0.0rc2/docs/Using Pawpaw with nltk.md` & `pawpaw-1.0.0rc3/docs/Using Pawpaw with nltk.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/Q&A/description.md` & `pawpaw-1.0.0rc3/docs/demos/Q&A/description.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/Q&A/solution.py` & `pawpaw-1.0.0rc3/docs/demos/Q&A/solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # INPUT
 text = """\na\n\nQ So I do first want to bring up exhibit No. 46, which is in the binder 
 in front of\nyou.\n\nAnd that is a letter [to] Alston\n& Bird...
 \n\nIs that correct?\n\nA This is correct.\n\nQ Okay."""
 
 # BUILD PARSER
-itor_split = arborform.Split(regex.compile(r'\n+(?=Q_? )', regex.DOTALL), desc='Q/A tuple')
+itor_split = arborform.Split(regex.compile(r'\n+(?=Q_? )', regex.DOTALL), non_boundary_desc='Q/A tuple')
 
 itor_filt = arborform.Filter(lambda i: i.str_startswith('Q'))  # toss "random text" stuff
 con = arborform.Connectors.Delegate(itor_filt)
 itor_split.connections.append(con)
 
 # Assumes only one answer per question
 itor_qa_split = arborform.Split(regex.compile(r'\n+(?=A_? )', regex.DOTALL), limit=1)
```

### Comparing `pawpaw-1.0.0rc2/docs/demos/class_grades/description.md` & `pawpaw-1.0.0rc3/docs/demos/class_grades/description.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/class_grades/input.txt` & `pawpaw-1.0.0rc3/docs/demos/class_grades/input.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/class_grades/parser_verbose.py` & `pawpaw-1.0.0rc3/docs/demos/class_grades/parser_verbose.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import regex
 from pawpaw import arborform
 
 def get_parser() -> arborform.Itorator:
     school_splitter = arborform.Split(
         regex.compile(r'(?<=(?:^|\n))(?=School =)', regex.DOTALL),
-        desc='school',
+        non_boundary_desc='school',
         tag='school splitter')
 
     name_grades = arborform.Extract(
         regex.compile(r'School = (?<name>.+?)\n(?<grades>.+)(?:$|\n)', regex.DOTALL),
         tag='school name & grades')
     con = arborform.Connectors.Children.Add(name_grades)
     school_splitter.connections.append(con)
 
     grade_splitter = arborform.Split(
         regex.compile(r'(?<=\n)(?=Grade =)', regex.DOTALL),
-        desc='grade',
+        non_boundary_desc='grade',
         tag='grade splitter')
     con = arborform.Connectors.Delegate(grade_splitter, lambda ito: ito.desc == 'grades')
     name_grades.connections.append(con)
 
     grade = arborform.Extract(
         regex.compile(r'Grade = (?<key>\d+)\nStudent number, Name\n(?<stu_num_names>.+?)\nStudent number, Score\n(?<stu_num_scores>.+)', regex.DOTALL),
         tag='grade & stu_num/name * stu_num/score')
```

### Comparing `pawpaw-1.0.0rc2/docs/demos/class_grades/solution.py` & `pawpaw-1.0.0rc3/docs/demos/class_grades/solution.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/gettysburg_address/gettysburg_address.txt` & `pawpaw-1.0.0rc3/docs/demos/gettysburg_address/gettysburg_address.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.py` & `pawpaw-1.0.0rc3/docs/demos/us_constitution/us_constitution.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     con = arborform.Connectors.Children.Add(a_extractor, lambda ito: ito.desc == 'article')
     a_desc.connections.append(con)
 
     # Section: only some articles have sections
     s_splitter = arborform.Split(
         regex.compile(r'(?<=\n+)(?=Section\.)', regex.DOTALL),
         boundary_retention=arborform.Split.BoundaryRetention.LEADING,
-        desc='section',
+        non_boundary_desc='section',
         tag='section splitter')
     con = arborform.Connectors.Children.Add(s_splitter, lambda ito: ito.desc == 'value' and ito.str_startswith('Section.'))
     a_extractor.connections.append(con)
     con = arborform.Connectors.Children.Add(pawpaw.nlp.SimpleNlp().itor, lambda ito: ito.desc == 'value' and not ito.str_startswith('Section.'))
     a_extractor.connections.append(con)
 
     s_extractor = arborform.Extract(regex.compile(r'Section\. (?<key>\d+)\.\n(?<value>.+)', regex.DOTALL))
```

### Comparing `pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.txt` & `pawpaw-1.0.0rc3/docs/demos/us_constitution/us_constitution.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/images/pawpaw.png` & `pawpaw-1.0.0rc3/images/pawpaw.png`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/__init__.py` & `pawpaw-1.0.0rc3/pawpaw/__init__.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/_type_magic.py` & `pawpaw-1.0.0rc3/pawpaw/_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/_version.py` & `pawpaw-1.0.0rc3/pawpaw/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import string
 import typing
 
 import regex
 
-__version__ = '1.0.0rc2'
+__version__ = '1.0.0rc3'
 """The str literal that build, setup, documentation, and other tools typically want."""
 
 class Version:
     _canonical_re = regex.compile(r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?(?:\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*)?$')
     """This pattern taken from https://peps.python.org/pep-0440/#appendix-b-parsing-version-strings-with-regular-expressions
     and expanded to support optional "local version identifier" (see https://peps.python.org/pep-0440/#local-version-identifiers)."""
```

### Comparing `pawpaw-1.0.0rc2/pawpaw/errors.py` & `pawpaw-1.0.0rc3/pawpaw/errors.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/infix.py` & `pawpaw-1.0.0rc3/pawpaw/infix.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/ito.py` & `pawpaw-1.0.0rc3/pawpaw/ito.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import bisect
 import collections.abc
 import json
+import os
 import types
 import typing
 if typing.TYPE_CHECKING:
     from _typeshed import SupportsRichComparison
 
 import regex
 
@@ -14,15 +15,14 @@
 from .util import find_escapes
 
 
 nuco = Infix(lambda x, y: y if x is None else x)
 """Null coalescing operator
 """
 
-
 class Ito:
     # region ctors & clone
 
     def __init__(
         self,
         src: str | Ito,
         start: int | None = None,
@@ -168,16 +168,16 @@
         yield from (cls(src, *s, desc=desc) for s in spans)
 
     @classmethod
     def from_gaps(
             cls,
             src: str | pawpaw.Ito,
             non_gaps: typing.Iterable[Span | pawpaw.Ito],
-            return_zero_widths: bool = False,
-            desc: str | None = None
+            desc: str | None = None,
+            return_zero_widths: bool = False
     ) -> typing.Iterable[pawpaw.Ito]:
         """Generate Itos based on negative space (gaps)
 
         Args:
             src: a str or Ito to use as the basis
             non_gaps: one or more Spans (relative to src) or Itos (whose .string matches basis) to be excluded from the result; must be ordered; overlaps are fine spans within the basis; can be unordered; overlaps are fine; zero-widths are fine
             return_zero_widths: If true, zero-width Itos will be returned for non-overlapping, adjacent non-gaps
@@ -492,15 +492,15 @@
             for i in range(*self.span):
                 yield self.clone(i, i + 1, clone_children=False)
 
     def __ne__(self, o: typing.Any) -> bool:
         return not self.__eq__(o)
 
     def __repr__(self) -> str:
-        return f'{type(self).__name__}({self._string.__repr__()}, {self.start}, {self.stop}, {self.desc.__repr__()})'
+        return f'{type(self).__name__}({self:span=%span, desc=%desc!r, substr=%substr!r})'
 
     def __str__(self) -> str:
         return self._string[slice(*self.span)]
 
     def __len__(self) -> int:
         return self.stop - self.start
 
@@ -600,15 +600,15 @@
                 else:  # 'stop'
                     sub = format(self.stop, fstr)
 
             elif directive in self._format_str_directives:
                 if directive == 'string':
                     sub = self._string
                 elif directive == 'desc':
-                    sub = self.desc
+                    sub = self.desc or ''
                 elif directive == 'substr':
                     sub = self.__str__()
                 else:  # 'value'
                     sub = str(self.value())
 
                 if (conv := m.group('conv')) is not None:
                     if conv == 'a':
@@ -765,15 +765,15 @@
             - Else returns a clone with children corresponding to the non-overlapping, non-contiguous gpas in self's children.
         """
         rv = self.clone(clone_children=False)
         
         if len(self) == 0:
             return rv
 
-        rv.children.add(*self.from_gaps(rv, self.children, False, desc))
+        rv.children.add(*self.from_gaps(rv, self.children, desc, False))
         return rv
 
     def split_iter(
             self,
             re: regex.Pattern,
             max_split: int = 0,
             keep_seps: bool = False,
@@ -880,14 +880,17 @@
     # endregion
 
     # region str equivalence methods
 
     def str_count(self, sub: str, start: int | None = None, end: int | None = None) -> int:
         return self._string.count(sub, *Span.from_indices(self, start, end).offset(self.start))
 
+    def str_eq(self, val: str) -> bool:
+        return len(self) == len(val) and self.str_startswith(val)
+
     # region endswtih, startswtih
         
     def str_endswith(
             self,
             suffix: str | typing.Tuple[str, ...],
             start: int | None = None,
             end: int | None = None
@@ -1286,14 +1289,28 @@
             values: typing.Dict[str, typing.Any] | None = None,
             predicates: typing.Dict[str, typing.Callable[[int, pawpaw.Ito], bool]] | None = None
     ) -> pawpaw.Ito | None:
         return pawpaw.query.find(path, self, values, predicates)
 
     # endregion
 
+    # region utility
+
+    def to_line_col(self, eol: str = os.linesep) -> tuple[int, int]:
+        prior_eol_idx = self.string.rfind(eol, 0, self.start)
+        if prior_eol_idx == -1:
+            line = 1
+            col = self.start + 1
+        else:
+            line = self.string.count(eol, 0, prior_eol_idx) + 2
+            col = self.start - prior_eol_idx
+
+        return line, col
+
+    # endregion
 
 class ChildItos(collections.abc.Sequence):
     def __init__(self, parent: pawpaw.Ito, *itos: pawpaw.Ito):
         self.__parent = parent
         self.__store: typing.List[pawpaw.Ito] = []
         self.add(*itos)
 
@@ -1501,15 +1518,15 @@
             ito._set_parent(self.__parent)
 
     # endregion
 
     # region __repr__
 
     def __repr__(self) -> str:
-        return f'{type(self).__name__}(parent={self.__parent.__repr__()}, *{self.__store.__repr__()}'    
+        return f'{type(self).__name__}(parent={self.__parent.__repr__()}, *{self.__store.__repr__()}'
 
     # endregion
 
 
 class Types:
     # Ito
     C_SQ_ITOS = typing.Sequence[Ito]
```

### Comparing `pawpaw-1.0.0rc2/pawpaw/span.py` & `pawpaw-1.0.0rc3/pawpaw/span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/util.py` & `pawpaw-1.0.0rc3/pawpaw/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/desc.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/itorator/desc.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/extract.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/itorator/extract.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/filter.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/itorator/filter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/itorator.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/itorator/itorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/value_func.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/itorator/value_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/postorator.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/postorator/postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/stacked_reduce.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/postorator/stacked_reduce.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/windowed_join.py` & `pawpaw-1.0.0rc3/pawpaw/arborform/postorator/windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/nlp/nlp.py` & `pawpaw-1.0.0rc3/pawpaw/nlp/nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             raise pawpaw.Errors.parameter_invalid_type('val', val, int)
 
     @property
     def re(self) -> regex.Pattern:
         return self._re
 
     def get_itor(self) -> pawpaw.arborform.Itorator:
-        rv = pawpaw.arborform.Split(self._re, desc='paragraph', tag='para splitter')
+        rv = pawpaw.arborform.Split(self._re, non_boundary_desc='paragraph', tag='para splitter')
 
         ws_trimmer = pawpaw.arborform.Itorator.wrap(lambda ito: [ito.str_strip(''.join(trimmable_ws))], tag='para trimmer')
         con = pawpaw.arborform.Connectors.Recurse(ws_trimmer)
         rv.connections.append(con)
 
         return rv
 
@@ -416,23 +416,23 @@
     )
 
     @property
     def re(self) -> regex.Pattern:
         return self._re
 
     def get_itor(self) -> pawpaw.arborform.Itorator:
-        return pawpaw.arborform.Split(Sentence().re, desc='sentence', tag='sentence')       
+        return pawpaw.arborform.Split(Sentence().re, non_boundary_desc='sentence', tag='sentence')       
 
 
 class SimpleNlp:
     _word_pat = r'\w(?:(?:\L<sqs>|-\s*)?\w)*'
 
     @classmethod
     def get_sentence(cls) -> pawpaw.arborform.Itorator:
-        return pawpaw.arborform.Split(Sentence().re, desc='sentence', tag='sentence')
+        return pawpaw.arborform.Split(Sentence().re, non_boundary_desc='sentence', tag='sentence')
 
     def __init__(self, number: Number | None = None, chars: bool = False):
         super().__init__()
 
         paragraph = Paragraph().get_itor()
 
         sentence = Sentence().get_itor()
```

### Comparing `pawpaw-1.0.0rc2/pawpaw/nlp/table.py` & `pawpaw-1.0.0rc3/pawpaw/nlp/table.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/query/_query.py` & `pawpaw-1.0.0rc3/pawpaw/query/_query.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/visualization/ascii_box.py` & `pawpaw-1.0.0rc3/pawpaw/visualization/ascii_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1098,15 +1098,17 @@
         self.s = s
 
         if not (isinstance(se, BoxDrawingChar) or isinstance(se, str)):
             raise Errors.parameter_invalid_type('se', se, BoxDrawingChar, str)
         self.se = se
 
     def _from_lines(self, *lines: Ito) -> typing.List[str]:
-        max_line = max(len(line) for line in lines)
+        # TODO: Handle SGR, unicode modifying graphemes, etc. to
+        # get max column width of printed lines
+        max_line = max(sum(1 for c in line if c.str_isprintable()) for line in lines)
 
         rv = [f'{self.nw}{str(self.n) * (max_line + 2)}{self.ne}']
 
         for line in lines:
             rv.append(f'{self.w} {str(line):^{max_line}} {self.e}')
 
         rv.append(f'{self.sw}{str(self.s) * (max_line + 2)}{self.se}')
```

### Comparing `pawpaw-1.0.0rc2/pawpaw/visualization/highlighter.py` & `pawpaw-1.0.0rc3/pawpaw/visualization/highlighter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/visualization/pepo/pepo.py` & `pawpaw-1.0.0rc3/pawpaw/visualization/pepo/pepo.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/visualization/sgr/sgr.py` & `pawpaw-1.0.0rc3/pawpaw/visualization/sgr/sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/visualization/sgr/palettes/palettes.py` & `pawpaw-1.0.0rc3/pawpaw/visualization/sgr/palettes/palettes.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/xml/xml_helper.py` & `pawpaw-1.0.0rc3/pawpaw/xml/xml_helper.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/pawpaw/xml/xml_parser.py` & `pawpaw-1.0.0rc3/pawpaw/xml/xml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,17 @@
             attrs_parent.children.add(*attrs)
             start_tag.children.add(attrs_parent)
 
         for tag in start_tag.find_all('**[d:' + xml.descriptors.TAG + ']'):
             qn = xml.QualifiedName.from_src(tag)
             tag.value_func = lambda i: qn
 
-        if (element._spans.char.stop + 2) < len(self._text) and self._text[element._spans.char.stop:element._spans.char.stop + 2] == '</':
+        if self._text[element._spans.char.stop-2:element._spans.char.stop] not in ('/>', '?>') \
+                and (element._spans.char.stop + 2) < len(self._text) \
+                and self._text[element._spans.char.stop:element._spans.char.stop + 2] == '</':
             end_tag = Ito(
                 self._text,
                 element._spans.char.stop,
                 self._text.index('>', element._spans.char.stop + 1) + 1,
                 xml.descriptors.END_TAG)
             for c in self._itor_extract_tag(end_tag):
                 c.value_func = lambda i: xml.QualifiedName.from_src(c)
@@ -165,15 +167,15 @@
 
             if last_child is not None:
                 if (t := self._find_text(last_child.ito.stop, child.ito.start)) is not None:
                     ito.children.add(t)
 
             last_child = child
 
-        if last_child is not None:
+        if last_child is not None and end_tag is not None:
             if (t := self._find_text(last_child.ito.stop, end_tag.start)) is not None:
                 ito.children.add(t)
 
         if end_tag is not None:
             stop = element[0].ito.start if len(element) > 0 else end_tag.start
             if (t := self._find_text(start_tag.stop, stop)) is not None:
                 ito.children.add(t)
```

### Comparing `pawpaw-1.0.0rc2/tests/test_child_itos.py` & `pawpaw-1.0.0rc3/tests/test_child_itos.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_invoke_func.py` & `pawpaw-1.0.0rc3/tests/test_invoke_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_ito.py` & `pawpaw-1.0.0rc3/tests/test_ito.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,19 +214,18 @@
 
     def test_repr(self):
         s = 'x123x'
         span = Span.from_indices(s, 1, -1)
         desc = 'd'
         for ito in Ito(s, *span, desc), IntIto(s, *span, desc):
             with self.subTest(string=s, ito=ito):
-                expected = f'{type(ito).__name__}({s.__repr__()}, {span.start}, {span.stop}, {desc.__repr__()})'
+                expected = f'{type(ito).__name__}(span=({ito.start}, {ito.stop}), desc={ito.desc!r}, substr={str(ito)!r})'
                 actual = ito.__repr__()
                 self.assertEqual(expected, actual)
-                self.assertEqual(ito, eval(actual))
-    
+
     def test_str(self):
         s = 'x123x'
         for span in Span(0, len(s)), Span(1, len(s) - 1):
             for ito in Ito(s, *span), IntIto(s, *span):
                 expected = s[slice(*span)]
                 for expression in 'ito.__str__()', 'str(ito)', "f'{ito}'":
                     with self.subTest(string=s, ito=ito, expression=expression):
```

### Comparing `pawpaw-1.0.0rc2/tests/test_ito_ctor.py` & `pawpaw-1.0.0rc3/tests/test_ito_ctor.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 if i.str_isspace():
                     expected.append(i.clone(desc=desc))
                 else:
                     non_gaps.append(i)
 
             for ngs in non_gaps, [ng.span for ng in non_gaps]:
                 with self.subTest(src=s, non_gaps=ngs):
-                    actual = [*Ito.from_gaps(s, ngs, desc=desc)]
+                    actual = [*Ito.from_gaps(s, ngs, desc)]
                     self.assertSequenceEqual(expected, actual)
 
     def test_from_gaps_src_ito_1(self):
         desc = 'non gap'
         for s in '', 'a', ' ', 'ab', ' ab', 'a b', 'ab ', ' a b ':
             s = f' {s} '
             src = Ito(s, 1, -1)
@@ -202,15 +202,15 @@
                 if i.str_isspace():
                     expected.append(i.clone(desc=desc))
                 else:
                     non_gaps.append(i)
 
             for ngs in non_gaps, [ng.span.offset(-1) for ng in non_gaps]:
                 with self.subTest(src=src, non_gaps=ngs):
-                    actual = [*Ito.from_gaps(src, ngs, desc=desc)]
+                    actual = [*Ito.from_gaps(src, ngs, desc)]
                     self.assertSequenceEqual(expected, actual)
 
     def test_from_gaps_src_str_2(self):
         src = ' abc '
         non_gap_starts = src.find('a'), src.find('c')
 
         for width in 0, 1:
@@ -255,82 +255,82 @@
                         actual = [*Ito.from_gaps(src, non_gaps)]
                         self.assertListEqual(expected, actual)
 
     def test_from_gaps_none(self):
         src = 'abc'
         desc = 'X'
         expected = Ito(src, desc=desc)
-        actual = next(Ito.from_gaps(src, [], desc=desc), None)
+        actual = next(Ito.from_gaps(src, [], desc), None)
         self.assertIsNotNone(actual)
         self.assertEqual(expected, actual)
 
     def test_from_gaps_identity(self):
         src = 'abc'
         desc = 'X'
-        actual = next(Ito.from_gaps(src, [Ito(src)], desc=desc), None)
+        actual = next(Ito.from_gaps(src, [Ito(src)], desc), None)
         self.assertIsNone(actual)
 
     def test_from_gaps_contiguous_non_gaps(self):
         src = 'abc'
         desc = 'X'
-        actual = next(Ito.from_gaps(src, Ito(src), desc=desc), None)
+        actual = next(Ito.from_gaps(src, Ito(src), desc), None)
         self.assertIsNone(actual)            
 
     def test_from_gaps_with_zero_widths(self):
         desc = 'non gap'
 
         with self.subTest(non_gap_count=2, non_gap_proximity='adjacent', non_gap_extent='contained'):
             s = ' abc '
             root = Ito(s, 1, -1)
             root.children.add(*root)
             expected = [Ito(root, i, i, desc) for i in range(1, len(root))]
-            rv = [*root.from_gaps(root, root.children, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, root.children, desc, True)]
             self.assertEqual(len(expected), len(rv))
             self.assertSequenceEqual(expected, rv)
 
         with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='contained'):
             overlapping_non_gaps = [Ito(s, *root.span), Ito(s, root.start + 1, root.stop)]
-            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, desc, True)]
             self.assertEqual(0, len(rv))
 
         with self.subTest(non_gap_count=3, non_gap_proximity='overlapping', non_gap_extent='contained'):
             overlapping_non_gaps = [Ito(s, root.start + i, root.stop) for i in range(0, len(root))]
-            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, desc, True)]
             self.assertEqual(0, len(rv))
 
         with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='non-contained'):
             overlapping_non_gaps = [Ito(s, 0, len(s) - 1), Ito(s, 1, len(s) + 2)]
-            rv = [*root.from_gaps(root, overlapping_non_gaps, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, overlapping_non_gaps, desc, True)]
             self.assertEqual(0, len(rv))
 
         with self.subTest(non_gap_count=1, non_gap_proximity='N/A', non_gap_extent='non-contained', location='prior'):
             ng_prior = [Ito(s, 0, 1)]
             rv = [*root.from_gaps(root, ng_prior, return_zero_widths=True, desc=desc)]
             self.assertEqual(1, len(rv))
             self.assertEqual(root.clone(desc=desc), rv[0])
 
         with self.subTest(non_gap_count=1, non_gap_proximity='N/A', non_gap_extent='non-contained', location='after'):
             ng_after = [Ito(s, -1)]
-            rv = [*root.from_gaps(root, ng_after, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, ng_after, desc, True)]
             self.assertEqual(1, len(rv))
             self.assertEqual(root.clone(desc=desc), rv[0])
 
         with self.subTest(non_gap_count=2, non_gap_proximity='overlapping', non_gap_extent='non-contained'):
             ng = ng_prior + ng_after
-            rv = [*root.from_gaps(root, ng, return_zero_widths=True, desc=desc)]
+            rv = [*root.from_gaps(root, ng, desc, True)]
             self.assertEqual(1, len(rv))
             self.assertEqual(root.clone(desc=desc), rv[0])
 
     def test_from_gaps_simple(self):
         s = 'abcd' * 10
         non_gaps = [*RandSpans(Span(1, 8), Span(0, 3)).generate(s)]
         desc = 'x'
         for cls_name, _class in (('Base (Ito)', Ito), ('Derived (IntIto)', IntIto)):
             with self.subTest(_class=cls_name):
-                for i in _class.from_gaps(s, non_gaps, desc=desc):
+                for i in _class.from_gaps(s, non_gaps, desc):
                     self.assertIsInstance(i, _class)
                     self.assertIs(s, i.string)
                     self.assertFalse(any(gap.start <= i.start <= i.stop <= gap.stop for gap in non_gaps))
                     self.assertEqual(desc, i.desc)
 
     def test_from_gaps_complex(self):
         s = 'abcd' * 10
@@ -342,20 +342,20 @@
                     if ordered:
                         ngs = non_gaps.copy()
                         ngs.sort(key=lambda i: i.start)
                         expected = [
                             _class(s, 0, min(gap.start for gap in non_gaps), desc),
                             _class(s, max(gap.stop for gap in non_gaps), desc=desc)
                         ]
-                        actual = [*_class.from_gaps(s, ngs, desc=desc)]
+                        actual = [*_class.from_gaps(s, ngs, desc)]
                         self.assertListEqual(expected, actual)
                     else:
                         ngs = non_gaps.copy()
                         with self.assertRaises(ValueError):
-                            [*_class.from_gaps(s, ngs, desc=desc)]
+                            [*_class.from_gaps(s, ngs, desc)]
 
     def test_from_substrings(self):
         string = 'abcd' * 10
         string = f' {string} '
 
         with self.subTest(spacing='Consecutive'):
             for size in ((1, 1), (2, 2), (1, 3), (2, 3)):
```

### Comparing `pawpaw-1.0.0rc2/tests/test_ito_descend.py` & `pawpaw-1.0.0rc3/tests/test_ito_descend.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_ito_regex_equivalence_methods.py` & `pawpaw-1.0.0rc3/tests/test_ito_regex_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_ito_serialization.py` & `pawpaw-1.0.0rc3/tests/test_ito_serialization.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_ito_str_equivalence_methods.py` & `pawpaw-1.0.0rc3/tests/test_ito_str_equivalence_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,26 @@
             with self.subTest(sub=sub):
                 self.assertEqual(str(i).count(sub), i.str_count(sub))
                 self.assertEqual(str(i).count(sub, 2, -2), i.str_count(sub, 2, -2))
                 self.assertEqual(str(i).count(sub, 3, -3), i.str_count(sub, 3, -3))
                 self.assertEqual(str(i).count(sub, 4), i.str_count(sub, 4))
                 self.assertEqual(str(i).count(sub, None, -4), i.str_count(sub, end=-4))
 
+    def test_str_eq(self):
+        s = 'aabba'
+        for i in range(0, len(s)):
+            for j in range(i, len(s)):
+                ito = Ito(s, i, j)
+                for x in range(0, len(s)):
+                    for y in range(x, len(s)):
+                        substr = s[x:y]
+                        with self.subTest(substr=substr, ito=str(ito)):
+                                expected = s == str(substr)
+                                self.assertEqual(expected, ito.str_eq(s))
+
     def test_str_endswith(self):
         s = f' {"abc" * 2} '
         ito = Ito(s, 1, -1)
 
         sep = None
         with self.subTest(src=s, sep=sep):
             with self.assertRaises(TypeError):
```

### Comparing `pawpaw-1.0.0rc2/tests/test_nlp.py` & `pawpaw-1.0.0rc3/tests/nlp/test_nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 [
                     'The U.S. Government decided against action.',
                 ]
             ),            
         ]
 
     def test_all(self):
-        sbd = pawpaw.arborform.Split(pawpaw.nlp.Sentence().re, desc='sentence')
+        sbd = pawpaw.arborform.Split(pawpaw.nlp.Sentence().re, non_boundary_desc='sentence')
 
         for td in self.test_data:
             with self.subTest(description=td.description, text=td.text):
                 text = pawpaw.Ito(td.text)
                 expected = [*pawpaw.Ito.from_substrings(text, *td.expected, desc='sentence')]
                 actual = [*sbd(text)]
                 self.assertListEqual(expected, actual)
```

### Comparing `pawpaw-1.0.0rc2/tests/test_query_and_traversal.py` & `pawpaw-1.0.0rc3/tests/test_query_and_traversal.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_span.py` & `pawpaw-1.0.0rc3/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_type_magic.py` & `pawpaw-1.0.0rc3/tests/test_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_util.py` & `pawpaw-1.0.0rc3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_version.py` & `pawpaw-1.0.0rc3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_xml_helper.py` & `pawpaw-1.0.0rc3/tests/test_xml_helper.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/test_xml_parser.py` & `pawpaw-1.0.0rc3/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/util.py` & `pawpaw-1.0.0rc3/tests/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_connectors.py` & `pawpaw-1.0.0rc3/tests/arborform/test_connectors.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_itorator.py` & `pawpaw-1.0.0rc3/tests/arborform/test_itorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_itorator_extract.py` & `pawpaw-1.0.0rc3/tests/arborform/test_itorator_extract.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_itorator_filter.py` & `pawpaw-1.0.0rc3/tests/arborform/test_itorator_filter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_itorator_split.py` & `pawpaw-1.0.0rc3/tests/arborform/test_itorator_split.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import typing
 
 import regex
 from pawpaw import Ito
 from pawpaw.arborform import Split
 from tests.util import _TestIto
 
@@ -11,14 +12,16 @@
     MIDDLE = 'MID'
     SUFFIX = 'SUF'
   
     @classmethod
     def str_from(cls, sep: str) -> str:
         return sep.join((cls.PREFIX, cls.MIDDLE, cls.MIDDLE, cls.SUFFIX))
     
+    SEP_DESC = 'sep'
+
     @classmethod
     def re_from(cls, sep: str) -> regex.Pattern:
         return regex.compile(regex.escape(sep), regex.DOTALL)
     
     @classmethod
     def expected_from(cls, s: str, sep: str, brt: Split.BoundaryRetention) -> typing.List[str]:
         if sep == '':
@@ -29,42 +32,44 @@
             del rv[0]
             for i, s in enumerate(rv):
                 rv[i] = sep + s
         elif brt == Split.BoundaryRetention.TRAILING:
             del rv[-1]
             for i, s in enumerate(rv):
                 rv[i] += sep
+        elif brt == Split.BoundaryRetention.DISTINCT:
+            rv = rv[:1] + list(itertools.chain.from_iterable((sep, i) for i in rv[1:]))
 
         return rv
     
     def test_iter_simple(self):
         for sep in ' ', '-':  # '', ' ', '-':
             s = self.str_from(sep)
             ito = Ito(s, desc='root')
             re = self.re_from(sep)
             for brt in Split.BoundaryRetention:
                 with self.subTest(string=s, separator=sep, boundary_retention=brt):
                     expected = self.expected_from(s, sep, brt)
-                    desc = 'split'
-                    split = Split(re, boundary_retention=brt, desc=desc)
+                    non_sep_desc = 'split'
+                    split = Split(re, boundary_retention=brt, boundary_desc=self.SEP_DESC, non_boundary_desc=non_sep_desc)
                     actual = [*split._transform(ito)]
                     self.assertListEqual(expected, [str(i) for i in actual])
-                    self.assertTrue(all(i.desc == desc for i in actual))
+                    self.assertTrue(all(i.desc in (self.SEP_DESC, non_sep_desc) for i in actual))
 
     def test_iter_sep_not_present(self):
         sep = 'XXX'
         s = self.str_from(' ')
         ito = Ito(s)
         re = regex.compile(regex.escape(sep))
         desc='post-split'
         for brt in Split.BoundaryRetention:
             for return_zero_split in True, False:
-                with self.subTest(string=s, separator=sep, boundary_retention=brt, return_zero_split=return_zero_split, desc=desc):
+                with self.subTest(string=s, separator=sep, boundary_retention=brt, return_zero_split=return_zero_split, non_boundary_desc=desc):
                     expected = [ito.clone(desc=desc)] if return_zero_split else []
-                    split = Split(re, boundary_retention=brt, return_zero_split=return_zero_split, desc=desc)
+                    split = Split(re, boundary_retention=brt, return_zero_split=return_zero_split, non_boundary_desc=desc)
                     actual = [*split._transform(ito)]
                     self.assertListEqual(expected, actual)
 
     @classmethod
     def zero_width_patterns(cls, sep: str) -> typing.Iterable[regex.Pattern]:
         esc_sep = regex.escape(sep)
         yield r'(?<=' + esc_sep + r')'  # look behind
@@ -80,15 +85,15 @@
                 with self.subTest(string=s, pattern=pat, boundary_retention=brt):
                     expected = re.split(s)
                     if brt == Split.BoundaryRetention.LEADING:
                         del expected[0]
                     elif brt == Split.BoundaryRetention.TRAILING:
                         del expected[-1]
                     desc = 'split'
-                    split = Split(re, boundary_retention=brt, desc=desc)
+                    split = Split(re, boundary_retention=brt, non_boundary_desc=desc)
                     actual = [*split._transform(ito)]
                     self.assertListEqual(expected, [str(i) for i in actual])
                     self.assertTrue(all(i.desc == desc for i in actual))
 
     def test_limit(self):
         s = 'abc'
         root = Ito(s)
```

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_itorator_value_func.py` & `pawpaw-1.0.0rc3/tests/arborform/test_itorator_value_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_postorator.py` & `pawpaw-1.0.0rc3/tests/arborform/test_postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/arborform/test_postorator_windowed_join.py` & `pawpaw-1.0.0rc3/tests/arborform/test_postorator_windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/visualization/test_sgr.py` & `pawpaw-1.0.0rc3/tests/visualization/test_sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/tests/visualization/test_visualization_ascii_box.py` & `pawpaw-1.0.0rc3/tests/visualization/test_visualization_ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/LICENSE` & `pawpaw-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/README.md` & `pawpaw-1.0.0rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,300 unit tests and counting!
+  - Over 4,500 unit tests and counting!
+  - Pure python, with only one external dependency: [regex](https://github.com/mrabarnett/mrab-regex)
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -262,15 +263,15 @@
 ### Verify Installation
 
 Whichever way you fetch Pawpaw, you can easily verify that it is installed correctly.  Just open Python prompt and type:
 
 ```python
 >>> from pawpaw import Ito
 >>> Ito('Hello, World!')
-Ito('Hello, World!', 0, 13, None)
+Ito(span=(0, 13), desc='', substr='Hello, World!')
 ```
   
 If your last line looks like this, you are up and running with Pawpaw!
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -22,15 +22,17 @@
 resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
 and Pawpaw datastructures in one go; with cross-linked nodes between trees -
 NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
 for downstream NLP consumption and b) *storing and searching* NLP generated
 content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
 Efficient pickling and JSON persistence - Security option enables persistence
 of index-only data, with reference strings re-injected during de-serialization
-- Stable & Defect Free - Over 4,300 unit tests and counting!
+- Stable & Defect Free - Over 4,500 unit tests and counting! - Pure python,
+with only one external dependency: [regex](https://github.com/mrabarnett/mrab-
+regex)
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -133,16 +135,16 @@
 tests: 1. Install with pip from GitHub: ``` pip install git+https://github.com/
 rlayers/pawpaw.git ``` 2. Install with conda from GitHub: ``` conda activate
 myenv conda install git pip pip install git+https://github.com/rlayers/
 pawpaw.git ``` 3. Clone the repo with git from GitHub: ``` git clone https://
 github.com/rlayers/pawpaw ``` ### Verify Installation Whichever way you fetch
 Pawpaw, you can easily verify that it is installed correctly. Just open Python
 prompt and type: ```python >>> from pawpaw import Ito >>> Ito('Hello, World!')
-Ito('Hello, World!', 0, 13, None) ``` If your last line looks like this, you
-are up and running with Pawpaw!
+Ito(span=(0, 13), desc='', substr='Hello, World!') ``` If your last line looks
+like this, you are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
 called *Ito*. Currently in release-candidate status, many components and
 features are production ready. However, documentation is still being written
 and some newer features are still undergoing work. A rough outline of which
 components are finalized is as follows: - [x] arborform - [x] itorator - [x]
```

### Comparing `pawpaw-1.0.0rc2/pyproject.toml` & `pawpaw-1.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc2/PKG-INFO` & `pawpaw-1.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawpaw
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: High Performance Text Processing & Segmentation Framework
 Project-URL: Homepage, https://github.com/rlayers/pawpaw
 Project-URL: Bug Tracker, https://github.com/rlayers/pawpaw/issues
 Author-email: "Robert L. Ayers" <rlayers@yahoo.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: extract-text,hierarchical-text-segmentation,information-extraction,knowledge-graph,nlp,python,text-processing,text-segmentation,xml-parser
@@ -61,15 +61,16 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,300 unit tests and counting!
+  - Over 4,500 unit tests and counting!
+  - Pure python, with only one external dependency: [regex](https://github.com/mrabarnett/mrab-regex)
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -284,15 +285,15 @@
 ### Verify Installation
 
 Whichever way you fetch Pawpaw, you can easily verify that it is installed correctly.  Just open Python prompt and type:
 
 ```python
 >>> from pawpaw import Ito
 >>> Ito('Hello, World!')
-Ito('Hello, World!', 0, 13, None)
+Ito(span=(0, 13), desc='', substr='Hello, World!')
 ```
   
 If your last line looks like this, you are up and running with Pawpaw!
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0rc2 Summary: High Performance
+Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0rc3 Summary: High Performance
 Text Processing & Segmentation Framework Project-URL: Homepage, https://
 github.com/rlayers/pawpaw Project-URL: Bug Tracker, https://github.com/rlayers/
 pawpaw/issues Author-email: "Robert L. Ayers"
 yahoo.com> License-Expression: MIT License-File: LICENSE Keywords: extract-
 text,hierarchical-text-segmentation,information-extraction,knowledge-
 graph,nlp,python,text-processing,text-segmentation,xml-parser Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
@@ -35,15 +35,17 @@
 resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
 and Pawpaw datastructures in one go; with cross-linked nodes between trees -
 NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
 for downstream NLP consumption and b) *storing and searching* NLP generated
 content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
 Efficient pickling and JSON persistence - Security option enables persistence
 of index-only data, with reference strings re-injected during de-serialization
-- Stable & Defect Free - Over 4,300 unit tests and counting!
+- Stable & Defect Free - Over 4,500 unit tests and counting! - Pure python,
+with only one external dependency: [regex](https://github.com/mrabarnett/mrab-
+regex)
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -146,16 +148,16 @@
 tests: 1. Install with pip from GitHub: ``` pip install git+https://github.com/
 rlayers/pawpaw.git ``` 2. Install with conda from GitHub: ``` conda activate
 myenv conda install git pip pip install git+https://github.com/rlayers/
 pawpaw.git ``` 3. Clone the repo with git from GitHub: ``` git clone https://
 github.com/rlayers/pawpaw ``` ### Verify Installation Whichever way you fetch
 Pawpaw, you can easily verify that it is installed correctly. Just open Python
 prompt and type: ```python >>> from pawpaw import Ito >>> Ito('Hello, World!')
-Ito('Hello, World!', 0, 13, None) ``` If your last line looks like this, you
-are up and running with Pawpaw!
+Ito(span=(0, 13), desc='', substr='Hello, World!') ``` If your last line looks
+like this, you are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
 called *Ito*. Currently in release-candidate status, many components and
 features are production ready. However, documentation is still being written
 and some newer features are still undergoing work. A rough outline of which
 components are finalized is as follows: - [x] arborform - [x] itorator - [x]
```

