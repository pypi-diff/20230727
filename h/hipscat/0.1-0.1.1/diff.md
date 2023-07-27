# Comparing `tmp/hipscat-0.1.tar.gz` & `tmp/hipscat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.1.tar", last modified: Fri Jul 14 14:08:34 2023, max compression
+gzip compressed data, was "hipscat-0.1.1.tar", last modified: Thu Jul 27 19:42:23 2023, max compression
```

## Comparing `hipscat-0.1.tar` & `hipscat-0.1.1.tar`

### file list

```diff
@@ -1,193 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-14 14:08:22.000000 hipscat-0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-14 14:08:22.000000 hipscat-0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 14:08:22.000000 hipscat-0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 14:08:22.000000 hipscat-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 14:08:22.000000 hipscat-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-14 14:08:22.000000 hipscat-0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-14 14:08:22.000000 hipscat-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 14:08:34.588762 hipscat-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 14:08:22.000000 hipscat-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 14:08:22.000000 hipscat-0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-14 14:08:22.000000 hipscat-0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-14 14:08:22.000000 hipscat-0.1/docs/guide/pixel_math.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 14:08:22.000000 hipscat-0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks/catalog_size_inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks/cone_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 14:08:22.000000 hipscat-0.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 14:08:22.000000 hipscat-0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-14 14:08:22.000000 hipscat-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:08:34.588762 hipscat-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20808 2023-07-14 14:08:22.000000 hipscat-0.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/association_catalog/partition_join_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/catalog_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/index/index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/partition_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/source_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/catalog/source_catalog/source_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/almanac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.576762 hipscat-0.1/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_math/pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/src/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/pixel_tree/pixel_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/src/hipscat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.572762 hipscat-0.1/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 14:08:34.000000 hipscat-0.1/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-14 14:08:22.000000 hipscat-0.1/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-14 14:08:22.000000 hipscat-0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/almanac/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/dataset.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/deprecated.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/index_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/margin_cache.yml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_order1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac/small_sky_to_small_sky_order1.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/almanac_exception/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/association_missing_join.yml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/association_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_catalog_path.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_primary_path.yml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/bad_type.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/index_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/margin_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/almanac_exception/standalone_source_catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.580762 hipscat-0.1/tests/data/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/dataset/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/index_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/index_catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/margin_cache/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.568761 hipscat-0.1/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_order1/point_map.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_source/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_source/partition_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 14:08:22.000000 hipscat-0.1/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.584762 hipscat-0.1/tests/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/index/test_index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_math/test_pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:08:34.588762 hipscat-0.1/tests/hipscat/util/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-14 14:08:22.000000 hipscat-0.1/tests/hipscat/util/test_healpix_pixel_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.684309 hipscat-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 19:42:11.000000 hipscat-0.1.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-27 19:42:11.000000 hipscat-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-27 19:42:11.000000 hipscat-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-27 19:42:11.000000 hipscat-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 19:42:11.000000 hipscat-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-27 19:42:11.000000 hipscat-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-27 19:42:23.684309 hipscat-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-27 19:42:11.000000 hipscat-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/guide/margin_cache_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    53485 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 19:42:11.000000 hipscat-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-27 19:42:11.000000 hipscat-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:42:23.684309 hipscat-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.656308 hipscat-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.664309 hipscat-0.1.1/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.664309 hipscat-0.1.1/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.664309 hipscat-0.1.1/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.664309 hipscat-0.1.1/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.664309 hipscat-0.1.1/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.668309 hipscat-0.1.1/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/cone_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_math/pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.668309 hipscat-0.1.1/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_alignment_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/pixel_tree/pixel_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:11.000000 hipscat-0.1.1/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.660308 hipscat-0.1.1/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 19:42:23.000000 hipscat-0.1.1/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.668309 hipscat-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.648308 hipscat-0.1.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.668309 hipscat-0.1.1/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/index_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/margin_cache.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/small_sky_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/almanac_exception/standalone_source_catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/pixel_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/aligned_2_3_inner.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/aligned_2_3_left.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/aligned_2_3_outer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/aligned_2_3_right.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/pixel_tree_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/pixel_tree_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/pixel_trees/pixel_tree_3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.648308 hipscat-0.1.1/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.672309 hipscat-0.1.1/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.648308 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_order1/point_map.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_source/partition_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.676309 hipscat-0.1.1/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:42:23.680309 hipscat-0.1.1/tests/hipscat/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 19:42:11.000000 hipscat-0.1.1/tests/hipscat/util/test_healpix_pixel_convertor.py
```

### Comparing `hipscat-0.1/.github/pull_request_template.md` & `hipscat-0.1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.github/workflows/build-documentation.yml` & `hipscat-0.1.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.github/workflows/linting.yml` & `hipscat-0.1.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.github/workflows/publish-to-pypi.yml` & `hipscat-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.github/workflows/smoke-test.yml` & `hipscat-0.1.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.github/workflows/testing-and-coverage.yml` & `hipscat-0.1.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/.gitignore` & `hipscat-0.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -134,7 +134,9 @@
 .vscode/
 
 # dask
 dask-worker-space/
 
 # tmp directory
 tmp/
