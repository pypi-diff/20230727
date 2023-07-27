# Comparing `tmp/mattress-0.0.3.tar.gz` & `tmp/mattress-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattress-0.0.3.tar", last modified: Wed Jul 26 16:28:44 2023, max compression
+gzip compressed data, was "mattress-0.0.4.tar", last modified: Thu Jul 27 16:56:30 2023, max compression
```

## Comparing `mattress-0.0.3.tar` & `mattress-0.0.4.tar`

### file list

```diff
@@ -1,231 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.663068 mattress-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-26 16:28:31.000000 mattress-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.627068 mattress-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.631068 mattress-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-26 16:28:31.000000 mattress-0.0.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 16:28:31.000000 mattress-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 16:28:31.000000 mattress-0.0.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 16:28:31.000000 mattress-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 16:28:31.000000 mattress-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 16:28:31.000000 mattress-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-26 16:28:31.000000 mattress-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 16:28:31.000000 mattress-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 16:28:31.000000 mattress-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 16:28:44.663068 mattress-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-26 16:28:31.000000 mattress-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-26 16:28:31.000000 mattress-0.0.3/docs/tutorial
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 16:28:31.000000 mattress-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 16:28:44.663068 mattress-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-26 16:28:31.000000 mattress-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.627068 mattress-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/src/mattress/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/TatamiNumericPointer.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/cpphelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.631068 mattress-0.0.3/src/mattress/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/src/mattress/extern/tatami/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/extern/tatami/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.627068 mattress-0.0.3/src/mattress/extern/tatami/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/src/mattress/extern/tatami/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/char2double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/colsums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/parallel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/print_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/read_h5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/read_mm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.627068 mattress-0.0.3/src/mattress/extern/tatami/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/dense/
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.639068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.643068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.643068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.643068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/
--rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.643068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31532 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.647068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.647068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/tatami.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.647068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.631068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/dense/
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    42562 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    62049 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.651068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.655068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.655068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/medians.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/sums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/variances.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.655068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.655068 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/convert_to_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.631068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.631068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-26 16:28:32.000000 mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.659068 mattress-0.0.3/src/mattress/include/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/include/Mattress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.663068 mattress-0.0.3/src/mattress/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/lib/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/lib/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-26 16:28:31.000000 mattress-0.0.3/src/mattress/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.635068 mattress-0.0.3/src/mattress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 16:28:44.000000 mattress-0.0.3/src/mattress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:28:44.663068 mattress-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 16:28:31.000000 mattress-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 16:28:31.000000 mattress-0.0.3/tests/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-26 16:28:31.000000 mattress-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-27 16:56:16.000000 mattress-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.367239 mattress-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.383239 mattress-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-27 16:56:16.000000 mattress-0.0.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 16:56:16.000000 mattress-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 16:56:16.000000 mattress-0.0.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 16:56:16.000000 mattress-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 16:56:16.000000 mattress-0.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 16:56:16.000000 mattress-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-27 16:56:16.000000 mattress-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 16:56:16.000000 mattress-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 16:56:16.000000 mattress-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-27 16:56:30.419239 mattress-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-27 16:56:16.000000 mattress-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 16:56:16.000000 mattress-0.0.4/docs/tutorial
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 16:56:16.000000 mattress-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-27 16:56:30.419239 mattress-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-27 16:56:16.000000 mattress-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.371239 mattress-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.387239 mattress-0.0.4/src/mattress/
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/TatamiNumericPointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 16:56:17.000000 mattress-0.0.4/src/mattress/extern/tatami/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.371239 mattress-0.0.4/src/mattress/extern/tatami/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress/extern/tatami/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/char2double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/colsums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/parallel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/print_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_h5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_mm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/tatami/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.395239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.399239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.403239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31574 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.407239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.407239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23308 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/tatami.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.375239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62084 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.411239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/medians.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/sums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/variances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 16:56:17.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.379239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.379239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.415239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-27 16:56:18.000000 mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/include/Mattress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/src/mattress/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/lib/dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 16:56:16.000000 mattress-0.0.4/src/mattress/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.391239 mattress-0.0.4/src/mattress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 16:56:30.000000 mattress-0.0.4/src/mattress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:56:30.419239 mattress-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 16:56:16.000000 mattress-0.0.4/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 16:56:16.000000 mattress-0.0.4/tox.ini
```

### Comparing `mattress-0.0.3/.coveragerc` & `mattress-0.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/.github/workflows/pypi-test.yml` & `mattress-0.0.4/.github/workflows/pypi-test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # This workflow will install Python dependencies, run tests and lint with a single version of Python
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Test the library
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+      - main
+    tags:
+      - "*"
+  pull_request:
 
 jobs:
   test:
     name: Running tests
     runs-on: ubuntu-latest
 
     steps:
@@ -25,14 +31,25 @@
         run: |
           python -m pip install --upgrade pip
           pip install flake8 pytest tox cython numpy
       - name: Test with tox
         run: |
           python setup.py build_ext --inplace
           tox
+      - name: Build docs
+        run: |
+          tox -e docs
+          touch ./docs/_build/html/.nojekyll
+      - name: GH Pages Deployment
+        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
+        uses: JamesIves/github-pages-deploy-action@4.1.3
+        with:
+          branch: gh-pages # The branch the action should deploy to.
+          folder: ./docs/_build/html
+          clean: true # Automatically remove deleted files from the deploy branch
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
@@ -43,14 +60,16 @@
         with:
           submodules: true
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.12.1
         env:
           CIBW_ARCHS_MACOS: x86_64 arm64
+          CIBW_ARCHS_LINUX: x86_64 # remove this later so we build for all linux archs
+          CIBW_PROJECT_REQUIRES_PYTHON: ">=3.9"
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
@@ -63,30 +82,14 @@
       - name: Build sdist
         run: pipx run build --sdist
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
-  gh_pages:
-    needs: [test]
-    runs-on: ubuntu-latest
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
-    steps:
-      - name: Build docs
-        run: |
-          tox -e docs
-      - run: touch ./docs/_build/html/.nojekyll
-      - name: GH Pages Deployment
-        uses: JamesIves/github-pages-deploy-action@4.1.3
-        with:
-          branch: gh-pages # The branch the action should deploy to.
-          folder: ./docs/_build/html
-          clean: true # Automatically remove deleted files from the deploy branch
-
   upload_pypi:
     needs: [test, build_wheels, build_sdist]
     runs-on: ubuntu-latest
     # upload to PyPI on every tag starting with 'v'
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
     # alternatively, to publish when a GitHub Release is created, use the following rule:
     # if: github.event_name == 'release' && github.event.action == 'published'
```

### Comparing `mattress-0.0.3/.gitignore` & `mattress-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/.readthedocs.yml` & `mattress-0.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/CONTRIBUTING.md` & `mattress-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/LICENSE.txt` & `mattress-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/PKG-INFO` & `mattress-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.3
+Version: 0.0.4
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.3/README.md` & `mattress-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/docs/Makefile` & `mattress-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/docs/conf.py` & `mattress-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/docs/index.md` & `mattress-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/docs/tutorial` & `mattress-0.0.4/docs/tutorial`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/setup.cfg` & `mattress-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/setup.py` & `mattress-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 if __name__ == "__main__":
     try:
         setup(
             use_scm_version={"version_scheme": "no-guess-dev"},
             ext_modules=[
                 Extension(
                     "mattress.core",
-                    ["src/mattress/lib/dense.cpp", "src/mattress/lib/common.cpp"],
+                    [
+                        "src/mattress/lib/dense.cpp",
+                        "src/mattress/lib/compressed_sparse.cpp",
+                        "src/mattress/lib/common.cpp",
+                    ],
                     include_dirs=[
                         "src/mattress/extern/tatami/include",
                         "src/mattress/include",
                     ],
                     language="c++",
                     extra_compile_args=[
                         "-std=c++17",
```

### Comparing `mattress-0.0.3/src/mattress/__init__.py` & `mattress-0.0.4/src/mattress/__init__.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/cpphelpers.py` & `mattress-0.0.4/src/mattress/cpphelpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,16 +48,22 @@
 lib.py_extract_ncol.restype = ct.c_int
 lib.py_extract_ncol.argtypes = [ct.c_void_p]
 lib.py_extract_sparse.restype = ct.c_int
 lib.py_extract_sparse.argtypes = [ct.c_void_p]
 lib.py_extract_row.argtypes = [ct.c_void_p, ct.c_int, ct.c_void_p]
 lib.py_extract_column.argtypes = [ct.c_void_p, ct.c_int, ct.c_void_p]
 
-
 lib.py_initialize_dense_matrix.restype = ct.c_void_p
