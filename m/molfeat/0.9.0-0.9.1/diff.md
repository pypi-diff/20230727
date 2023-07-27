# Comparing `tmp/molfeat-0.9.0.tar.gz` & `tmp/molfeat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.9.0.tar", last modified: Mon Jul 10 19:41:46 2023, max compression
+gzip compressed data, was "molfeat-0.9.1.tar", last modified: Thu Jul 27 20:47:45 2023, max compression
```

## Comparing `molfeat-0.9.0.tar` & `molfeat-0.9.1.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.071054 molfeat-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/5_community_contribution.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-10 19:38:29.000000 molfeat-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-10 19:38:29.000000 molfeat-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-10 19:38:29.000000 molfeat-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-07-10 19:38:29.000000 molfeat-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-10 19:41:46.067054 molfeat-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-10 19:38:29.000000 molfeat-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.051054 molfeat-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.047053 molfeat-0.9.0/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   110397 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/community/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/community/contributions.md
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/community/get_involved.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.055054 molfeat-0.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/custom_model_store.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60168 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 19:38:29.000000 molfeat-0.9.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-10 19:38:29.000000 molfeat-0.9.0/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-10 19:38:29.000000 molfeat-0.9.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33609 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.063054 molfeat-0.9.0/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-10 19:38:29.000000 molfeat-0.9.0/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.059054 molfeat-0.9.0/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-10 19:41:46.000000 molfeat-0.9.0/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:41:40.000000 molfeat-0.9.0/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 19:41:45.000000 molfeat-0.9.0/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.047053 molfeat-0.9.0/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/nb/etl/
--rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/chemberta-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/chemgpt-fix-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/dgl-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/entropy-transforner-zinc-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/featurizer-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-10 19:38:29.000000 molfeat-0.9.0/nb/etl/molt5-etl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-10 19:38:29.000000 molfeat-0.9.0/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-10 19:38:29.000000 molfeat-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:41:46.071054 molfeat-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:41:46.067054 molfeat-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 19:38:29.000000 molfeat-0.9.0/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.907130 molfeat-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.879130 molfeat-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/5_community_contribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-27 20:43:14.000000 molfeat-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-27 20:43:14.000000 molfeat-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-27 20:43:14.000000 molfeat-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-07-27 20:43:14.000000 molfeat-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 20:47:45.907130 molfeat-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-27 20:43:14.000000 molfeat-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.883130 molfeat-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.875130 molfeat-0.9.1/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   110397 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/community/contributions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/community/get_involved.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.887130 molfeat-0.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/custom_model_store.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60168 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-27 20:43:14.000000 molfeat-0.9.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-27 20:43:14.000000 molfeat-0.9.1/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-27 20:43:14.000000 molfeat-0.9.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.895130 molfeat-0.9.1/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.895130 molfeat-0.9.1/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.899130 molfeat-0.9.1/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.903130 molfeat-0.9.1/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-27 20:43:14.000000 molfeat-0.9.1/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.891130 molfeat-0.9.1/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:47:38.000000 molfeat-0.9.1/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 20:47:45.000000 molfeat-0.9.1/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.879130 molfeat-0.9.1/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.903130 molfeat-0.9.1/nb/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/chemberta-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/chemgpt-fix-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/dgl-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/entropy-transforner-zinc-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/featurizer-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 20:43:14.000000 molfeat-0.9.1/nb/etl/molt5-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 20:43:14.000000 molfeat-0.9.1/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-27 20:43:14.000000 molfeat-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:47:45.907130 molfeat-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:47:45.907130 molfeat-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 20:43:14.000000 molfeat-0.9.1/tests/test_viz.py
```

### Comparing `molfeat-0.9.0/.github/CODE_OF_CONDUCT.md` & `molfeat-0.9.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/5_community_contribution.yaml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/5_community_contribution.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.9.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `molfeat-0.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/workflows/doc.yml` & `molfeat-0.9.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/workflows/release.yml` & `molfeat-0.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.github/workflows/test.yml` & `molfeat-0.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/.gitignore` & `molfeat-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/CHANGELOG.md` & `molfeat-0.9.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/LICENSE` & `molfeat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/PKG-INFO` & `molfeat-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.9.0
+Version: 0.9.1
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.9.0 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.1 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.9.0/README.md` & `molfeat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/api/molfeat.calc.md` & `molfeat-0.9.1/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/assets/css/custom-molfeat.css` & `molfeat-0.9.1/docs/assets/css/custom-molfeat.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 :root {
-  --datamol-primary: #217EBB;
-  --datamol-secondary: #343a40;
+  --molfeat-primary: #217EBB;
+  --molfeat-secondary: #5f6d7a;
 
   /* Primary color shades */
-  --md-primary-fg-color: var(--datamol-primary);
-  --md-primary-fg-color--light: var(--datamol-primary);
-  --md-primary-fg-color--dark: var(--datamol-primary);
-  --md-primary-bg-color: var(--datamol-secondary);
-  --md-primary-bg-color--light: var(--datamol-secondary);
-  --md-text-link-color: var(--datamol-secondary);
+  --md-primary-fg-color: var(--molfeat-primary);
+  --md-primary-fg-color--light: var(--molfeat-primary);
+  --md-primary-fg-color--dark: var(--molfeat-primary);
+  --md-primary-bg-color: var(--molfeat-secondary);
+  --md-primary-bg-color--light: var(--molfeat-secondary);
+  --md-text-link-color: var(--molfeat-secondary);
 
   /* Accent color shades */
-  --md-accent-fg-color: var(--datamol-secondary);
-  --md-accent-fg-color--transparent: var(--datamol-secondary);
-  --md-accent-bg-color: var(--datamol-secondary);
-  --md-accent-bg-color--light: var(--datamol-secondary);
+  --md-accent-fg-color: var(--molfeat-secondary);
+  --md-accent-fg-color--transparent: var(--molfeat-secondary);
+  --md-accent-bg-color: var(--molfeat-secondary);
+  --md-accent-bg-color--light: var(--molfeat-secondary);
 }
 
 :root>* {
   /* Code block color shades */
   --md-code-bg-color: hsla(0, 0%, 96%, 1);
   --md-code-fg-color: hsla(200, 18%, 26%, 1);
 
   /* Footer */
-  --md-footer-bg-color: var(--datamol-primary);
+  --md-footer-bg-color: var(--molfeat-primary);
   /* --md-footer-bg-color--dark: hsla(0, 0%, 0%, 0.32); */
-  --md-footer-fg-color: var(--datamol-secondary);
-  --md-footer-fg-color--light: var(--datamol-secondary);
-  --md-footer-fg-color--lighter: var(--datamol-secondary);
+  --md-footer-fg-color: var(--molfeat-secondary);
+  --md-footer-fg-color--light: var(--molfeat-secondary);
+  --md-footer-fg-color--lighter: var(--molfeat-secondary);
 
 }
 
 .md-header {
   background-image: linear-gradient(to right, #1E2F6C, #217EBB);
 }
 
 .md-footer {
   background-image: linear-gradient(to right, #1E2F6C, #217EBB);
 }
 
 .md-tabs {
-  background-image: linear-gradient(to right, #F4F6F9, #C3CFE2);
+  background-image: linear-gradient(to right, #F4F6F9, #CCE3f8);
 }
 
 .md-header__topic {
   color: rgb(255, 255, 255);
 }
 
 .md-source__repository,
@@ -59,15 +59,24 @@
 .md-copyright,
 .md-footer-meta.md-typeset a,
 .md-version {
   color: rgb(255, 255, 255) !important;
 }
 
 .md-search__form {
-  background-color: rgba(255, 255, 255, 0.2);
+  background-color: rgba(255, 255, 255, 0.4);
+}
+
+.md-search-result__article:hover {
+  background-color: #CCE3f8;
+}
+
+.md-search-result__more:hover,
+.md-search-result__more:focus {
+  background-color: #CCE3f8 !important;
 }
 
 .md-search__input {
   color: #222222 !important;
 }
 
 .md-header__topic {
```