+
+**/.DS_Store
```

### Comparing `hipscat-0.1/.pre-commit-config.yaml` & `hipscat-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/LICENSE` & `hipscat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/PKG-INFO` & `hipscat-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.1
+Version: 0.1.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.1/README.md` & `hipscat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/docs/Makefile` & `hipscat-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/docs/conf.py` & `hipscat-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/docs/guide/contributing.rst` & `hipscat-0.1.1/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/docs/guide/directory_scheme.rst` & `hipscat-0.1.1/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/docs/guide/pixel_math.md` & `hipscat-0.1.1/docs/guide/pixel_math.md`

 * *Files 22% similar despite different names*

```diff
@@ -156,76 +156,49 @@
 
 ### pixel_is_polar
 Because of the nature of spherical coordinate systems, hipscat runs into some tricky edge cases at the poles. To ensure we can appropriately handle those problems, we need to check if a pixel is one of the four 'polar pixels'.
 
 #### Algorithm
 In the ring id scheme for `healpix`, the first and last 4 pixels are the polar pixels. To determine whether a nest scheme pixel is at the poles, all we have to do is convert the pixel into the ring scheme and determine if it falls at the beginning or end of the range 0 -> npix. So, if in the ring scheme the pix is `<= 3`, or `>= npix - 4`, we can safely assume that it is a polar pixel.
 
-### get_truncated_margin_pixels
-For pixels that are at the poles, our margin bounding box isn't set up to handle the data that is on the other side of the hemisphere from the partition. So when we calculate the boundaries, we truncate declination values outside of the range -90 -> 90. However, we obviously still want to include neighbor margin data that is affected by this truncation, namely the 3 margin pixels that are also polar pixels.
-
-#### Algorithm
-We want to find the 3 pixels at the healpix order of our margins that are polar. This is all of the pixels around the given pole _except_ the one that is contained within our partition pixel. 
+## Margin Bounding
+After constraining our data points using the `get_margin` code in `pixel_margins`, we then move on to our more accurate bound checking by calculating the distance between a given data point and the approximate boundaries of the healpixel.
 
-For the north pole, this is straightforwardly done by converting our partition pixel into the ring id scheme and returning the values between 0 and 3 that aren't equal to it.
+![diagram showing the spherical triangle formed by the data point and two boundary points with a perpendicular bisector.](margin_cache_diagram.png)
 
-For the south pole, we have to do a little more complicated math, due to the fact that the southern polar pixels aren't the same values at any healpix order. To find the at polar pixel at the `margin_order` that is contained by the partition pixel (and therefore to be excluded), we can take advantage of the fact that in the nest scheme the southern partition of a pixel is equal to `4 * pix` (see the algorithm section of `get_edge` above for more info), so to get the excluded southern pixel all we have to do is find the difference between `order` and `margin_order`, and multiply our `pix` value by `4 ** d_order`.
+To approximate this distance, we get the perpendicular bisector of the triangle made with the datapoint and the two closest boundary points. To find the the perpendicular bisector of this triangle (which is approximately the shortest distance between the data point and the healpix polygon), we will have to find
 
-## Margin Bounding
-After constraining our data points using the `get_margin` code in `pixel_margins`, we then move on to our more accurate bound checking by building bounding boxes that include a region approximately one `margin_threshold` wide around the original healpixel.
+$\sin(a) = \sin(A)\sin(x)$
 