-lib.py_initialize_dense_matrix.argtypes = [
+lib.py_initialize_dense_matrix.argtypes = [ct.c_int, ct.c_int, ct.c_char_p, ct.c_void_p]
+
+lib.py_initialize_compressed_sparse_matrix.restype = ct.c_void_p
+lib.py_initialize_compressed_sparse_matrix.argtypes = [
     ct.c_int,
     ct.c_int,
+    ct.c_uint64,
     ct.c_char_p,
     ct.c_void_p,
-    ct.c_char,
+    ct.c_char_p,
+    ct.c_void_p,
+    ct.c_void_p,
+    ct.c_uint8,
 ]
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml` & `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml` & `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/.github/workflows/run-tests.yaml` & `mattress-0.0.4/src/mattress/extern/tatami/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/CMakeLists.txt` & `mattress-0.0.4/src/mattress/extern/tatami/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/LICENSE` & `mattress-0.0.4/src/mattress/extern/tatami/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/README.md` & `mattress-0.0.4/src/mattress/extern/tatami/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/docs/Doxyfile` & `mattress-0.0.4/src/mattress/extern/tatami/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/CMakeLists.txt` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/README.md` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/char2double.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/char2double.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/colsums.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/colsums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/parallel.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/print_vector.h` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/print_vector.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/read_h5.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_h5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/read_mm.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/read_mm.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/Options.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/Options.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -88,13 +88,13 @@
      * Note that this may not be filled if extraction was performed with a `SparseExtractMode` that did not extract the indices.
      */
     std::vector<Index> index;
 
     /**
      * @param n Number of structural non-zeros.
      */
-    SparseRangeCopy(Index n) : number(n), index(n), value(n) {}
+    SparseRangeCopy(Index n) : number(n), value(n), index(n) {}
 };
 
 }
 
 #endif
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/base/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/base/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -191,40 +191,40 @@
         for (Index_ i = 0; i < index_length; ++i, ++buffer) {
             *buffer = values[index_start[i] * dim_secondary + x]; 
         }
         return;
     }
 
 public:
-    std::unique_ptr<FullDenseExtractor<Value_, Index_> > dense_row(const Options& opt) const {
+    std::unique_ptr<FullDenseExtractor<Value_, Index_> > dense_row(const Options&) const {
         auto ptr = new DenseBase<true, DimensionSelectionType::FULL>(this);
         return std::unique_ptr<FullDenseExtractor<Value_, Index_> >(ptr);
     }
 
-    std::unique_ptr<BlockDenseExtractor<Value_, Index_> > dense_row(Index_ block_start, Index_ block_length, const Options& opt) const {
+    std::unique_ptr<BlockDenseExtractor<Value_, Index_> > dense_row(Index_ block_start, Index_ block_length, const Options&) const {
         auto ptr = new DenseBase<true, DimensionSelectionType::BLOCK>(this, block_start, block_length);
         return std::unique_ptr<BlockDenseExtractor<Value_, Index_> >(ptr);
     }
 
-    std::unique_ptr<IndexDenseExtractor<Value_, Index_> > dense_row(std::vector<Index_> indices, const Options& opt) const {
+    std::unique_ptr<IndexDenseExtractor<Value_, Index_> > dense_row(std::vector<Index_> indices, const Options&) const {
         auto ptr = new DenseBase<true, DimensionSelectionType::INDEX>(this, std::move(indices));
         return std::unique_ptr<IndexDenseExtractor<Value_, Index_> >(ptr);
     }
 
-    std::unique_ptr<FullDenseExtractor<Value_, Index_> > dense_column(const Options& opt) const {
+    std::unique_ptr<FullDenseExtractor<Value_, Index_> > dense_column(const Options&) const {
         auto ptr = new DenseBase<false, DimensionSelectionType::FULL>(this);
         return std::unique_ptr<FullDenseExtractor<Value_, Index_> >(ptr);
     }
 
-    std::unique_ptr<BlockDenseExtractor<Value_, Index_> > dense_column(Index_ block_start, Index_ block_length, const Options& opt) const {
+    std::unique_ptr<BlockDenseExtractor<Value_, Index_> > dense_column(Index_ block_start, Index_ block_length, const Options&) const {
         auto ptr = new DenseBase<false, DimensionSelectionType::BLOCK>(this, block_start, block_length);
         return std::unique_ptr<BlockDenseExtractor<Value_, Index_> >(ptr);
     }
 
-    std::unique_ptr<IndexDenseExtractor<Value_, Index_> > dense_column(std::vector<Index_> indices, const Options& opt) const {
+    std::unique_ptr<IndexDenseExtractor<Value_, Index_> > dense_column(std::vector<Index_> indices, const Options&) const {
         auto ptr = new DenseBase<false, DimensionSelectionType::INDEX>(this, std::move(indices));
         return std::unique_ptr<IndexDenseExtractor<Value_, Index_> >(ptr);
     }
 };
 
 /**
  * Column-major matrix.
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -42,19 +42,18 @@
     void dense(Index_, ExtractType_, Index_ length, Value_* left_buffer, const Value_* right_buffer) const {
         for (Index_ i = 0; i < length; ++i) {
             delayed_arith_run<op_, true>(left_buffer[i], right_buffer[i]);
         }
     }
 
     template<bool, bool needs_value, bool needs_index, typename Value_, typename Index_>
-    Index_ sparse(Index_ idx, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
+    Index_ sparse(Index_, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
         // Don't bother storing an explicit zero for MULTIPLY operations when either entry is zero.
         constexpr bool must_have_both = (op_ == DelayedArithOp::MULTIPLY);
         return delayed_binary_isometric_sparse_operation<must_have_both, needs_value, needs_index>(
-            idx, 
             left, 
             right, 
             value_buffer, 
             index_buffer, 
             [](Value_& l, Value_ r) { delayed_arith_run<op_, true>(l, r); }
         );
     }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,18 @@
     void dense(Index_, ExtractType_, Index_ length, Value_* left_buffer, const Value_* right_buffer) const {
         for (Index_ i = 0; i < length; ++i) {
             delayed_boolean_run<op_>(left_buffer[i], right_buffer[i]);
         }
     }
 
     template<bool, bool needs_value, bool needs_index, typename Value_, typename Index_>
-    Index_ sparse(Index_ idx, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
+    Index_ sparse(Index_, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
         // None of the operations will return zero if one entry is zero and the other entry is non-zero...
         // except for equality, but then, the sparse() method would never even be used.
         return delayed_binary_isometric_sparse_operation<false, needs_value, needs_index>(
-            idx, 
             left, 
             right, 
             value_buffer, 
             index_buffer, 
             [](Value_& l, Value_ r) { delayed_boolean_run<op_>(l, r); }
         );
     }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,18 @@
     void dense(Index_, ExtractType_, Index_ length, Value_* left_buffer, const Value_* right_buffer) const {
         for (Index_ i = 0; i < length; ++i) {
             delayed_compare_run<op_>(left_buffer[i], right_buffer[i]);
         }
     }
 
     template<bool, bool needs_value, bool needs_index, typename Value_, typename Index_>
-    Index_ sparse(Index_ idx, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
+    Index_ sparse(Index_, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer) const {
         // None of the operations will return zero if one entry is zero and the other entry is non-zero...
         // except for equality, but then, the sparse() method would never even be used.
         return delayed_binary_isometric_sparse_operation<false, needs_value, needs_index>(
-            idx, 
             left, 
             right, 
             value_buffer, 
             index_buffer, 
             [](Value_& l, Value_ r) { delayed_compare_run<op_>(l, r); }
         );
     }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #ifndef TATAMI_BINARY_HELPER_UTILS_H
 #define TATAMI_BINARY_HELPER_UTILS_H
 
 namespace tatami {
 
 template<bool must_have_both, bool needs_value, bool needs_index, typename Value_, typename Index_, class Function_>
-Index_ delayed_binary_isometric_sparse_operation(Index_ idx, const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer, Function_ fun) {
+Index_ delayed_binary_isometric_sparse_operation(const SparseRange<Value_, Index_>& left, const SparseRange<Value_, Index_>& right, Value_* value_buffer, Index_* index_buffer, Function_ fun) {
     Index_ lcount = 0, rcount = 0, output = 0;
 
     auto advance_left = [&]() -> void {
         if constexpr(needs_value) {
             value_buffer[output] = left.value[lcount];
             fun(value_buffer[output], 0);
         }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -491,19 +491,19 @@
     protected:
         const DelayedBind* parent;
         std::vector<std::unique_ptr<Extractor<selection_, sparse_, Value_, Index_> > > workspaces;
         typename std::conditional<selection_ == DimensionSelectionType::INDEX, std::vector<Index_>, bool>::type indices;
         size_t last_segment = 0;
 
     private:
-        static size_t choose_segment_raw(size_t i, const std::vector<Index_>& cumulative) {
+        static size_t choose_segment_raw(Index_ i, const std::vector<Index_>& cumulative) {
             return std::upper_bound(cumulative.begin(), cumulative.end(), i) - cumulative.begin() - 1;
         }
 
-        static void choose_segment(size_t i, size_t& last_segment, const std::vector<Index_>& cumulative) {
+        static void choose_segment(Index_ i, size_t& last_segment, const std::vector<Index_>& cumulative) {
             if (cumulative[last_segment] > i) {
                 if (last_segment && cumulative[last_segment - 1] <= i) {
                     --last_segment;
                 } else {
                     last_segment = choose_segment_raw(i, cumulative);
                 }
             } else if (cumulative[last_segment + 1] <= i) {
@@ -513,15 +513,15 @@
                     last_segment = choose_segment_raw(i, cumulative);
                 }
             }
             return;
         }
 
     protected:
-        size_t choose_segment(size_t i) {
+        size_t choose_segment(Index_ i) {
             choose_segment(i, last_segment, parent->cumulative);
             return last_segment;
         }
 
     public:
         const Index_* index_start() const {
             if (workspaces.empty()) {
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         std::vector<size_t> cached;
 
     protected:
         StoredPointer primary_start(Index_ i, Index_ start) {
             bool do_cache = !cached.empty();
             if (do_cache) {
                 auto val = cached[i];
-                if (val != -1) {
+                if (val != static_cast<size_t>(-1)) {
                     return val;
                 }
             }
 
             auto outstart = this->parent->indptrs[i];
             if (start) { // Jumping ahead if non-zero.
                 auto iIt = this->parent->indices.begin() + outstart;
@@ -263,15 +263,15 @@
 
             auto iIt = this->parent->indices.begin() + this->parent->indptrs[i];
             auto eIt = this->parent->indices.begin() + this->parent->indptrs[i + 1]; 
 
             if (subset[0]) { // Only jumping ahead if the start is non-zero.
                 bool do_cache = !cached.empty();
                 if (do_cache) {
-                    if (cached[i] != -1) { // retrieving the jump from cache, if we came here before.
+                    if (cached[i] != static_cast<size_t>(-1)) { // retrieving the jump from cache, if we came here before.
                         iIt += cached[i];
                     } else {
                         auto iIt2 = std::lower_bound(iIt, eIt, subset[0]);
                         cached[i] = iIt2 - iIt;
                         iIt = iIt2;
                     }
                 } else {
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 
     // What was the last requested index on the secondary dimension?
     StoredIndex_ last_request = 0;
 
 public:
     SparseSecondaryExtractorCore() = default;
 
-    SparseSecondaryExtractorCore(StoredIndex_ mi, Index_ length) : max_index(mi), current_indices(length), current_indptrs(length) {}
+    SparseSecondaryExtractorCore(StoredIndex_ mi, Index_ length) : current_indptrs(length), current_indices(length), max_index(mi) {}
 
 private:
     template<class IndexStorage_, class PointerStorage_>
     void reset_to_lower_bound(Index_ index_primary, Index_ primary, const IndexStorage_& all_indices, const PointerStorage_& indptrs) {
         const auto& indices = sparse_utils::get_indices<PointerStorage_>(all_indices, primary);
         auto limit = sparse_utils::get_upper_limit(indices, indptrs, primary);
 
         const auto& curptr = current_indptrs[index_primary];
         auto raw_ptr = CustomPointerModifier_::get(curptr);
 
         auto& curdex = current_indices[index_primary];
-        if (raw_ptr != limit) {
+        if (static_cast<decltype(limit)>(raw_ptr) != limit) {
             curdex = indices[raw_ptr];
         } else {
             curdex = max_index;
         }
     }
 
 private:
@@ -99,15 +99,15 @@
         auto limit = sparse_utils::get_upper_limit(indices, indptrs, primary);
 
         // Having a peek at the index of the next non-zero element; maybe we're
         // lucky enough that the requested index is below this, as would be the
         // case for consecutive or near-consecutive accesses.
         CustomPointerModifier_::increment(curptr, indices, limit);
         auto raw_ptr = CustomPointerModifier_::get(curptr);
-        if (raw_ptr == limit) {
+        if (static_cast<decltype(limit)>(raw_ptr) == limit) {
             curdex = max_index;
             skip(primary);
             return;
         }
 
         curdex = indices[raw_ptr];
         if (curdex > secondary) {
@@ -121,15 +121,15 @@
         }
 
         // Otherwise we need to search indices above the existing position.
         // We do a quick increment to cut down the search space; don't
         // need to pay the cost of using increment() here, as the lower
         // bound search is going to be faster than any increment.
         ++raw_ptr;
-        auto next_ptr = std::lower_bound(indices.begin() + raw_ptr, indices.begin() + limit, secondary) - indices.begin();
+        decltype(limit) next_ptr = std::lower_bound(indices.begin() + raw_ptr, indices.begin() + limit, secondary) - indices.begin();
         CustomPointerModifier_::set(curptr, next_ptr);
 
         if (next_ptr == limit) {
             curdex = max_index;
             skip(primary);
             return;
         }
@@ -202,15 +202,15 @@
         auto& curdex = current_indices[index_primary];
         curdex = decrement_fail;
         auto& curptr = current_indptrs[index_primary];
 
         // Can't decrement anymore, in which case we quit. 
         auto lower_limit = sparse_utils::get_lower_limit(indptrs, primary);
         auto raw_ptr = CustomPointerModifier_::get(curptr);
-        if (raw_ptr == lower_limit) {
+        if (static_cast<decltype(lower_limit)>(raw_ptr) == lower_limit) {
             skip(primary);
             return;
         }
 
         const auto& indices = sparse_utils::get_indices<PointerStorage_>(all_indices, primary);
 
         // Having a peek at the index of the next non-zero element and seeing
@@ -222,41 +222,41 @@
             curdex = candidate;
             skip(primary);
             return;
         }
 
         if (candidate == secondary) {
             CustomPointerModifier_::decrement(curptr, indices, lower_limit);
-            if (raw_ptr != lower_limit) {
+            if (static_cast<decltype(lower_limit)>(raw_ptr) != lower_limit) {
                 curdex = indices[raw_ptr - 1]; // cheap decrement to inspect the next-lowest element.
             }
             store(primary, curptr);
             return;
         }
 
         // Otherwise, searching indices below the current position. We need to
         // increment to get back to the current position, as it is still possible
         // that the next position is at 'raw_ptr - 1'.
         ++raw_ptr;
-        auto next_ptr = std::lower_bound(indices.begin() + lower_limit, indices.begin() + raw_ptr, secondary) - indices.begin();
+        decltype(raw_ptr) next_ptr = std::lower_bound(indices.begin() + lower_limit, indices.begin() + raw_ptr, secondary) - indices.begin();
         CustomPointerModifier_::set(curptr, next_ptr);
         if (next_ptr == raw_ptr) {
             skip(primary);
             return;
         }
 
         if (indices[next_ptr] == secondary) {
-            if (next_ptr != lower_limit) {
+            if (static_cast<decltype(lower_limit)>(next_ptr) != lower_limit) {
                 curdex = indices[next_ptr - 1]; // cheap decrement to inspect the next-lowest element.
             }
             store(primary, curptr);
             return;
         }
 
-        if (next_ptr != lower_limit) {
+        if (static_cast<decltype(lower_limit)>(next_ptr) != lower_limit) {
             curdex = indices[next_ptr - 1]; // cheap decrement to inspect the next-lowest element.
         }
         skip(primary);
         return;
     }
 
     template<class IndexStorage_, class PointerStorage_, class StoreFunction_, class SkipFunction_>
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     const IndexStorage_& indices, 
     const PointerStorage_& indptrs, 
     std::vector<std::pair<size_t, size_t> >& cached) 
 {
     bool do_cache = !cached.empty();
     if (do_cache) {
         auto val = cached[i];
-        if (val.first != -1) {
+        if (val.first != static_cast<size_t>(-1)) {
             return val;
         }
     }
 
     auto iIt = indices.begin() + sparse_utils::get_lower_limit(indptrs, i);
     auto eIt = indices.begin() + sparse_utils::get_upper_limit(indices, indptrs, i);
 
@@ -121,15 +121,15 @@
 
     auto iIt = indices.begin() + sparse_utils::get_lower_limit(indptrs, i);
     auto eIt = indices.begin() + sparse_utils::get_upper_limit(indices, indptrs, i);
 
     if (indices[0]) { // Only jumping ahead if the start is non-zero.
         bool do_cache = !cached.empty();
         if (do_cache) {
-            if (cached[i] != -1) { // retrieving the jump from cache, if we came here before.
+            if (cached[i] != static_cast<size_t>(-1)) { // retrieving the jump from cache, if we came here before.
                 iIt += cached[i];
             } else {
                 auto iIt2 = std::lower_bound(iIt, eIt, subset[0]);
                 cached[i] = iIt2 - iIt;
                 iIt = iIt2;
             }
         } else {
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return indptrs[primary + 1];
     }
 }
 
 template<class PointerStorage_, typename Index_>
 auto get_lower_limit(const PointerStorage_& indptrs, Index_ primary) {
     if constexpr(is_fragmented<PointerStorage_>()) {
-        return 0;
+        return static_cast<size_t>(0);
     } else {
         return indptrs[primary];
     }
 }
 
 }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/medians.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/medians.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     auto otherdim = (row_ ? p->ncol() : p->nrow());
 
     if (p->sparse()) {
         Options opt;
         opt.sparse_extract_index = false;
         opt.sparse_ordered_index = false; // we'll be sorting by value anyway.
 
-        parallelize([&](int t, Index_ s, Index_ l) -> void {
+        parallelize([&](int, Index_ s, Index_ l) -> void {
             auto ext = consecutive_extractor<row_, true>(p, s, l, opt);
 
             std::vector<Value_> buffer(otherdim);
             auto vbuffer = buffer.data();
             for (Index_ i = s, e = s + l; i < e; ++i) {
                 auto range = ext->fetch_copy(i, vbuffer, NULL);
                 auto n = range.number;
@@ -102,15 +102,15 @@
                         output[i] = tmp / 2;
                     }
                 }
             }
         }, dim, threads);
 
     } else {
-        parallelize([&](int t, Index_ s, Index_ l) -> void {
+        parallelize([&](int, Index_ s, Index_ l) -> void {
             std::vector<Value_> buffer(otherdim);
             auto ext = consecutive_extractor<row_, false>(p, s, l);
             for (Index_ i = s, e = s + l; i < e; ++i) {
                 ext->fetch_copy(i, buffer.data());
                 output[i] = compute_median<Output_>(buffer.data(), otherdim);
             }
         }, dim, threads);
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/sums.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/sums.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
                 }
             }, dim, threads);
 
         } else {
             parallelize([&](size_t, Index_ s, Index_ l) {
                 auto ext = consecutive_extractor<!row_, true>(p, 0, otherdim, s, l);
                 auto len = ext->block_length;
-                std::vector<Value_> vbuffer(ext->block_length);
-                std::vector<Index_> ibuffer(ext->block_length);
+                std::vector<Value_> vbuffer(len);
+                std::vector<Index_> ibuffer(len);
+
                 for (Index_ i = 0; i < otherdim; ++i) {
                     auto out = ext->fetch(i, vbuffer.data(), ibuffer.data());
                     for (Index_ j = 0; j < out.number; ++j) {
                         output[out.index[j]] += out.value[j];
                     }
                 }
             }, dim, threads);
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/utils.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,21 @@
  * @tparam Index_ Integer type for the number of tasks.
  *
  * @param fun Function that executes a contiguous range of tasks.
  * @param tasks Number of tasks.
  * @param threads Number of threads.
  */
 template<bool parallel_ = true, class Function_, typename Index_>
-void parallelize(Function_ fun, Index_ tasks, size_t threads) {
+void parallelize(Function_ fun, Index_ tasks, size_t
 #if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
+    threads // wrap here to avoid used variable warnings (which are in turn converted to errors).
+#endif
+) {
+#if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
+
     if constexpr(parallel_) {
 
         if (threads > 1) {
 #ifndef TATAMI_CUSTOM_PARALLEL
             Index_ worker_size = (tasks / threads) + (tasks % threads > 0); // Ceiling of an integer division.
             threads = (tasks / worker_size) + (tasks % worker_size > 0); // Set the actual number of required threads.
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/stats/variances.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/stats/variances.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 std::pair<Output_, Output_> compute_direct(const SparseRange<Value_, Index_>& range, size_t n) {
     if (n < 1) {
         return both_NaN<Output_>();
     }
 
     Output_ mean = std::accumulate(range.value, range.value + range.number, static_cast<Output_>(0))/n;
     Output_ var = 0;
-    for (size_t j = 0; j < range.number; ++j) {
+    for (Index_ j = 0; j < range.number; ++j) {
         var += (range.value[j] - mean) * (range.value[j] - mean);
     }
     var += mean * mean * (n - range.number);
 
     return std::make_pair(mean, finish_variance_direct(var, n));
 }
 
@@ -150,15 +150,15 @@
  * Note that this choice has no effect on the computed means or variances, besides some differences due to numeric imprecision.
  * @param subtract Value to subtract from each sparse index before using it to index into `means`, `vars` and `nonzeros`.
  * This is only relevant if `means` and friends do not hold statistics for all target vectors, but just a contiguous block, e.g., during parallelization.
  */
 template<typename Value_, typename Index_, typename Output_, typename Nonzero_>
 void compute_running(const SparseRange<Value_, Index_>& range, Output_* means, Output_* vars, Nonzero_* nonzeros, int& count, bool skip_zeros = true, Index_ subtract = 0) {
     ++count;
-    for (size_t j = 0; j < range.number; ++j) {
+    for (Index_ j = 0; j < range.number; ++j) {
         if (!skip_zeros || range.value[j]) { 
             auto ri = range.index[j] - subtract;
             auto& curM = means[ri];
             auto& curS = vars[ri];
             auto& curNZ = nonzeros[ri];
             ++curNZ;
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,16 @@
  * @tparam Value_ Type of matrix value.
  * @tparam Index_ Type of index value.
  * @tparam IndexStorage_ Vector containing the subset indices.
  */
 template<int margin_, typename Value_, typename Index_, class IndexStorage_>
 class DelayedSubset : public Matrix<Value_, Index_> {
 private:
-    typedef typename std::remove_const<typename std::remove_reference<decltype(std::declval<IndexStorage_>()[0])>::type>::type storage_type;
-
     static void finish_assembly(
-        const std::vector<std::pair<storage_type, Index_> >& collected,
+        const std::vector<std::pair<Index_, Index_> >& collected,
         const IndexStorage_& indices, 
         std::vector<Index_>& reverse_mapping,
         std::vector<Index_>& unique_and_sorted,
         Index_ mapping_dim,
         std::vector<std::pair<Index_, Index_> >& mapping_duplicates,
         std::vector<Index_>& mapping_duplicates_pool
     ) {
@@ -64,15 +62,15 @@
 public:
     /**
      * @param p Pointer to the underlying (pre-subset) matrix.
      * @param idx Vector of 0-based indices to use for subsetting on the rows (if `margin_ = 0`) or columns (if `margin_ = 1`).
      * These may be duplicated and/or unsorted.
      */
     DelayedSubset(std::shared_ptr<const Matrix<Value_, Index_> > p, IndexStorage_ idx) : mat(std::move(p)), indices(std::move(idx)) {
-        std::vector<std::pair<storage_type, Index_> > collected;
+        std::vector<std::pair<Index_, Index_> > collected;
         collected.reserve(indices.size());
         for (Index_ i = 0, end = indices.size(); i < end; ++i) {
             collected.emplace_back(indices[i], i);
         }
         std::sort(collected.begin(), collected.end());
 
         finish_assembly(
@@ -87,15 +85,15 @@
 
         return;
     }
 
     /**
      * @cond
      */
-    DelayedSubset(std::shared_ptr<const Matrix<Value_, Index_> > p, const std::vector<std::pair<storage_type, Index_> >& collected, IndexStorage_ idx) : 
+    DelayedSubset(std::shared_ptr<const Matrix<Value_, Index_> > p, const std::vector<std::pair<Index_, Index_> >& collected, IndexStorage_ idx) : 
         mat(std::move(p)), indices(std::move(idx)) 
     {
         finish_assembly(
             collected,
             indices, 
             reverse_mapping, 
             unique_and_sorted,
@@ -384,15 +382,15 @@
 
     /***************************************************
      ************ Block parallel extraction ************
      ***************************************************/
 private:
     void transplant_indices(
         std::vector<Index_>& local, 
-        std::vector<std::pair<storage_type, Index_> >& collected, 
+        std::vector<std::pair<Index_, Index_> >& collected, 
         std::vector<Index_>& reverse_mapping) 
     const {
         std::sort(collected.begin(), collected.end());
 
         reverse_mapping.resize(collected.size());
         local.reserve(collected.size());
 
@@ -402,15 +400,15 @@
             }
             reverse_mapping[current.second] = local.size() - 1;
         }
     }
 
     void transplant_indices(
         std::vector<Index_>& local,
-        std::vector<std::pair<storage_type, Index_> >& collected, 
+        std::vector<std::pair<Index_, Index_> >& collected, 
         std::vector<std::pair<Index_, Index_> >& dups,
         std::vector<Index_>& pool) 
     const {
         std::sort(collected.begin(), collected.end());
 
         Index_ mapping_dim = margin_ == 0 ? mat->nrow() : mat->ncol();
         dups.resize(mapping_dim);
@@ -432,15 +430,15 @@
     template<bool sparse_>
     struct BlockParallelExtractor : public ParallelExtractor<DimensionSelectionType::BLOCK, sparse_> {
         BlockParallelExtractor(const DelayedSubset* parent, const Options& opt, Index_ bs, Index_ bl) {
             this->block_start = bs;
             this->block_length = bl;
 
             const auto& parent_indices = parent->indices;
-            std::vector<std::pair<storage_type, Index_> > collected;
+            std::vector<std::pair<Index_, Index_> > collected;
             collected.reserve(bl);
 
             auto block_end = bs + bl;
             for (Index_ i = bs; i < block_end; ++i) {
                 if constexpr(sparse_) {
                     collected.emplace_back(parent_indices[i], i);
                 } else {
@@ -499,15 +497,15 @@
     struct IndexParallelExtractor : public ParallelExtractor<DimensionSelectionType::INDEX, sparse_> {
         IndexParallelExtractor(const DelayedSubset* parent, const Options& opt, std::vector<Index_> idx) {
             Index_ il = idx.size();
             this->index_length = il;
             indices = std::move(idx);
 
             const auto& parent_indices = parent->indices;
-            std::vector<std::pair<storage_type, Index_> > collected;
+            std::vector<std::pair<Index_, Index_> > collected;
             collected.reserve(il);
             for (Index_ i = 0; i < il; ++i) {
                 if constexpr(sparse_) {
                     collected.emplace_back(parent_indices[indices[i]], indices[i]);
                 } else {
                     collected.emplace_back(parent_indices[indices[i]], i);
                 }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,16 @@
  * @tparam Value_ Type of matrix value.
  * @tparam Index_ Integer type of index value.
  * @tparam IndexStorage_ Vector containing the subset indices.
  */
 template<int margin_, typename Value_, typename Index_, class IndexStorage_>
 class DelayedSubsetUnique : public Matrix<Value_, Index_> {
 private:
-    typedef typename std::remove_const<typename std::remove_reference<decltype(std::declval<IndexStorage_>()[0])>::type>::type storage_type;
-
     static void finish_assembly(
-        const std::vector<std::pair<storage_type, Index_> >& collected,
+        const std::vector<std::pair<Index_, Index_> >& collected,
         const IndexStorage_& indices, 
         std::vector<Index_>& reverse_mapping,
         std::vector<Index_>& sorted,
         Index_ mapping_dim,
         std::vector<Index_>& mapping_single
     ) {
         sorted.reserve(indices.size());
@@ -57,15 +55,15 @@
     /**
      * @param p Pointer to the underlying (pre-subset) matrix.
      * @param idx Vector of 0-based indices to use for subsetting on the rows (if `margin_ = 0`) or columns (if `margin_ = 1`).
      * This should be unique, but may be unsorted.
      * @param check Whether to check `idx` for unique values.
      */
     DelayedSubsetUnique(std::shared_ptr<const Matrix<Value_, Index_> > p, IndexStorage_ idx, bool check = true) : mat(std::move(p)), indices(std::move(idx)) {
-        std::vector<std::pair<storage_type, Index_> > collected;
+        std::vector<std::pair<Index_, Index_> > collected;
         collected.reserve(indices.size());
         for (Index_ i = 0, end = indices.size(); i < end; ++i) {
             collected.emplace_back(indices[i], i);
         }
         std::sort(collected.begin(), collected.end());
 
         if (check) {
@@ -88,15 +86,15 @@
             mapping_single
         );
     }
 
     /**
      * @cond
      */
-    DelayedSubsetUnique(std::shared_ptr<const Matrix<Value_, Index_> > p, const std::vector<std::pair<storage_type, Index_> >& collected, IndexStorage_ idx) : 
+    DelayedSubsetUnique(std::shared_ptr<const Matrix<Value_, Index_> > p, const std::vector<std::pair<Index_, Index_> >& collected, IndexStorage_ idx) : 
         mat(std::move(p)), indices(std::move(idx)) 
     {
         finish_assembly(
             collected,
             indices, 
             reverse_mapping, 
             sorted,
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,14 @@
  * @param idx Instance of the index vector.
  *
  * @return A pointer to a `DelayedSubset` instance.
  */
 template<int margin_, typename Value_, typename Index_, class IndexStorage_>
 std::shared_ptr<Matrix<Value_, Index_> > make_DelayedSubset(std::shared_ptr<const Matrix<Value_, Index_> > p, IndexStorage_ idx) {
     typedef typename std::remove_reference<IndexStorage_>::type PureIndexStorage_;
-    typedef typename std::remove_const<typename std::remove_reference<decltype(std::declval<IndexStorage_>()[0])>::type>::type storage_type;
 
     bool is_unsorted = false;
     for (Index_ i = 0, end = idx.size(); i < end; ++i) {
         if (i) {
             if (idx[i] < idx[i-1]) {
                 is_unsorted = true;
                 break;
@@ -66,15 +65,15 @@
         } else {
             return std::shared_ptr<Matrix<Value_, Index_> >(
                 new DelayedSubsetSorted<margin_, Value_, Index_, PureIndexStorage_>(std::move(p), std::move(idx), false)
             );
         }
     }
 
-    std::vector<std::pair<storage_type, Index_> > collected;
+    std::vector<std::pair<Index_, Index_> > collected;
     collected.reserve(idx.size());
     for (Index_ i = 0, end = idx.size(); i < end; ++i) {
         collected.emplace_back(idx[i], i);
     }
     std::sort(collected.begin(), collected.end());
 
     bool has_duplicates = false;
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/subset/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/subset/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/tatami.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/tatami.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 #define TATAMI_TATAMI_HPP
 
 #include "dense/DenseMatrix.hpp"
 
 #include "sparse/CompressedSparseMatrix.hpp"
 #include "sparse/SemiCompressedSparseMatrix.hpp"
 #include "sparse/FragmentedSparseMatrix.hpp"
+#include "sparse/convert_to_compressed_sparse.hpp"
+#include "sparse/convert_to_fragmented_sparse.hpp"
 
 #include "isometric/unary/DelayedUnaryIsometricOp.hpp"
 #include "isometric/binary/DelayedBinaryIsometricOp.hpp"
 
 #include "other/DelayedBind.hpp"
 #include "other/DelayedCast.hpp"
 #include "other/DelayedTranspose.hpp"
 
 #include "subset/DelayedSubsetBlock.hpp"
 #include "subset/make_DelayedSubset.hpp"
 
 #include "utils/compress_sparse_triplets.hpp"
-#include "utils/convert_to_sparse.hpp"
 #include "utils/convert_to_dense.hpp"
 #include "utils/wrap_shared_ptr.hpp"
 #include "utils/ArrayView.hpp"
 #include "utils/SomeNumericArray.hpp"
 #include "utils/bind_intersection.hpp"
 #include "utils/Oracles.hpp"
 #include "utils/process_consecutive_indices.hpp"
 
+#include "utils/convert_to_sparse.hpp"
+
 #include "stats/sums.hpp"
 #include "stats/variances.hpp"
 #include "stats/medians.hpp"
 
 #define TATAMI_VERSION_MAJOR 1
 #define TATAMI_VERSION_MINOR 0
 #define TATAMI_VERSION_PATCH 0
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -134,27 +134,28 @@
     /**
      * @param x Pointer to an existing array of `double`s.
      * @param n Length of the array pointed to by `x`.
      */
     SomeNumericArray(const double* x, size_t n) : f64(x), len(n), type(F64) {}
 
 private:
-    Type type;
-    size_t len;
-
     const int8_t* i8 = NULL;
     const uint8_t* u8 = NULL;
     const int16_t* i16 = NULL;
     const uint16_t* u16 = NULL;
     const int32_t* i32 = NULL;
     const uint32_t* u32 = NULL;
     const int64_t* i64 = NULL;
     const uint64_t* u64 = NULL;
     const float* f32 = NULL;
     const double* f64 = NULL;
+
+    size_t len;
+    Type type;
+
 public:
     /**
      * @param i Positional index on the array.
      * @return Value of the `i`-th element as a `T`.
      */
     T operator[](size_t i) const {
         switch (type) {
@@ -175,14 +176,15 @@
             case U64:
                 return u64[i];
             case F32:
                 return f32[i];
             case F64:
                 return f64[i];
         }
+        return 0; // shouldn't reach here, but whatever.
     }
 
     /**
      * @return Length of the array, in terms of the number of elements of the specified type.
      */
     size_t size() const {
         return len;
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     };
 
     // Finding the intersection of all names and creating a mapping.
     const auto& first_ptr = inputs[0];
     auto first_ids = ids[0];
     std::unordered_set<int> in_use(first_ids, first_ids + otherlen(first_ptr));
 
-    for (int i = 1; i < n; ++i) {
+    for (size_t i = 1; i < n; ++i) {
         std::vector<int> intersection;
         intersection.reserve(in_use.size());
 
         const auto& current = inputs[i];
         size_t current_other = otherlen(current);
         auto current_ids = ids[i];
 
@@ -73,24 +73,24 @@
 
         in_use = std::unordered_set<int>(intersection.begin(), intersection.end());
     }
 
     std::unordered_map<int, int> mapping;
     std::vector<int> as_vec(in_use.begin(), in_use.end());
     std::sort(as_vec.begin(), as_vec.end());
-    for (int s = 0; s < as_vec.size(); ++s) {
+    for (size_t s = 0, send = as_vec.size(); s < send; ++s) {
         mapping[as_vec[s]] = s;
     }
 
     // Applying the mapping. 
     std::vector<std::shared_ptr<Matrix> > collected;
     collected.reserve(inputs.size());
     std::vector<size_t> indices;
 
-    for (int i = 0; i < n; ++i) {
+    for (size_t i = 0; i < n; ++i) {
         const auto& current = inputs[i];
         size_t current_other = otherlen(current);
         auto current_ids = ids[i];
 
         std::vector<size_t> reorder(mapping.size());
         for (size_t j = 0; j < current_other; ++j) {
             auto it = mapping.find(current_ids[j]);
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             compress_triplets::order(order_status, indices, cols, rows);
         }
 
         // Reordering values in place. This (i) saves memory, and (ii) allows
         // us to work with classes U and V that may not have well-defined copy
         // constructors (e.g., if they refer to external memory).
         for (size_t i = 0; i < indices.size(); ++i) {
-            if (indices[i] == -1) {
+            if (indices[i] == static_cast<size_t>(-1)) {
                 continue;
             }
 
             size_t current = i, replacement = indices[i];
             indices[i] = -1;
 
             while (replacement != i) {
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -16,39 +16,37 @@
  */
 
 namespace tatami {
 
 /**
  * @tparam row_ Whether to return a row-major matrix.
  * @tparam StoredValue_ Type of data values to be stored in the output.
- * @tparam Matrix_ Input matrix class, most typically a `tatami::Matrix`.
+ * @tparam InputValue_ Type of data values in the input.
+ * @tparam InputIndex_ Integer type for the indices in the input.
  *
  * @param incoming Pointer to a `tatami::Matrix`.
  * @param[out] store Pointer to an array of length equal to the product of the dimensions of `incoming`.
  * On output, this is filled with values from `incoming` in row- or column-major format depending on `row_`.
  * @param threads Number of threads to use.
  */
-template <bool row_, typename StoredValue_, class Matrix_>
-void convert_to_dense(const Matrix_* incoming, StoredValue_* store, int threads = 1) {
-    typedef typename Matrix_::index_type Index_;
-    typedef typename Matrix_::value_type Value_;
-
-    size_t NR = incoming->nrow();
-    size_t NC = incoming->ncol();
-    size_t primary = (row_ ? NR : NC);
-    size_t secondary = (row_ ? NC : NR);
+template <bool row_, typename StoredValue_, typename InputValue_, typename InputIndex_>
+void convert_to_dense(const Matrix<InputValue_, InputIndex_>* incoming, StoredValue_* store, int threads = 1) {
+    InputIndex_ NR = incoming->nrow();
+    InputIndex_ NC = incoming->ncol();
+    InputIndex_ primary = (row_ ? NR : NC);
+    InputIndex_ secondary = (row_ ? NC : NR);
 
     if (row_ == incoming->prefer_rows()) {
-        constexpr bool same_type = std::is_same<Value_, StoredValue_>::value;
-        parallelize([&](size_t, Index_ start, Index_ length) -> void {
-            std::vector<Value_> temp(same_type ? 0 : secondary);
+        constexpr bool same_type = std::is_same<InputValue_, StoredValue_>::value;
+        parallelize([&](size_t, InputIndex_ start, InputIndex_ length) -> void {
+            std::vector<InputValue_> temp(same_type ? 0 : secondary);
             auto store_copy = store + start * secondary;
-            auto wrk = consecutive_extractor<row_, false, Value_, Index_>(incoming, start, length);
+            auto wrk = consecutive_extractor<row_, false>(incoming, start, length);
 
-            for (Index_ p = start, e = start + length; p < e; ++p, store_copy += secondary) {
+            for (InputIndex_ p = start, e = start + length; p < e; ++p, store_copy += secondary) {
                 if constexpr(same_type) {
                     wrk->fetch_copy(p, store_copy);
                 } else {
                     auto ptr = wrk->fetch(p, temp.data());
                     std::copy(ptr, ptr + secondary, store_copy);
                 }
             }
@@ -56,54 +54,56 @@
 
     } else {
         // We iterate on the incoming matrix's preferred dimension, under the
         // assumption that it may be arbitrarily costly to extract in the
         // non-preferred dim; it is thus cheaper to do cache-unfriendly inserts
         // into the output buffers. 
 
-        parallelize([&](size_t, Index_ start, Index_ length) -> void {
-            auto wrk = consecutive_extractor<!row_, false, Value_, Index_>(incoming, 0, secondary, start, length);
+        parallelize([&](size_t, InputIndex_ start, InputIndex_ length) -> void {
+            auto wrk = consecutive_extractor<!row_, false>(incoming, 0, secondary, start, length);
             auto len = wrk->block_length;
-            std::vector<Value_> temp(len);
+            std::vector<InputValue_> temp(len);
             auto store_copy = store + start * secondary;
 
-            for (Index_ s = 0; s < secondary; ++s, ++store_copy) {
+            for (InputIndex_ s = 0; s < secondary; ++s, ++store_copy) {
                 auto ptr = wrk->fetch(s, temp.data());
                 auto bptr = store_copy;
-                for (size_t p = 0; p < len; ++p, bptr += secondary) {
+                for (InputIndex_ p = 0; p < len; ++p, bptr += secondary) {
                     *bptr = ptr[p]; 
                 }
             }
         }, primary, threads);
     }
 
     return;
 }
 
 /**
  * @tparam row Whether to return a row-major matrix.
  * @tparam Value_ Type of data values in the output interface.
  * @tparam Index Integer type for the indices in the output interface.
  * @tparam StoredValue_ Type of data values to be stored in the output.
- * @tparam Matrix_ Input matrix class, most typically a `tatami::Matrix`.
+ * @tparam InputValue_ Type of data values in the input.
+ * @tparam InputIndex_ Integer type for the indices in the input.
  *
  * @param incoming Pointer to a `tatami::Matrix`.
  * @param threads Number of threads to use.
  *
  * @return A pointer to a new `tatami::DenseMatrix` with the same dimensions and type as the matrix referenced by `incoming`.
  * If `row = true`, the matrix is row-major, otherwise it is column-major.
  */
 template <
     bool row_, 
     typename Value_ = double, 
     typename Index = int, 
     typename StoredValue_ = Value_, 
-    class Matrix_
+    typename InputValue_,
+    typename InputIndex_
 >
-inline std::shared_ptr<Matrix<Value_, Index> > convert_to_dense(const Matrix_* incoming, int threads = 1) {
+inline std::shared_ptr<Matrix<Value_, Index> > convert_to_dense(const Matrix<InputValue_, InputIndex_>* incoming, int threads = 1) {
     size_t NR = incoming->nrow();
     size_t NC = incoming->ncol();
     std::vector<StoredValue_> buffer(NR * NC);
     convert_to_dense<row_>(incoming, buffer.data(), threads);
     return std::shared_ptr<Matrix<Value_, Index> >(new DenseMatrix<row_, Value_, Index, decltype(buffer)>(NR, NC, std::move(buffer)));
 }
 
@@ -122,23 +122,24 @@
  *
  * @return A pointer to a new `tatami::DenseMatrix` with the same dimensions and type as the matrix referenced by `incoming`.
  */
 template <
     typename Value_ = double,
     typename Index_ = int,
     typename StoredValue_ = Value_,
-    class Matrix_
+    typename InputValue_,
+    typename InputIndex_
 >
-std::shared_ptr<Matrix<Value_, Index_> > convert_to_dense(const Matrix_* incoming, int order, int threads = 1) {
+std::shared_ptr<Matrix<Value_, Index_> > convert_to_dense(const Matrix<InputValue_, InputIndex_>* incoming, int order, int threads = 1) {
     if (order < 0) {
         order = static_cast<int>(!incoming->prefer_rows()); 
     }
     if (order == 0) {
-        return convert_to_dense<true, Value_, Index_, StoredValue_, Matrix_>(incoming, threads);
+        return convert_to_dense<true, Value_, Index_, StoredValue_>(incoming, threads);
     } else {
-        return convert_to_dense<false, Value_, Index_, StoredValue_, Matrix_>(incoming, threads);
+        return convert_to_dense<false, Value_, Index_, StoredValue_>(incoming, threads);
     }
 }
 
 }
 
 #endif
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/include/tatami_test/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami/include/tatami_test/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/CMakeLists.txt` & `mattress-0.0.4/src/mattress/extern/tatami/tests/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,26 +34,27 @@
     src/isometric/binary/compare_helpers.cpp
     src/isometric/binary/boolean_helpers.cpp
 
     src/sparse/CompressedSparseMatrix.cpp
     src/sparse/FragmentedSparseMatrix.cpp
     src/sparse/SemiCompressedSparseMatrix.cpp
     src/sparse/SparseSecondaryExtractorCore.cpp
+    src/sparse/convert_to_compressed_sparse.cpp
+    src/sparse/convert_to_fragmented_sparse.cpp
 
     src/stats/sums.cpp
     src/stats/variances.cpp
     src/stats/medians.cpp
     src/stats/ranges.cpp
     src/stats/parallelize.cpp
 
     src/utils/wrap_shared_ptr.cpp
     src/utils/SomeNumericArray.cpp
     src/utils/ArrayView.cpp
     src/utils/convert_to_dense.cpp
-    src/utils/convert_to_sparse.cpp
     src/utils/bind_intersection.cpp
     src/utils/compress_sparse_triplets.cpp
     src/utils/Oracles.cpp
     src/utils/process_consecutive_indices.cpp
 )
 
 target_link_libraries(
@@ -87,14 +88,17 @@
     target_link_libraries(libtest OpenMP::OpenMP_CXX)
     target_link_libraries(cuspartest OpenMP::OpenMP_CXX)
 endif()
 
 target_compile_definitions(libtest PRIVATE DEBUG=1)
 target_compile_definitions(cuspartest PRIVATE CUSTOM_PARALLEL_TEST=1)
 
+target_compile_options(libtest PRIVATE -Wall -Wextra -Wpedantic -Werror)
+target_compile_options(cuspartest PRIVATE -Wall -Wextra -Wpedantic -Werror)
+
 set(CODE_COVERAGE OFF CACHE BOOL "Enable coverage testing")
 if(CODE_COVERAGE AND CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
     target_compile_options(libtest PRIVATE -O0 -g --coverage)
     target_link_options(libtest PRIVATE --coverage)
 endif()
 
 # Making the tests discoverable.
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/README.md` & `mattress-0.0.4/src/mattress/extern/tatami/tests/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     EXPECT_EQ(mat.prefer_rows_proportion(), 0);
 
     EXPECT_EQ(mat.nrow(), 10);
     EXPECT_EQ(mat.ncol(), 20);
 
     {
         auto wrk = mat.dense_column();
-        for (size_t i = 0; i < mat.ncol(); ++i) {
+        for (size_t i = 0, end = mat.ncol(); i < end; ++i) {
             auto start = contents.begin() + i * mat.nrow();
             std::vector<double> expected(start, start + mat.nrow());
             EXPECT_EQ(wrk->fetch(i), expected);
         }
     }
 
     {
         auto wrk = mat.dense_row();
-        for (size_t i = 0; i < mat.nrow(); ++i) {
+        for (size_t i = 0, end = mat.nrow(); i < end; ++i) {
             std::vector<double> expected(mat.ncol());
-            for (size_t j = 0; j < mat.ncol(); ++j) {
+            for (size_t j = 0, jend = mat.ncol(); j < jend; ++j) {
                 expected[j] = contents[j * mat.nrow() + i];
             }
             EXPECT_EQ(wrk->fetch(i), expected);
         }
     }
 
     EXPECT_FALSE(mat.uses_oracle(true));
@@ -136,15 +136,15 @@
     auto param = GetParam(); 
     bool FORWARD = std::get<0>(param);
     size_t JUMP = std::get<1>(param);
     tatami_test::test_simple_row_access(dense_row.get(), dense_column.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(dense_column.get(), dense_row.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DenseMatrix,
     DenseFullAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4) // jump, to test the workspace's memory.
     )
 );
@@ -180,15 +180,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
 
     tatami_test::test_sliced_row_access(dense_column.get(), dense_row.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_row_access(dense_row.get(), dense_column.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DenseMatrix,
     DenseSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.45 }),
@@ -229,15 +229,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
 
     tatami_test::test_indexed_row_access(dense_column.get(), dense_row.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_row_access(dense_row.get(), dense_column.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DenseMatrix,
     DenseIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.05 }),
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_column_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithAdditionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -118,15 +118,15 @@
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithAdditionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.35 }),
@@ -157,15 +157,15 @@
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithAdditionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 6 }),
@@ -216,15 +216,15 @@
     tatami_test::test_simple_column_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithSubtractionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -248,15 +248,15 @@
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithSubtractionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.541 }), 
@@ -285,15 +285,15 @@
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithSubtractionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 10 }), 
@@ -343,15 +343,15 @@
     tatami_test::test_simple_column_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithMultiplicationFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -373,15 +373,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithMultiplicationBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.35 }),
@@ -409,15 +409,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithMultiplicationIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 11 }),
@@ -469,15 +469,15 @@
     tatami_test::test_simple_column_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithDivisionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -501,15 +501,15 @@
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithDivisionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.541 }), 
@@ -538,15 +538,15 @@
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithDivisionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 7 }),
@@ -603,15 +603,15 @@
     tatami_test::test_simple_column_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithPowerFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -633,15 +633,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithPowerBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.35 }),
@@ -668,15 +668,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithPowerIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 11 }),
@@ -728,15 +728,15 @@
     tatami_test::test_simple_column_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithModuloFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -760,15 +760,15 @@
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithModuloBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.541 }),
@@ -797,15 +797,15 @@
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithModuloIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 7 }),
@@ -858,15 +858,15 @@
     tatami_test::test_simple_column_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithIntegerDivisionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
 );
@@ -890,15 +890,15 @@
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithIntegerDivisionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.541 }),
@@ -927,15 +927,15 @@
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1];
         tatami_test::test_indexed_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(mixed_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithIntegerDivisionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 7 }),
@@ -984,15 +984,15 @@
     tatami_test::test_oracle_column_access(wrapped_right.get(), ref.get(), randomized);
 
     tatami_test::test_oracle_row_access(wrapped_both.get(), ref.get(), randomized);
     tatami_test::test_oracle_row_access(wrapped_left.get(), ref.get(), randomized);
     tatami_test::test_oracle_row_access(wrapped_right.get(), ref.get(), randomized);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BinaryArith,
     BinaryArithOracleTest,
     ::testing::Values(true, false)  // use random or consecutive oracle.
 );
 
 class BinaryArithOracleTest2 : public ::testing::Test, public BinaryArithUtils {};
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         r *= val;
     }
     tatami::DenseRowMatrix<double> ref(nrow, ncol, std::move(refvec));
     quick_test_all(dense_mod.get(), &ref);
     quick_test_all(sparse_mod.get(), &ref);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithScalar,
     ArithCommutativeScalarTest,
     ::testing::Values(5, 0.1, -0.7, 0)
 );
 
 /***********************************
  ********* NON-COMMUTATIVE *********
@@ -322,15 +322,15 @@
     tatami_test::test_simple_column_access<true>(dense_mod.get(), &ref, true, 1);
     tatami_test::test_simple_row_access<true>(dense_mod.get(), &ref, true, 1);
 
     tatami_test::test_simple_column_access<true>(sparse_mod.get(), &ref, true, 1);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), &ref, true, 1);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithScalar,
     ArithNonCommutativeScalarTest,
     ::testing::Combine(
         ::testing::Values(5, 0.1, -0.7, 0),
         ::testing::Values(true, false)
     )
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     tatami_test::test_simple_column_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorAdditionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or by column
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
@@ -126,15 +126,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorAdditionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
@@ -165,15 +165,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorAdditionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
@@ -257,15 +257,15 @@
     tatami_test::test_simple_column_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorSubtractionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -291,15 +291,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorSubtractionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -330,15 +330,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorSubtractionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -408,15 +408,15 @@
     tatami_test::test_simple_column_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorMultiplicationFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
     )
@@ -441,15 +441,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorMultiplicationBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
@@ -480,15 +480,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorMultiplicationIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
@@ -584,15 +584,15 @@
     tatami_test::test_simple_column_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorDivisionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -618,15 +618,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorDivisionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -657,15 +657,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorDivisionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -759,15 +759,15 @@
     tatami_test::test_simple_column_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorPowerFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -793,15 +793,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorPowerBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -832,15 +832,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorPowerIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -931,15 +931,15 @@
     tatami_test::test_simple_column_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorModuloFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -965,15 +965,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorModuloBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -1004,15 +1004,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorModuloIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -1104,15 +1104,15 @@
     tatami_test::test_simple_column_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorIntegerDivisionFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // by row or by column
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -1138,15 +1138,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
         tatami_test::test_sliced_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
         tatami_test::test_sliced_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorIntegerDivisionBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -1177,15 +1177,15 @@
     {
         size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
         tatami_test::test_indexed_row_access<true>(dense_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
         tatami_test::test_indexed_row_access<true>(sparse_mod.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     }
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorIntegerDivisionIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false), // on the right or left
         ::testing::Values(true, false), // iterate forward or back
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -1238,15 +1238,15 @@
     tatami_test::test_oracle_column_access(wrapped_dense_mod.get(), dense_mod.get(), std::get<1>(param));
     tatami_test::test_oracle_column_access(wrapped_sparse_mod.get(), sparse_mod.get(), std::get<1>(param));
 
     tatami_test::test_oracle_row_access(wrapped_dense_mod.get(), dense_mod.get(), std::get<1>(param));
     tatami_test::test_oracle_row_access(wrapped_sparse_mod.get(), sparse_mod.get(), std::get<1>(param));
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorOracleTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or add by column.
         ::testing::Values(true, false)  // use random or consecutive oracle.
     )
 );
@@ -1416,23 +1416,23 @@
     auto copy = simulated;
 
     if (GetParam()) {
         auto op = tatami::make_DelayedDivideVectorHelper<true, 0>(std::move(solo_zero));
         dense_mod = tatami::make_DelayedUnaryIsometricOp(dense, op);
         sparse_mod = tatami::make_DelayedUnaryIsometricOp(sparse, op);
 
-        for (int c = 0; c < ncol; ++c) {
+        for (size_t c = 0; c < ncol; ++c) {
             copy[c] = careful_division(copy[c], 0.0);
         }
     } else {
         auto op = tatami::make_DelayedDivideVectorHelper<true, 1>(std::move(solo_zero));
         dense_mod = tatami::make_DelayedUnaryIsometricOp(dense, op);
         sparse_mod = tatami::make_DelayedUnaryIsometricOp(sparse, op);
 
-        for (int r = 0; r < nrow; ++r) {
+        for (size_t r = 0; r < nrow; ++r) {
             copy[r * ncol] = careful_division(copy[r * ncol], 0.0);
         }
     }
 
     tatami::DenseRowMatrix<double> ref(nrow, ncol, std::move(copy));
 
     EXPECT_FALSE(dense_mod->sparse());
@@ -1483,23 +1483,23 @@
     auto copy = simulated;
 
     if (GetParam()) {
         auto op = tatami::make_DelayedPowerVectorHelper<true, 0>(std::move(solo_zero));
         dense_mod = tatami::make_DelayedUnaryIsometricOp(dense, op);
         sparse_mod = tatami::make_DelayedUnaryIsometricOp(sparse, op);
 
-        for (int c = 0; c < ncol; ++c) {
+        for (size_t c = 0; c < ncol; ++c) {
             copy[c] = std::pow(copy[c], 0.0);
         }
     } else {
         auto op = tatami::make_DelayedPowerVectorHelper<true, 1>(std::move(solo_zero));
         dense_mod = tatami::make_DelayedUnaryIsometricOp(dense, op);
         sparse_mod = tatami::make_DelayedUnaryIsometricOp(sparse, op);
 
-        for (int r = 0; r < nrow; ++r) {
+        for (size_t r = 0; r < nrow; ++r) {
             copy[r * ncol] = std::pow(copy[r * ncol], 0.0);
         }
     }
 
     tatami::DenseRowMatrix<double> ref(nrow, ncol, std::move(copy));
 
     EXPECT_FALSE(dense_mod->sparse());
@@ -1570,12 +1570,12 @@
     tatami_test::test_simple_column_access<true>(dense_mod.get(), &ref, true, 1);
     tatami_test::test_simple_column_access<true>(sparse_mod.get(), &ref, true, 1);
 
     tatami_test::test_simple_row_access<true>(dense_mod.get(), &ref, true, 1);
     tatami_test::test_simple_row_access<true>(sparse_mod.get(), &ref, true, 1);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ArithVector,
     ArithVectorZeroedTest,
     ::testing::Values(true, false) // add by row, or by column
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     }
     tatami::DenseRowMatrix<double> ref(nrow, ncol, std::move(refvec));
 
     quick_test_all(dense_mod.get(), &ref);
     quick_test_all(sparse_mod.get(), &ref);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BooleanScalar,
     BooleanScalarTest,
     ::testing::Values(true, false)
 );
 
 TEST(BooleanNotTest, Basic) {
     size_t nrow = 23, ncol = 41;
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     }
     
     tatami::DenseRowMatrix<double> ref(this->nrow, this->ncol, std::move(refvec));
     quick_test_all(dense_mod.get(), &ref);
     quick_test_all(sparse_mod.get(), &ref);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     BooleanVector,
     BooleanVectorTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or by column
         ::testing::Values(true, false) // check sparse case
     )
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -211,12 +211,12 @@
     }
     tatami::DenseRowMatrix<double> ref(nrow, ncol, std::move(refvec));
 
     quick_test_all(dense_mod.get(), &ref);
     quick_test_all(sparse_mod.get(), &ref);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     CompareScalar,
     CompareScalarTest,
     ::testing::Values(0, -1, 1)
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     }
     
     tatami::DenseRowMatrix<double> ref(this->nrow, this->ncol, std::move(refvec));
     quick_test_all(dense_mod.get(), &ref);
     quick_test_all(sparse_mod.get(), &ref);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     CompareVector,
     CompareVectorTest,
     ::testing::Combine(
         ::testing::Values(true, false), // add by row, or by column
         ::testing::Values(true, false) // check sparse case
     )
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/isometric/utils.h` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/isometric/utils.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         std::vector<int>{ 10, 20 },
         std::vector<int>{ 5, 2, 5 },
         std::vector<int>{ 5, 10, 20 },
         std::vector<int>{ 5, 0, 5 }
     );
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedBind,
     DelayedBindFullAccessTest,
     ::testing::Combine(
         spawn_bind_scenarios(),
         ::testing::Values(true, false), // bind by row or by column
         ::testing::Values(true, false), // forward or backward traversal.
         ::testing::Values(1, 3) // jump, to test the workspace's memory.
@@ -196,15 +196,15 @@
     tatami_test::test_sliced_column_access(bound_sparse.get(), manual.get(), FORWARD, JUMP, RFIRST, RLAST);
     tatami_test::test_sliced_column_access(bound_dense.get(), manual.get(), FORWARD, JUMP, RFIRST, RLAST);
 
     tatami_test::test_sliced_row_access(bound_sparse.get(), manual.get(), FORWARD, JUMP, CFIRST, CLAST);
     tatami_test::test_sliced_row_access(bound_dense.get(), manual.get(), FORWARD, JUMP, CFIRST, CLAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedBind,
     DelayedBindSlicedAccessTest,
     ::testing::Combine(
         spawn_bind_scenarios(),
         ::testing::Values(true, false), // bind by row or by column
         ::testing::Values(true, false), // forward or backward traversal.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -235,15 +235,15 @@
     tatami_test::test_indexed_column_access(bound_sparse.get(), manual.get(), FORWARD, JUMP, RFIRST, STEP);
     tatami_test::test_indexed_column_access(bound_dense.get(), manual.get(), FORWARD, JUMP, RFIRST, STEP);
 
     tatami_test::test_indexed_row_access(bound_sparse.get(), manual.get(), FORWARD, JUMP, CFIRST, STEP);
     tatami_test::test_indexed_row_access(bound_dense.get(), manual.get(), FORWARD, JUMP, CFIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedBind,
     DelayedBindIndexedAccessTest,
     ::testing::Combine(
         spawn_bind_scenarios(),
         ::testing::Values(true, false), // bind by row or by column
         ::testing::Values(true, false), // forward or backward traversal.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
@@ -332,15 +332,15 @@
     EXPECT_FALSE(bound->uses_oracle(true));
     EXPECT_TRUE(wrapped_bound->uses_oracle(true));
 
     tatami_test::test_oracle_column_access(wrapped_bound.get(), bound.get(), random);
     tatami_test::test_oracle_row_access(wrapped_bound.get(), bound.get(), random);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedBind,
     DelayedBindOracleTest,
     ::testing::Combine(
         ::testing::Values(
             std::vector<int>{ 100 },
             std::vector<int>{ 150, 100 },
             std::vector<int>{ 50, 200, 150 }
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -109,50 +109,48 @@
     tatami_test::test_simple_column_access(cast_fsparse_value.get(), fsparse_ref.get(), FORWARD, JUMP);
 
     auto cast_sparse_index = tatami::make_DelayedCast<double, int>(sparse_index);
     tatami_test::test_simple_row_access(cast_sparse_index.get(), sparse.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(cast_sparse_index.get(), sparse.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedCast,
     DelayedCastFullAccess,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3) // jump, to test the workspace memory.
     )
 );
 
 /****************************************************
  ****************************************************/
 
-class DelayedCastBlockAccess : public CastTest<std::tuple<bool, size_t, std::vector<double> > > {};
+class DelayedCastBlockAccess : public CastTest<std::tuple<size_t, std::vector<double> > > {};
 
 TEST_P(DelayedCastBlockAccess, Dense) {
     auto param = GetParam(); 
-    bool FORWARD = std::get<0>(param);
-    size_t JUMP = std::get<1>(param);
-    auto interval_info = std::get<2>(param);
+    size_t JUMP = std::get<0>(param);
+    auto interval_info = std::get<1>(param);
     size_t RFIRST = interval_info[0] * nrow, RLAST = interval_info[1] * nrow;
     size_t CFIRST = interval_info[0] * ncol, CLAST = interval_info[1] * ncol;
 
     auto cast_dense = tatami::make_DelayedCast<double, int>(dense);
     tatami_test::test_sliced_row_access(cast_dense.get(), dense.get(), true, JUMP, CFIRST, CLAST);
     tatami_test::test_sliced_column_access(cast_dense.get(), dense.get(), true, JUMP, RFIRST, RLAST);
 
     auto cast_fdense = tatami::make_DelayedCast<double, int>(fdense);
     tatami_test::test_sliced_row_access(cast_fdense.get(), fdense_ref.get(), true, JUMP, CFIRST, CLAST);
     tatami_test::test_sliced_column_access(cast_fdense.get(), fdense_ref.get(), true, JUMP, RFIRST, RLAST);
 }
 
 TEST_P(DelayedCastBlockAccess, Sparse) {
     auto param = GetParam();
-    bool FORWARD = std::get<0>(param);
-    size_t JUMP = std::get<1>(param);
-    auto interval_info = std::get<2>(param);
+    size_t JUMP = std::get<0>(param);
+    auto interval_info = std::get<1>(param);
     size_t RFIRST = interval_info[0] * nrow, RLAST = interval_info[1] * nrow;
     size_t CFIRST = interval_info[0] * ncol, CLAST = interval_info[1] * ncol;
 
     auto cast_sparse = tatami::make_DelayedCast<double, int>(sparse);
     tatami_test::test_sliced_row_access(cast_sparse.get(), sparse.get(), true, JUMP, CFIRST, CLAST);
     tatami_test::test_sliced_column_access(cast_sparse.get(), sparse.get(), true, JUMP, RFIRST, RLAST);
 
@@ -165,55 +163,52 @@
     tatami_test::test_sliced_column_access(cast_fsparse_value.get(), fsparse_ref.get(), true, JUMP, RFIRST, RLAST);
 
     auto cast_sparse_index = tatami::make_DelayedCast<double, int>(sparse_index);
     tatami_test::test_sliced_row_access(cast_sparse_index.get(), sparse.get(), true, JUMP, CFIRST, CLAST);
     tatami_test::test_sliced_column_access(cast_sparse_index.get(), sparse.get(), true, JUMP, RFIRST, RLAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedCast,
     DelayedCastBlockAccess,
     ::testing::Combine(
-        ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to check the workspace memory
         ::testing::Values(
             std::vector<double>({ 0, 0.6 }), 
             std::vector<double>({ 0.5, 0.75 }),
             std::vector<double>({ 0.24, 1 })
         )
     )
 );
 
 /****************************************************
  ****************************************************/
 
-class DelayedCastIndexAccess : public CastTest<std::tuple<bool, size_t, std::vector<double> > > {};
+class DelayedCastIndexAccess : public CastTest<std::tuple<size_t, std::vector<double> > > {};
 
 TEST_P(DelayedCastIndexAccess, Dense) {
     auto param = GetParam(); 
-    bool FORWARD = std::get<0>(param);
-    size_t JUMP = std::get<1>(param);
-    auto interval_info = std::get<2>(param);
+    size_t JUMP = std::get<0>(param);
+    auto interval_info = std::get<1>(param);
     size_t RFIRST = interval_info[0] * nrow, RSTEP = interval_info[1] * nrow;
     size_t CFIRST = interval_info[0] * ncol, CSTEP = interval_info[1] * ncol;
 
     auto cast_dense = tatami::make_DelayedCast<double, int>(dense);
     tatami_test::test_indexed_row_access(cast_dense.get(), dense.get(), true, JUMP, CFIRST, CSTEP);
     tatami_test::test_indexed_column_access(cast_dense.get(), dense.get(), true, JUMP, RFIRST, RSTEP);
 
     auto cast_fdense = tatami::make_DelayedCast<double, int>(fdense);
     tatami_test::test_indexed_row_access(cast_fdense.get(), fdense_ref.get(), true, JUMP, CFIRST, CSTEP);
     tatami_test::test_indexed_column_access(cast_fdense.get(), fdense_ref.get(), true, JUMP, RFIRST, RSTEP);
 }
 
 TEST_P(DelayedCastIndexAccess, Sparse) {
     auto param = GetParam();
-    bool FORWARD = std::get<0>(param);
-    size_t JUMP = std::get<1>(param);
-    auto interval_info = std::get<2>(param);
+    size_t JUMP = std::get<0>(param);
+    auto interval_info = std::get<1>(param);
     size_t RFIRST = interval_info[0] * nrow, RSTEP = interval_info[1] * nrow;
     size_t CFIRST = interval_info[0] * ncol, CSTEP = interval_info[1] * ncol;
 
     auto cast_sparse = tatami::make_DelayedCast<double, int>(sparse);
     tatami_test::test_indexed_row_access(cast_sparse.get(), sparse.get(), true, JUMP, CFIRST, CSTEP);
     tatami_test::test_indexed_column_access(cast_sparse.get(), sparse.get(), true, JUMP, RFIRST, RSTEP);
 
@@ -226,19 +221,18 @@
     tatami_test::test_indexed_column_access(cast_fsparse_value.get(), fsparse_ref.get(), true, JUMP, RFIRST, RSTEP);
 
     auto cast_sparse_index = tatami::make_DelayedCast<double, int>(sparse_index);
     tatami_test::test_indexed_row_access(cast_sparse_index.get(), sparse.get(), true, JUMP, CFIRST, CSTEP);
     tatami_test::test_indexed_column_access(cast_sparse_index.get(), sparse.get(), true, JUMP, RFIRST, RSTEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedCast,
     DelayedCastIndexAccess,
     ::testing::Combine(
-        ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to check the workspace memory
         ::testing::Values(
             std::vector<double>({ 0, 0.015 }), 
             std::vector<double>({ 0.5, 0.025 }),
             std::vector<double>({ 0.666, 0.055 })
         )
     )
@@ -276,15 +270,15 @@
     tatami_test::test_oracle_column_access(wrapped_cast_dense.get(), cast_dense.get(), random);
     tatami_test::test_oracle_column_access(wrapped_cast_sparse.get(), cast_sparse.get(), random);
 
     tatami_test::test_oracle_row_access(wrapped_cast_dense.get(), cast_dense.get(), random);
     tatami_test::test_oracle_row_access(wrapped_cast_sparse.get(), cast_sparse.get(), random);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedCast,
     DelayedCastOracleTest,
     ::testing::Values(true, false)  // use random or consecutive oracle.
 );
 
 /****************************************************
  ****************************************************/
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     auto param = GetParam(); 
     bool FORWARD = std::get<0>(param);
     size_t JUMP = std::get<1>(param);
     tatami_test::test_simple_column_access(tdense.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(tsparse.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     TransposeTest,
     TransposeFullTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4, 10, 20) // jump, to test the workspace's memory.
     )
 );
@@ -95,15 +95,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * tdense->nrow(), LAST = interval_info[1] * tdense->nrow();
 
     tatami_test::test_sliced_column_access(tdense.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_column_access(tsparse.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     TransposeTest,
     TransposeBlockTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4), // jumps (to test workspace memory)
         ::testing::Values(
             std::vector<double>({ 0, 0.44 }),
@@ -135,15 +135,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
 
     tatami_test::test_indexed_row_access(tdense.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_row_access(tsparse.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     TransposeTest,
     TransposeIndexTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.05 }),
@@ -178,15 +178,15 @@
     tatami_test::test_oracle_column_access(wrapped_dense.get(), tdense.get(), random);
     tatami_test::test_oracle_column_access(wrapped_sparse.get(), tsparse.get(), random);
 
     tatami_test::test_oracle_row_access(wrapped_dense.get(), tdense.get(), random);
     tatami_test::test_oracle_row_access(wrapped_sparse.get(), tsparse.get(), random);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     TransposeTest,
     TransposeOracleTest,
     ::testing::Values(true, false)  // use random or consecutive oracle.
 );
 
 TEST(TransposeTest, ConstOverload) {
     int nrow = 10, ncol = 15;
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,22 @@
     indices.push_back(2);
     values.push_back(2);
     indptr.back() = indices.size();
     tatami_test::throws_error([&]() { tatami::CompressedSparseColumnMatrix<double, int> mat(10, 20, values, indices, indptr); }, "strictly increasing");
     tatami_test::throws_error([&]() { tatami::CompressedSparseRowMatrix<double, int> mat(20, 10, values, indices, indptr); }, "strictly increasing");
 }
 
+TEST(CompressedSparseMatrix, OddTypes) {
+    // Checking for compilation warnings here when the interface and storage types are different.
+    std::vector<uint8_t> values;
+    std::vector<uint16_t> indices;
+    std::vector<uint64_t> indptr(11);
+    tatami::CompressedSparseRowMatrix<double, int, decltype(values), decltype(indices), decltype(indptr)> rmat(10, 20, values, indices, indptr);
+}
+
 /*************************************
  *************************************/
 
 class SparseTestMethods {
 protected:
     size_t nrow = 200, ncol = 100;
     std::shared_ptr<tatami::NumericMatrix> dense, sparse_row, sparse_column;
@@ -142,15 +150,15 @@
     auto param = GetParam(); 
     bool FORWARD = std::get<0>(param);
     size_t JUMP = std::get<1>(param);
     tatami_test::test_simple_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     CompressedSparseMatrix,
     SparseFullAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4, 10, 20) // jump, to test the workspace's memory.
     )
 );
@@ -184,15 +192,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
 
     tatami_test::test_sliced_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     CompressedSparseMatrix,
     SparseSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.51 }),
@@ -233,15 +241,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
 
     tatami_test::test_indexed_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     CompressedSparseMatrix,
     SparseIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.05 }),
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     auto param = GetParam(); 
     bool FORWARD = std::get<0>(param);
     size_t JUMP = std::get<1>(param);
     tatami_test::test_simple_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     FragmentedSparseMatrix,
     FragmentedSparseFullAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4, 10, 20) // jump, to test the workspace's memory.
     )
 );
