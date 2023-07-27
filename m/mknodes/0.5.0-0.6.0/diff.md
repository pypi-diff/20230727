# Comparing `tmp/mknodes-0.5.0.tar.gz` & `tmp/mknodes-0.6.0.tar.gz`

## Comparing `mknodes-0.5.0.tar` & `mknodes-0.6.0.tar`

### file list

```diff
@@ -1,86 +1,91 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.5.0/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.5.0/Makefile
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.5.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.5.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.5.0/docs/gen_pages.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.5.0/docs/gen_qt.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkadmonition.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkannotations.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkimage.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkinstallguide.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mklink.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mklist.py
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mknode.py
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkpage.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/helpers.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/linkprovider.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_admonition.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_annotations.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_image.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_linkreplacer.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_modulepage.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_nav.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.5.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.5.0/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.5.0/README.md
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.6.0/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.6.0/Makefile
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.6.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 mknodes-0.6.0/docs/gen_pages.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.6.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkannotations.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkimage.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mklink.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mklist.py
+-rw-r--r--   0        0        0     8975 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mknode.py
+-rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/introduce_nodes.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/resources/codeofconduct.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/debugging.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/packageinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_admonition.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_annotations.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_image.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_linkreplacer.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_modulepage.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_nav.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_packageinfo.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.6.0/README.md
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 mknodes-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mknodes-0.6.0/PKG-INFO
```

### Comparing `mknodes-0.5.0/.pre-commit-config.yaml` & `mknodes-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/Makefile` & `mknodes-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mkdocs.yml` & `mknodes-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/.github/workflows/build.yml` & `mknodes-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/.github/workflows/documentation.yml` & `mknodes-0.6.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/docs/gen_pages.py` & `mknodes-0.6.0/docs/gen_pages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """Generate the code reference pages and navigation."""
 
-from __future__ import annotations
+from __future__ import annotations as _annotations
 
 import pathlib
 
 import mknodes
 from mknodes import manual
 
 
 HEADER = "Don't write docs. Code them."
 WARNING = "This is all very alpha and subject to change."
 FOOTER = """Thats it. We created a website without touching any .md file
 and without having to care about file paths at at all.
 Now check out what we have created!
 """
 
+annotations = mknodes.MkAnnotations()
+annotations[1] = "We will use annotations to explain things a bit."  # (1)
+
 # this Nav object is basically the root of everything. It corresponds to your root
 # SUMMARY.md.
-
 root_nav = mknodes.MkNav()
 
 # Let's begin with the start page. This is your index.md file.
 page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
 
 # The next 6 lines are generating the page you are looking at right now.
 page.add_header(HEADER, level=3)
-page.add_admonition(WARNING, typ="danger", title="Warning!")
+admonition = page.add_admonition(WARNING, typ="danger", title="Warning!")
+annotations[2] = admonition  # (2)
 page += "This is the source code for building this website:"
 code = pathlib.Path(__file__).read_text()
 page.add_code(code)
+page += annotations
 page += FOOTER
 
 # now we will create the nav section and its pages one by one.
 manual.create_page_1(root_nav)
 manual.create_page_2(root_nav)
 manual.create_page_3(root_nav)
```

### Comparing `mknodes-0.5.0/docs/gen_qt.py` & `mknodes-0.6.0/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/__init__.py` & `mknodes-0.6.0/mknodes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,8 @@
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
     "MkInstallGuide",
 ]
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `mknodes-0.5.0/mknodes/mkadmonition.py` & `mknodes-0.6.0/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkannotations.py` & `mknodes-0.6.0/mknodes/mkannotations.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkbinaryimage.py` & `mknodes-0.6.0/mknodes/mkbinaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkblock.py` & `mknodes-0.6.0/mknodes/mkblock.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkcode.py` & `mknodes-0.6.0/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkcontainer.py` & `mknodes-0.6.0/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkcritic.py` & `mknodes-0.6.0/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkdiagram.py` & `mknodes-0.6.0/mknodes/mkdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkdoc.py` & `mknodes-0.6.0/mknodes/mkdoc.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkdocstrings.py` & `mknodes-0.6.0/mknodes/mkdocstrings.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkimage.py` & `mknodes-0.6.0/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkinstallguide.py` & `mknodes-0.6.0/mknodes/mkinstallguide.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mklink.py` & `mknodes-0.6.0/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mklist.py` & `mknodes-0.6.0/mknodes/mklist.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mknav.py` & `mknodes-0.6.0/mknodes/mknav.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,24 +96,26 @@
         """
         navi = mknav.MkNav(section=section, parent=self)
         self._register(navi)
         return navi
 
     def add_index_page(
         self,
+        title: str | None = None,
+        *,
         hide_toc: bool = False,
         hide_nav: bool = False,
     ) -> mkpage.MkPage:
         page = mkpage.MkPage(
             path="index.md",
             hide_toc=hide_toc,
             hide_nav=hide_nav,
             parent=self,
         )
-        self.nav[None] = page
+        self.nav[title] = page
         return page
 
     def virtual_files(self) -> dict[str, str]:
         return {str(self.path): self.to_markdown()}
 
     def to_markdown(self) -> str:
         nav = mkdocs_gen_files.Nav()
```