-To get this bounding box, we
-- find a `scale` factor to apply to the original healpixel boundaries that increases the resolution by one `margin_threshold`
-- sample a set of points along the boundary of a healpixel
-- apply an affine transformation to these points to center them on the original healpixel
+$a = \arcsin(\sin(A),\sin(x))$
 
-resulting in a box that covers a border region of one `margin_threshold` around the original healpixel.
+where $a$ is the bisector, $x$ is the arc between our data point and one of the boundary points, and $A$ is the angle between that arc and the arc of the healpix boundary.
 
-We then can input these points into an astropy `regions.PolygonPixelRegion` object that we can the use to quickly check different datapoints against, resulting in a set of data for the final `neighbors.parquet` file.
+This identity comes from [Napier's rules for right spherical triangles](https://en.wikipedia.org/wiki/Spherical_trigonometry#Napier's_rules_for_right_spherical_triangles).
 
-### get_margin_scale
-Finds the scale factor that we want to use to scale up the healpixel bounds by to include the neighbor margin.
+we already have $x$ from our separation calculations, but we're going to need to calculate the angle $A$. to do this, we can make use of the [spherical law of cosines](https://en.wikipedia.org/wiki/Spherical_law_of_cosines). let's use the identity
 
-#### Algorithm
-- get the resolution of our `pixel_order` (sqrt of the pixel area)
-- add the `margin_threshold` to the resolution and square it.
-- divide this new area against the original pixel area to find the scale factor.
+$\cos(y) = \cos(x)\cos(z) + \sin(x)\sin(z)\cos(A)$
 
-### get_margin_bounds_and_wcs
-Given a healpixel and a scale factor, generate a `regions.PolygonPixelRegion` polygon and an `astropy.wcs.WCS` object containing the points of the healpixel scaled around the centroid by a factor of `scale`. Used in conjunction with `get_margin_scale` to perform an affine transform on a set of coordinates sampled from the boundaries of a healpixel.
+from there we can solve for A with
 
-By returning it as a pixel region along with a wcs object, we can quickly check data points against our polygon.
+$\sin(x)\sin(z)\cos(A) = \cos(y) - \cos(x)\cos(z)$
 
-In the case where `pixel_order` is less than 2, we divide the polygon into 4 or 16 different polygon regions (orders **0** and **1** respectively), each with their own `WCS` object. We do this because `PolygonPixelRegions` start to break down with large bounding boxes at the granular coordinate spaces that we're using.
+$\cos(A) = {\cos(y) - \cos(x)\cos(z) \over \sin(x)\sin(z)}$
 