### Comparing `molfeat-0.9.0/docs/assets/css/custom.css` & `molfeat-0.9.1/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/benchmark.ipynb` & `molfeat-0.9.1/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/community/contributions.md` & `molfeat-0.9.1/docs/community/contributions.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/community/get_involved.md` & `molfeat-0.9.1/docs/community/get_involved.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/developers/contribute.md` & `molfeat-0.9.1/docs/developers/contribute.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/developers/create-plugin.md` & `molfeat-0.9.1/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/developers/register-plugin.md` & `molfeat-0.9.1/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/images/logo-black.png` & `molfeat-0.9.1/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/images/logo-black.svg` & `molfeat-0.9.1/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/images/logo-title.svg` & `molfeat-0.9.1/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/images/logo.png` & `molfeat-0.9.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/images/logo.svg` & `molfeat-0.9.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/index.md` & `molfeat-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/add_your_own.ipynb` & `molfeat-0.9.1/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/custom_model_store.ipynb` & `molfeat-0.9.1/docs/tutorials/custom_model_store.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/datacache.ipynb` & `molfeat-0.9.1/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/graphs.ipynb` & `molfeat-0.9.1/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/integrations.ipynb` & `molfeat-0.9.1/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.9.1/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/save_and_load.ipynb` & `molfeat-0.9.1/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.9.1/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.9.1/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/env.yml` & `molfeat-0.9.1/env.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/mkdocs.yml` & `molfeat-0.9.1/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
       - molfeat.trans:
           - molfeat.trans.base: api/molfeat.trans.base.md
           - molfeat.trans.fp: api/molfeat.trans.fp.md
           - molfeat.trans.graph: api/molfeat.trans.graph.md
           - molfeat.trans.struct: api/molfeat.trans.struct.md
           - molfeat.trans.concat: api/molfeat.trans.concat.md
           - molfeat.trans.pretrained:
+              - Base Pretrained Models: api/molfeat.trans.pretrained.base.md
               - HuggingFace: api/molfeat.trans.pretrained.hf_transformers.md
               - Graphormer: api/molfeat.trans.pretrained.graphormer.md
               - DGL: api/molfeat.trans.pretrained.dgl_pretrained.md
               - FCD: api/molfeat.trans.pretrained.fcd.md
       - molfeat.store: api/molfeat.store.md
       - molfeat.plugins: api/molfeat.plugins.md
       - molfeat.utils: api/molfeat.utils.md
```

### Comparing `molfeat-0.9.0/molfeat/calc/__init__.py` & `molfeat-0.9.1/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/_atom_bond_features.py` & `molfeat-0.9.1/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/_map4.py` & `molfeat-0.9.1/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/_mhfp.py` & `molfeat-0.9.1/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/atom.py` & `molfeat-0.9.1/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/base.py` & `molfeat-0.9.1/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/bond.py` & `molfeat-0.9.1/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/cats.py` & `molfeat-0.9.1/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/descriptors.py` & `molfeat-0.9.1/molfeat/calc/descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/fingerprints.py` & `molfeat-0.9.1/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/pharmacophore.py` & `molfeat-0.9.1/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/shape.py` & `molfeat-0.9.1/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/skeys.py` & `molfeat-0.9.1/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/calc/tree.py` & `molfeat-0.9.1/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/data/cats_features.fdef` & `molfeat-0.9.1/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/data/elements.xz` & `molfeat-0.9.1/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/data/elements_completed.xz` & `molfeat-0.9.1/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/data/origin.xz` & `molfeat-0.9.1/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/data/skey_parameters.csv` & `molfeat-0.9.1/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/plugins/entry_point.py` & `molfeat-0.9.1/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/plugins/factories.py` & `molfeat-0.9.1/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/store/loader.py` & `molfeat-0.9.1/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/store/modelcard.py` & `molfeat-0.9.1/molfeat/store/modelcard.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/store/modelstore.py` & `molfeat-0.9.1/molfeat/store/modelstore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/base.py` & `molfeat-0.9.1/molfeat/trans/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from molfeat.calc import get_calculator
 from molfeat.calc.base import _CALCULATORS
 from molfeat.utils import datatype
 from molfeat.utils.cache import _Cache, FileCache, MPDataCache
 from molfeat.utils.cache import CacheList
 from molfeat.utils.commons import fn_to_hex
 from molfeat.utils.commons import hex_to_fn
+from molfeat.utils.commons import is_callable
 from molfeat.utils.parsing import get_input_args
 from molfeat.utils.parsing import import_from_string
 from molfeat.utils.state import map_dtype
 from molfeat.utils.state import ATOM_FEATURIZER_MAPPING
 from molfeat.utils.state import BOND_FEATURIZER_MAPPING
 from molfeat.utils.state import ATOM_FEATURIZER_MAPPING_REVERSE
 from molfeat.utils.state import BOND_FEATURIZER_MAPPING_REVERSE