@@ -211,15 +211,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
 
     tatami_test::test_sliced_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     FragmentedSparseMatrix,
     FragmentedSparseSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.51 }),
@@ -260,15 +260,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
 
     tatami_test::test_indexed_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     FragmentedSparseMatrix,
     FragmentedSparseIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.05 }),
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     auto param = GetParam(); 
     bool FORWARD = std::get<0>(param);
     size_t JUMP = std::get<1>(param);
     tatami_test::test_simple_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP);
     tatami_test::test_simple_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     SemiCompressedSparseMatrix,
     SemiSparseFullAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 4, 10, 20) // jump, to test the workspace's memory.
     )
 );
@@ -186,15 +186,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, LAST = interval_info[1] * ncol;
 
     tatami_test::test_sliced_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     SemiCompressedSparseMatrix,
     SemiSparseSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.51 }),
@@ -235,15 +235,15 @@
     auto interval_info = std::get<2>(param);
     size_t FIRST = interval_info[0] * ncol, STEP = interval_info[1] * ncol;
 
     tatami_test::test_indexed_row_access(sparse_column.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_row_access(sparse_row.get(), dense.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     SemiCompressedSparseMatrix,
     SemiSparseIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
         ::testing::Values(1, 3), // jump, to test the workspace's memory.
         ::testing::Values(
             std::vector<double>({ 0, 0.05 }),
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 class FragmentedSparseSecondaryExtractorCoreTest : public SparseSecondaryExtractorCoreTest {
 protected:
     struct FragmentedCore : public tatami::SparseSecondaryExtractorCore<int, int, size_t, SimpleModifier<int, size_t> > {
         FragmentedCore(int max_index, const std::vector<std::vector<int> >& idx) :
             tatami::SparseSecondaryExtractorCore<int, int, size_t, SimpleModifier<int, size_t> >(max_index, idx.size())
         {
             auto length = idx.size();
-            for (int i = 0; i < length; ++i) {
+            for (size_t i = 0; i < length; ++i) {
                 this->current_indices[i] = (idx[i].empty() ? 0 : idx[i].front());
             }
             this->closest_current_index = (length ? *std::min_element(this->current_indices.begin(), this->current_indices.end()) : max_index);
             return;
         } 
 
     public:
@@ -529,8 +529,7 @@
         EXPECT_TRUE(test.search(18, n, identity, indices, store_fun, skip_fun)); // jump to end works correctly.
         EXPECT_EQ(results, expected(-1, 4, -1));
 
         EXPECT_TRUE(test.search(15, n, identity, indices, store_fun, skip_fun)); // decrement.
         EXPECT_EQ(results, expected(5, -1, -1));
     }
 }
-
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/medians.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/medians.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     ref = tatami::column_medians(dense_row.get());
     EXPECT_EQ(ref.size(), order);
     EXPECT_EQ(ref, tatami::column_medians(dense_column.get()));
     EXPECT_EQ(ref, tatami::column_medians(sparse_row.get()));
     EXPECT_EQ(ref, tatami::column_medians(sparse_column.get()));
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ComputingDimMedians,
     MedianTriangularTest,
     ::testing::Values(13, 22, 51, 80) // mix of even and odd numbers
 );
 
 TEST(ComputingDimMedians, RowMediansNaN) {
     auto dense = std::unique_ptr<tatami::NumericMatrix>(new tatami::DenseRowMatrix<double>(111, 0, std::vector<double>()));
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/ranges.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/ranges.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     EXPECT_EQ(ref, tatami::column_ranges(dense_column.get(), 3));
     EXPECT_EQ(ref, tatami::column_ranges(sparse_row.get(), 3));
     EXPECT_EQ(ref, tatami::column_ranges(sparse_column.get(), 3));
 }
 
 /********************************************/
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ComputingDimExtremes,
     ComputingDimExtremesTest,
     ::testing::Values(
         std::make_pair(0.1, 10.0),   // only above.
         std::make_pair(-10.0, -0.4), // only below
         std::make_pair(-5.0, 5.0)    // mix of values above and below zero.
     )
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/sums.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/sums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/stats/variances.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/stats/variances.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         std::vector<int> ref_nzeros(NR);
         auto wrk = sparse_column->sparse_column();
 
         for (int c = 0; c < static_cast<int>(NC); ++c) {
             auto range = wrk->fetch_copy(c, vbuffer.data(), ibuffer.data());
             vbuffer[0] = 0; 
             tatami::stats::variances::compute_running(range, running_means.data(), running_vars.data(), running_nzeros.data(), c);
-            for (size_t r = 1; r < range.number; ++r) {
+            for (int r = 1; r < range.number; ++r) {
                 ref_nzeros[range.index[r]] += (range.value[r] != 0);
             }
         }
         tatami::stats::variances::finish_running(NR, running_means.data(), running_vars.data(), running_nzeros.data(), NC);
 
         EXPECT_EQ(ref_nzeros, running_nzeros);
     }
@@ -144,15 +144,15 @@
         std::vector<int> ref_nzeros(NR);
         auto wrk = sparse_column->sparse_column();
 
         for (int c = 0; c < static_cast<int>(NC); ++c) {
             auto range = wrk->fetch_copy(c, vbuffer.data(), ibuffer.data());
             vbuffer[0] = 0; 
             tatami::stats::variances::compute_running(range, running_means2.data(), running_vars2.data(), running_nzeros2.data(), c, false);
-            for (size_t r = 0; r < range.number; ++r) {
+            for (int r = 0; r < range.number; ++r) {
                 ++ref_nzeros[range.index[r]];
             }
         }
         tatami::stats::variances::finish_running(NR, running_means2.data(), running_vars2.data(), running_nzeros2.data(), NC);
 
         EXPECT_EQ(ref_nzeros, running_nzeros2);
         for (size_t i = 0; i < NR; ++i) {
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     tatami_test::test_simple_row_access(sparse_subbed2.get(), ref.get(), FORWARD, JUMP);
 
     tatami_test::test_simple_column_access(dense_subbed.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_subbed.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_subbed2.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubset,
     SubsetFullAccessTest,
     ::testing::Combine(
         ::testing::Values(2, 5, 10), // step size.
         ::testing::Values(false, true), // whether to support duplicate indices.
         ::testing::Values(true, false), // whether to require sorted indices.
         ::testing::Values(true, false), // iterate forward or back, to test the workspace's memory.
@@ -210,15 +210,15 @@
     tatami_test::test_sliced_row_access(sparse_subbed2.get(), ref.get(), true, JUMP, CFIRST, CLAST);
 
     tatami_test::test_sliced_column_access(dense_subbed.get(), ref.get(), true, JUMP, RFIRST, RLAST);
     tatami_test::test_sliced_column_access(sparse_subbed.get(), ref.get(), true, JUMP, RFIRST, RLAST);
     tatami_test::test_sliced_column_access(sparse_subbed2.get(), ref.get(), true, JUMP, RFIRST, RLAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubset,
     SubsetSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(2, 5, 10), // step size.
         ::testing::Values(false, true), // whether to support duplicate indices.
         ::testing::Values(true, false), // whether to require sorted indices.
         ::testing::Values(1, 3), // jump, to check the workspace memory
@@ -272,15 +272,15 @@
     tatami_test::test_indexed_row_access(dense_subbed.get(), ref.get(), true, JUMP, CFIRST, STEP);
     tatami_test::test_indexed_row_access(sparse_subbed.get(), ref.get(), true, JUMP, CFIRST, STEP);
 
     tatami_test::test_indexed_column_access(dense_subbed.get(), ref.get(), true, JUMP, RFIRST, STEP);
     tatami_test::test_indexed_column_access(sparse_subbed.get(), ref.get(), true, JUMP, RFIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubset,
     SubsetIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(2, 5, 10), // step size.
         ::testing::Values(false, true), // whether to support duplicate indices.
         ::testing::Values(true, false), // whether to require sorted indices.
         ::testing::Values(1, 3), // jump, to check the workspace memory
@@ -400,15 +400,15 @@
 
     tatami::DelayedSubset<0, double, int, decltype(sub)> manual(dense, sub);
     auto ref = reference_on_rows(sub);
     tatami_test::test_simple_row_access(&manual, ref.get(), true, 1);
     tatami_test::test_simple_column_access(&manual, ref.get(), true, 1);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubset,
     SubsetConstructorTest,
     ::testing::Combine(
         ::testing::Values(false, true), // whether to support duplicate indices.
         ::testing::Values(true, false)  // whether to require sorted indices.
     )
 );
@@ -456,15 +456,15 @@
     tatami_test::test_oracle_column_access(wrapped_dense_subbed.get(), dense_subbed.get(), random);
     tatami_test::test_oracle_column_access(wrapped_sparse_subbed.get(), sparse_subbed.get(), random);
 
     tatami_test::test_oracle_row_access(wrapped_dense_subbed.get(), dense_subbed.get(), random);
     tatami_test::test_oracle_row_access(wrapped_sparse_subbed.get(), sparse_subbed.get(), random);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubset,
     SubsetOracleTest,
     ::testing::Combine(
         ::testing::Values(2, 5, 10), // step size.
         ::testing::Values(false, true), // whether to support duplicate indices.
         ::testing::Values(true, false), // whether to require sorted indices.
         ::testing::Values(true, false)  // use random or consecutive oracle.
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     bool FORWARD = std::get<2>(param);
     bool JUMP = std::get<3>(param);
 
     tatami_test::test_simple_column_access(dense_block.get(), ref.get(), FORWARD, JUMP);
     tatami_test::test_simple_column_access(sparse_block.get(), ref.get(), FORWARD, JUMP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubsetBlock,
     SubsetBlockFullAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // row or column subsetting, respectively.
         ::testing::Values(
             std::make_pair(0.0, 0.5),
             std::make_pair(0.25, 0.8),
@@ -137,15 +137,15 @@
     auto interval_info = std::get<4>(param);
     int FIRST = interval_info[0] * dense_block->nrow(), LAST = interval_info[1] * dense_block->nrow();
 
     tatami_test::test_sliced_column_access(dense_block.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
     tatami_test::test_sliced_column_access(sparse_block.get(), ref.get(), FORWARD, JUMP, FIRST, LAST);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubsetBlock,
     SubsetBlockSlicedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // row or column subsetting, respectively.
         ::testing::Values(
             std::make_pair(0.0, 0.5),
             std::make_pair(0.25, 0.8),
@@ -188,15 +188,15 @@
     auto interval_info = std::get<4>(param);
     int FIRST = interval_info[0] * dense_block->nrow(), STEP = interval_info[1] * dense_block->nrow();
 
     tatami_test::test_indexed_column_access(dense_block.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
     tatami_test::test_indexed_column_access(sparse_block.get(), ref.get(), FORWARD, JUMP, FIRST, STEP);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubsetBlock,
     SubsetBlockIndexedAccessTest,
     ::testing::Combine(
         ::testing::Values(true, false), // row or column subsetting, respectively.
         ::testing::Values(
             std::make_pair(0.0, 0.5),
             std::make_pair(0.25, 0.8),
@@ -226,15 +226,14 @@
         auto simulated = tatami_test::simulate_sparse_vector<double>(NR * NC, 0.2);
         auto dense = std::shared_ptr<tatami::NumericMatrix>(new tatami::DenseRowMatrix<double>(NR, NC, simulated));
         auto sparse = tatami::convert_to_sparse<false>(dense.get()); // column-major.
 
         double full =  (std::get<0>(param) ? NR : NC);
         int first = full * std::get<1>(param).first;
         int last = full * std::get<1>(param).second;
-        auto block_length = last - first;
 
         if (std::get<0>(param)) {
             dense_block = tatami::make_DelayedSubsetBlock<0>(dense, first, last);
             sparse_block = tatami::make_DelayedSubsetBlock<0>(sparse, first, last);
             wrapped_dense_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(dense), first, last);
             wrapped_sparse_block = tatami::make_DelayedSubsetBlock<0>(tatami_test::make_CrankyMatrix(sparse), first, last);
         } else {
@@ -257,15 +256,15 @@
     tatami_test::test_oracle_column_access(wrapped_dense_block.get(), dense_block.get(), random);
     tatami_test::test_oracle_column_access(wrapped_sparse_block.get(), sparse_block.get(), random);
 
     tatami_test::test_oracle_row_access(wrapped_dense_block.get(), dense_block.get(), random);
     tatami_test::test_oracle_row_access(wrapped_sparse_block.get(), sparse_block.get(), random);
 }
 
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     DelayedSubsetBlock,
     SubsetBlockOracleTest,
     ::testing::Combine(
         ::testing::Values(true, false), // row or column subsetting, respectively.
         ::testing::Values(
             std::make_pair(0.0, 0.5),
             std::make_pair(0.25, 0.8),
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -180,16 +180,15 @@
             EXPECT_FALSE(converted->sparse());
             tatami_test::test_simple_row_access(converted.get(), &smat, true, 1);
             tatami_test::test_simple_column_access(converted.get(), &smat, true, 1);
         }
     }
 }
 
-
-INSTANTIATE_TEST_CASE_P(
+INSTANTIATE_TEST_SUITE_P(
     ConvertToDense,
     ConvertToDenseTest,
     ::testing::Combine(
         ::testing::Values(10, 50, 100), // number of rows
         ::testing::Values(10, 50, 100)  // number of columns
     )
 );
```

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp` & `mattress-0.0.4/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/CMakeLists.txt` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/LICENSE` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/README.md` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/docs/Doxyfile` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp` & `mattress-0.0.4/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/lib/common.cpp` & `mattress-0.0.4/src/mattress/lib/common.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress/lib/dense.cpp` & `mattress-0.0.4/src/mattress/lib/dense.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 #include "Mattress.h"
 #include <string>
 #include <stdexcept>
 #include <cstring>
 #include <cstdint>
 
 template<typename T>
-Mattress* initialize_dense_matrix(int nr, int nc, const T* ptr, bool byrow) { 
+Mattress* initialize_dense_matrix(int nr, int nc, const T* ptr) { 
     tatami::ArrayView<T> view(ptr, static_cast<size_t>(nr) * static_cast<size_t>(nc));
-    if (byrow) {
-        return new Mattress(new tatami::DenseRowMatrix<double, int, decltype(view)>(nr, nc, view));
-    } else {
-        return new Mattress(new tatami::DenseColumnMatrix<double, int, decltype(view)>(nr, nc, view));
-    }
+    return new Mattress(new tatami::DenseRowMatrix<double, int, decltype(view)>(nr, nc, view));
 }
 
 extern "C" {
 
-Mattress* py_initialize_dense_matrix(int nr, int nc, const char* type, void* ptr, int byrow) {
+Mattress* py_initialize_dense_matrix(int nr, int nc, const char* type, void* ptr) {
     if (std::strcmp(type, "float64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<double*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<double*>(ptr));
 
     } else if (std::strcmp(type, "float32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<float*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<float*>(ptr));
 
     } else if (std::strcmp(type, "int64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int64_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int64_t*>(ptr));
 
     } else if (std::strcmp(type, "int32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int32_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int32_t*>(ptr));
 
     } else if (std::strcmp(type, "int16") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int16_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int16_t*>(ptr));
 
     } else if (std::strcmp(type, "int8") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<int8_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<int8_t*>(ptr));
 
     } else if (std::strcmp(type, "uint64") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint64_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint64_t*>(ptr));
 
     } else if (std::strcmp(type, "uint32") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint32_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint32_t*>(ptr));
 
     } else if (std::strcmp(type, "uint16") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint16_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint16_t*>(ptr));
 
     } else if (std::strcmp(type, "uint8") == 0) {
-        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint8_t*>(ptr), byrow);
+        return initialize_dense_matrix(nr, nc, reinterpret_cast<uint8_t*>(ptr));
     }
 
     throw std::runtime_error("unrecognized array type '" + std::string(type) + "' for dense matrix initialization");
     return NULL;
 }
 
 }
```

### Comparing `mattress-0.0.3/src/mattress/utils.py` & `mattress-0.0.4/src/mattress/utils.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.3/src/mattress.egg-info/PKG-INFO` & `mattress-0.0.4/src/mattress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.3
+Version: 0.0.4
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.3/src/mattress.egg-info/SOURCES.txt` & `mattress-0.0.4/src/mattress.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
 src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
 src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
 src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
 src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
 src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
 src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
+src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
+src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
 src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
 src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
 src/mattress/extern/tatami/include/tatami/stats/medians.hpp
 src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
 src/mattress/extern/tatami/include/tatami/stats/sums.hpp
 src/mattress/extern/tatami/include/tatami/stats/utils.hpp
 src/mattress/extern/tatami/include/tatami/stats/variances.hpp
@@ -130,29 +132,30 @@
 src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
 src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
 src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
 src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
 src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
 src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
 src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
+src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
+src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
 src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
 src/mattress/extern/tatami/tests/src/stats/medians.cpp
 src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
 src/mattress/extern/tatami/tests/src/stats/ranges.cpp
 src/mattress/extern/tatami/tests/src/stats/sums.cpp
 src/mattress/extern/tatami/tests/src/stats/variances.cpp
 src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
 src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
 src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
 src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
 src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
 src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
 src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
 src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
-src/mattress/extern/tatami/tests/src/utils/convert_to_sparse.cpp
 src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
 src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
 src/mattress/extern/tatami_hdf5/.git
 src/mattress/extern/tatami_hdf5/.gitignore
 src/mattress/extern/tatami_hdf5/CMakeLists.txt
 src/mattress/extern/tatami_hdf5/LICENSE
 src/mattress/extern/tatami_hdf5/README.md
@@ -170,10 +173,12 @@
 src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
 src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
 src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
 src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
 src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
 src/mattress/include/Mattress.h
 src/mattress/lib/common.cpp
+src/mattress/lib/compressed_sparse.cpp
 src/mattress/lib/dense.cpp
 tests/conftest.py
-tests/test_dense.py
+tests/test_dense.py
+tests/test_sparse.py
```

### Comparing `mattress-0.0.3/tox.ini` & `mattress-0.0.4/tox.ini`

 * *Files identical despite different names*