### Comparing `mknodes-0.5.0/mknodes/mknode.py` & `mknodes-0.6.0/mknodes/mknode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkpage.py` & `mknodes-0.6.0/mknodes/mkpage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkpageinclude.py` & `mknodes-0.6.0/mknodes/mkpageinclude.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mkshields.py` & `mknodes-0.6.0/mknodes/mkshields.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mksnippet.py` & `mknodes-0.6.0/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mksourceandresult.py` & `mknodes-0.6.0/mknodes/mksourceandresult.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mktabcontainer.py` & `mknodes-0.6.0/mknodes/mktabcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mktable.py` & `mknodes-0.6.0/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mktabs.py` & `mknodes-0.6.0/mknodes/mktabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/mktext.py` & `mknodes-0.6.0/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/node.py` & `mknodes-0.6.0/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.6.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,22 @@
 import pathlib
 import re
 
 from typing import TYPE_CHECKING
 import urllib.parse
 
 from mkdocs.plugins import BasePlugin
-import mkdocs.utils
 
 
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.structure.files import Files
     from mkdocs.structure.pages import Page
 
 logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
-logger.addFilter(mkdocs.utils.warning_filter)
 
 # For Regex, match groups are:
 #       0: Whole markdown link e.g. [Alt-text](url)
 #       1: Alt text
 #       2: Full URL e.g. url + hash anchor
 #       3: Filename e.g. filename.md
 #       4: File extension e.g. .md, .png, etc.
```

### Comparing `mknodes-0.5.0/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.6.0/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/classnodes/mkclasspage.py` & `mknodes-0.6.0/mknodes/classnodes/mkclasspage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/classnodes/mkclasstable.py` & `mknodes-0.6.0/mknodes/classnodes/mkclasstable.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,20 @@
         kls: type,
         shorten_lists_after: int = 10,
     ) -> dict[str, str]:
         """Return a table row for given class.
 
         Includes columns for child and parent classes including links.
         """
-        subclasses = [subkls for subkls in kls.__subclasses__() if self.filter_fn(subkls)]
+        subclasses = [
+            subkls
+            for subkls in kls.__subclasses__()
+            if self.filter_fn(subkls)
+            and not subkls.__qualname__.endswith("]")  # filter generic subclasses
+        ]
         subclass_links = [helpers.link_for_class(sub) for sub in subclasses]
         subclass_str = helpers.to_html_list(
             subclass_links,
             shorten_after=shorten_lists_after,
         )
         parents = kls.__bases__
         parent_links = [helpers.link_for_class(parent) for parent in parents]
```

### Comparing `mknodes-0.5.0/mknodes/manual/page_1.py` & `mknodes-0.6.0/mknodes/manual/page_1.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/manual/page_2.py` & `mknodes-0.6.0/mknodes/manual/page_2.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/manual/page_3.py` & `mknodes-0.6.0/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.6.0/mknodes/modulenodes/mkmodulepage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.6.0/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/utils/classhelpers.py` & `mknodes-0.6.0/mknodes/utils/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/utils/connectionbuilder.py` & `mknodes-0.6.0/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/utils/helpers.py` & `mknodes-0.6.0/mknodes/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,26 +138,32 @@
     elif kls.__module__.startswith(("PyQt", "PySide")):
         mod = kls.__module__.replace("PySide6.", "").replace("PyQt6.", "")
         url = f"{BASE_URL}{mod}/{kls.__qualname__.replace('.', '/')}.html"
         link = linked(url, title=kls.__name__)
     elif kls.__module__.startswith("prettyqt"):
         link = linked(kls.__qualname__)
     else:
-        try:
-            dist = metadata.distribution(kls.__module__.split(".")[0])
-        except metadata.PackageNotFoundError:
-            link = linked(kls.__qualname__)
+        module = kls.__module__.split(".")[0]
+        qual_name = kls.__qualname__.split("[")[0]  # to split off generics part
+        if url := homepage_for_distro(module):
+            link = linked(url, title=qual_name)
         else:
-            if url := dist.metadata["Home-Page"]:
-                link = linked(url, title=kls.__qualname__)
-            else:
-                link = linked(kls.__qualname__)
+            link = linked(qual_name)
     return styled(link, **kwargs)
 
 
+def homepage_for_distro(dist_name: str):
+    try:
+        dist = metadata.distribution(dist_name)
+    except metadata.PackageNotFoundError:
+        return None
+    else:
+        return dist.metadata["Home-Page"]
+
+
 def label_for_class(klass: type) -> str:
     if klass.__module__.startswith("prettyqt."):
         parts = klass.__module__.split(".")
         return f"{parts[1]}.{klass.__name__}"
     return f"{klass.__module__.split('.')[-1]}.{klass.__name__}"
```

### Comparing `mknodes-0.5.0/mknodes/utils/inventorymanager.py` & `mknodes-0.6.0/mknodes/utils/inventorymanager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
+import abc
+
+from collections.abc import Mapping
+import itertools
 import logging
 import os
 import pathlib
 import types
 
 from mkdocstrings import inventory
 
 
 logger = logging.getLogger(__name__)
 
 
-class InventoryManager:
+class InventoryManager(Mapping, metaclass=abc.ABCMeta):
     def __init__(self):
         self.inv_files: list[inventory.Inventory] = []
 
     def add_inv_file(self, path: str | os.PathLike):
         with pathlib.Path(path).open("rb") as file:
             inv = inventory.Inventory.parse_sphinx(file)
         self.inv_files.append(inv)
@@ -27,15 +31,21 @@
             case str():
                 path = name
             case _:
                 raise TypeError(name)
         for inv_file in self.inv_files:
             if path in inv_file:
                 return inv_file[path]
-        return None
+        raise KeyError(name)
+
+    def __iter__(self):
+        return itertools.chain(*[inv_file.keys() for inv_file in self.inv_files])
+
+    def __len__(self):
+        return sum(len(i) for i in self.inv_files)
 
 
 if __name__ == "__main__":
     inv_manager = InventoryManager()
     inv_manager.add_inv_file("mknodes/utils/objects.inv")
     file = inv_manager.inv_files[0]
-    print(file.keys())
+    print(len(inv_manager))
```

### Comparing `mknodes-0.5.0/mknodes/utils/mermaid.py` & `mknodes-0.6.0/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/mknodes/utils/noderesolver.py` & `mknodes-0.6.0/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/tests/test_annotations.py` & `mknodes-0.6.0/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/tests/test_nav.py` & `mknodes-0.6.0/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/tests/data/nav_tree/test_file.md` & `mknodes-0.6.0/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/.gitignore` & `mknodes-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/LICENSE` & `mknodes-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/README.md` & `mknodes-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.5.0/pyproject.toml` & `mknodes-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 ]
 
 requires-python = ">=3.10"
 dependencies = [
     "typing_extensions",
     "mkdocs-gen-files",
     "mkdocs",
+    "PyYAML >=5.1",
 ]
 license = "MIT"
 
 
 [project.entry-points."mkdocs.plugins"]
 linkreplacer = "mknodes.__linkreplacer:LinkReplacerPlugin"
```

### Comparing `mknodes-0.5.0/PKG-INFO` & `mknodes-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: docs,docstrings,documentation,framework,internet,markdown
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Internet
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.10
 Requires-Dist: mkdocs
 Requires-Dist: mkdocs-gen-files
+Requires-Dist: pyyaml>=5.1
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # MkNodes
 
 <p align="center">
     <em>Generate docs with ease.</em>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.5.0 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.6.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Documentation Classifier: Topic :: Internet Classifier: Topic :: Text
 Processing :: Markup :: Markdown Requires-Python: >=3.10 Requires-Dist: mkdocs
-Requires-Dist: mkdocs-gen-files Requires-Dist: typing-extensions Description-
-Content-Type: text/markdown # MkNodes
+Requires-Dist: mkdocs-gen-files Requires-Dist: pyyaml>=5.1 Requires-Dist:
+typing-extensions Description-Content-Type: text/markdown # MkNodes
                            Generate docs with ease.
 [![build](https://github.com/phil65/mknodes/workflows/Build/badge.svg)](https:/
 /github.com/phil65/mknodes/actions) [![codecov](https://codecov.io/gh/phil65/
 mknodes/branch/master/graph/badge.svg)](https://codecov.io/gh/phil65/mknodes)
 [![PyPI version](https://badge.fury.io/py/mknodes.svg)](https://badge.fury.io/
 py/mknodes) --- **Documentation**: https://phil65.github.io/mknodes/ **Source
 Code**: https://github.com/phil65/mknodes --- ## Development ### Setup
```