@@ -194,14 +195,18 @@
         else:
             self.featurizer = get_calculator(featurizer, **params)
 
         self.cols_to_keep = None
         self._fitted = False
 
         self._save_input_args()
+        if self.featurizer and not (
+            isinstance(self.featurizer, str) or is_callable(self.featurizer)
+        ):
+            raise AttributeError(f"Featurizer {self.featurizer} must be a callable or a string")
 
     def _save_input_args(self):
         """Save the input arguments of a transformer to the attribute
         `_input_args` of the object.
         """
 
         # NOTE(hadim): don't override existing _input_args so
@@ -315,15 +320,17 @@
                     **cpy.parallel_kwargs,
                 )
             else:
                 features = [self._transform(mol) for mol in mols]
         if not ignore_errors:
             for ind, feat in enumerate(features):
                 if feat is None:
-                    raise ValueError(f"Cannot transform molecule at index {ind}")
+                    raise ValueError(
+                        f"Cannot transform molecule at index {ind}. Please check logs (set verbose to True) to see errors!"
+                    )
 
         return features
 
     def __len__(self):
         """Compute featurizer length"""
 
         # check length and _length attribute
```

### Comparing `molfeat-0.9.0/molfeat/trans/concat.py` & `molfeat-0.9.1/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/fp.py` & `molfeat-0.9.1/molfeat/trans/fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/graph/adj.py` & `molfeat-0.9.1/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/graph/tree.py` & `molfeat-0.9.1/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/pretrained/base.py` & `molfeat-0.9.1/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.9.1/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/pretrained/fcd.py` & `molfeat-0.9.1/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.9.1/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.9.1/molfeat/trans/pretrained/hf_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import List
 from typing import Union
 from typing import Optional
 
 import os
 import uuid
 import torch
 import tempfile
```

### Comparing `molfeat-0.9.0/molfeat/trans/struct/esm.py` & `molfeat-0.9.1/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/trans/struct/prot1D.py` & `molfeat-0.9.1/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/cache.py` & `molfeat-0.9.1/molfeat/utils/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         if isinstance(mols, str) or not isinstance(mols, Iterable):
             mols = [mols]
 
         # copy if possible to prevent parallel issues
         try:
             cacher = copy.deepcopy(self)
             n_jobs = self.n_jobs
-        except:
+        except:  # noqa
             # cannot parallelize process, ensure n_jobs is 0
             cacher = self
             n_jobs = 0
         return dm.parallelized(
             cacher.get, mols, n_jobs=n_jobs, progress=self.verbose, tqdm_kwargs=dict(leave=False)
         )
 
@@ -353,15 +353,15 @@
             # this needs to be done to prevent operating on close files
             self.cache = {}
         if delete:
             if self.cache_file is not None:
                 for path in glob.glob(str(self.cache_file) + "*"):
                     try:
                         os.unlink(path)