-#### Algorithm
-- get a sample of the healpixel boundaries (4 * `step`)
-- find the centroid of the boundary coordinates, apply the `scale` to it, and find the difference from the original to find the translation values.
-    - this translation keeps the bounding box centered on the orignal healpixel, as an affine transform scales from the origin of the coordinate system.
-- build the [affine transform](https://en.wikipedia.org/wiki/Affine_transformation#Image_transformation) matrix.
-- convert the boundary coordinates into [homogeneous coordinates](https://en.wikipedia.org/wiki/Homogeneous_coordinates).
-- apply the affine transform to the now homogeneous coordinates.
-- build the polygon(s) and wcs object(s) for the now transformed points.
+$A = {\arccos({\cos(y) - \cos(x)\cos(z) \over \sin(x)\sin(z)})}$
 
+and now we have all the information to find the bisector and compare it to our margin threshold! 
 ### check_margin_bounds
-Given a set of ra and dec coordinates as well as a list of `regions.PolygonPixelRegion` and `astropy.wcs.WCS` tuples (see `get_margin_bounds_and_wcs` above), return a 1-dimmensional array of booleans on whether a given ra and dec coordinate pair are contained within any of the given bounding boxes.
+Given a set of ra and dec coordinates as well as the healpixel, healpix order, margin threshold, and the step value of sampled `healpy` boundaries, return a 1-dimmensional array of booleans on whether a given ra and dec coordinate pair are contained within any of the given bounding boxes.
 
 #### Implementation
-For ever entry into `poly_and_wcs`, we convert our set of coordinates into pixel values using the `astropy.wcs.utils.skycoord_to_pixel` function then use the built in `contains` function to return the list of bound checks.
+We take a chunk of our points and generate a set matrix of points with a shape (size_of_chunk, number_of_boundary_points) with all of our data points repeated along the first axis. Then, we generate a matrix of the same shape with the boundary points repeated as well and then put both of those matrices into a `SkyCoord` so that we can calculate the separations between all of them. We also find all of the distances between adjacent boundary points, so that we can find know the distance of each boundary segment. For each data point, we find the boundary point with the minimum separation, and then find which of the two adjacent boundary points has the smaller separation from the datapoint. From there, we can do the above calculations to get the perpendicular bisector and compare this against the `margin_threshold`. For checking around the corners of the healpixel, where the data point may not actually form a neat triangle with it's closest boundary points, we check to see if the minimum distance is less than the margin threshold and return True if it is. This way, we'll keep any data points that fall within the margin threshold but would return NaN with our perpendicular bisector calculations.
 
-### check_polar_margin_bounds
-For healpixels that surround the poles, the affine transform math breaks down directly around the poles, making it much harder for us to properly check margin data on the opposite hemisphere to our pixel. To solve this problem, we can use the `get_truncated_pixels` to find out what margin data falls around the poles, and then manually check the angular distance between those points and the boundaries of the given partition pixel to find out if the data point falls within a `margin_threshold` distance. While this sort of N^2 calculation isn't practical or desired for the larger dataset, this edge case usually only affects a small amount of the total potential margin cache data for a given catalog.
-
-#### Algorithm
-- Find the ratio of the `margin_order` (i.e. the order that our margin pixels are at) to the `order` of the larger partition pixel so that we can find the approximate range of samples to take from the `hp.boundaries` of our healpixel, giving us a set of points that define the border of the pixel along the poles.
-    - Even at very high `step` values, this generally doesn't return a large number of points to check against, since even having a small difference between `order` and `margin_order` leads to exponentially smaller values of this ratio.
-    - Higher `step` values didn't meaningfully increase the accuracy for `margin_threshold` checks so the default is value 1000, but we've left `step` as variable so that should more granularity be needed a user can adjust this value.
-- Make sure none of these `polar_boundaries` values fall outside of the range -90 -> 90 declination, as sometimes `hp.boundaries` can return values a few millionths lower or higher at highly granular `step` values.
-- Get the angular distance of our `r_asc` and `dec` values and our boundary values.
-- Return `True` for any coordinates that have a distance less than or equal to `margin_threshold`.
+To speed up our calculations, the inner loops of calculations is compiled with the `numba` JIT compiler.
 
 ## HiPSCat ID
 
 This index is defined as a 64-bit integer which has two parts:
 
 * healpix pixel (at order 19)
 * incrementing counter (within same healpix, for uniqueness)
```

### Comparing `hipscat-0.1/docs/notebooks/catalog_size_inspection.ipynb` & `hipscat-0.1.1/docs/notebooks/catalog_size_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/pyproject.toml` & `hipscat-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 requires-python = ">=3.8"
 dependencies = [
     "healpy",
     "pandas",
     "setuptools_scm",
     "pyarrow",
     "astropy",
-    "regions",
     "typing-extensions>=4.3.0",
+    "numba"
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "mypy", # Used for static type checking of files
     "pylint", # Used for static linting of files
```

### Comparing `hipscat-0.1/src/.pylintrc` & `hipscat-0.1.1/src/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
            ex,
            Run,
+           ra,
            _
 
 # Good variable names regexes, separated by a comma. If names match any regex,
 # they will always be accepted
 good-names-rgxs=
 
 # Include a hint for the correct naming format with invalid-name.
```

### Comparing `hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog.py` & `hipscat-0.1.1/src/hipscat/catalog/association_catalog/association_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, Union
 
 import pandas as pd
 
-from hipscat.catalog import CatalogType
 from hipscat.catalog.association_catalog.association_catalog_info import AssociationCatalogInfo
 from hipscat.catalog.association_catalog.partition_join_info import PartitionJoinInfo
+from hipscat.catalog.catalog_type import CatalogType
 from hipscat.catalog.dataset.dataset import Dataset
 from hipscat.io import FilePointer, paths
 
 
 class AssociationCatalog(Dataset):
     """A HiPSCat Catalog for enabling fast joins between two HiPSCat catalogs
 
@@ -39,15 +39,17 @@
 
         Returns:
             pd.DataFrame with each row being a pair of pixels from the primary and join catalogs
         """
         return self.join_info.data_frame
 
     @staticmethod
-    def _get_partition_join_info_from_pixels(join_pixels: JoinPixelInputTypes) -> PartitionJoinInfo:
+    def _get_partition_join_info_from_pixels(
+        join_pixels: JoinPixelInputTypes,
+    ) -> PartitionJoinInfo:
         if isinstance(join_pixels, PartitionJoinInfo):
             return join_pixels
         if isinstance(join_pixels, pd.DataFrame):
             return PartitionJoinInfo(join_pixels)
         raise TypeError("join_pixels must be of type PartitionJoinInfo or DataFrame")
 
     @classmethod
```

### Comparing `hipscat-0.1/src/hipscat/catalog/association_catalog/association_catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/association_catalog/association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/association_catalog/partition_join_info.py` & `hipscat-0.1.1/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/dataset/base_catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/dataset/base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/dataset/catalog_info_factory.py` & `hipscat-0.1.1/src/hipscat/catalog/dataset/catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/dataset/dataset.py` & `hipscat-0.1.1/src/hipscat/catalog/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/index/index_catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/index/index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/partition_info.py` & `hipscat-0.1.1/src/hipscat/catalog/partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/catalog/source_catalog/source_catalog_info.py` & `hipscat-0.1.1/src/hipscat/catalog/source_catalog/source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/inspection/almanac.py` & `hipscat-0.1.1/src/hipscat/inspection/almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/inspection/almanac_info.py` & `hipscat-0.1.1/src/hipscat/inspection/almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.1.1/src/hipscat/inspection/visualize_catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 NB: Testing validity of generated plots is currently not tested in our unit test suite.
 """
 
 import healpy as hp
 import numpy as np
 from matplotlib import pyplot as plt
 
-from hipscat.catalog import Catalog, PartitionInfo
+from hipscat.catalog import Catalog
 from hipscat.io import file_io, paths
 
 
 def _read_point_map(catalog_base_dir):
     """Read the object spatial distribution information from a healpix FITS file.
 
     Args:
@@ -51,31 +51,28 @@
         catalog (`hipscat.catalog.Catalog`) Catalog to display
         projection (str) The map projection to use. Valid values include:
             - moll - Molleweide projection (default)
             - gnom - Gnomonic projection
             - cart - Cartesian projection
             - orth - Orthographic projection
     """
-    pixels = catalog.get_pixels()
-
-    catalog_orders = pixels[PartitionInfo.METADATA_ORDER_COLUMN_NAME].unique()
-    catalog_orders.sort()
-    max_order = catalog_orders[-1]
+    pixels = catalog.partition_info.get_healpix_pixels()
+    max_order = catalog.partition_info.get_highest_order()
 
     order_map = np.full(hp.order2npix(max_order), hp.pixelfunc.UNSEEN)
 
-    for _, pixel in pixels.iterrows():
-        explosion_factor = 4 ** (max_order - pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME])
+    for pixel in pixels:
+        explosion_factor = 4 ** (max_order - pixel.order)
         exploded_pixels = [
             *range(
-                pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] * explosion_factor,
-                (pixel[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] + 1) * explosion_factor,
+                pixel.pixel * explosion_factor,
+                (pixel.pixel + 1) * explosion_factor,
             )
         ]
-        order_map[exploded_pixels] = pixel[PartitionInfo.METADATA_ORDER_COLUMN_NAME]
+        order_map[exploded_pixels] = pixel.order
     _plot_healpix_map(
         order_map,
         projection,
         f"Catalog pixel density map - {catalog.catalog_name}",
         draw_map=draw_map,
     )
```

### Comparing `hipscat-0.1/src/hipscat/io/__init__.py` & `hipscat-0.1.1/src/hipscat/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/io/file_io/__init__.py` & `hipscat-0.1.1/src/hipscat/io/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/io/file_io/file_io.py` & `hipscat-0.1.1/src/hipscat/io/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.1.1/src/hipscat/io/file_io/file_pointer.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/io/paths.py` & `hipscat-0.1.1/src/hipscat/io/paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/io/write_metadata.py` & `hipscat-0.1.1/src/hipscat/io/write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/pixel_math/__init__.py` & `hipscat-0.1.1/src/hipscat/pixel_math/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """Utilities for performing fun math on healpix pixels"""
 
 from .healpix_pixel import HealpixPixel
 from .healpix_pixel_convertor import HealpixInputTypes, get_healpix_pixel
 from .hipscat_id import compute_hipscat_id, hipscat_id_to_healpix
-from .margin_bounding import (
-    check_margin_bounds,
-    check_polar_margin_bounds,
-    get_margin_bounds_and_wcs,
-    get_margin_scale,
-)
+from .margin_bounding import check_margin_bounds
 from .partition_stats import (
     compute_pixel_map,
     empty_histogram,
     generate_alignment,
     generate_constant_pixel_map,
     generate_destination_pixel_map,
     generate_histogram,
 )
-from .pixel_margins import get_edge, get_margin, get_truncated_margin_pixels, pixel_is_polar
+from .pixel_margins import get_edge, get_margin, pixel_is_polar
```

### Comparing `hipscat-0.1/src/hipscat/pixel_math/healpix_pixel_convertor.py` & `hipscat-0.1.1/src/hipscat/pixel_math/healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.1.1/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.1.1/src/hipscat/pixel_math/partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.1.1/src/hipscat/pixel_math/pixel_margins.py`

 * *Files 22% similar despite different names*

```diff
@@ -131,55 +131,7 @@
 
     # in the ring numbering scheme, the first and last 4 pixels are the poles.
     if ring_pix <= 3:
         return (True, "North")
     if ring_pix >= npix - 4:
         return (True, "South")
     return (False, "")
-
-
-def get_truncated_margin_pixels(order, pix, margin_order):
-    """Given a polar healpixel, find the margin pixels at order highest_k that will be
-    truncated at the poles. In other words, find the margin pixels that are also
-    polar pixels.
-
-    Args:
-        order (int): the healpix order of the pixel that we wish to
-            find the truncated margin pixels for.
-        pix (int): the healpixel we wish to find the truncated margin pixels for.
-        margin_order (int): the healpixel order that our margin pixels are at. Must
-            be larger than `order`.
-    Returns:
-        a list of margin pixels at margin_order order that will be truncated at
-            the poles, i.e. the margin pixels that are also polar pixels
-            themselves. In the case that pix is a polar pixel, it will return
-            3 pixels, otherwise it will return an empty list.
-    """
-    if margin_order <= order:
-        raise ValueError("margin_order must be larger than order")
-
-    partition_nside = hp.order2nside(order)
-    margin_nside = hp.order2nside(margin_order)
-
-    polar, pole = pixel_is_polar(order, pix)
-
-    if not polar:
-        return []
-
-    truncs = []
-
-    if pole == "North":
-        excluded_pixel = hp.nest2ring(partition_nside, pix)
-        for i in range(4):
-            if i != excluded_pixel:
-                truncs.append(hp.ring2nest(margin_nside, i))
-    else:
-        d_order = margin_order - order
-        excluded_pixel_nest = (4**d_order) * pix
-        excluded_pixel_ring = hp.nest2ring(margin_nside, excluded_pixel_nest)
-        npix = hp.nside2npix(margin_nside)
-
-        for j in range(npix - 4, npix):
-            if j != excluded_pixel_ring:
-                truncs.append(hp.ring2nest(margin_nside, j))
-
-    return truncs
```

### Comparing `hipscat-0.1/src/hipscat/pixel_tree/pixel_node.py` & `hipscat-0.1.1/src/hipscat/pixel_tree/pixel_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     }
 
     def __init__(
         self,
         pixel: HealpixInputTypes,
         node_type: PixelNodeType,
         parent: PixelNode | None,
-        children: List[PixelNode] | None = None,
     ) -> None:
         """Inits PixelNode with its attributes
 
         Raises:
             ValueError: Invalid arguments for the specified pixel type
         """
 
@@ -54,18 +53,14 @@
             raise ValueError("Parent node must be at order one less than current node")
 
         self.pixel = pixel
         self.node_type = node_type
         self.parent = parent
         self.children = []
 
-        if children is not None:
-            for child in children:
-                self.add_child_node(child)
-
         if self.parent is not None:
             self.parent.add_child_node(self)
 
     @property
     def hp_order(self):
         """The order of the HealpixPixel the node is at"""
         return self.pixel.order
@@ -92,14 +87,25 @@
 
         if len(self.children) >= self._NODE_TYPE_MAX_CHILDREN[self.node_type]:
             raise OverflowError("Node already has the maximum amount of children")
 
         insert_index = bisect(list(map(lambda node: node.hp_pixel, self.children)), child.hp_pixel)
         self.children.insert(insert_index, child)
 
+    def remove_child_link(self, node):
+        """Remove a link to a child node from the node. This removes it from the list of children,
+        but does not delete the node
+
+        Args:
+            node: the node object to remove
+        """
+        if node not in self.children:
+            raise ValueError("Node not a child node, cannot remove")
+        self.children.remove(node)
+
     def get_all_leaf_descendants(self) -> List[PixelNode]:
         """Gets all descendant nodes that are leaf nodes.
 
         Leafs nodes correspond to pixels that have data files containing astronomical objects, so
         this method is used to get the files containing all astronomical objects within the pixel.
 
         This function called on a leaf node returns a list including the node itself and only itself
```

### Comparing `hipscat-0.1/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.1.1/src/hipscat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.1
+Version: 0.1.1
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.1/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.1.1/src/hipscat.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
 docs/requirements.txt
 docs/guide/contributing.rst
 docs/guide/directory_scheme.rst
+docs/guide/margin_cache_diagram.png
 docs/guide/pixel_math.md
 docs/notebooks/catalog_size_inspection.ipynb
 docs/notebooks/cone_search.ipynb
 src/.pylintrc
 src/hipscat/__init__.py
 src/hipscat/_version.py
 src/hipscat/py.typed
@@ -56,21 +57,24 @@
 src/hipscat/io/__init__.py
 src/hipscat/io/paths.py
 src/hipscat/io/write_metadata.py
 src/hipscat/io/file_io/__init__.py
 src/hipscat/io/file_io/file_io.py
 src/hipscat/io/file_io/file_pointer.py
 src/hipscat/pixel_math/__init__.py
+src/hipscat/pixel_math/cone_filter.py
 src/hipscat/pixel_math/healpix_pixel.py
 src/hipscat/pixel_math/healpix_pixel_convertor.py
 src/hipscat/pixel_math/hipscat_id.py
 src/hipscat/pixel_math/margin_bounding.py
 src/hipscat/pixel_math/partition_stats.py
 src/hipscat/pixel_math/pixel_margins.py
 src/hipscat/pixel_tree/__init__.py
+src/hipscat/pixel_tree/pixel_alignment.py
+src/hipscat/pixel_tree/pixel_alignment_types.py
 src/hipscat/pixel_tree/pixel_node.py
 src/hipscat/pixel_tree/pixel_node_type.py
 src/hipscat/pixel_tree/pixel_tree.py
 src/hipscat/pixel_tree/pixel_tree_builder.py
 tests/.pylintrc
 tests/conftest.py
 tests/data/almanac/catalog.yml
@@ -90,14 +94,21 @@
 tests/data/almanac_exception/index_missing_primary.yml
 tests/data/almanac_exception/margin_missing_primary.yml
 tests/data/almanac_exception/standalone_source_catalog.yml
 tests/data/catalog/catalog_info.json
 tests/data/dataset/catalog_info.json
 tests/data/index_catalog/catalog_info.json
 tests/data/margin_cache/catalog_info.json
+tests/data/pixel_trees/aligned_2_3_inner.csv
+tests/data/pixel_trees/aligned_2_3_left.csv
+tests/data/pixel_trees/aligned_2_3_outer.csv
+tests/data/pixel_trees/aligned_2_3_right.csv
+tests/data/pixel_trees/pixel_tree_1.csv
+tests/data/pixel_trees/pixel_tree_2.csv
+tests/data/pixel_trees/pixel_tree_3.csv
 tests/data/small_sky/catalog_info.json
 tests/data/small_sky/partition_info.csv
 tests/data/small_sky/point_map.fits
 tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
 tests/data/small_sky_order1/catalog_info.json
 tests/data/small_sky_order1/partition_info.csv
 tests/data/small_sky_order1/point_map.fits
@@ -132,11 +143,12 @@
 tests/hipscat/io/file_io/test_file_pointers.py
 tests/hipscat/pixel_math/test_healpix_pixel.py
 tests/hipscat/pixel_math/test_hipscat_id.py
 tests/hipscat/pixel_math/test_margin_bounding.py
 tests/hipscat/pixel_math/test_partition_stats.py
 tests/hipscat/pixel_math/test_pixel_margins.py
 tests/hipscat/pixel_tree/conftest.py
+tests/hipscat/pixel_tree/test_pixel_alignment.py
 tests/hipscat/pixel_tree/test_pixel_node.py
 tests/hipscat/pixel_tree/test_pixel_tree.py
 tests/hipscat/pixel_tree/test_pixel_tree_builder.py
 tests/hipscat/util/test_healpix_pixel_convertor.py
```

### Comparing `hipscat-0.1/tests/.pylintrc` & `hipscat-0.1.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/conftest.py` & `hipscat-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.1.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky/point_map.fits` & `hipscat-0.1.1/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.1.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.1.1/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py` & `hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py` & `hipscat-0.1.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/dataset/test_dataset.py` & `hipscat-0.1.1/tests/hipscat/catalog/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/index/test_index_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/index/test_index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/test_catalog_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/test_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.1.1/tests/hipscat/catalog/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/conftest.py` & `hipscat-0.1.1/tests/hipscat/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,45 +10,42 @@
 
 @pytest.fixture
 def root_pixel_node_data():
     return {
         "pixel": HealpixPixel(-1, -1),
         "node_type": PixelNodeType.ROOT,
         "parent": None,
-        "children": None,
     }
 
 
 @pytest.fixture
 def root_pixel_node(root_pixel_node_data):
     return PixelNode(**root_pixel_node_data)
 
 
 @pytest.fixture
 def inner_pixel_node_data(root_pixel_node):
     return {
         "pixel": HealpixPixel(0, 1),
         "node_type": PixelNodeType.INNER,
         "parent": root_pixel_node,
-        "children": None,
     }
 
 
 @pytest.fixture
 def inner_pixel_node(inner_pixel_node_data):
     return PixelNode(**inner_pixel_node_data)
 
 
 @pytest.fixture
 def leaf_pixel_node_data(inner_pixel_node):
     return {
         "pixel": HealpixPixel(1, 12),
         "node_type": PixelNodeType.LEAF,
         "parent": inner_pixel_node,
-        "children": None,
     }
 
 
 @pytest.fixture
 def leaf_pixel_node(leaf_pixel_node_data):
     return PixelNode(**leaf_pixel_node_data)
```

### Comparing `hipscat-0.1/tests/hipscat/inspection/test_almanac.py` & `hipscat-0.1.1/tests/hipscat/inspection/test_almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/inspection/test_almanac_info.py` & `hipscat-0.1.1/tests/hipscat/inspection/test_almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.1.1/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/io/conftest.py` & `hipscat-0.1.1/tests/hipscat/io/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.1.1/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.1.1/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/io/test_paths.py` & `hipscat-0.1.1/tests/hipscat/io/test_paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.1.1/tests/hipscat/io/test_write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.1.1/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/pixel_math/test_partition_stats.py` & `hipscat-0.1.1/tests/hipscat/pixel_math/test_partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_node.py` & `hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,7 +142,21 @@
 
 def test_get_leaf_descendants_with_multiple_leafs(root_pixel_node, leaf_pixel_node, leaf_pixel_node_data):
     leaf_pixel_node_data["pixel"] = HealpixPixel(
         leaf_pixel_node_data["pixel"].order, leaf_pixel_node_data["pixel"].pixel + 1
     )
     second_leaf = PixelNode(**leaf_pixel_node_data)
     assert root_pixel_node.get_all_leaf_descendants() == [leaf_pixel_node, second_leaf]
+
+
+def test_remove_child_link(root_pixel_node, inner_pixel_node):
+    assert inner_pixel_node in root_pixel_node.children
+    assert len(root_pixel_node.children) == 1
+    root_pixel_node.remove_child_link(inner_pixel_node)
+    assert inner_pixel_node not in root_pixel_node.children
+    assert len(root_pixel_node.children) == 0
+
+
+def test_remove_child_link_wrong_node_errors(root_pixel_node, leaf_pixel_node):
+    assert leaf_pixel_node not in root_pixel_node.children
+    with pytest.raises(ValueError):
+        leaf_pixel_node.remove_child_link(leaf_pixel_node)
```

### Comparing `hipscat-0.1/tests/hipscat/pixel_tree/test_pixel_tree.py` & `hipscat-0.1.1/tests/hipscat/pixel_tree/test_pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.1/tests/hipscat/util/test_healpix_pixel_convertor.py` & `hipscat-0.1.1/tests/hipscat/util/test_healpix_pixel_convertor.py`

 * *Files identical despite different names*