-                    except:
+                    except:  # noqa
                         pass
         else:
             self._initialize_cache()
 
     def update(self, new_cache: Mapping[Any, Any]):
         """Update the cache with new values
```

### Comparing `molfeat-0.9.0/molfeat/utils/commons.py` & `molfeat-0.9.1/molfeat/utils/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Type
 from typing import Callable
 from typing import Iterable
 from typing import Optional
 from typing import List
 from typing import Union
 
+import types
 import os
 import inspect
 import hashlib
 import pickle
 import functools
 import torch
 import numpy as np
@@ -21,14 +22,24 @@
 
 from rdkit.Chem import rdMolDescriptors
 from rdkit.Chem import rdMolAlign
 from rdkit.Chem import SaltRemover
 from molfeat.utils import datatype
 
 
+FUNCTYPES = (types.FunctionType, types.MethodType, functools.partial)
+
+
+def is_callable(func):
+    r"""
+    Check if func is a function or a callable
+    """
+    return func and (isinstance(func, FUNCTYPES) or callable(func))
+
+
 def sha256sum(filepath: Union[str, os.PathLike]):
     """Return the sha256 sum hash of a file or a directory
 
     Args:
         filepath: The path to the file to compute the MD5 hash on.
     """
     if dm.fs.is_dir(filepath):
```

### Comparing `molfeat-0.9.0/molfeat/utils/const.py` & `molfeat-0.9.1/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/converters.py` & `molfeat-0.9.1/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/datatype.py` & `molfeat-0.9.1/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/log.py` & `molfeat-0.9.1/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/parsing.py` & `molfeat-0.9.1/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/pooler.py` & `molfeat-0.9.1/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/requires.py` & `molfeat-0.9.1/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/utils/state.py` & `molfeat-0.9.1/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat/viz.py` & `molfeat-0.9.1/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/molfeat.egg-info/PKG-INFO` & `molfeat-0.9.1/molfeat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.9.0
+Version: 0.9.1
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.9.0 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.9.1 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.9.0/molfeat.egg-info/SOURCES.txt` & `molfeat-0.9.1/molfeat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/api/molfeat.calc.md
 docs/api/molfeat.plugins.md
 docs/api/molfeat.store.md
 docs/api/molfeat.trans.base.md
 docs/api/molfeat.trans.concat.md
 docs/api/molfeat.trans.fp.md
 docs/api/molfeat.trans.graph.md
+docs/api/molfeat.trans.pretrained.base.md
 docs/api/molfeat.trans.pretrained.dgl_pretrained.md
 docs/api/molfeat.trans.pretrained.fcd.md
 docs/api/molfeat.trans.pretrained.graphormer.md
 docs/api/molfeat.trans.pretrained.hf_transformers.md
 docs/api/molfeat.trans.struct.md
 docs/api/molfeat.utils.md
 docs/api/molfeat.viz.md
```

### Comparing `molfeat-0.9.0/nb/etl/chemberta-etl.ipynb` & `molfeat-0.9.1/nb/etl/chemberta-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/nb/etl/chemgpt-fix-etl.ipynb` & `molfeat-0.9.1/nb/etl/chemgpt-fix-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/nb/etl/dgl-etl.ipynb` & `molfeat-0.9.1/nb/etl/dgl-etl.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9746588446022247%*

 * *Differences: {"'cells'": "{5: {'outputs': {0: {'text': {insert: [(0, 'Downloading "*

 * *            'gin_supervised_contextpred_pre_trained.pth from '*

 * *            "https://data.dgl.ai/dgllife/pre_trained/gin_supervised_contextpred.pth...\\n')], "*

 * *            "delete: [0]}}}, 'source': {insert: [(1, 'gin_contextpred= ModelInfo(\\n'), (2, '    "*

 * *            'name = "gin_supervised_contextpred",\\n\'), (8, \'    description="GIN neural network '*

 * *            'model pre-trained with supervised learning and context prediction on  […]*

```diff
@@ -101,14 +101,47 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "Downloading gin_supervised_contextpred_pre_trained.pth from https://data.dgl.ai/dgllife/pre_trained/gin_supervised_contextpred.pth...\n",
+                        "Pretrained model loaded\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# an example of supervised GIN model\n",
+                "gin_contextpred= ModelInfo(\n",
+                "    name = \"gin_supervised_contextpred\",\n",
+                "    inputs = \"smiles\",\n",
+                "    type=\"pretrained\",\n",
+                "    group=\"dgllife\",\n",
+                "    version=0,\n",
+                "    submitter=\"Datamol\",\n",
+                "    description=\"GIN neural network model pre-trained with supervised learning and context prediction on molecules from ChEMBL.\",\n",
+                "    representation=\"graph\",\n",
+                "    require_3D=False,\n",
+                "    tags = [\"GIN\", \"dgl\", \"pytorch\", \"graph\"],\n",
+                "    authors= [\"Weihua Hu\", \"Bowen Liu\", \"Joseph Gomes\", \"Marinka Zitnik\", \"Percy Liang\", \"Vijay Pande\", \"Jure Leskovec\"],\n",
+                "    reference = \"https://arxiv.org/abs/1905.12265\" \n",
+                ")\n",
+                "gin_contextpred_model = dgllife.model.load_pretrained('gin_supervised_contextpred')\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
                         "Downloading gin_supervised_masking_pre_trained.pth from https://data.dgl.ai/dgllife/pre_trained/gin_supervised_masking.pth...\n",
                         "Pretrained model loaded\n"
                     ]
                 }
             ],
             "source": [
                 "# an example of supervised GIN model\n",
@@ -127,164 +160,263 @@
                 "    reference = \"https://arxiv.org/abs/1905.12265\" \n",
                 ")\n",
                 "gin_masking_model = dgllife.model.load_pretrained('gin_supervised_masking')\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from molfeat.store.modelstore import ModelStore\n",
                 "store = ModelStore()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "['gin_supervised_contextpred',\n",
+                            "['cats2d',\n",
+                            " 'cats3d',\n",
+                            " 'scaffoldkeys',\n",
+                            " 'gin_supervised_edgepred',\n",
+                            " 'gin_supervised_infomax',\n",
+                            " 'gin_supervised_masking',\n",
                             " 'jtvae_zinc_no_kl',\n",
+                            " 'map4',\n",
+                            " 'secfp',\n",
                             " 'pcqm4mv2_graphormer_base',\n",
+                            " 'ChemBERTa-77M-MLM',\n",
+                            " 'ChemBERTa-77M-MTR',\n",
                             " 'ChemGPT-1.2B',\n",
+                            " 'ChemGPT-19M',\n",
                             " 'ChemGPT-4.7M',\n",
-                            " 'DeepChem-ChemBERTa-77M-MLM',\n",
-                            " 'DeepChem-ChemBERTa-77M-MTR',\n",
-                            " 'maccs']"
+                            " 'GPT2-Zinc480M-87M',\n",
+                            " 'MolT5',\n",
+                            " 'Roberta-Zinc480M-102M',\n",
+                            " 'pharm2D-cats',\n",
+                            " 'pharm2D-default',\n",
+                            " 'pharm2D-gobbi',\n",
+                            " 'pharm2D-pmapper',\n",
+                            " 'pharm3D-cats',\n",
+                            " 'pharm3D-gobbi',\n",
+                            " 'pharm3D-pmapper',\n",
+                            " 'atompair-count',\n",
+                            " 'avalon',\n",
+                            " 'desc2D',\n",
+                            " 'desc3D',\n",
+                            " 'ecfp-count',\n",
+                            " 'ecfp',\n",
+                            " 'erg',\n",
+                            " 'estate',\n",
+                            " 'fcfp-count',\n",
+                            " 'fcfp',\n",
+                            " 'maccs',\n",
+                            " 'pattern',\n",
+                            " 'rdkit',\n",
+                            " 'topological-count',\n",
+                            " 'topological',\n",
+                            " 'electroshape',\n",
+                            " 'usr',\n",
+                            " 'usrcat']"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "[x.name for x in store.available_models]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "1fffc7c2d6d144f79c41c8b2d944a68c",
+                            "model_id": "10895bee541a41ed98689c2e74da8225",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0.00/7.12M [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-14 17:42:54.663 | INFO     | molfeat.store.modelstore:register:124 - Successfuly registered model gin_supervised_edgepred !\n"
+                        "\u001b[32m2023-07-20 17:45:12.918\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mmolfeat.store.modelstore\u001b[0m:\u001b[36mregister\u001b[0m:\u001b[36m147\u001b[0m - \u001b[1mSuccessfuly registered model gin_supervised_edgepred !\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "store.register(gin_edgepred, model=gin_edgepred_model, force=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "fe97498dacb14aefba894664eb48d21a",
+                            "model_id": "eb859420bcfa4bf0a0e5660fbb0c3ff2",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0.00/7.12M [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-14 17:43:03.718 | INFO     | molfeat.store.modelstore:register:124 - Successfuly registered model gin_supervised_infomax !\n"
+                        "\u001b[32m2023-07-20 17:45:21.508\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mmolfeat.store.modelstore\u001b[0m:\u001b[36mregister\u001b[0m:\u001b[36m147\u001b[0m - \u001b[1mSuccessfuly registered model gin_supervised_infomax !\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "store.register(gin_infomax, model=gin_infomax_model, force=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "2b263cfa9945403398b9f3c8c0a4d63a",
+                            "model_id": "7dda56220b3c48878c040997a4f9d525",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0.00/7.12M [00:00<?, ?B/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-14 17:43:17.363 | INFO     | molfeat.store.modelstore:register:124 - Successfuly registered model gin_supervised_masking !\n"
+                        "\u001b[32m2023-07-20 17:45:30.070\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mmolfeat.store.modelstore\u001b[0m:\u001b[36mregister\u001b[0m:\u001b[36m147\u001b[0m - \u001b[1mSuccessfuly registered model gin_supervised_masking !\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "store.register(gin_masking, model=gin_masking_model, force=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "95155893ec7d4d5eab4de463283d2ed6",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "  0%|          | 0.00/7.12M [00:00<?, ?B/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "\u001b[32m2023-07-20 17:45:38.305\u001b[0m | \u001b[1mINFO    \u001b[0m | \u001b[36mmolfeat.store.modelstore\u001b[0m:\u001b[36mregister\u001b[0m:\u001b[36m147\u001b[0m - \u001b[1mSuccessfuly registered model gin_supervised_contextpred !\u001b[0m\n"
+                    ]
+                }
+            ],
+            "source": [
+                "store.register(gin_contextpred, model=gin_contextpred_model, force=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "['gin_supervised_contextpred',\n",
+                            "['cats2d',\n",
+                            " 'cats3d',\n",
+                            " 'scaffoldkeys',\n",
+                            " 'gin_supervised_contextpred',\n",
                             " 'gin_supervised_edgepred',\n",
                             " 'gin_supervised_infomax',\n",
                             " 'gin_supervised_masking',\n",
                             " 'jtvae_zinc_no_kl',\n",
+                            " 'map4',\n",
+                            " 'secfp',\n",
                             " 'pcqm4mv2_graphormer_base',\n",
+                            " 'ChemBERTa-77M-MLM',\n",
+                            " 'ChemBERTa-77M-MTR',\n",
                             " 'ChemGPT-1.2B',\n",
+                            " 'ChemGPT-19M',\n",
                             " 'ChemGPT-4.7M',\n",
-                            " 'DeepChem-ChemBERTa-77M-MLM',\n",
-                            " 'DeepChem-ChemBERTa-77M-MTR',\n",
-                            " 'maccs']"
+                            " 'GPT2-Zinc480M-87M',\n",
+                            " 'MolT5',\n",
+                            " 'Roberta-Zinc480M-102M',\n",
+                            " 'pharm2D-cats',\n",
+                            " 'pharm2D-default',\n",
+                            " 'pharm2D-gobbi',\n",
+                            " 'pharm2D-pmapper',\n",
+                            " 'pharm3D-cats',\n",
+                            " 'pharm3D-gobbi',\n",
+                            " 'pharm3D-pmapper',\n",
+                            " 'atompair-count',\n",
+                            " 'avalon',\n",
+                            " 'desc2D',\n",
+                            " 'desc3D',\n",
+                            " 'ecfp-count',\n",
+                            " 'ecfp',\n",
+                            " 'erg',\n",
+                            " 'estate',\n",
+                            " 'fcfp-count',\n",
+                            " 'fcfp',\n",
+                            " 'maccs',\n",
+                            " 'pattern',\n",
+                            " 'rdkit',\n",
+                            " 'topological-count',\n",
+                            " 'topological',\n",
+                            " 'electroshape',\n",
+                            " 'usr',\n",
+                            " 'usrcat']"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "[x.name for x in store.available_models]"
             ]
@@ -302,15 +434,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "dd64925fe6617865d410306d2b64fa69b44b63a36aad85fd11f7d4e4dc7609f3"
             }
         }
```

### Comparing `molfeat-0.9.0/nb/etl/entropy-transforner-zinc-etl.ipynb` & `molfeat-0.9.1/nb/etl/entropy-transforner-zinc-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/nb/etl/featurizer-etl.ipynb` & `molfeat-0.9.1/nb/etl/featurizer-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/nb/etl/molt5-etl.ipynb` & `molfeat-0.9.1/nb/etl/molt5-etl.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/pyproject.toml` & `molfeat-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_atom_bond_calculator.py` & `molfeat-0.9.1/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_descriptors.py` & `molfeat-0.9.1/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_fp.py` & `molfeat-0.9.1/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_graphs.py` & `molfeat-0.9.1/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_pharmacophore.py` & `molfeat-0.9.1/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_pretrained.py` & `molfeat-0.9.1/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_prot_embed.py` & `molfeat-0.9.1/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_state.py` & `molfeat-0.9.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.9.0/tests/test_utils.py` & `molfeat-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

