# Comparing `tmp/NZMATH-1.1.0.tar.gz` & `tmp/nzmath-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NZMATH-1.1.0.tar", last modified: Tue May 31 11:51:16 2011, max compression
+gzip compressed data, was "nzmath-3.0.0.tar", last modified: Thu Jul 27 06:39:23 2023, max compression
```

## Comparing `NZMATH-1.1.0.tar` & `nzmath-3.0.0.tar`

### file list

```diff
@@ -1,128 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      542 2011-05-31 11:51:16.000000 NZMATH-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/data/
--rw-r--r--   0 root         (0) root         (0)   556049 2011-05-31 05:46:58.000000 NZMATH-1.1.0/data/discriminant.csv
--rw-r--r--   0 root         (0) root         (0)     1334 2011-05-31 11:51:16.000000 NZMATH-1.1.0/HISTORY.txt
--rw-r--r--   0 root         (0) root         (0)     8994 2011-05-31 11:51:16.000000 NZMATH-1.1.0/CHANGES.txt
--rw-r--r--   0 root         (0) root         (0)     1555 2011-05-31 11:51:16.000000 NZMATH-1.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3191 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmathconf.py.example
--rw-r--r--   0 root         (0) root         (0)      955 2011-05-31 11:51:16.000000 NZMATH-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/manual/
--rw-r--r--   0 root         (0) root         (0)    56520 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/prime_decomp.pdf
--rw-r--r--   0 root         (0) root         (0)   107196 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/finitefield.pdf
--rw-r--r--   0 root         (0) root         (0)    80349 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.factor.pdf
--rw-r--r--   0 root         (0) root         (0)    80730 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/lattice.pdf
--rw-r--r--   0 root         (0) root         (0)    87178 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/ecpp.pdf
--rw-r--r--   0 root         (0) root         (0)    59084 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/compatibility.pdf
--rw-r--r--   0 root         (0) root         (0)    72543 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/gcd.pdf
--rw-r--r--   0 root         (0) root         (0)    77283 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/round2.pdf
--rw-r--r--   0 root         (0) root         (0)    60644 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.ratfunc.pdf
--rw-r--r--   0 root         (0) root         (0)   148103 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.uniutil.pdf
--rw-r--r--   0 root         (0) root         (0)    58298 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/multiplicative.pdf
--rw-r--r--   0 root         (0) root         (0)   109468 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/equation.pdf
--rw-r--r--   0 root         (0) root         (0)    97104 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.misc.pdf
--rw-r--r--   0 root         (0) root         (0)    77155 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/bigrange.pdf
--rw-r--r--   0 root         (0) root         (0)   100919 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.termorder.pdf
--rw-r--r--   0 root         (0) root         (0)    81959 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.methods.pdf
--rw-r--r--   0 root         (0) root         (0)    89908 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.formalsum.pdf
--rw-r--r--   0 root         (0) root         (0)   113485 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/group.pdf
--rw-r--r--   0 root         (0) root         (0)  1363265 2011-05-31 11:50:59.000000 NZMATH-1.1.0/manual/nzmath_doc.pdf
--rw-r--r--   0 root         (0) root         (0)    64569 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.find.pdf
--rw-r--r--   0 root         (0) root         (0)    52308 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.mpqs.pdf
--rw-r--r--   0 root         (0) root         (0)    60288 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.ecm.pdf
--rw-r--r--   0 root         (0) root         (0)    84791 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/squarefree.pdf
--rw-r--r--   0 root         (0) root         (0)   103841 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.ring.pdf
--rw-r--r--   0 root         (0) root         (0)    68869 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.multivar.pdf
--rw-r--r--   0 root         (0) root         (0)    65585 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/arygcd.pdf
--rw-r--r--   0 root         (0) root         (0)   167218 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/ring.pdf
--rw-r--r--   0 root         (0) root         (0)    86370 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/intresidue.pdf
--rw-r--r--   0 root         (0) root         (0)    95711 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/quad.pdf
--rw-r--r--   0 root         (0) root         (0)   149316 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/algfield.pdf
--rw-r--r--   0 root         (0) root         (0)   126805 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/real.pdf
--rw-r--r--   0 root         (0) root         (0)   119773 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.multiutil.pdf
--rw-r--r--   0 root         (0) root         (0)   127469 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/permute.pdf
--rw-r--r--   0 root         (0) root         (0)   214428 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/matrix.pdf
--rw-r--r--   0 root         (0) root         (0)   106739 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/imaginary.pdf
--rw-r--r--   0 root         (0) root         (0)    75872 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/bigrandom.pdf
--rw-r--r--   0 root         (0) root         (0)    93564 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/arith1.pdf
--rw-r--r--   0 root         (0) root         (0)   154446 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/module.pdf
--rw-r--r--   0 root         (0) root         (0)   107249 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/prime.pdf
--rw-r--r--   0 root         (0) root         (0)   105816 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/rational.pdf
--rw-r--r--   0 root         (0) root         (0)   164976 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/elliptic.pdf
--rw-r--r--   0 root         (0) root         (0)    88719 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/vector.pdf
--rw-r--r--   0 root         (0) root         (0)    89038 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/config.pdf
--rw-r--r--   0 root         (0) root         (0)    80902 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/algorithm.pdf
--rw-r--r--   0 root         (0) root         (0)    96328 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/combinatorial.pdf
--rw-r--r--   0 root         (0) root         (0)    76934 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/cubic_root.pdf
--rw-r--r--   0 root         (0) root         (0)    98557 2011-05-31 09:56:11.000000 NZMATH-1.1.0/manual/factor.util.pdf
--rw-r--r--   0 root         (0) root         (0)   102355 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.hensel.pdf
--rw-r--r--   0 root         (0) root         (0)    74539 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.groebner.pdf
--rw-r--r--   0 root         (0) root         (0)    90399 2011-05-31 09:56:12.000000 NZMATH-1.1.0/manual/poly.univar.pdf
--rw-r--r--   0 root         (0) root         (0)       54 2011-05-31 11:51:16.000000 NZMATH-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9877 2011-05-31 11:51:16.000000 NZMATH-1.1.0/tutorial.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/
--rw-r--r--   0 root         (0) root         (0)     5189 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/cubic_root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/poly/
--rw-r--r--   0 root         (0) root         (0)    13778 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/multivar.py
--rw-r--r--   0 root         (0) root         (0)    26258 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/univar.py
--rw-r--r--   0 root         (0) root         (0)     5545 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/groebner.py
--rw-r--r--   0 root         (0) root         (0)     9239 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/factor.py
--rw-r--r--   0 root         (0) root         (0)     2636 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/ratfunc.py
--rw-r--r--   0 root         (0) root         (0)    12575 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/formalsum.py
--rw-r--r--   0 root         (0) root         (0)    17023 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/hensel.py
--rw-r--r--   0 root         (0) root         (0)    22988 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/ring.py
--rw-r--r--   0 root         (0) root         (0)    58787 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/uniutil.py
--rw-r--r--   0 root         (0) root         (0)    11683 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/termorder.py
--rw-r--r--   0 root         (0) root         (0)      223 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24881 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/poly/multiutil.py
--rw-r--r--   0 root         (0) root         (0)     8413 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/arith1.py
--rw-r--r--   0 root         (0) root         (0)     3960 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/vector.py
--rw-r--r--   0 root         (0) root         (0)     6348 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/bigrange.py
--rw-r--r--   0 root         (0) root         (0)     8383 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/real.py
--rw-r--r--   0 root         (0) root         (0)    37730 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/module.py
--rw-r--r--   0 root         (0) root         (0)    33195 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/finitefield.py
--rw-r--r--   0 root         (0) root         (0)     6063 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/algorithm.py
--rw-r--r--   0 root         (0) root         (0)    17396 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/combinatorial.py
--rw-r--r--   0 root         (0) root         (0)    53635 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/elliptic.py
--rw-r--r--   0 root         (0) root         (0)    28341 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/prime.py
--rw-r--r--   0 root         (0) root         (0)     4717 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/arygcd.py
--rw-r--r--   0 root         (0) root         (0)    31789 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/rational.py
--rw-r--r--   0 root         (0) root         (0)      765 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/compatibility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/config/
--rw-r--r--   0 root         (0) root         (0)     3191 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/config/nzmathconf.py
--rw-r--r--   0 root         (0) root         (0)    63940 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/matrix.py
--rw-r--r--   0 root         (0) root         (0)     7604 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/squarefree.py
--rw-r--r--   0 root         (0) root         (0)     6653 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/lattice.py
--rw-r--r--   0 root         (0) root         (0)    27592 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/algfield.py
--rw-r--r--   0 root         (0) root         (0)    15508 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/ecpp.py
--rw-r--r--   0 root         (0) root         (0)    13682 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/factor/
--rw-r--r--   0 root         (0) root         (0)     8654 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/methods.py
--rw-r--r--   0 root         (0) root         (0)     3600 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/find.py
--rw-r--r--   0 root         (0) root         (0)    27008 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/mpqs.py
--rw-r--r--   0 root         (0) root         (0)     9007 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/ecm.py
--rw-r--r--   0 root         (0) root         (0)     6804 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/misc.py
--rw-r--r--   0 root         (0) root         (0)      166 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9164 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/factor/util.py
--rw-r--r--   0 root         (0) root         (0)     2457 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/bigrandom.py
--rw-r--r--   0 root         (0) root         (0)    32986 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/quad.py
--rw-r--r--   0 root         (0) root         (0)     2390 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/gcd.py
--rw-r--r--   0 root         (0) root         (0)     7777 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/config.py
--rw-r--r--   0 root         (0) root         (0)     9603 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/equation.py
--rw-r--r--   0 root         (0) root         (0)    25724 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/ring.py
--rw-r--r--   0 root         (0) root         (0)    19769 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/permute.py
--rw-r--r--   0 root         (0) root         (0)     1242 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/multiplicative.py
--rw-r--r--   0 root         (0) root         (0)    10834 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/intresidue.py
--rw-r--r--   0 root         (0) root         (0)     8142 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/imaginary.py
--rw-r--r--   0 root         (0) root         (0)    16574 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/round2.py
--rw-r--r--   0 root         (0) root         (0)    14283 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/prime_decomp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2011-05-31 11:51:16.000000 NZMATH-1.1.0/nzmath/plugin/math/
--rw-r--r--   0 root         (0) root         (0)      998 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/plugin/math/_mpmath.py
--rw-r--r--   0 root         (0) root         (0)      614 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/plugin/math/default.py
--rw-r--r--   0 root         (0) root         (0)      998 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/plugin/math/__init__.py
--rw-r--r--   0 root         (0) root         (0)      256 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      767 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1162 2011-05-31 05:46:58.000000 NZMATH-1.1.0/nzmath/plugins.py
--rw-r--r--   0 root         (0) root         (0)     1950 2011-05-31 11:51:16.000000 NZMATH-1.1.0/README.txt
--rw-r--r--   0 root         (0) root         (0)     2272 2011-05-31 11:51:16.000000 NZMATH-1.1.0/ACKNOWLEDGEMENTS.txt
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.786937 nzmath-3.0.0/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1555 2023-05-25 06:40:05.000000 nzmath-3.0.0/LICENSE
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2705 2023-07-27 06:39:23.785937 nzmath-3.0.0/PKG-INFO
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2027 2023-07-27 06:20:52.000000 nzmath-3.0.0/README.txt
+-rwxr-xr-x   0 satoru   (197609) なし       (197121)      800 2023-07-27 06:38:58.000000 nzmath-3.0.0/pyproject.toml
+-rw-r--r--   0 satoru   (197609) なし       (197121)       38 2023-07-27 06:39:23.787938 nzmath-3.0.0/setup.cfg
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.520946 nzmath-3.0.0/src/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      790 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    27475 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/algfield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6061 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/algorithm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2346 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/all.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    10111 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/arith1.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4717 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/arygcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2456 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/bigrandom.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6324 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/bigrange.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    18853 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/combinatorial.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      962 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/compatibility.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.522946 nzmath-3.0.0/src/config/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3216 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/config/nzmathconf.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8005 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/config.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5188 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/cubic_root.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    15623 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/ecpp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    53548 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/elliptic.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9601 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/equation.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.546945 nzmath-3.0.0/src/factor/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      166 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9206 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/ecm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3752 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/find.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8654 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/methods.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6817 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/misc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    27139 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/mpqs.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9156 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/factor/util.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    33296 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/finitefield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2389 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/gcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13682 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/group.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8182 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/imaginary.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    10806 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/intresidue.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6622 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/lattice.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    64136 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/matrix.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    37722 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/module.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1242 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/multiplicative.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.556945 nzmath-3.0.0/src/nzmath.egg-info/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2705 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/PKG-INFO
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2412 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/SOURCES.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)        1 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/dependency_links.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)      326 2023-07-27 06:39:23.000000 nzmath-3.0.0/src/nzmath.egg-info/top_level.txt
+-rw-r--r--   0 satoru   (197609) なし       (197121)    21369 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/permute.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.559945 nzmath-3.0.0/src/plugin/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      256 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/__init__.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.566945 nzmath-3.0.0/src/plugin/math/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      998 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1005 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/_mpmath.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      614 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugin/math/default.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1162 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/plugins.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.608943 nzmath-3.0.0/src/poly/
+-rw-r--r--   0 satoru   (197609) なし       (197121)      223 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/__init__.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14884 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/array.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     9210 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/factor.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    12870 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/formalsum.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4771 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/groebner.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16993 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/hensel.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    24835 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/multiutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13718 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/multivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2769 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/ratfunc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    22954 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/ring.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    13939 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/termorder.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    58733 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/uniutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    26211 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/poly/univar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    34893 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/prime.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14333 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/prime_decomp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    33044 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/quad.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    31782 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/rational.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8399 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/real.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    26077 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/ring.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16533 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/round2.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1096 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/sequence.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7604 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/squarefree.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4027 2022-03-28 07:06:53.000000 nzmath-3.0.0/src/vector.py
+drwxr-xr-x   0 satoru   (197609) なし       (197121)        0 2023-07-27 06:39:23.783939 nzmath-3.0.0/tests/
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4451 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAlgfield.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1928 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAlgorithm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1479 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testAll.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5386 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testArith1.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1130 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testArygcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2809 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testBigrandom.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2339 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testBigrange.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    11714 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCombinatorial.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1502 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCompatibility.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1266 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testCubic_root.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3393 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testEcpp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    11731 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testElliptic.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5321 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testEquation.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2864 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorEcm.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3799 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMethods.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4539 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMisc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3284 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorMpqs.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2770 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFactorUtil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    12587 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFiniteField.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5698 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testFormalsum.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2023 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGcd.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4429 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGroebner.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4247 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testGroup.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2655 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testImaginary.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6764 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testIntresidue.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)      555 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testLattice.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    16528 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMatrix.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2598 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMatrixFiniteField.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    15370 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testModule.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1298 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultiplicative.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     8007 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultiutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5293 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testMultivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4626 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPermute.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1473 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPlugins.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5569 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyArray.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     3540 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyFactor.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7325 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyHensel.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4970 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPolyRing.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7563 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPrime.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6453 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testPrime_decomp.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6075 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testQuad.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1312 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRatfunc.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14984 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRational.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     2686 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testReal.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4472 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRing.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     4103 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testRound2.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1286 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testSequence.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     5140 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testSquarefree.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     7687 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testTermOrder.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)    14563 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testUniutil.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     6981 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testUnivar.py
+-rw-r--r--   0 satoru   (197609) なし       (197121)     1918 2022-03-28 07:06:53.000000 nzmath-3.0.0/tests/testVector.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `NZMATH-1.1.0/LICENSE.txt` & `nzmath-3.0.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2003-2011 development group
+Copyright (c) 2003-2022 development group
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
     * Redistributions of source code must retain the above copyright
```

### Comparing `NZMATH-1.1.0/nzmathconf.py.example` & `nzmath-3.0.0/src/config/nzmathconf.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 # net availability
 # ----------------
 #
 # Some functions will connect to the Net.
 # Desktop machines are usually connected to the Net, but notebooks
 # may have connectivity only occasionally.
 #
-# If you have net connectivity now, set as the following:
-#HAVE_NET = True
-#CHECK_NET = False
+# If sometimes you have net connectivity, set as the following:
+HAVE_NET = True
+CHECK_NET = False
 # Or, if your machine is not connected, set as the following:
 #HAVE_NET = False
 #CHECK_NET = False
-# The default values mean "I don't know; check it later":
-HAVE_NET = None
-CHECK_NET = True
+# Or you can let NZMATH check connectivity every time, set as the following:
+#HAVE_NET = None
+#CHECK_NET = True
 
 #
 # psyco
 # -----
 #
 # psyco is a package providing JIT compiler for Python.
 # http://psyco.sourceforge.net/
```

### Comparing `NZMATH-1.1.0/nzmath/cubic_root.py` & `nzmath-3.0.0/src/cubic_root.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 def c_root_p(a, p):
     """
     Return the cubic root modulo p.
     (i.e. a^3 = x (mod p))
     """
     if (a % p) == 0:
         return [0]
-    if p == 2 or p == 3 : 
+    if p == 2 or p == 3 :
         return [a % p]
     if (p % 3) == 2:
-        return [pow(a, (((2 * p) - 1) / 3), p)]
+        return [pow(a, (((2 * p) - 1) // 3), p)]
     p_div_3, p_mod_3 = divmod((p - 1), 3)
     # Compute e,q
     e = 0
     temp = p_div_3
     tempmod = p_mod_3
 
     while tempmod == 0:
         e += 1
         temp, tempmod = divmod(temp, 3)
-    q = (p - 1) / (3 ** e)
-    search_range = (p - 1) / 2
+    q = (p - 1) // (3 ** e)
+    search_range = (p - 1) >> 1
     h = 2
     while pow(h, p_div_3, p) == 1:
         h = random.randrange(2, search_range)
     sym = pow(h, p_div_3, p)
     g = pow(h, q, p)
     # Initialize
     y = g
     r = e
     if q % 3 == 2:
-        x = pow(a, (q - 2) / 3, p)
+        x = pow(a, (q - 2) // 3, p)
     else:
-        x = pow(a, (((2 * q) - 2) / 3), p)
+        x = pow(a, (((2 * q) - 2) // 3), p)
 
     b = (pow(a, 2, p) * pow(x, 3, p)) % p
     x = (a * x) % p
     while (b % p) != 1:
         # Find exponent
         b_pow = pow(b, 3, p)
         m = 1
@@ -78,24 +78,24 @@
         return c_symbol(a, 0, b1, b2)
     else:
         return c_symbol(a, 0, p, 0)
 
 def c_symbol(a1, a2, b1, b2):
     """
     Return the (Jacobi) cubic residue symbol of 2 Eisenstein Integers ((a1+a2*w)/(b1+b2*w)).
-    assume that b1+b2*w is not divisable 1-w. 
+    assume that b1+b2*w is not divisable 1-w.
     """
     r1, r2, j1 = _divides(a1, a2)
     r1, r2, i1 = _FormAdj_w(r1, r2)
     d1, d2, i2 = _FormAdj_w(b1, b2)
     m = (d1 - 1) / 3
     n = d2 / 3
     t = ((m * j1) + (-(m + n) * i1)) % 3
     a1, a2 = r1, r2
-    b1, b2 = d1, d2    
+    b1, b2 = d1, d2
     nrm_a, nrm_b = arygcd._ap_norm_w(a1, a2, b1, b2)
     if nrm_a < nrm_b:
         tmpre, tmpim = a1, a2
         a1, a2 = b1, b2
         b1, b2 = tmpre, tmpim
         m = (b1 - 1) / 3
         n = b2 / 3
```

### Comparing `NZMATH-1.1.0/nzmath/poly/multivar.py` & `nzmath-3.0.0/src/poly/multivar.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Class definitions of multivariate polynomials.
 
 The polynomials are immutable data types, under the public API.  If
 one tries to manipulate its underlying data attributes, immutability
 will be able to be broken.
 """
 
-from __future__ import division
+
 import logging
 import warnings
 import nzmath.ring as _ring
 import nzmath.poly.formalsum as formalsum
 
 
 _log = logging.getLogger('nzmath.poly.multivar')
@@ -135,15 +135,15 @@
         if len(self) != len(other):
             raise TypeError("different length indices")
         return self.__class__([min(i, j) for (i, j) in zip(self, other)])
 
     def lcm(self, other):
         """
         Return the least common multiple.
-        
+
         lcm((i1, ..., in), (j1, ..., jn)) = (max(i1, j1), ..., max(in, jn))
         """
         if len(self) != len(other):
             raise TypeError("different length indices")
         return self.__class__([max(i, j) for (i, j) in zip(self, other)])
 
     def total_degree(self):
@@ -184,15 +184,15 @@
     def __init__(self, coefficients, **kwds):
         """
         BasicPolynomial(coefficients [, keyword_arguments...])
 
         coefficients can be any dict initial values.
         """
         PolynomialInterface.__init__(self)
-        self._coefficients = dict([(TermIndices(i), c) for (i, c) in dict(coefficients).iteritems()])
+        self._coefficients = dict([(TermIndices(i), c) for (i, c) in dict(coefficients).items()])
         if "number_of_variables" in kwds:
             self.number_of_variables = kwds.pop("number_of_variables")
         else:
             self.number_of_variables = 0
             for i in self.iterbases():
                 if len(i) > self.number_of_variables:
                     self.number_of_variables = len(i)
@@ -232,30 +232,30 @@
                     continue
                 assert len(ds) == len(do)
                 indices = ds + do
                 if indices in mul_coeff:
                     mul_coeff[indices] += cs*co
                 else:
                     mul_coeff[indices] = cs*co
-        return self.construct_with_default([(d, c) for (d, c) in mul_coeff.iteritems() if c])
+        return self.construct_with_default([(d, c) for (d, c) in mul_coeff.items() if c])
 
     def scalar_mul(self, scale):
         """
         Return the result of scalar multiplication.
         """
         return self.construct_with_default([(i, c * scale) for (i, c) in self if c])
 
     def term_mul(self, term):
         """
         Return the result of multiplication with the given term.
         The term can be given as a tuple (degree indices, coeff)
         or as a Polynomial instance.
         """
         if isinstance(term, PolynomialInterface):
-            degrees, coeff = iter(term).next()
+            degrees, coeff = next(iter(term))
         else:
             degrees, coeff = term
         return self.construct_with_default([(d + degrees, c * coeff) for (d, c) in self])
 
     def __pow__(self, index):
         """
         self ** index
@@ -315,15 +315,15 @@
                 result = polynomial([(i * 2, c ** 2)])
         # binomial
         elif data_length == 2:
             (i1, c1), (i2, c2) = [(i, c) for (i, c) in self]
             result = polynomial({i1 * 2: c1**2, i1 + i2: c1*c2*2, i2 * 2: c2**2})
         # general (recursive)
         else:
-            half = data_length // 2
+            half = data_length >> 1
             coefficients = [(i, c) for (i, c) in self]
             left, right = polynomial(coefficients[:half], **self._init_kwds), polynomial(coefficients[half:])
             result = left.square() + left * right * 2 + right.square()
         return result
 
     def __hash__(self):
         """
@@ -343,29 +343,29 @@
         If 'target' is a tuple of indices, it has to be sorted and
         'value' also has to be a tuple of the same length.
 
         Note that the result will not be a univar polynomial nor a
         scalar.
         """
         result = {}
-        if isinstance(target, (int, long)):
+        if isinstance(target, int):
             for i, c in self:
                 deg, index = i[target], i[:target] + (0,) + i[target + 1:]
                 if index in result:
                     result[index] += c * value ** deg
                 else:
                     result[index] = c * value ** deg
         elif len(target) == len(value):
             substituted = self
             for var, val in zip(target[::-1], value[::-1]):
                 substituted = substituted(var, val)
             return substituted
         else:
             raise TypeError("argument lengths mismatsch")
-        return self.__class__([(i, c) for (i, c) in result.iteritems() if c], **self._init_kwds)
+        return self.__class__([(i, c) for (i, c) in result.items() if c], **self._init_kwds)
 
     def __len__(self):
         """
         Return the number of data entries.
         """
         return len(self._coefficients)
 
@@ -376,41 +376,41 @@
         """
         return self._coefficients.get(index, 0)
 
     def iterterms(self):
         """
         iterator for (degree, coefficient) pairs.
         """
-        return self._coefficients.iteritems()
+        return iter(self._coefficients.items())
 
     def itercoefficients(self):
         """
         iterator for coefficients.
         """
-        return self._coefficients.itervalues()
+        return iter(self._coefficients.values())
 
     def iterbases(self):
         """
         iterator for degrees.
         """
-        return self._coefficients.iterkeys()
+        return iter(self._coefficients.keys())
 
     def partial_differentiate(self, target):
         """
         Return the polynomial obtained by partial differentiation with
         the 'target' index variable.
         """
         partial = {}
         for i, c in self:
             index_diffed = list(i)
             target_degree = index_diffed[target]
             index_diffed[target] -= 1
             index_diffed = tuple(i)
             partial[index_diffed] = target_degree * c
-        return self.construct_with_default([(i, c) for (i, c) in partial.iteritems() if c])
+        return self.construct_with_default([(i, c) for (i, c) in partial.items() if c])
 
     def erase_variable(self, target=0):
         """
         Erase a variable from the polynomial.  The target variable is
         specified by the position in indices.
 
         The method takes no care about resulting polynomial type, i.e.
@@ -421,32 +421,32 @@
         for term, coeff in self:
             term = term[:target] + term[target + 1:]
             if term in result:
                 result[term] += coeff
             else:
                 result[term] = coeff
 
-        return self.__class__([(d, c) for (d, c) in result.iteritems() if c],
+        return self.__class__([(d, c) for (d, c) in result.items() if c],
                               number_of_variables=(self.number_of_variables - 1),
                               **self._init_kwds)
 
     def combine_similar_terms(self, target):
         """
         Combine similar terms and return the resulting univariate
         polynomial with polynomial coefficients in the form of list of
         (degree, coefficient) pairs.  The target variable is specified
         by the position in indices.
         """
         zero = self.construct_with_default(())
         result = {}
         for i, c in self:
             result[i[target]] = result.get(i[target], zero) + self.__class__([(i, c)], **self._init_kwds)
-        for i, c in result.iteritems():
+        for i, c in result.items():
             result[i] = c.erase_variable(target)
-        return result.items()
+        return list(result.items())
 
     def __repr__(self): # debug use
         return "BasicPolynomial(%s)" % repr(self._coefficients)
 
     def construct_with_default(self, maindata):
         """
         Create a new multivar polynomial of the same class with self,
```

### Comparing `NZMATH-1.1.0/nzmath/poly/univar.py` & `nzmath-3.0.0/src/poly/univar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Univariate Polynomials
 
 The polynomials are immutable data types, under the public API.  If
 one tries to manipulate its underlying data attributes, immutability
 will be able to be broken.
 """
 
-from __future__ import division
+
 import warnings
 import nzmath.ring as _ring
 import nzmath.poly.formalsum as formalsum
 
 
 class PolynomialInterface(formalsum.FormalSumContainerInterface):
     """
@@ -35,14 +35,18 @@
             return formalsum.FormalSumContainerInterface.__eq__(self, other)
         sterms = [t for t in self.iterterms() if t[1]]
         sterms.sort()
         oterms = [t for t in other.iterterms() if t[1]]
         oterms.sort()
         return sterms == oterms
 
+    def __hash__(self):
+       val = sum([hash(t) for t in self.iterterms() if t[1]])
+       return val
+
     def __pow__(self, index):
         """
         self ** index
         """
         raise NotImplementedError("should be overridden")
 
     def ring_mul(self, other):
@@ -53,30 +57,30 @@
         for ds, cs in self:
             for do, co in other:
                 term_degree = ds + do
                 if term_degree in mul_coeff:
                     mul_coeff[term_degree] += cs*co
                 else:
                     mul_coeff[term_degree] = cs*co
-        return self.construct_with_default(sorted([(d, c) for (d, c) in mul_coeff.iteritems() if c]))
+        return self.construct_with_default(sorted([(d, c) for (d, c) in mul_coeff.items() if c]))
 
     def scalar_mul(self, scale):
         """
         Return the result of scalar multiplication.
         """
         return self.construct_with_default([(d, c * scale) for (d, c) in self if c])
 
     def term_mul(self, term):
         """
         Return the result of multiplication with the given term.
         The term can be given as a tuple (degree, coeff) or as a
         Polynomial instance.
         """
         if isinstance(term, PolynomialInterface):
-            degree, coeff = iter(term).next()
+            degree, coeff = next(iter(term))
         else:
             degree, coeff = term
         return self.construct_with_default([(d + degree, c * coeff) for (d, c) in self])
 
     def square(self):
         """
         Return square of this polynomial.
@@ -161,27 +165,27 @@
         """
         sum_coeff = dict(iter(self))
         for term, coeff in other:
             if term in sum_coeff:
                 sum_coeff[term] += coeff
             else:
                 sum_coeff[term] = coeff
-        return self.construct_with_default([(d, c) for (d, c) in sum_coeff.iteritems() if c])
+        return self.construct_with_default([(d, c) for (d, c) in sum_coeff.items() if c])
 
     def __sub__(self, other):
         """
         self - other
         """
         dif_coeff = dict(iter(self))
         for term, coeff in other:
             if term in dif_coeff:
                 dif_coeff[term] -= coeff
             else:
                 dif_coeff[term] = -coeff
-        return self.construct_with_default([(d, c) for (d, c) in dif_coeff.iteritems() if c])
+        return self.construct_with_default([(d, c) for (d, c) in dif_coeff.items() if c])
 
     def __mul__(self, other):
         """
         self * other
 
         If type of other is Polynomial, do multiplication in ring.
         Otherwise, do scalar multiplication.
@@ -231,17 +235,17 @@
         if data_length == 1:
             return self.construct_with_default([(d*2, c**2) for (d, c) in self])
         # binomial
         if data_length == 2:
             (d1, c1), (d2, c2) = self.terms()
             return self.construct_with_default({d1*2:c1**2, d1+d2:c1*c2*2, d2*2:c2**2})
         # general (inefficient)
-        items = self._coefficients.items()
+        items = list(self._coefficients.items())
         fst, snd = {}, {}
-        if data_length % 2 == 1:
+        if data_length & 1:
             b, c = items.pop()
             fst[b] = c
         while items:
             b, c = items.pop()
             fst[b] = c
             b, c = items.pop()
             snd[b] = c
@@ -285,42 +289,42 @@
                 power_of_2 = power_of_2.square()
         return power_product
 
     def __call__(self, val):
         """
         substitution
         """
-        items = self._coefficients.items()
+        items = list(self._coefficients.items())
         if not items:
             return 0*val
         d, c = items.pop()
         result = c * val**d
         for d, c in items:
             result += c * val**d
         return result
 
     def iterterms(self):
         """
         iterator for (degree, coefficient) pairs.
         The iterator is equivalent to
           zip(self.iterbases(), self.itercoefficients())
         """
-        return self._coefficients.iteritems()
+        return iter(self._coefficients.items())
 
     def itercoefficients(self):
         """
         iterator for coefficients.
         """
-        return self._coefficients.itervalues()
+        return iter(self._coefficients.values())
 
     def iterbases(self):
         """
         iterator for degrees.
         """
-        return self._coefficients.iterkeys()
+        return iter(self._coefficients.keys())
 
     def __getitem__(self, degree):
         """
         Return the coefficient of specified degree.
         If there is no term of degree, return 0.
         """
         return self._coefficients.get(degree, 0)
@@ -342,14 +346,17 @@
         """
         self == other
         """
         if self is other:
             return True
         return PolynomialInterface.__eq__(self, other)
 
+    def __hash__(self):
+        return PolynomialInterface.__hash__(self)
+
     def __repr__(self): # for debug
         return "%s(%s)" % (self.__class__.__name__, repr(self._coefficients))
 
 
 class SortedPolynomial (PolynomialInterface):
     """
     SortedPolynomial stores terms of a polynomial in sorted manner.
@@ -362,50 +369,41 @@
         'coefficients' can be any dict initial values.
         Optionally '_sorted' can be True if the coefficients is
         already sorted.
         """
         PolynomialInterface.__init__(self, coefficients, **kwds)
         self.sorted = []
         if not _sorted or isinstance(coefficients, dict):
-            for t in dict(coefficients).iteritems():
+            for t in dict(coefficients).items():
                 self._insort(t)
         else:
             self.sorted = list(coefficients)
         self._init_kwds = kwds
         self._init_kwds['_sorted'] = True
 
     def _insort(self, term):
         """
         Insert the term into self.seorted list, and keep it sorted.
 
         - This method is destructive.
         - This method is not in a part of the API.
-        - The code is just adapting bisect.insort_right to the
-          context.
         """
-        lo, hi = 0, len(self.sorted)
-        while lo < hi:
-            mid = (lo + hi) // 2
-            if term[0] < self.sorted[mid][0]:
-                hi = mid
-            else:
-                lo = mid + 1
-        self.sorted.insert(lo, term)
+        self.sorted.insert(self._bisect(term[0]), term)
 
     def _bisect(self, degree):
         """
         Return the index where to insert term of degree.
 
         - This method is not in a part of the API.
         - The code is just adapting bisect.bisect_right to the
           context.
         """
         lo, hi = 0, len(self.sorted)
         while lo < hi:
-            mid = (lo + hi) // 2
+            mid = (lo + hi) >> 1
             if degree < self.sorted[mid][0]:
                 hi = mid
             else:
                 lo = mid + 1
         return lo
 
     def __pos__(self):
@@ -422,50 +420,50 @@
 
     def __add__(self, other):
         """
         self + other
         """
         if self.sorted:
             iter_self = iter(self.sorted)
-            self_term = iter_self.next()
+            self_term = next(iter_self)
         else:
             self_term = None
         if other.sorted:
             iter_other = iter(other.sorted)
-            other_term = iter_other.next()
+            other_term = next(iter_other)
         else:
             other_term = None
         sorted = []
         while self_term and other_term:
             compared = cmp(self_term[0], other_term[0])
             if compared < 0:
                 sorted.append(self_term)
                 try:
-                    self_term = iter_self.next()
+                    self_term = next(iter_self)
                 except StopIteration:
                     self_term = None
                     break
             elif compared == 0:
                 c = self_term[1] + other_term[1]
                 if c:
                     sorted.append((self_term[0], c))
                 try:
-                    self_term = iter_self.next()
+                    self_term = next(iter_self)
                 except StopIteration:
                     self_term = None
                 try:
-                    other_term = iter_other.next()
+                    other_term = next(iter_other)
                 except StopIteration:
                     other_term = None
                 if self_term is None or other_term is None:
                     break
             else:
                 sorted.append(other_term)
                 try:
-                    other_term = iter_other.next()
+                    other_term = next(iter_other)
                 except StopIteration:
                     other_term = None
                     break
         if other_term is None and self_term:
             sorted.append(self_term)
             for term in iter_self:
                 sorted.append(term)
@@ -479,50 +477,50 @@
         """
         self - other
 
         It is something like merge sort.
         """
         if self.sorted:
             iter_self = iter(self.sorted)
-            self_term = iter_self.next()
+            self_term = next(iter_self)
         else:
             self_term = None
         if other.sorted:
             iter_other = iter(other.sorted)
-            other_term = iter_other.next()
+            other_term = next(iter_other)
         else:
             other_term = None
         sorted = []
         while self_term and other_term:
             compared = cmp(self_term[0], other_term[0])
             if compared < 0:
                 sorted.append(self_term)
                 try:
-                    self_term = iter_self.next()
+                    self_term = next(iter_self)
                 except StopIteration:
                     self_term = None
                     break
             elif compared == 0:
                 c = self_term[1] - other_term[1]
                 if c:
                     sorted.append((self_term[0], c))
                 try:
-                    self_term = iter_self.next()
+                    self_term = next(iter_self)
                 except StopIteration:
                     self_term = None
                 try:
-                    other_term = iter_other.next()
+                    other_term = next(iter_other)
                 except StopIteration:
                     other_term = None
                 if self_term is None or other_term is None:
                     break
             else:
                 sorted.append((other_term[0], -other_term[1]))
                 try:
-                    other_term = iter_other.next()
+                    other_term = next(iter_other)
                 except StopIteration:
                     other_term = None
                     break
         if other_term is None and self_term:
             sorted.append(self_term)
             for term in iter_self:
                 sorted.append(term)
@@ -585,15 +583,15 @@
         # suppose self is black and other is red.
         black_left_degree, black_right_degree = self.sorted[0][0], self.sorted[-1][0]
         red_left_degree, red_right_degree = other.sorted[0][0], other.sorted[-1][0]
         left_degree = min(black_left_degree, red_left_degree)
         right_degree = max(black_right_degree, red_right_degree)
         # we assert here that order is of ascending. (is it correct?)
         assert left_degree < right_degree
-        half_degree = (left_degree + right_degree) // 2
+        half_degree = (left_degree + right_degree) >> 1
         black_half_index = self._bisect(half_degree)
         red_half_index = other._bisect(half_degree)
         if not black_half_index:
             return (self.downshift_degree(black_left_degree).ring_mul_karatsuba(other)).upshift_degree(black_left_degree)
         if not red_half_index:
             return (self.ring_mul_karatsuba(other.downshift_degree(red_left_degree))).upshift_degree(red_left_degree)
         club = polynomial([(d - left_degree, c) for (d, c) in self.sorted[:black_half_index]])
@@ -651,15 +649,15 @@
         # binomial
         if data_length == 2:
             (d1, c1), (d2, c2) = [(d, c) for (d, c) in self]
             return polynomial({d1*2:c1**2, d1+d2:c1*c2*2, d2*2:c2**2})
         # general (Karatsuba)
         right_degree = self.sorted[-1][0]
         left_degree = self.sorted[0][0]
-        half_degree = (right_degree + left_degree) // 2
+        half_degree = (right_degree + left_degree) >> 1
         half_index = self._bisect(half_degree)
         fst = polynomial([(d - left_degree, c) for (d, c) in self.sorted[:half_index]])
         snd = polynomial([(d - half_degree, c) for (d, c) in self.sorted[half_index:]])
         fst_squared = fst.square()
         snd_squared = snd.square()
         karatsuba = (fst + snd).square() - fst_squared - snd_squared
         if left_degree:
@@ -796,14 +794,18 @@
             return True
         if not isinstance(other, SortedPolynomial):
             return PolynomialInterface.__eq__(self, other)
         if [t for t in self if t[1]] == [t for t in other if t[1]]:
             return True
         return False
 
+    def __hash__(self):
+        val = sum([hash(t) for t in self if t[1]])
+        return val
+
     def __call__(self, val):
         """
         substitution
         """
         items = list(self.sorted)
         if not items:
             return 0 * val
@@ -813,11 +815,11 @@
         while len(items) > 0:
             (e, f) = items.pop()
             result = result * val_pow.setdefault(d - e, val ** (d - e)) + f
             d = e
         if d:
             return result * val_pow.get(d, val ** d)
         else:
-            return result 
+            return result
 
     def __repr__(self): # debug
         return repr(self.sorted)
```

### Comparing `NZMATH-1.1.0/nzmath/poly/groebner.py` & `nzmath-3.0.0/src/poly/groebner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Groebner basis
 """
 
-from __future__ import division
+
 import nzmath.compatibility
 import nzmath.ring as ring
 
 
 def s_polynomial(f, g, order):
     """
     Return S-polynomial of f and g with respect to the order.
@@ -114,15 +114,15 @@
             lb_g = order.leading_term(g)[0]
             lcm_f_g = lb_f.lcm(lb_g)
             if lcm_f_g == lb_f + lb_g: # disjoint
                 treat.add((i, j))
                 treat.add((j, i))
             else:
                 # keep lcms sorted, and so pairs in paralell
-                k = _bisect(lcms, lcm_f_g, order)
+                k = order.bisect(lcms, lcm_f_g)
                 pairs.insert(k, (i, j))
                 lcms.insert(k, lcm_f_g)
 
     # main loop
     while pairs:
         i, j = pairs.pop(0)
         lcm_f_g = lcms.pop(0)
@@ -140,39 +140,14 @@
                 hindex = len(groebner)
                 for i, f in enumerate(groebner):
                     lb_f = order.leading_term(f)[0]
                     lcm_f_h = lb_f.lcm(lb_h)
                     if lcm_f_h == lb_f + lb_h: # disjoint
                         treat.add((i, hindex))
                     else:
-                        k = _bisect(lcms, lcm_f_h, order)
+                        k = order.bisect(lcms, lcm_f_h)
                         pairs.insert(k, (i, hindex))
                         lcms.insert(k, lcm_f_h)
                 groebner.append(h)
 
     # finish
     return groebner
-
-def _bisect(a, x, order, lo=0, hi=None):
-    """
-    Return the index where to insert item x in list a, assuming a is
-    sorted with the order.
-
-    The return value i is such that all e in a[:i] have e <= x, and
-    all e in a[i:] have e > x.  So if x already appears in the list,
-    a.insert(x) will insert just after the rightmost x already there.
-
-    Optional args lo (default 0) and hi (default len(a)) bound the
-    slice of a to be searched.
-
-    This function is based on the bisect.bisect_right of the Python
-    standard library.
-    """
-
-    if hi is None:
-        hi = len(a)
-    while lo < hi:
-        mid = (lo + hi) // 2
-        if order.cmp(x, a[mid]) < 0:
-            hi = mid
-        else: lo = mid + 1
-    return lo
```

### Comparing `NZMATH-1.1.0/nzmath/poly/factor.py` & `nzmath-3.0.0/src/poly/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 import nzmath.arith1 as arith1
 import nzmath.prime as prime
 import nzmath.rational as rational
 import nzmath.combinatorial as combinatorial
 import nzmath.intresidue as intresidue
 import nzmath.finitefield as finitefield
 import nzmath.poly.uniutil as uniutil
@@ -169,15 +169,15 @@
     coefficientRing = f.getCoefficientRing()
     if isinstance(coefficientRing, intresidue.IntegerResidueClassRing):
         p = coefficientRing.m
     elif isinstance(coefficientRing, finitefield.FinitePrimeField):
         p = coefficientRing.getCharacteristic()
     else:
         raise TypeError("unknown ring (%s)" % repr(coefficientRing))
-    half = p // 2
+    half = p >> 1
     g = {}
     for i, c in f.iterterms():
         if c.n > half:
             g[i] = c.n - p
         else:
             g[i] = c.n
     return uniutil.polynomial(g, rational.theIntegerRing)
@@ -193,15 +193,15 @@
     """
     weight = 0
     for c in f.itercoefficients():
         weight += abs(c)**2
     weight = arith1.floorsqrt(weight) + 1
     degree = f.degree()
     lc = f[degree]
-    m = degree // 2 + 1
+    m = (degree >> 1) + 1
     bound = 1
     for i in range(1, m):
         b = combinatorial.binomial(m - 1, i) * weight + \
             combinatorial.binomial(m - 1, i - 1) * lc
         if bound < b:
             bound = b
     return bound
```

### Comparing `NZMATH-1.1.0/nzmath/poly/ratfunc.py` & `nzmath-3.0.0/src/poly/ratfunc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 rational functions
 """
 
-from __future__ import division
+
 import nzmath.ring as ring
 import nzmath.poly.ring as poly_ring
 
 
 class RationalFunction(ring.QuotientFieldElement):
     """
     The class of rational functions.
@@ -47,14 +47,20 @@
         equality test
         """
         try:
             return ring.QuotientFieldElement.__eq__(self, other)
         except AttributeError:
             return NotImplemented
 
+    def __hash__(self):
+        try:
+            return ring.QuotientFieldElement.__hash__(self)
+        except AttributteError:
+            return NotImplemented
+
     def __call__(self, *args):
         """
         evaluation
 
         The type of args depends on the type of polynomials
         representing numerator and denominator.
         """
```

### Comparing `NZMATH-1.1.0/nzmath/poly/formalsum.py` & `nzmath-3.0.0/src/poly/formalsum.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 import nzmath.compatibility
 
 
 class FormalSumContainerInterface (object):
     """
     Interface of formal sum container.
-    Do not instanciate.
+    Do not instantiate.
     """
     def __iter__(self):
         """
         Return the iterator.
         It is an alias of iterterms.
         """
         return self.iterterms()
@@ -85,21 +85,25 @@
         if self_bases != other_bases:
             return False
         for base in self_bases:
             if self[base] != other[base]:
                 return False
         return True
 
+    def __hash__(self):
+        val = sum([hash(self[base]) for base in set(self.iterbases())]) 
+        return val
+
     def __ne__(self, other):
         """
         self != other
         """
         return not self.__eq__(other)
 
-    def __nonzero__(self):
+    def __bool__(self):
         """
         Return True, if self has some nonzero coefficients.
         False, otherwise.
         """
         for c in self.itercoefficients():
             if c:
                 return True
@@ -120,27 +124,27 @@
         """
         sum_coeff = dict(self.iterterms())
         for base, coeff in other:
             if base in sum_coeff:
                 sum_coeff[base] += coeff
             else:
                 sum_coeff[base] = coeff
-        return self.construct_with_default([(b, c) for (b, c) in sum_coeff.iteritems() if c])
+        return self.construct_with_default([(b, c) for (b, c) in sum_coeff.items() if c])
 
     def __sub__(self, other):
         """
         self - other
         """
         sub_coeff = dict(self.iterterms())
         for base, coeff in other:
             if base in sub_coeff:
                 sub_coeff[base] -= coeff
             else:
                 sub_coeff[base] = -coeff
-        return self.construct_with_default([(b, c) for (b, c) in sub_coeff.iteritems() if c])
+        return self.construct_with_default([(b, c) for (b, c) in sub_coeff.items() if c])
 
     def __neg__(self):
         """
         -self
         """
         raise NotImplementedError("method '__neg__' should be overridden")
 
@@ -185,27 +189,27 @@
         """
         raise NotImplementedError("method 'iterbases' must be overridden")
 
     def terms(self):
         """
         Return a list of terms as (base, coefficient) pairs.
         """
-        return [t for t in self.iterterms()]
+        return list(self.iterterms())
 
     def coefficients(self):
         """
         Return a list of all coefficients.
         """
-        return [c for c in self.itercoefficients()]
+        return list(self.itercoefficients())
 
     def bases(self):
         """
         Return a list of all bases.
         """
-        return [b for b in self.iterbases()]
+        return list(self.iterbases())
 
     def terms_map(self, func):
         """
         Create a new formal sum container by applying func to each
         term.  func must be a function taking 2 arguments.
         """
         terms = []
@@ -311,40 +315,44 @@
             return True
         if not isinstance(other, DictFormalSum):
             return FormalSumContainerInterface.__eq__(self, other)
         if self._data == other._data:
             return True
         return False
 
+    def __hash__(self):
+        val = sum([hash(ele) for ele in self._data]) 
+        return val
+   
     def __getitem__(self, base):
         """
         self[base]
 
         no KeyError will be raised. Insteads, it returns defaultvalue
         specified on time of initialization.
         """
         return self._data.get(base, self._defaultvalue)
 
     def iterterms(self):
         """
         iterator for (base, coefficient) pairs.
         """
-        return self._data.iteritems()
+        return iter(self._data.items())
 
     def itercoefficients(self):
         """
         iterator for coefficients.
         """
-        return self._data.itervalues()
+        return iter(self._data.values())
 
     def iterbases(self):
         """
         iterator for bases.
         """
-        return self._data.iterkeys()
+        return iter(self._data.keys())
 
     def __len__(self):
         """
         len(self)
 
         Return the number of terms.
         """
@@ -429,14 +437,18 @@
             return True
         if not isinstance(other, ListFormalSum):
             return FormalSumContainerInterface.__eq__(self, other)
         if set(self._data) == set(other._data):
             return True
         return False
 
+    def __hash__(self):
+        val = sum([hash(ele) for ele in set(self._data)]) 
+        return val
+
     def __getitem__(self, base):
         """
         self[base]
 
         no KeyError will be raised. Insteads, it returns defaultvalue
         specified on time of initialization.
         """
```

### Comparing `NZMATH-1.1.0/nzmath/poly/hensel.py` & `nzmath-3.0.0/src/poly/hensel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 If you need lifted factors only once, you may want to use lift_upto
 function.  On the other hand, if you might happen to need another
 lift, you would directly use one of the lifters and its lift method
 for consecutive lifts.
 """
 
-from __future__ import division
+
 import sys
 import nzmath.arith1 as arith1
 import nzmath.rational as rational
 import nzmath.poly.ring as polyring
 
 
 # module globals
@@ -331,28 +331,28 @@
             self.dis.append(self.f.coefficients_map(lambda c: (c // q) % self.p))
             rest -= self.dis[-1].scalar_mul(q)
             q *= self.p
         if self.f != rest:
             self.dis.append(rest.scalar_exact_division(q))
 
     @classmethod
-    def from_factors(cls, target, factors, p, ubound=sys.maxint):
+    def from_factors(cls, target, factors, p, ubound=sys.maxsize):
         """
         Create and return an instance of HenselLiftSimultaneously,
         whose factors are lifted by HenselLiftMulti upto ubound (if it
         is smaller than sys.maxint, or upto sys.maxint).
 
         HenselLiftSimultaneously.from_factors(f, factors, p)
 
         The parameters satisfy that:
           f == a1*...*ar (mod p)
         with a prime number p and ai's in factors.
         """
         lifter = HenselLiftMulti.from_factors(target, factors, p)
-        interbound = min(ubound, sys.maxint)
+        interbound = min(ubound, sys.maxsize)
         while lifter.p < interbound:
             lifter.lift_factors()
             lifter.lift_ladder()
         new = cls(target, lifter.a, lifter.b, (lifter.s, lifter.t), lifter.p)
         new.first_lift()
         return new
 
@@ -374,15 +374,15 @@
         if len(self.dis) > 1:
             mini_target = self.dis[0] + self.dis[1].scalar_mul(self.p)
             self._assertEqualModulo(self.f, mini_target, self.p**2)
         else:
             mini_target = self.dis[0]
         aj, bj = [], []
         self.uis, self.yis, self.zis = [], {}, {}
-        for i in xrange(self.r - 1):
+        for i in range(self.r - 1):
             dividend = mini_target - self.gis[i] * self.his[i]
             self.uis.append(dividend.scalar_exact_division(self.p))
             self.yis[i], self.zis[i] = self._solve_yz(i)
             aj.append(self.gis[i] + self.zis[i].scalar_mul(self.q))
             bj.append(self.his[i] + self.yis[i].scalar_mul(self.q))
             self._assertEqualModulo(mini_target, aj[i]*bj[i], self.q*self.p)
             mini_target = bj[i]
@@ -410,15 +410,15 @@
             mini_target = self.dis[j]
         else:
             mini_target = the_zero
 
         self.ais[-2], self.ais[-1] = self.ais[-1], self.ais[0]
         self.bis[-2], self.bis[-1] = self.bis[-1], self.bis[0]
         aj, bj = [], []
-        for i in xrange(self.r - 1):
+        for i in range(self.r - 1):
             yi, zi = self.yis[i], self.zis[i]
             dividend = self.ais[-2][i]*yi + self.bis[-2][i]*zi - self.uis[i]
             v_j = dividend.scalar_exact_division(self.p)
             if j == 2:
                 self.uis[i] = mini_target - v_j - yi*zi
             else:
                 self.uis[i] = mini_target - v_j - (yi*zi).scalar_mul(self.p**(j - 2))
@@ -499,14 +499,14 @@
     target == product(factors) mod p
     POSTCONDITIONS:
     there exist k s.t. q == p**k >= bound and
     target == product(result) mod q
     """
     if len(factors) == 2:
         lifter = HenselLiftPair.from_factors(target, factors[0], factors[1], p)
-    elif bound < sys.maxint:
+    elif bound < sys.maxsize:
         lifter = HenselLiftMulti.from_factors(target, factors, p)
     else:
         lifter = HenselLiftSimultaneously.from_factors(target, factors, p)
     while lifter.q < bound:
         lifter.lift()
     return lifter.factors, lifter.q
```

### Comparing `NZMATH-1.1.0/nzmath/poly/ring.py` & `nzmath-3.0.0/src/poly/ring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 base classes for polynomial rings and rational function fields.
 """
 
-from __future__ import division
+
 import nzmath.ring as ring
 import nzmath.poly.termorder as termorder
 import nzmath.poly.univar as univar
 import nzmath.poly.multivar as multivar
 
 
 class PolynomialRing(ring.CommutativeRing):
@@ -283,15 +283,15 @@
         """
         if not elem.getRing().issubring(self.ring):
             return False
         if self.generators == [self.ring.zero]:
             return elem == self.ring.zero
         return not self.reduce(elem)
 
-    def __nonzero__(self):
+    def __bool__(self):
         """
         Report whether the ideal is zero ideal or not.  Of course,
         False is for zero ideal.
         """
         return self.generators and self.generators != [self.ring.zero]
 
     def __repr__(self):
```

### Comparing `NZMATH-1.1.0/nzmath/poly/uniutil.py` & `nzmath-3.0.0/src/poly/uniutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Utilities for univar.
 
 The module provides higher level interfaces to univar classes and
 functions.
 """
 
-from __future__ import division
+
 import logging
 import nzmath.arith1 as arith1
 import nzmath.bigrandom as bigrandom
 import nzmath.gcd as gcd
 import nzmath.rational as rational
 import nzmath.ring as ring
 import nzmath.poly.univar as univar
@@ -27,15 +27,15 @@
 
 class OrderProvider(object):
     """
     OrderProvider provides order and related operations.
     """
     def __init__(self, order=termorder.ascending_order):
         """
-        Do not instanciate OrderProvider.
+        Do not instantiate OrderProvider.
         This initializer should be called from descendant:
           OrderProvider.__init__(self, order)
         where order is default to termorder.ascending_order.
         """
         if type(self) is OrderProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         self.order = order
@@ -83,15 +83,15 @@
 
     The class should be used as a mix-in.
 
     REQUIRE: OrderProvider
     """
     def __init__(self):
         """
-        Do not instanciate DivisionProvider.
+        Do not instantiate DivisionProvider.
         This initializer should be called from descendant.
         """
         if type(self) is DivisionProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         self._reduced = {}
 
     def __divmod__(self, other):
@@ -152,15 +152,15 @@
             return dividend
         upperbound = min(degree * 2, div_deg) + 1
         populate = False
         if not self._reduced:
             populate = True
         else:
             i = min(self._reduced.keys())
-            while i in self._reduced.keys():
+            while i in list(self._reduced.keys()):
                 i += 1
             if i < upperbound:
                 populate = True
         if populate:
             self._populate_reduced(degree, lc, upperbound)
         if div_deg > degree * 2:
             dividend_degrees = sorted(dividend.iterbases(), reverse=True)
@@ -183,34 +183,34 @@
         if not self:
             raise ZeroDivisionError("polynomial division or modulo by zero.")
         polynom %= self
         if index == 1 or not polynom:
             return polynom
         elif polynom.degree() == 0:
             return self.getRing().createElement([(0, polynom[0]**index)])
-        acoefficient = polynom.itercoefficients().next()
+        acoefficient = next(polynom.itercoefficients())
         one = ring.getRing(acoefficient).one
         power_product = self.construct_with_default([(0, one)])
         if index:
             power_of_2 = polynom
             while index:
-                if index % 2 == 1:
+                if index & 1:
                     power_product = self.mod(power_product * power_of_2)
                 power_of_2 = self.mod(power_of_2.square())
                 index //= 2
         return power_product
 
     def _populate_reduced(self, degree, lc, upperbound):
         """
         Populate self._reduced.
 
         degree, lc is of self, and self._reduced is populated up to
         the given upperbound.
         """
-        one = ring.getRing(self.itercoefficients().next()).one
+        one = ring.getRing(next(self.itercoefficients())).one
         if not self._reduced:
             minimum = degree
             redux = self.construct_with_default([(degree - 1, one)])
         else:
             minimum = max(self._reduced.keys()) + 1
             redux = self._reduced[minimum - 1]
         moniced = self.scalar_mul(one / lc)
@@ -254,15 +254,15 @@
         while stride * 2 <= maximum:
             stride += stride
             if stride not in self._reduced:
                 redux = self.mod(redux.square())
             else:
                 redux = self._reduced[stride]
             binary[stride] = redux
-        binarykeys = sorted(binary.keys(), reverse=True)
+        binarykeys = sorted(list(binary.keys()), reverse=True)
         for deg in (d for d in degrees if d > maxreduced):
             pickup = []
             rest = deg
             for key in binarykeys:
                 if rest < key:
                     continue
                 rest -= key
@@ -695,15 +695,15 @@
             if delta == 1 and h != g:
                 h = g
             elif delta > 1 and (g != one or h != one):
                 h = g * (h * g) ** (delta - 1)
 
     def subresultant_extgcd(self, other):
         """
-        Return (A, B, P) s.t. A*self+B*other=P, 
+        Return (A, B, P) s.t. A*self+B*other=P,
         where P is the greatest common divisor of given polynomials.
         They must be in the polynomial ring and its coefficient ring must
         be a UFD.
 
         Reference: Kida's paper p.18
         """
         order = termorder.ascending_order
@@ -737,15 +737,15 @@
 
     - A client of this mix-in class should use DivisionProvider also.
     - A client of this mix-in class must have attribute ch, which
       stores the prime characteristic of the coefficient ring.
     """
     def __init__(self, ch):
         """
-        Do not instanciate PrimeCharacteristicFunctionsProvider.
+        Do not instantiate PrimeCharacteristicFunctionsProvider.
         This initializer should be called from descendant.
         """
         if type(self) is PrimeCharacteristicFunctionsProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         self.ch = ch
 
     def __pow__(self, index, mod=None):
@@ -756,15 +756,15 @@
         the main class so that the __pow__ defined here would be
         preceded in method resolution order.  For example:
 
         class Client (PrimeCharacteristicFunctionsProvider
                       DivisionProvider,
                       Polynomial):
         """
-        if not isinstance(index, (int, long)):
+        if not isinstance(index, int):
             raise TypeError("index must be an integer.")
         if index < 0:
             raise ValueError("index must be a non-negative integer.")
         if mod is not None:
             return mod.mod_pow(self, index)
         if index > 0:
             if not self:
@@ -775,21 +775,21 @@
                 index //= self.ch
             if q > 1:
                 powered = self.construct_with_default([(d * q, c ** q) for (d, c) in self])
             else:
                 powered = self
         if index == 1:
             return powered
-        acoefficient = self.itercoefficients().next()
+        acoefficient = next(self.itercoefficients())
         one = ring.getRing(acoefficient).one
         power_product = self.construct_with_default([(0, one)])
         if index:
             power_of_2 = powered
             while index:
-                if index % 2 == 1:
+                if index & 1:
                     power_product *= power_of_2
                 power_of_2 = power_of_2.square()
                 index //= 2
         return power_product
 
     def mod_pow(self, polynom, index):
         """
@@ -798,15 +798,15 @@
         if not self:
             raise ZeroDivisionError("polynomial division or modulo by zero.")
         polynom %= self
         if index == 1 or not polynom:
             return polynom
         elif polynom.degree() == 0:
             return self.getRing().createElement([(0, polynom[0]**index)])
-        acoefficient = polynom.itercoefficients().next()
+        acoefficient = next(polynom.itercoefficients())
         cardfq = card(ring.getRing(acoefficient))
         final_product = self.getRing().one
         qpow = polynom
         # q-th power expansion
         while index:
             index, small = divmod(index, cardfq)
             if small == 1:
@@ -823,15 +823,15 @@
         Return polynom ** index % self for small index (0 < index < q).
         """
         # binary powering
         power_product = self.getRing().one
         if index > 0:
             power_of_2 = polynom
             while index:
-                if index % 2 == 1:
+                if index & 1:
                     power_product = self.mod(power_product * power_of_2)
                     if index == 1:
                         break
                 power_of_2 = self.mod(power_of_2.square())
                 index //= 2
         else:
             raise ValueError("this private method requires index > 0")
@@ -865,15 +865,15 @@
                         result[i] = r
                     a = c
                 i += 1
             f = b
         if self.order.degree(f) > 0:
             f = f.pthroot()
             subresult = f.squarefree_decomposition()
-            for i, g in subresult.iteritems():
+            for i, g in subresult.items():
                 result[i*self.ch] = g
         return result
 
     def pthroot(self):
         """
         Return a polynomial obtained by sending X**p to X, where p is
         the characteristic.  If the polynomial does not consist of
@@ -890,15 +890,15 @@
         having degree 1 and all irreducible factors of A2 having
         degree 2, then the result is:
           {1: A1, 2: A2}.
 
         The given polynomial must be square free, and its coefficient
         ring must be a finite field.
         """
-        Fq = ring.getRing(self.itercoefficients().next())
+        Fq = ring.getRing(next(self.itercoefficients()))
         q = card(Fq)
         f = self
         x = f.construct_with_default([(1, Fq.one)])
         w = x
         i = 1
         result = {}
         while i*2 <= self.order.degree(f):
@@ -917,15 +917,15 @@
     def split_same_degrees(self, degree):
         """
         Return the irreducible factors of the polynomial.  The
         polynomial must be a product of irreducible factors of the
         given degree.
         """
         r = self.order.degree(self) // degree
-        Fq = ring.getRing(self.itercoefficients().next())
+        Fq = ring.getRing(next(self.itercoefficients()))
         q = card(Fq)
         p = Fq.getCharacteristic()
         if degree == 1:
             result = []
             X = self.construct_with_default([(1, Fq.one)])
             f = self
             while not f[0]:
@@ -946,15 +946,15 @@
             if p == 2:
                 G = self.construct_with_default(())
                 for i in range(degree):
                     G = G + randpoly
                     randpoly = self.mod(randpoly.square())
             else:
                 one = self.construct_with_default([(0, Fq.one)])
-                G = pow(randpoly, (q**degree - 1)//2, self) - one
+                G = pow(randpoly, (q**degree - 1) >> 1, self) - one
             subresult = []
             while result:
                 h = result.pop()
                 if self.order.degree(h) == degree:
                     subresult.append(h)
                     continue
                 z = h.gcd(G)
@@ -975,17 +975,17 @@
         """
         result = []
         lc = self.order.leading_coefficient(self)
         if lc != ring.getRing(lc).one:
             self = self.scalar_exact_division(lc)
             result.append((self.getRing().one*lc, 1))
         squarefreefactors = self.squarefree_decomposition()
-        for m, f in squarefreefactors.iteritems():
+        for m, f in squarefreefactors.items():
             distinct_degree_factors = f.distinct_degree_factorization()
-            for d, g in distinct_degree_factors.iteritems():
+            for d, g in distinct_degree_factors.items():
                 if d == self.order.degree(g):
                     result.append((g, m))
                 else:
                     for irred in g.split_same_degrees(d):
                         result.append((irred, m))
         return result
 
@@ -1047,15 +1047,15 @@
         black_least_degree = self.order.tail_degree(self)
         black_most_degree = self.order.degree(self)
         red_least_degree = self.order.tail_degree(other)
         red_most_degree = self.order.degree(other)
         least_degree = min(black_least_degree, red_least_degree)
         most_degree = max(black_most_degree, red_most_degree)
         assert least_degree < most_degree
-        half_degree = (least_degree + most_degree) // 2
+        half_degree = (least_degree + most_degree) >> 1
 
         if black_least_degree > half_degree:
             return self.downshift_degree(black_least_degree).ring_mul_karatsuba(other).upshift_degree(black_least_degree)
         if red_least_degree > half_degree:
             return self.ring_mul_karatsuba(other.downshift_degree(red_least_degree)).upshift_degree(red_least_degree)
 
         black = self.downshift_degree(least_degree)
@@ -1077,15 +1077,15 @@
         if not self:
             return self
 
         polynomial = self.construct_with_default
         data_length = len(self)
         # monomial
         if data_length == 1:
-            d, c = iter(self).next()
+            d, c = next(iter(self))
             if d:
                 return polynomial([(d*2, c**2)])
             else:
                 return polynomial([(0, c**2)])
         # binomial
         if data_length == 2:
             (d1, c1), (d2, c2) = [(d, c) for (d, c) in self]
@@ -1094,15 +1094,15 @@
             return polynomial({d1*2:c1**2, d1+d2:c1*c2*2, d2*2:c2**2}, _sorted=False)
         # general (Karatsuba)
         least_degree = self.order.tail_degree(self)
         if least_degree:
             chopped = self.downshift_degree(least_degree)
         else:
             chopped = self
-        half_degree = self.order.degree(self) // 2
+        half_degree = self.order.degree(self) >> 1
         fst, snd = chopped.split_at(half_degree)
         fst_squared = fst.square()
         snd_squared = snd.square()
         karatsuba = (fst + snd).square() - fst_squared - snd_squared
         result = (fst_squared +
                   karatsuba.upshift_degree(half_degree) +
                   snd_squared.upshift_degree(half_degree * 2))
@@ -1115,15 +1115,15 @@
 class VariableProvider(object):
     """
     VariableProvider provides the variable name and other cariable
     related methods.
     """
     def __init__(self, varname):
         """
-        Do not instanciate VariableProvider.
+        Do not instantiate VariableProvider.
         This initializer should be called from descendant.
         """
         if type(self) is VariableProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         self.variable = varname
 
     def getVariable(self):
@@ -1141,15 +1141,15 @@
 
 class RingElementProvider(ring.CommutativeRingElement):
     """
     Provides interfaces for ring.CommutativeRingElement.
     """
     def __init__(self):
         """
-        Do not instanciate RingElementProvider.
+        Do not instantiate RingElementProvider.
         This initializer should be called from descendant:
           RingElementProvider.__init__(self)
         """
         if type(self) is RingElementProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         ring.CommutativeRingElement.__init__(self)
         self._coefficient_ring = None
@@ -1192,16 +1192,16 @@
 
         - coefficients: initializer for polynomial coefficients
         - coeffring: commutative ring
         """
         if coeffring is None:
             raise TypeError("argument `coeffring' is required")
         coefficients = dict(coefficients)
-        if coefficients and coefficients.itervalues().next() not in coeffring:
-            coefficients = [(d, coeffring.createElement(c)) for (d, c) in coefficients.iteritems()]
+        if coefficients and next(iter(coefficients.values())) not in coeffring:
+            coefficients = [(d, coeffring.createElement(c)) for (d, c) in coefficients.items()]
             _sorted = False
         kwds["coeffring"] = coeffring
         univar.SortedPolynomial.__init__(self, coefficients, _sorted, **kwds)
         OrderProvider.__init__(self, termorder.ascending_order)
         RingElementProvider.__init__(self)
         self.set_coefficient_ring(coeffring)
 
@@ -1267,15 +1267,15 @@
 
     def __getitem__(self, degree):
         """
         Return the coefficient of specified degree.
         If there is no term of degree, return 0.
         """
         result = univar.SortedPolynomial.__getitem__(self, degree)
-        if result is 0:
+        if result == 0: # 'is 0'-->'== 0'
             result = self._coefficient_ring.zero
         return result
 
 
 class DomainPolynomial(PseudoDivisionProvider,
                        RingPolynomial):
     """
@@ -1297,15 +1297,15 @@
 
     def discriminant(self):
         """
         Return discriminant of the polynomial.
         """
         df = self.differentiate()
         lc = self.leading_coefficient()
-        if self.degree() % 4 in (2, 3):
+        if self.degree() & 3 in (2, 3):
             sign = -1
         else:
             sign = 1
         if self.getCoefficientRing().getCharacteristic() == 0:
             if lc != 1:
                 return sign * self.resultant(df) / lc
             else:
@@ -1364,21 +1364,21 @@
     Polynomial with integer coefficients.
 
     This class is required because special initialization must be done
     for built-in int/long.
     """
     def __init__(self, coefficients, coeffring=None, _sorted=False, **kwds):
         dc = dict(coefficients)
-        coefficients = [(d, rational.IntegerIfIntOrLong(c)) for (d, c) in dc.iteritems()]
+        coefficients = [(d, rational.IntegerIfIntOrLong(c)) for (d, c) in dc.items()]
         UniqueFactorizationDomainPolynomial.__init__(self, coefficients, coeffring, _sorted, **kwds)
 
     def normalize(self):
         """
         returns the unique normalized polynomial g
-        which is associate to self (so g=u*self for some unit in coeffring). 
+        which is associate to self (so g=u*self for some unit in coeffring).
         For IntegerPolynomial, g is positive.
         """
         if self.leading_coefficient() < 0:
             return -self
         return self
 
 class FieldPolynomial(DivisionProvider,
@@ -1465,15 +1465,15 @@
 
     def discriminant(self):
         """
         Return discriminant of the polynomial.
         """
         df = self.differentiate()
         lc = self.leading_coefficient()
-        if self.degree() % 4 in (2, 3):
+        if self.degree() & 3 in (2, 3):
             sign = -1
         else:
             sign = 1
         if self.getCoefficientRing().getCharacteristic() == 0:
             return sign * self.resultant(df) / lc
         else:
             return sign * self.resultant(df) * lc**(self.degree() - df.degree() - 2)
@@ -1647,14 +1647,14 @@
 
 def init_coefficient_ring(coefficients):
     """
     Return a ring to which all coefficients belong.  The argument
     coefficients is a dictionary whose values are the coefficients.
     """
     myRing = None
-    for c in coefficients.itervalues():
+    for c in coefficients.values():
         cring = ring.getRing(c)
         if not myRing or myRing != cring and myRing.issubring(cring):
             myRing = cring
         elif not cring.issubring(myRing):
             myRing = myRing.getCommonSuperring(cring)
     return myRing
```

### Comparing `NZMATH-1.1.0/nzmath/poly/termorder.py` & `nzmath-3.0.0/src/poly/termorder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Term Order for polynomials.
 """
 
 import re
+import nzmath.compatibility
 import nzmath.ring as ring
 
 
 _INTERFACE_MSG = "%s is interface"
 
 class TermOrderInterface (object):
     """
@@ -38,21 +39,71 @@
         self.comparator = comparator
 
     def cmp(self, left, right):
         """
         Compare two indices left and right and determine precedence by
         self.comparator.
         """
-        raise NotImplementedError(_INTERFACE_MSG % self.__class__.__name__)
+        return self.comparator(left, right)
+
+    def bisect(self, array, elem, lo=0, hi=None):
+        """
+        Return the index where to insert item `elem' in a list `array',
+        assuming array is sorted with the order.  (In the following,
+        a refers `array' and x refers `elem')
+
+        The return value i is such that all e in a[:i] have e <= x, and
+        all e in a[i:] have e > x.  So if x already appears in the list,
+        a.insert(x) will insert just after the rightmost x already there.
+
+        Optional args lo (default 0) and hi (default len(a)) bound the
+        slice of a to be searched.
+
+        This function is based on the bisect.bisect_right of the Python
+        standard library.
+        """
+        if hi is None:
+            hi = len(array)
+        while lo < hi:
+            mid = (lo + hi) >> 1
+            if self.cmp(elem, array[mid]) < 0:
+                hi = mid
+            else: lo = mid + 1
+        return lo
 
     def format(self, polynom, **kwds):
         """
         Return the formatted string of the polynomial.
         """
-        raise NotImplementedError(_INTERFACE_MSG % self.__class__.__name__)
+        return self.comparator(left, right)
+
+    def bisect(self, array, elem, lo=0, hi=None):
+        """
+        Return the index where to insert item `elem' in a list `array',
+        assuming array is sorted with the order.  (In the following,
+        a refers `array' and x refers `elem')
+
+        The return value i is such that all e in a[:i] have e <= x, and
+        all e in a[i:] have e > x.  So if x already appears in the list,
+        a.insert(x) will insert just after the rightmost x already there.
+
+        Optional args lo (default 0) and hi (default len(a)) bound the
+        slice of a to be searched.
+
+        This function is based on the bisect.bisect_right of the Python
+        standard library.
+        """
+        if hi is None:
+            hi = len(array)
+        while lo < hi:
+            mid = (lo + hi) >> 1
+            if self.cmp(elem, array[mid]) < 0:
+                hi = mid
+            else: lo = mid + 1
+        return lo
 
     def leading_coefficient(self, polynom):
         """
         Return the leading coefficient of polynomial 'polynom' with
         respect to the term order.
         """
         raise NotImplementedError(_INTERFACE_MSG % self.__class__.__name__)
@@ -79,33 +130,27 @@
         'comparator' can be any callable that accepts two integers and
         returns 0, 1 or -1 just like cmp, i.e. if they are equal it
         returns 0, first one is greater 1, and otherwise -1.
         Theoretically acceptable comparator is only the cmp function.
         """
         TermOrderInterface.__init__(self, comparator)
 
-    def cmp(self, left, right):
-        """
-        Compare two indices left and right and determine precedence by
-        self.comparator.
-        """
-        return self.comparator(left, right)
-
     def format(self, polynom, varname="X", reverse=False):
         """
         Return the formatted string of the polynomial.
 
         - 'polynom' must be a univariate polynomial.
         - 'varname' can be set to the name of the variable (default to
           'X').
         - 'reverse' can be either True or False. If it's True, terms
           appear in reverse (descending) order.
         """
-        degrees = [base for base in polynom.iterbases()]
-        degrees.sort(cmp=self.comparator)
+        degrees = _sort_with_cmp(
+            [base for base in polynom.iterbases()],
+            self.comparator)
         if reverse:
             degrees.reverse()
         str_terms = [("%s * %s ** %d" % (polynom[d], varname, d)) for d in degrees if polynom[d]]
         # constant
         if 0 in degrees and polynom[0]:
             const_term = str(polynom[0])
             if (hasattr(polynom, "getCoefficientRing") and
@@ -194,33 +239,25 @@
         """
         'comparator' accepts two tuples of integers, each of which
         represents power indices of the term, and returns 0, 1 or -1
         just like cmp built-in function.
         """
         self.comparator = comparator
 
-    def cmp(self, left, right):
-        """
-        Compare two indices left and right and determine precedence by
-        self.comparator.
-        """
-        return self.comparator(left, right)
-
     def format(self, polynom, varnames=None, reverse=False, **kwds):
         """
         Return the formatted string of the polynomial.
 
         An additional keyword argument 'varnames' is required to name
         variables.
         """
         if varnames is None:
             raise TypeError("keyword argument 'varnames' is required")
 
-        bases = polynom.bases()
-        bases.sort(cmp=self.comparator)
+        bases = _sort_with_cmp(polynom.bases(), self.comparator)
         if reverse:
             bases.reverse()
 
         result = " + ".join([self._format_term((base, polynom[base]), varnames) for base in bases if polynom[base]])
         # minus terms
         result = self._PLUS_MINUS.sub("- ", result)
         # coefficient is 1 (or -1)
@@ -280,15 +317,15 @@
     def _max(self, indices_list):
         """
         Return the maximum indices with respect to the comparator.
         """
         if not indices_list:
             raise ValueError("max() arg is an empty sequence")
         it = iter(indices_list)
-        maxi = it.next()
+        maxi = next(it)
         for indices in it:
             if self.comparator(maxi, indices) < 0:
                 maxi = indices
         return maxi
 
 
 def weight_order(weight, tie_breaker=None):
@@ -342,7 +379,33 @@
         return cmp(sum_left, sum_right)
     return cmp(right[::-1], left[::-1])
 
 
 lexicographic_order = MultivarTermOrder(cmp)
 total_degree_lexicographic_order = MultivarTermOrder(_total_degree_lexicographic)
 total_degree_reverse_lexicographic_order = MultivarTermOrder(_total_degree_reverse_lexicographic)
+
+
+### for compatibility function
+def _sort_with_cmp(seq, mycmp):
+    """
+    Return the sorted seq by using the comparator function mycmp.
+    """
+    
+    try:
+        return sorted(seq, cmp=mycmp)
+    except TypeError: # cmp is no longer available
+        class internal_cmp:
+            def __init__(self, obj):
+                self.obj = obj
+            def __gt__(self, other):
+                return mycmp(self.obj, other.obj) > 0
+            def __ge__(self, other):
+                return mycmp(self.obj, other.obj) >= 0
+            def __lt__(self, other):
+                return mycmp(self.obj, other.obj) < 0
+            def __le__(self, other):
+                return mycmp(self.obj, other.obj) <= 0
+            def __cmp__(self, other):
+                return mycmp(self.obj, other.obj)
+        return sorted(seq, key=internal_cmp)
+
```

### Comparing `NZMATH-1.1.0/nzmath/poly/multiutil.py` & `nzmath-3.0.0/src/poly/multiutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Multivariate polynomial extenders.
 """
 
-from __future__ import division
+
 import nzmath.rational as rational
 import nzmath.ring as ring
 import nzmath.poly.termorder as termorder
 import nzmath.poly.ring as poly_ring
 import nzmath.poly.uniutil as uniutil
 import nzmath.poly.multivar as multivar
 import nzmath.poly.ratfunc as ratfunc
@@ -17,15 +17,15 @@
 
 class OrderProvider (object):
     """
     OrderProvider provides order and related operations.
     """
     def __init__(self, order):
         """
-        Do not instanciate OrderProvider.
+        Do not instantiate OrderProvider.
         This initializer should be called from descendant:
           OrderProvider.__init__(self, order)
         """
         if type(self) is OrderProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         self.order = order
 
@@ -79,30 +79,30 @@
         """
         Unnest the nested polynomial q by inserting outer variable at
         the given position.
         """
         q_coeff = {}
         for d, cpoly in q:
             for inner_d, inner_c in cpoly:
-                if isinstance(inner_d, (int, long)):
+                if isinstance(inner_d, int):
                     inner_d = [inner_d]
                 else:
                     inner_d = list(inner_d)
                 inner_d.insert(outer, d)
                 q_coeff[tuple(inner_d)] = inner_c
         return self.__class__(q_coeff, coeffring=coeffring)
 
 
 class RingElementProvider (ring.CommutativeRingElement):
     """
     Provides interfaces for ring.CommutativeRingElement.
     """
     def __init__(self):
         """
-        Do not instanciate RingElementProvider.
+        Do not instantiate RingElementProvider.
         This initializer should be called from descendant:
           RingElementProvider.__init__(self)
         """
         if type(self) is RingElementProvider:
             raise NotImplementedError(_MIXIN_MSG % self.__class__.__name__)
         ring.CommutativeRingElement.__init__(self)
         self._coefficient_ring = None
@@ -286,15 +286,15 @@
 
         Keyword arguments should include:
         - coeffring: domain
         - number_of_variables: the number of variables
         """
         if "number_of_variables" not in kwds:
             coefficients = dict(coefficients)
-            for i in coefficients.iterkeys():
+            for i in coefficients.keys():
                 kwds["number_of_variables"] = len(i)
                 break
         multivar.BasicPolynomial.__init__(self, coefficients, **kwds)
         NestProvider.__init__(self)
         PseudoDivisionProvider.__init__(self)
         RingElementProvider.__init__(self)
         coeffring = None
@@ -616,15 +616,15 @@
         """
         if not elem.getRing().issubring(self.ring):
             return False
         if self.generators == [self.ring.zero]:
             return elem == self.ring.zero
         return not self.reduce(elem)
 
-    def __nonzero__(self):
+    def __bool__(self):
         """
         Report whether the ideal is zero ideal or not.  Of course,
         False is for zero ideal.
         """
         return self.generators and self.generators != [self.ring.zero]
 
     def __repr__(self):
```

### Comparing `NZMATH-1.1.0/nzmath/arith1.py` & `nzmath-3.0.0/src/arith1.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,107 +9,163 @@
 from nzmath.plugins import MATHMODULE as math
 
 
 def floorsqrt(a):
     """
     Return the floor of square root of the given integer.
     """
-    if a < 2 ** 59:
+    if a < (1 << 59):
         return int(math.sqrt(a))
     else:
-        b_old = a
-        b = pow(10, log(a, 10)//2 + 1)
-        while b_old > b:
-            b_old, b = b, (b+a//b)//2
-        return b_old
+        # Newton method
+        x = pow(10, (log(a, 10) >> 1) + 1) # compute initial value
+        while True:
+            x_new = (x + a//x) >> 1
+            if x <= x_new:
+                return x
+            x = x_new
 
-def floorpowerroot(n, k):
+def floorpowerroot(n, k, return_power = False):
     """
     Return the floor of k-th power root of the given integer n.
+    Use Newton method.
     """
     if k == 1:
-        return n
+        if return_power:
+            return n, n
+        else:
+            return n
     elif k == 2:
-        return floorsqrt(n)
-    if n < 0:
-        if not (k & 1):
+        rslt = floorsqrt(n)
+        if return_power:
+            return rslt, rslt ** 2
+        else:
+            return rslt
+
+    if n <= 0:
+        if 0 == n:
+            if return_power:
+                return 0, 0
+            else:
+                return 0
+        elif 0 == k & 1:
             raise ValueError("%d has no real %d-th root." % (n, k))
         else:
             sign = -1
             n = -n
     else:
         sign = 1
 
-    a = floorsqrt(n)
-    b = 0
-    while a > b:
-        c = (a + b) // 2
-        if c**k > n:
-            a = c
-        else:
-            if b == c:
-                a = b
-                break
-            b = c
-    while (a+1)**k <= n: # needed when floorsqrt(n) is already small.
-        a += 1
+    # compute initial values
+    exp, rem = divmod(log(n) + 1, k)
+    if 0 != rem: # not ceiling
+        exp += 1
+    q = n >> (exp * (k - 1))
+    x = 1 << exp
+
+    # iteration by tangent approximation
+    while True:
+        x += (q - x) // k
+        z = x ** (k - 1)
+        q = n // z
+        if x <= q:
+            break
 
     if sign < 0:
-        a = -a
-    return a
+        x = -x
+
+    if return_power:
+        return x, x * z
+    else:
+        return x
+
+def powerDetection(n, largest_exp=False):
+    """
+    param positive integer n
+    param boolean largest_exp
+    return integer x, k s.t. n == x ** k
+           (2 <= k if exist else x, k == n, 1)
+           if largest_exp is true then return largest k
+    """
+    from nzmath.prime import generator_eratosthenes as generator_eratosthenes
+
+    ge = generator_eratosthenes(log(n, 2))
+    for exp in ge:
+        power_root, power = floorpowerroot(n, exp, True)
+        if power == n:
+            if largest_exp:
+                x, k = powerDetection(power_root, True)
+                return x, k * exp
+            else:
+                return power_root, exp
+
+    return n, 1
 
 def legendre(a, m):
     """
     This function returns the Legendre symbol (a/m).
     If m is an odd composite then this is the Jacobi symbol.
     """
     a = a % m
     symbol = 1
     while a != 0:
-        while a % 2 == 0:
-            a = a//2
-            if m % 8 == 3 or m % 8 == 5:
+        while a & 1 == 0:
+            a >>= 1
+            if m & 7 == 3 or m & 7 == 5:
                 symbol = -symbol
         a, m = m, a
-        if a % 4 == 3 and m % 4 == 3:
+        if a & 3 == 3 and m & 3 == 3:
             symbol = -symbol
         a = a % m
     if m == 1:
         return symbol
     return 0
 
-def modsqrt(a, p):
+def modsqrt(n, p, e=1):
     """
-    This function returns one of the square roots of 'a' for mod 'p'.
-    'p' must be an odd prime.
-    """
-    symbol = legendre(a, p)
+    This function returns one of the square roots of n for mod p**e.
+    p must be an odd prime.
+    e must be a positive integer.
+    If 1 < e then n must be relatively prime with p.
+    """
+    if 1 < e:
+        x = modsqrt(n, p)
+        if 0 == x:
+            raise ValueError("if 1 < e then n must be relatively prime with p")
+        ppower = p
+        z = inverse(x << 1, p)
+        for i in range(e - 1):
+            x += (n - x ** 2) // ppower * z % p * ppower
+            ppower *= p
+        return x
+    
+    symbol = legendre(n, p)
     if symbol == 1:
-        pmod8 = p % 8
+        pmod8 = p & 7
         if pmod8 != 1:
-            a = a % p
+            n %= p
             if pmod8 == 3 or pmod8 == 7:
-                x = pow(a, (p+1)//4, p)
-            else: # p%8==5
-                x = pow(a, (p+3)//8, p)
+                x = pow(n, (p >> 2) + 1, p)
+            else: # p & 7==5
+                x = pow(n, (p >> 3) + 1, p)
                 c = pow(x, 2, p)
-                if c != a:
-                    x = (x * pow(2, (p-1)//4, p)) % p
-        else: #p%8==1
+                if c != n:
+                    x = (x * pow(2, p >> 2, p)) % p
+        else: #p & 7==1
             d = 2
             while legendre(d, p) != -1:
                 d = random.randrange(3, p)
             s, t = vp(p-1, 2)
-            A = pow(a, t, p)
+            A = pow(n, t, p)
             D = pow(d, t, p)
             m = 0
             for i in range(1, s):
-                if pow(A*(D**m), 2**(s-1-i), p) == (p-1):
-                    m += 2**i
-            x = (pow(a, (t+1)//2, p) * pow(D, m//2, p)) % p
+                if pow(A * pow(D, m, p), 1 << (s-1-i), p) == p - 1:
+                    m += 1 << i
+            x = (pow(n, (t+1) >> 1, p) * pow(D, m >> 1, p)) % p
         return x
     elif symbol == 0:
         return 0
     else:
         raise ValueError("There is no solution")
 
 def expand(n, m):
@@ -120,31 +176,31 @@
     k = []
     while n >= m:
         k.append(n % m)
         n //= m
     k.append(n)
     return k
 
-def inverse(x, p):
+def inverse(x, n):
     """
-    This function returns inverse of x for modulo p.
+    This function returns inverse of x for modulo n.
     """
-    x = x % p
-    y = gcd.extgcd(p, x)
+    x = x % n
+    y = gcd.extgcd(n, x)
     if y[2] == 1:
         if y[1] < 0:
-            r = p + y[1]
+            r = n + y[1]
             return r
         else:
             return y[1]
-    raise ZeroDivisionError("There is no inverse for %d modulo %d." % (x, p))
+    raise ZeroDivisionError("There is no inverse for %d modulo %d." % (x, n))
 
 def CRT(nlist):
     """
-    This function is Chinese Remainder Theorem using Algorithm 2.1.7 
+    This function is Chinese Remainder Theorem using Algorithm 2.1.7
     of C.Pomerance and R.Crandall's book.
 
     For example:
     >>> CRT([(1,2),(2,3),(3,5)])
     23
     """
     r = len(nlist)
@@ -211,36 +267,44 @@
     (2, 25)
 
     That means, 100 is 2 times divisible by 2, and the factor 25 of
     100 is indivisible by 2.
 
     The optional argument k will be added to the valuation.
     """
-    while not (n % p):
+    q = p
+    while not (n % q):
         k += 1
-        n //= p
-    return (k, n)
+        q *= p
+
+    return (k, n // (q // p))
 
 class _Issquare:
     """
     A class for testing whether a number is square or not.
     The function issquare is an instance of the class, indeed.
     """
     q11 = [1, 1, 0, 1, 1, 1, 0, 0, 0, 1, 0]
-    q63 = [1, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0]
-    q64 = [1, 1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0]
-    q65 = [1, 1, 0, 0, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 0, 0, 1]
+    q63 = [1, 1, 0, 0, 1, 0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1,
+           0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1, 0, 0,
+           1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0]
+    q64 = [1, 1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0,
+           0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0,
+           0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0]
+    q65 = [1, 1, 0, 0, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0,
+           0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 0, 0, 0,
+           0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 0, 0, 1]
 
     def __call__(self, c):
         """
         Test whether a given number is a square number or not.  If
         the number is a square number, the function returns its square
         root.  Otherwise zero is returned.
         """
-        t = c % 64
+        t = c & 63
         if not self.q64[t]:
             return 0
         r = c % 45045  # 45045 = 63 * 65 * 11
         if not self.q63[r % 63]:
             return 0
         if not self.q65[r % 65]:
             return 0
@@ -308,15 +372,15 @@
     1 will be returned.
 
     If iterable is an iterator, it will be exhausted.
     """
     iterator = iter(iterable)
     if init is None:
         try:
-            result = iterator.next()
+            result = next(iterator)
         except StopIteration:
             return 1 # empty product
     else:
         result = init
     for item in iterator:
         result *= item
     return result
```

### Comparing `NZMATH-1.1.0/nzmath/vector.py` & `nzmath-3.0.0/src/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 
 class Vector (object):
     """
     Class Vector is an elemental class of vector.
     """
     def __init__(self, compo):
         self.compo = list(compo)
@@ -18,14 +18,18 @@
 
     def __iter__(self):
         return iter(self.compo)
 
     def __eq__(self, other):
         return self.compo == other.compo
 
+    def __hash__(self):
+        val = sum([hash(ele) for ele in self.compo]) 
+        return val
+
     def __ne__(self, other):
         return self.compo != other.compo
 
     def __add__(self, other):
         if isinstance(other, Vector):
             if len(self) == len(other):
                 tmp = [s + c for (s, c) in zip(self.compo, other.compo)]
```

### Comparing `NZMATH-1.1.0/nzmath/bigrange.py` & `nzmath-3.0.0/src/bigrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 def range(start, stop=None, step=None):
     """
     Generate range like finite integer sequence but can generate more
     than sys.maxint elements.
     """
     if step is None:
         step = 1
-    elif not isinstance(step, (int, long)):
+    elif not isinstance(step, int):
         raise ValueError("non-integer step for range()")
-    if not isinstance(start, (int, long)):
+    if not isinstance(start, int):
         raise ValueError("non-integer arg 1 for range()")
     if stop is None:
         start, stop = 0, start
-    elif not isinstance(stop, (int, long)):
+    elif not isinstance(stop, int):
         raise ValueError("non-integer stop for range()")
 
     if step > 0:
         n = start
         while n < stop:
             yield n
             n += step
```

### Comparing `NZMATH-1.1.0/nzmath/real.py` & `nzmath-3.0.0/src/real.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 real -- real numbers and the real number field.
 
 The module real provides arbitrary precision real numbers and their
 utilities.  The functions provided are corresponding to the math
 standard module.
 """
 
-from __future__ import division
+
 import itertools
 import warnings
 
 import nzmath.arith1 as arith1
 import nzmath.rational as rational
 import nzmath.ring as ring
 from nzmath.plugins import MATHMODULE as math, FLOATTYPE as Float, \
      CHECK_REAL_OR_COMPLEX as check_real_or_complex
 
 
 class Real(ring.FieldElement):
     """
-    Real is a class of real. 
+    Real is a class of real.
     This class is only for consistency for other Ring object.
     """
 
-    convertable = (Float, int, long, rational.Rational)
+    convertable = (Float, int, int, rational.Rational)
 
     def __init__(self, value):
         """
         value will be wrapped in Float.
         """
         ring.FieldElement.__init__(self)
         if isinstance(value, rational.Rational):
@@ -114,14 +114,17 @@
         if isinstance(other, Real):
             return self.data == other.data
         elif isinstance(other, self.convertable):
             return self.data == other
         else:
             return NotImplemented
 
+    def __hash__(self):
+        return hash(self.data)
+
     def getRing(self):
         """
         Return the real field instance.
         """
         return theRealField
 
 
@@ -139,15 +142,15 @@
     def __str__(self):
         return "R"
 
     def __repr__(self):
         return "%s()" % (self.__class__.__name__, )
 
     def __contains__(self, element):
-        if isinstance(element, (int, long, float, Float, Real, rational.Rational)):
+        if isinstance(element, (int, float, Float, Real, rational.Rational)):
             return True
         else:
             try:
                 if check_real_or_complex(element):
                     return True
             except TypeError:
                 if hasattr(element, 'conjugate'):
@@ -307,15 +310,15 @@
     given iterator.
     """
     stock = []
     b = rational.Rational(1, 2)
     l = -1
     for term in iterator:
         stock.append(term)
-        for i in xrange(l, -1, -1):
+        for i in range(l, -1, -1):
             stock[i] += stock[i+1]
         yield b * stock[0]
         b /= 2
         l += 1
 
 # constants
 theRealField = RealField()
```

### Comparing `NZMATH-1.1.0/nzmath/module.py` & `nzmath-3.0.0/src/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 module, ideal etc. for number field
 """
-from __future__ import division
+
 
 from nzmath.algfield import BasicAlgNumber, MatAlgNumber
 import nzmath.arith1 as arith1
 import nzmath.gcd as gcd
 import nzmath.vector as vector
 import nzmath.matrix as matrix
 import nzmath.rational as rational
 import nzmath.ring as ring
 import nzmath.prime as prime
+from functools import reduce
 
 
 class Submodule(matrix.RingMatrix):
     """
     Submodule is a class for submodules (typically, Z^n).
     we assume that coeff_ring is PID.
     (i.e. hermite normal form (HNF) for matrices exists.)
@@ -350,15 +351,15 @@
         return new_module
 
     def __mul__(self, other):
         """
         return self * other (as ideal computation)
         """
         if isinstance(other, 
-            (int, long, rational.Integer, rational.Rational)):
+            (int, rational.Integer, rational.Rational)):
             return self._rational_mul(other)
         #try:
         #     use __contains__ function?
         #    if other in self.number_field:
         if isinstance(other, (BasicAlgNumber, MatAlgNumber)):
             return self._scalar_mul(other)
         #except: # other is a module
@@ -472,15 +473,15 @@
         return sol
 
     def __pow__(self, other):
         """
         self ** other (based on ideal multiplication)
         """
         if other <= 0:
-            raise ValueError, "only support non-negative powering" 
+            raise ValueError("only support non-negative powering") 
         mul_part = self.copy()
         index = other
         while True:
             if index & 1:
                 try:
                     sol *= mul_part
                 except NameError:
@@ -824,15 +825,15 @@
         return Ideal_with_generator(new_generator)
 
     def __pow__(self, other):
         """
         self ** other (based on ideal multiplication)
         """
         if other <= 0:
-            raise ValueError, "only support non-negative powering" 
+            raise ValueError("only support non-negative powering") 
         mul_part = self.copy()
         index = other
         while True:
             if index & 1:
                 try:
                     sol *= mul_part
                 except NameError:
@@ -900,15 +901,15 @@
             (self.generator[j].denom for j in range(k)) )
         gen_list = [gen_denom * self.generator[j] for j in range(k)]
         int_I = Ideal_with_generator(gen_list)
         R = 1
         norm_I = int_I.norm()
         l_I = int_I.smallest_rational()
         if l_I.denominator > 1:
-            raise ValueError, "input an integral ideal"
+            raise ValueError("input an integral ideal")
         else:
             l_I = l_I.numerator
         while True:
             lmda = [R for i in range(k)]
             while lmda[0] > 0:
                 alpha = lmda[0] * gen_list[0]
                 for i in range(1, k):
```

### Comparing `NZMATH-1.1.0/nzmath/finitefield.py` & `nzmath-3.0.0/src/finitefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 finite fields.
 """
 
-from __future__ import division
+
 import logging
 import nzmath.gcd as gcd
 import nzmath.bigrandom as bigrandom
 import nzmath.bigrange as bigrange
 import nzmath.arith1 as arith1
 import nzmath.prime as prime
 import nzmath.ring as ring
@@ -22,26 +22,26 @@
 
 
 class FiniteFieldElement(ring.FieldElement):
     """
     The base class for all finite field element.
     """
     def __init__(self):
-        # This class is abstract and can not be instanciated.
+        # This class is abstract and can not be instantiated.
         if type(self) is FiniteFieldElement:
             raise NotImplementedError("the class FiniteFieldElement is abstract")
         ring.FieldElement.__init__(self)
 
 
 class FiniteField(ring.Field):
     """
     The base class for all finite fields.
     """
     def __init__(self, characteristic):
-        # This class is abstract and can not be instanciated.
+        # This class is abstract and can not be instantiated.
         if type(self) is FiniteField:
             raise NotImplementedError("the class FiniteField is abstract")
         ring.Field.__init__(self)
         self.char = characteristic
         self._orderfactor = None  # postpone the initialization
 
     def card(self):
@@ -92,15 +92,15 @@
 
         if element == self.one or self.char == 2:
             return 1 # element of cyclic group order 2**n-1 also always 1
 
         # generic method:successive squaring
         # generalized Legendre symbol definition:
         #    (self/_ring) := self ** ((card(_ring)-1)/2)
-        x = element ** ((card(self)-1) // 2)
+        x = element ** ((card(self)-1) >> 1)
         if x == self.one:
             return 1
         elif x == -self.one:
             return -1
         raise ValueError("element must be not in field")
 
     def TonelliShanks(self, element):
@@ -118,15 +118,15 @@
 
         a = element
         n = self.createElement(self.char+1)
         while self.Legendre(n) != -1:
             n = self.random_element(2, card(self)) # field maybe large
         y = z = n ** q
         r = e
-        x = a ** ((q-1) // 2)
+        x = a ** ((q-1) >> 1)
         b = a * (x ** 2)
         x = a * x
         while True:
             if b == self.one:
                 return x
             m = 1
             while m < r:
@@ -146,15 +146,15 @@
         """ Return square root if exist.
         """
         if not element or element == self.one:
             return element # trivial case
 
         # element of characteristic 2 always exist square root
         if  self.char == 2:
-            return element ** ((card(self)) // 2)
+            return element ** ((card(self)) >> 1)
 
         # otherwise,
         return self.TonelliShanks(element)
 
 
 class FinitePrimeFieldElement(intresidue.IntegerResidueClass, FiniteFieldElement):
     """
@@ -234,14 +234,17 @@
     def __eq__(self, other):
         if self is other:
             return True
         if isinstance(other, FinitePrimeField):
             return self.char == other.char
         return False
 
+    def __hash__(self):
+        return self.char
+
     def __ne__(self, other):
         return not (self == other)
 
     def __str__(self):
         return "F_%d" % self.char
 
     def __repr__(self):
@@ -412,27 +415,27 @@
 
     def __add__(self, other):
         """
         self + other
 
         other can be an element of either F_q, F_p or Z.
         """
-        if other is 0 or other is self.field.zero:
+        if other == 0 or other is self.field.zero: # 'is 0'-->'== 0'
             return self
         return self._op(other, "__add__")
 
     __radd__ = __add__
 
     def __sub__(self, other):
         """
         self - other
 
         other can be an element of either F_q, F_p or Z.
         """
-        if other is 0 or other is self.field.zero:
+        if other == 0 or other is self.field.zero: # 'is 0'-->'== 0'
             return self
         return self._op(other, "__sub__")
 
     def __rsub__(self, other):
         """
         other - self
 
@@ -442,15 +445,15 @@
 
     def __mul__(self, other):
         """
         self * other
 
         other can be an element of either F_q, F_p or Z.
         """
-        if other is 1 or other is self.field.one:
+        if other == 1 or other is self.field.one: # 'is 1'-->'== 1'
             return self
         return self._op(other, "__mul__")
 
     __rmul__ = __mul__
 
     def __truediv__(self, other):
         return self * other.inverse()
@@ -489,19 +492,22 @@
             if self.field == other.field:
                 if self.rep == other.rep:
                     return True
         except AttributeError:
             pass
         return False
 
+    def __hash__(self):
+        return hash(self.rep)
+
     def __ne__(self, other):
         return not (self == other)
 
-    def __nonzero__(self):
-        return self.rep.__nonzero__()
+    def __bool__(self):
+        return bool(self.rep)
 
     def __repr__(self):
         return "%s(%s, %s)" % (self.__class__.__name__, repr(self.rep), repr(self.field))
 
     def trace(self):
         """
         Return the absolute trace.
@@ -566,15 +572,15 @@
         finite field extended over prime field.
 
         characteristic must be prime. n_or_modulus can be:
           1) an integer greater than 1, or
           2) a polynomial in a polynomial ring of F_p with degree
              greater than 1.
         """
-        if isinstance(n_or_modulus, (int, long)):
+        if isinstance(n_or_modulus, int):
             n = n_or_modulus
             if n <= 1:
                 raise ValueError("degree of extension must be > 1.")
             # choose a method among three variants:
             #modulus = cls._random_irriducible(characteristic, n)
             #modulus = cls._small_irriducible(characteristic, n)
             modulus = cls._primitive_polynomial(characteristic, n)
@@ -636,15 +642,15 @@
 
         REF: Lidl & Niederreiter, Introduction to finite fields and
              their applications.
         """
         cardinality = char ** degree
         basefield = FinitePrimeField.getInstance(char)
         const = basefield.primitive_element()
-        if degree % 2:
+        if degree & 1:
             const = -const
         cand = uniutil.polynomial({0:const, degree:basefield.one}, basefield)
         maxorder = factor_misc.FactoredInteger((cardinality - 1) // (char - 1))
         var = uniutil.polynomial({1:basefield.one}, basefield)
         while not (cand.isirreducible() and
                    all(pow(var, int(maxorder) // p, cand).degree() > 0 for p in maxorder.prime_divisors())):
             # randomly modify the polynomial
@@ -667,15 +673,15 @@
         """
         return self.char ** self.degree
 
     def createElement(self, seed):
         """
         Create an element of the field.
         """
-        if isinstance(seed, (int, long)):
+        if isinstance(seed, int):
             expansion = arith1.expand(seed, card(self.basefield))
             return ExtendedFieldElement(
                 uniutil.FiniteFieldPolynomial(enumerate(expansion), self.basefield),
                 self)
         elif seed in self.basefield:
             return ExtendedFieldElement(
                 uniutil.FiniteFieldPolynomial([(0, seed)], self.basefield),
```

### Comparing `NZMATH-1.1.0/nzmath/algorithm.py` & `nzmath-3.0.0/src/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     powering by using left-right binary method.
     (assume that index >= 0)
     """
     import math
     square = _set_square(mul, square)
     if not index:
         return one
-    spot = 1 << long(math.log(index, 2))
+    spot = 1 << int(math.log(index, 2))
     sol = one
     while True:
         if spot & index:
             try:
                 sol = mul(sol, element)
             except: # one is None!
                 sol = element
@@ -105,15 +105,15 @@
     window size is selected by average analystic optimization
     (assume that index >= 0)
     """
     import math
     square = _set_square(mul, square)
     if not index:
         return one
-    log_n = long(math.log(index, 2))
+    log_n = int(math.log(index, 2))
     # Find the proper window size
     size = 2
     pow_size = 2
     while log_n > (size + 1) * (size + 2) * (pow_size - 1):
         pow_size <<= 1
         size += 1
     # Precomputation
```

### Comparing `NZMATH-1.1.0/nzmath/combinatorial.py` & `nzmath-3.0.0/src/combinatorial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Combinatorial functions
 """
 
+import bisect
 import itertools
 from nzmath.rational import Integer, Rational
 
 
 def binomial(n, m):
     """
     The binomial coefficient.
@@ -13,17 +14,17 @@
 
     n must be a positive integer and m must be a non-negative integer.
     For convinience, binomial(n, n+i) = 0 for positive i, and
     binomial(0,0) = 1.
 
     In other cases, it raises an exception.
     """
-    if not isinstance(n, (int, long)):
+    if not isinstance(n, int):
         raise TypeError("integer is expected, %s detected." % n.__class__)
-    if not isinstance(m, (int, long)):
+    if not isinstance(m, int):
         raise TypeError("integer is expected, %s detected." % m.__class__)
     if n == m >= 0 or m == 0 and n > 0:
         return 1
     if n <= 0:
         raise ValueError("non-positive number: %d" % n)
     if m < 0:
         raise ValueError("negative number: %d" % m)
@@ -37,30 +38,30 @@
         retval /= (i + 1)
     return Integer(retval)
 
 def factorial(n):
     """
     Return n! for non negative integer n.
     """
-    if not isinstance(n, (int, long)):
+    if not isinstance(n, int):
         raise TypeError("integer is expected, %s detected." % n.__class__)
     elif n < 0:
         raise ValueError("argument must not be a negative integer.")
     elif n < 1500:
         # naive loop is best for small n.
         result = 1
-        for i in xrange(2, n + 1):
+        for i in range(2, n + 1):
             result *= i
         return Integer(result)
     # The following algorithm keeps temporary results rather small as
     # possible in order to make the function run faster than the naive
     # loop.
-    l = range(1, n + 1)
+    l = list(range(1, n + 1))
     while len(l) > 1:
-        for i in xrange(len(l) // 2):
+        for i in range(len(l) >> 1):
             l[i] *= l.pop()
     return Integer(l.pop())
 
 def bernoulli(n):
     """
     Return n-th Bernoulli number.
     """
@@ -88,47 +89,14 @@
     if n & 1:
         return Integer(0)
     E = {0:Integer(1)}
     for i in range(2, n + 1, 2):
         E[i] = sum([-binomial(i, j) * E[j] for j in range(0, i, 2)])
     return E[n]
 
-def combination_index_generator(n, m):
-    """
-    Generate indices of m elment subsets of n element set.
-
-    For example:
-    >>> for idx in combinationIndexGenerator(5,3):
-    ...     print idx
-    ...
-    [0, 1, 2]
-    [0, 1, 3]
-    [0, 1, 4]
-    [0, 2, 3]
-    [0, 2, 4]
-    [0, 3, 4]
-    [1, 2, 3]
-    [1, 2, 4]
-    [1, 3, 4]
-    [2, 3, 4]
-    >>>
-    """
-    assert n >= m > 0
-    idx = range(m)
-    while True:
-        yield list(idx)
-        for i in range(1, m+1):
-            if idx[-i] != n-i:
-                idx[-i] += 1
-                for j in range(i-1, 0, -1):
-                    idx[-j] = idx[-j-1] + 1
-                break
-        else:
-            raise StopIteration
-
 def fallingfactorial(n, m):
     """
     Return the falling factorial; n to the m falling, i.e. n(n-1)..(n-m+1).
 
     For Example:
     >>> fallingfactorial(7, 3)
     210
@@ -156,15 +124,15 @@
     Return multinomial coefficient.
 
     parts MUST be a sequence of natural numbers and n==sum(parts) holds.
     """
     if n != sum(parts):
         raise ValueError("sum of parts must be equal to n.")
     for part in parts:
-        if not isinstance(part, (int, long)) or part < 0:
+        if not isinstance(part, int) or part < 0:
             raise ValueError("parts must be a sequence of natural numbers.")
     # binomial case
     if len(parts) == 2:
         return binomial(n, parts[0])
     # other cases
     result = factorial(n)
     for part in parts:
@@ -184,15 +152,15 @@
     if n == m:
         return 1
     elif n < m or n*m < 0:
         return 0
     elif m == 0:
         return 0
     elif m == 1:
-        if n % 2:
+        if n & 1:
             sign = 1
         else:
             sign = -1
         return sign * factorial(n - 1)
     elif m == n - 1:
         return -binomial(n, 2)
     else:
@@ -227,15 +195,15 @@
     elif n < 0:
         return stirling2_negative(-m, -n)
     elif m == 1:
         return 1
     elif m == 2:
         return 2**(n - 1) - 1
     elif m == n - 1:
-        return n * m // 2
+        return n * m >> 1
     else:
         r = 0
         b = m
         l = 1
         while 1:
             if l & 1:
                 r -= b * l**n
@@ -288,22 +256,150 @@
 
     The Bell number b is defined by:
       b(n) = \sum_{i=0}^{n} S(n, i)
     where S denotes Stirling number of the second kind.
     """
     return sum([stirling2(n, i) for i in range(n + 1)])
 
+
+# generators
+def combination_index_generator(n, m):
+    """
+    Generate indices of m elment subsets of n element set.
+
+    The number of generated indices is binomial(n, m).
+
+    For example,
+    combinationIndexGenerator(5,3) generates the following lists:
+        [0, 1, 2]
+        [0, 1, 3]
+        [0, 1, 4]
+        [0, 2, 3]
+        [0, 2, 4]
+        [0, 3, 4]
+        [1, 2, 3]
+        [1, 2, 4]
+        [1, 3, 4]
+        [2, 3, 4]
+    """
+    assert n >= m > 0
+    idx = list(range(m))
+    while True:
+        yield list(idx)
+        for i in range(1, m+1):
+            if idx[-i] != n-i:
+                idx[-i] += 1
+                for j in range(i-1, 0, -1):
+                    idx[-j] = idx[-j-1] + 1
+                break
+        else:
+            return # raise StopIteration (RuntimeError by PEP479)
+
+
+def permutation_generator(n):
+    """
+    Generate all permutations of n elements as lists.
+
+    The number of generated lists is n!, so be careful to use big n.
+
+    For example,
+    permutationGenerator(3) generates the following lists:
+        [0, 1, 2]
+        [0, 2, 1]
+        [1, 0, 2]
+        [1, 2, 0]
+        [2, 0, 1]
+        [2, 1, 0]
+    """
+    # traverse tree by depth first
+    perm = list(range(n))
+    unused = []
+    while True:
+        # leaf is reached, thus yield the value.
+        yield list(perm)
+
+        # track back until node with subtree yet to be traversed
+        last = n - 1
+        unused.append(perm[-1])
+        while last and perm[last - 1] > unused[-1]:
+            last -= 1
+            unused.append(perm[last])
+
+        # exhausted
+        if not last:
+            break
+
+        # assert unused == sorted(unused)
+        # replace with just bigger than perm[last - 1]
+        index = bisect.bisect(unused, perm[last - 1])
+        unused[index], perm[last - 1] = perm[last - 1], unused[index]
+        # replace remaining part
+        perm[last:] = unused
+        del unused[:]
+
+
+def dyck_word_generator(n, alphabet=(0, 1)):
+    """
+    Generate all Dyck words of length 2*n as tuples.
+
+    The Dyck words are words on a two character alphabet.
+    The number of each character in a word is equal, 
+    and the number of the second character never exceeds the first
+    in any initial parts of the word.
+
+    The number of generated words is the n-th Catalan number.
+
+    The alphabet is {0, 1} by default, but you can pass it into the
+    optional argument 'alphabet'.
+
+    For example,
+    >>> for word in dyck_word_generator(3, alphabet=("(", ")")):
+    ...     print("".join(word))
+    ... 
+    ()()()
+    ()(())
+    (())()
+    (()())
+    ((()))
+    >>> 
+    """
+    if n == 0:
+        yield ()
+        return # raise StopIteration() (RuntimeError by PEP479)
+    else:
+        # memo[i] is a list of Dyck words of length 2*i
+        memo = [[()]]
+        alpha, beta = (alphabet[0],), (alphabet[1],)
+
+    # prepare up to n-1
+    for i in range(1, n):
+        memo.append([])
+        for j in range(i):
+            for p in memo[j]:
+                prefix = alpha + p + beta
+                for q in memo[i - j - 1]:
+                    memo[i].append(prefix + q)
+        
+    # output
+    for j in range(n):
+        for p in memo[j]:
+            prefix = alpha + p + beta
+            for q in memo[n - j - 1]:
+                yield prefix + q
+
+
+# partition related functions and classes
 def partition_generator(n, maxi=None):
     """
     Generate partitions of n.
     If maxi is given, then parts are limited to at most maxi.
     """
     if not n:
         yield ()
-        raise StopIteration
+        return # raise StopIteration (RuntimeError by PEP479)
     if maxi is None or maxi > n:
         maxi = n
     partition = [maxi]
     rest = n - maxi
     while True:
         key = partition[-1]
         while rest >= key:
@@ -315,15 +411,15 @@
         yield tuple(partition)
 
         try:
             # wind up all 1's.
             first_one = partition.index(1)
             if not first_one:
                 # partition was [1]*n means all partitions have been generated.
-                raise StopIteration
+                return # raise StopIteration (RuntimeError by PEP479)
             rest = len(partition) - first_one
             del partition[first_one:]
         except ValueError:
             # 1 is not found
             rest = 0
 
         partition[-1] -= 1
@@ -395,16 +491,16 @@
                 # wind up all 1's.
                 first_one = self.partition.index(1)
                 self.rest = len(self.partition) - first_one
                 del self.partition[first_one:]
             else:
                 self.rest = 0
         except Exception:
-            print self.partition
-            print self.rest
+            print(self.partition)
+            print(self.rest)
 
     def push(self):
         """
         On each end of backtrack, the tail of partition has to be
         decreased and the decrement is cancelled by an increment of
         rest.
         """
@@ -442,15 +538,15 @@
             if self.shouldterminate():
                 break
             self.push()
 
 
 class LimitedMaximumPartitionDriver(PartitionDriver):
     """
-    Only limit the muximum of parts.
+    Only limit the maximum of parts.
     """
     def __init__(self):
         PartitionDriver.__init__(self)
         self.limit = 0
 
     def set_parameters(self, integer, limit):
         """
@@ -489,15 +585,15 @@
 
     def pull(self):
         """
         Pull the maximum odd part obtainable from rest to partition.
         """
         if self.partition and self.rest >= self.partition[-1]:
             part = self.partition[-1]
-        elif self.rest % 2:
+        elif self.rest & 1:
             part = self.rest
         else:
             part = self.rest - 1
 
         self.partition.append(part)
         self.rest -= part
 
@@ -518,27 +614,27 @@
 
     def set_parameters(self, integer, limit):
         """
         Set parameters for generate:
           integer: the number to be partitioned
           limit: the maximum of parts
         """
-        if not (limit % 2):
+        if not (limit & 1):
             limit -= 1
         LimitedMaximumPartitionDriver.set_parameters(self, integer, limit)
 
     def pull(self):
         """
         Pull the maximum odd part obtainable from rest to partition.
         """
         if self.partition and self.rest >= self.partition[-1]:
             part = self.partition[-1]
         elif self.rest >= self.limit:
             part = self.limit
-        elif self.rest % 2:
+        elif self.rest & 1:
             part = self.rest
         else:
             part = self.rest - 1
 
         self.partition.append(part)
         self.rest -= part
 
@@ -552,17 +648,17 @@
         return driver.generate(n, maxi)
 
 
 def partition_numbers_upto(n):
     """
     Return the partition numbers for 0 to '''n''' (inclusive).
     """
-    penta = list(itertools.izip(
+    penta = list(zip(
         itertools.takewhile(lambda k: k <= n, _pentagonal()),
-        itertools.cycle((1, 1, -1, -1))))                 
+        itertools.cycle((1, 1, -1, -1))))
     p = [1]
     for i in range(1, n + 1):
         s = 0
         for k, sign in penta:
             if k > i:
                 break
             s += sign * p[i - k]
@@ -572,16 +668,16 @@
 def _pentagonal():
     """
     Generates pentagonal and skew pentagonal numbers.
     (1, 2, 5, 7, 12, 15, ...)
     """
     j = 1
     while True:
-        yield j*(3*j - 1)//2
-        yield j*(3*j + 1)//2
+        yield j*(3*j - 1) >> 1
+        yield j*(3*j + 1) >> 1
         j += 1
 
 def partition_number(n):
     """
     Return the partition number for '''n'''.
     """
     return partition_numbers_upto(n)[-1]
@@ -600,58 +696,13 @@
         if i == last_index:
             conj.extend([i + 1] * part)
         elif part != partition[i + 1]:
             conj.extend([i + 1] * (part - partition[i + 1]))
     conj.reverse()
     return tuple(conj)
 
-def permutation_generator(n):
-    """
-    Generate all permutations of n elements as lists.
-
-    The number of generated list is n!, so be careful to use big n.
-
-    For example:
-    >>> for perm in permutationGenerator(3):
-    ...     print perm
-    ...
-    [0, 1, 2]
-    [0, 2, 1]
-    [1, 0, 2]
-    [1, 2, 0]
-    [2, 0, 1]
-    [2, 1, 0]
-    >>>
-    """
-    # traverse tree by depth first, using a stack
-    stack = [[0]]
-    unused = set(range(1, n))
-    while True:
-        if unused:
-            # yet on inner node
-            part = stack[-1] + [min(unused)]
-            stack.append(part)
-            unused.discard(min(unused))
-            continue
-        # leaf is reached, thus yield the value.
-        perm = stack.pop()
-        yield perm
-        # track back until node with subtree yet to be traversed
-        unused.add(perm[-1])
-        while stack and stack[-1][-1] > max(unused):
-            part = stack.pop()
-            unused.add(part[-1])
-        else:
-            if not stack:
-                # end of stack means traversal is done
-                break
-            prev = stack[-1][-1]
-            replacer = min(d for d in unused if d > prev)
-            stack[-1][-1] = replacer
-            unused.discard(replacer)
-            unused.add(prev)
-
 
 # aliases
 combinationIndexGenerator = combination_index_generator
 partitionGenerator = partition_generator
 permutationGenerator = permutation_generator
+DyckWordGenerator = dyck_word_generator
```

### Comparing `NZMATH-1.1.0/nzmath/elliptic.py` & `nzmath-3.0.0/src/elliptic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-""" Elliptic Curves over finite field. 
+""" Elliptic Curves over finite field.
 """
 
-from __future__ import division
+
 import logging
 import random
 
 import nzmath.poly.uniutil as uniutil
 import nzmath.poly.multiutil as multiutil
 import nzmath.poly.termorder as termorder
 import nzmath.arith1 as arith1
@@ -37,15 +37,15 @@
 def _strMultiPoly(poly, symbol=["x","y"], asc=False):
     """return format string of MultiVarPolynomial for EC"""
     def Weierstrasscmp(left, right):
         sum_left, sum_right = sum(left), sum(right)
         if sum_left != sum_right:
             return -cmp(sum_left, sum_right)
         return -cmp(right, left)
-    
+
     return termorder.MultivarTermOrder(Weierstrasscmp).format(MultiVarPolynomial(poly,symbol), symbol, asc)
 
 
 def _PolyMod(f, g):
     """
     return f (mod g)
     """
@@ -98,15 +98,15 @@
             character = basefield.getCharacteristic()
             self.basefield = basefield
         except:
             # backward compatibility support
             if isinstance(basefield, rational.RationalField) or (not basefield):
                 character = 0
                 self.basefield = rational.theRationalField
-            elif isinstance(basefield, (int,long)):
+            elif isinstance(basefield, int):
                 character = basefield
                 if character == 1 or character < 0:
                     raise ValueError("basefield characteristic must be 0 or prime.")
                 self.basefield = finitefield.FinitePrimeField.getInstance(character)
             else:
                 raise ValueError("basefield must be FiniteField.")
 
@@ -175,15 +175,15 @@
         if self.a3:
             dictL[(0, 1)] = self.a3
         if self.a4:
             dictR[1] = self.a4
         if self.a6:
             dictR[0] = self.a6
         return ("%s = %s" %
-                (str(_strMultiPoly(dictL)), 
+                (str(_strMultiPoly(dictL)),
                  str(_strUniPoly(_UniVarPolynomial(dictR, self.basefield)))))
 
     def simple(self):
         """
         Transform
           E:y^2+a1*x*y+a3*y = x^3+a2*x^2+a4*x+a6
         to
@@ -211,15 +211,15 @@
             return EC([rational.Rational(self.a1+2*V[2], V[0]),
                        rational.Rational(self.a2-V[2]*self.a1+3*V[1]-V[2]**2, V[0]**2),
                        rational.Rational(self.a3+V[1]*self.a1+2*V[3], V[0]**3),
                        rational.Rational(self.a4-V[2]*self.a3+2*V[1]*self.a2-(V[3]+V[1]*V[2])*self.a1+3*V[1]**2-2*V[2]*V[3], V[0]**4),
                        rational.Rational(self.a6+V[1]*self.a4+V[1]**2*self.a2+V[1]**3-V[3]*self.a3-V[3]**2-V[1]*V[3]*self.a1, V[0]**6)])
         else:
             for v in V:
-                if not isinstance(v, (int, long)) and not (v in self.basefield):
+                if not isinstance(v, int) and not (v in self.basefield):
                     raise ValueError("transform V must be integer sequence.")
             v = self.basefield.createElement(V[0]).inverse()
             return EC([(self.a1+2*V[2])*v,
                        ((self.a2-V[2]*self.a1+3*V[1]-V[2]**2)*v**2),
                        ((self.a3+V[1]*self.a1+2*V[3])*v**3),
                        ((self.a4-V[2]*self.a3+2*V[1]*self.a2-(V[3]+V[1]*V[2])*self.a1+3*V[1]**2-2*V[2]*V[3])*v**4),
                        ((self.a6+V[1]*self.a4+V[1]**2*self.a2+V[1]**3-V[3]*self.a3-V[3]**2-V[1]*V[3]*self.a1)*v**6)], self.basefield)
@@ -472,22 +472,22 @@
                                          1:self.b2*self.b8 - self.b4*self.b6,
                                          0:self.b4*self.b8 - self.b6**2},
                                         self.basefield)
 
         # recursive calculation
         i = 5
         while i < loopbound:
-            if i % 2 != 0:
-                j = (i - 1)//2
-                if j % 2 != 0:
+            if i & 1:
+                j = (i - 1) >> 1
+                if j & 1:
                     f[i] = f[j+2]*f[j]**3 - e**2*f[j-1]*f[j+1]**3
                 else:
                     f[i] = e**2*f[j+2]*f[j]**3 - f[j-1]*f[j+1]**3
             else:
-                j = i//2
+                j = i >> 1
                 f[i] = (f[j+2]*f[j-1]**2 - f[j-2]*f[j+1]**2) * f[j]
             i += 1
 
         # final result
         if not Number:
             for i in range(2, loopbound, 2):
                 f[i] = 2*f[i]
@@ -500,15 +500,15 @@
     Elliptic curves over Q.
     """
     def __init__(self, coefficient):
         field = rational.RationalField()
         coeffs_list = []
         if isinstance(coefficient, list):
             for c in coefficient:
-                if isinstance(c, (int, long)):
+                if isinstance(c, int):
                     coeff = field.createElement(c)
                 elif c in field:
                     coeff = c
                 else:
                     raise ValueError("coefficient not in basefield.")
                 coeffs_list.append(coeff)
 
@@ -551,24 +551,24 @@
 
         # parameter parse
         try:
             character = basefield.getCharacteristic()
             field = basefield
         except AttributeError:
             # backward compatibility
-            if isinstance(basefield, (int, long)):
+            if isinstance(basefield, int):
                 field = finitefield.FinitePrimeField.getInstance(basefield)
                 character = basefield
             else:
                 raise ValueError("basefield must be FiniteField object.")
 
         coeffs_list = []
         if isinstance(coefficient, list):
             for c in coefficient:
-                if isinstance(c, (int, long)):
+                if isinstance(c, int):
                     coeff = field.createElement(c)
                 elif c in field:
                     coeff = c
                 else:
                     raise ValueError("coefficient not in basefield.")
                 coeffs_list.append(coeff)
 
@@ -578,29 +578,29 @@
         zero = self.basefield.zero
         one = self.basefield.one
 
         # format attribute
         if self.ch == 2:
             if len(self) == 5:
                 # FIXME
-                if coeffs_list[0] % 2 == one and coeffs_list[2] % 2 == coeffs_list[3] % 2 == zero and coeffs_list[4]:
+                if coeffs_list[0] & 1 == one and coeffs_list[2] & 1 == coeffs_list[3] & 1 == zero and coeffs_list[4]:
                     self.a1 = one
                     self.a2 = coeffs_list[1]
                     self.a3 = zero
                     self.a4 = zero
                     self.a6 = coeffs_list[4]
                     self.b2 = one
                     self.b4 = zero
                     self.b6 = zero
                     self.b8 = self.a6
                     self.c4 = one
                     self.c6 = one
                     self.disc = self.a6
                     self.j = self.disc.inverse()
-                elif coeffs_list[0] % 2 == coeffs_list[1] % 2 == zero and coeffs_list[2]:
+                elif coeffs_list[0] & 1 == coeffs_list[1] & 1 == zero and coeffs_list[2]:
                     self.a1 = zero
                     self.a2 = zero
                     self.a3 = coeffs_list[2]
                     self.a4 = coeffs_list[3]
                     self.a6 = coeffs_list[4]
                     self.b2 = zero
                     self.b4 = zero
@@ -749,15 +749,15 @@
             _log.debug("l = %d" % l)
             traces.append(self._Schoof_mod_l(l))
 
         del self.division_polynomials # temporary attribute deleted
 
         trace = arith1.CRT(traces)
         modulus = arith1.product(prime_moduli)
-        if trace > modulus//2:
+        if trace > (modulus >> 1):
             trace -= modulus
         assert abs(trace) <= 2*arith1.floorsqrt(card(self.basefield)), str(self)
         return trace
 
     def _Schoof_mod2(self):
         """
         Return (#E(F_q) mod 2, 2).  char(F_q) > 3 is required.
@@ -808,56 +808,56 @@
             f, P = self._sub1(w, x_frob - x, lth_div)
 
             if _PolyGCD(lth_div, P).degree() == 0: # coprime
                 _log.debug("%s $$$$" % str((0, l)))
                 return (0, l)
 
             # there exist non trivial common divisors
-            g0 = _PolyPow(E, (bfsize - 1) // 2, lth_div) #y^(q-1)
+            g0 = _PolyPow(E, (bfsize - 1) >> 1, lth_div) #y^(q-1)
             P = self._sub2(w, g0, f[3], lth_div)
 
             if _PolyGCD(lth_div, P).degree() > 0:
                 _log.debug("%s $$" % str((2*w % l, l)))
                 return (2*w % l, l)
             else:
                 _log.debug("%s $$$" % str((-2*w % l, l)))
                 return (-2*w % l, l)
 
         else: # coprime (GCD(P, lth_div).degree() == 0)
             Y = x - x_frobfrob
-            g0 = _PolyPow(E, (bfsize - 1) // 2, lth_div) #y^(q-1)
+            g0 = _PolyPow(E, (bfsize - 1) >> 1, lth_div) #y^(q-1)
             g1 = _PolyPow(g0, bfsize + 1, lth_div) #y^(q^2-1)
             f = -self._sub2(k, g1, f3, lth_div)
             h1 = _PolyMulRed([f, f], lth_div)
-            if k % 2 == 0:
+            if k & 1 == 0:
                 g = (_PolyMulRed([Y, E, f3], lth_div) - f0) * 4
                 h0 = _PolyMulRed([g, g], lth_div)
                 aux1 = _PolyMulRed([f0, h0], lth_div) + h1
                 X_d = _PolyMulRed([E, f3, h0], lth_div)
             else:
                 g = (_PolyMulRed([Y, f3], lth_div) - _PolyMulRed([E, f0], lth_div)) * 4
                 h0 = _PolyMulRed([g, g], lth_div)
                 aux1 = _PolyMulRed([E, _PolyMulRed([f0, h0], lth_div) + h1], lth_div)
                 X_d = _PolyMulRed([f3, h0], lth_div)
             X_n = _PolyMulRed([X_d, x_frobfrob + x_frob + x], lth_div) - aux1
 
             # loop of t
             e_q = _PolyPow(self.cubic, bfsize, lth_div)
-            for t in range(1, (l - 1)//2 + 1):
+            for t in range(1, ((l - 1) >> 1) + 1):
                 Z_d_x, Z_n_x = self._Z_x(t, D, e_q, bfsize, lth_div)
                 # X_n * Z_d_x == X_d * Z_n_x (mod lth_div)?
                 if not _PolyMod(X_n * Z_d_x - X_d * Z_n_x, lth_div):
                     break
             else: # loop of t exhausted
                 _log.debug("%s @@@" % str((0, l)))
                 return (0, l)
 
             # found: X_n * Z_d_x == X_d * Z_n_x (mod lth_div)
             y0 = _PolyMulRed([-2*x_frobfrob - x, X_d], lth_div) + aux1
-            if k % 2 == 0:
+            if k & 1 == 0:
                 Y_d = _PolyMulRed([E, D[k], g, X_d], lth_div)
             else:
                 Y_d = _PolyMulRed([D[k], g, X_d], lth_div)
             Y_n = -_PolyMulRed([g1, Y_d], lth_div) - _PolyMulRed([f, y0], lth_div)
             Z_d_y, Z_n_y = self._Z_y(t, D, g0, bfsize, lth_div)
 
             # Y_n * Z_d_y == Y_d * Z_n_y (mod lth_div)?
@@ -881,15 +881,15 @@
         The aim is to compute x^q - x mod D_{l} or x^{q^2} - x mod D_{l}.
         """
         D = self.division_polynomials
         f = {}
         f[0] = _PolyMulRed([D[k-1], D[k+1]], lth_div)
         f[3] = _PolyMulRed([D[k], D[k]], lth_div)
         f[4] = _PolyMulRed([t, f[3]], lth_div)
-        if k % 2 == 0:
+        if k & 1 == 0:
             P = _PolyMulRed([f[4], self.cubic], lth_div) + f[0]
         else:
             P = f[4] + _PolyMulRed([f[0], self.cubic], lth_div)
         return f, P
 
     def _sub2(self, k, g, t, lth_div):
         """
@@ -903,33 +903,33 @@
 
         The aim is to compute y^q - y mod D_{l} or y^{q^2} - y mod D_{l}.
         """
         D = self.division_polynomials
         fk = _PolyMulRed([4 * g, t, D[k]], lth_div)
         f1 = _PolyMulRed([D[k-1], D[k-1], D[k+2]], lth_div)
         f2 = _PolyMulRed([D[k-2], D[k+1], D[k+1]], lth_div)
-        if k % 2 == 0:
+        if k & 1 == 0:
             cubic = self.cubic
             P = _PolyMulRed([fk, cubic, cubic], lth_div) - f1 + f2
         else:
             P = fk - f1 + f2
         return P
 
     def _Z_x(self, t, D, e_q, bfsize, lth_div):
         d = _PolyPow(D[t], 2 * bfsize, lth_div)
         n = _PolyPow(_PolyMulRed([D[t-1], D[t+1]], lth_div), bfsize, lth_div)
-        if t % 2 == 0:
+        if t & 1 == 0:
             d = _PolyMulRed([e_q, d], lth_div)
         else:
             n = _PolyMulRed([e_q, n], lth_div)
         return d, n
 
     def _Z_y(self, t, D, g0, bfsize, lth_div):
         E = self.cubic
-        if t % 2 == 0:
+        if t & 1 == 0:
             d = _PolyPow(_PolyMulRed([4 * E, E, D[t], D[t], D[t]], lth_div), bfsize, lth_div)
         else:
             d = _PolyPow(_PolyMulRed([4 * D[t], D[t], D[t]], lth_div), bfsize, lth_div)
         z0 = _PolyPow(_PolyMulRed([D[t-1], D[t-1], D[t+2]], lth_div) - _PolyMulRed([D[t-2], D[t+1], D[t+1]], lth_div), bfsize, lth_div)
         n = _PolyMulRed([g0, z0], lth_div)
         return d, n
 
@@ -1222,15 +1222,15 @@
         """
         return f_P(D_Q)
         this is used for Tate/Weil pairing
 
         suppose that P be an m-torsion point .
         support point R must be in neither groups generated by P nor Q.
 
-        return False if parameters lack any conditions above. 
+        return False if parameters lack any conditions above.
 
         NOTE: algorithm limitations forced that assume R is not P-Q .
         """
         # check order
         if m < 2 or not (m % self.ch):
             raise ValueError("order more than 1 and not be divisible by characteristic")
 
@@ -1340,15 +1340,15 @@
         j = 1
         while j <= m:
             Plist.append(R)
             R = self.add(R, P)
             j += 1
         R = self.mul(2*m, P)
         k = -m
-        Plist_rev = map(self.mul, [-1]*(m+1), Plist) # make reverse point mapping
+        Plist_rev = list(map(self.mul, [-1]*(m+1), Plist)) # make reverse point mapping
         j = 0
         while k <= m:
             S = self.add(Q, self.mul(k, R))
             if S in Plist:
                 j = Plist.index(S)
                 break
             elif S in Plist_rev:
@@ -1410,17 +1410,17 @@
 
         # step 2. decompose N.
         r = gcd.gcd(card(simplified.basefield) - 1, N)
         _log.debug("r = %d, N = %d" % (r, N))
         r_factor = factor_misc.FactoredInteger(r)
         N1, N2 = 1, N
         for p in r_factor.prime_divisors():
-            k, N2 = arith1.vp(N2, p=p)  
+            k, N2 = arith1.vp(N2, p=p)
             N1 *= p**k
-    
+
         _log.debug("loop")
         while 1:
             P1 = self.infpoint
             while P1 == self.infpoint:
                 P1 = simplified.point()
             P2 = self.infpoint
             while P2 == self.infpoint:
@@ -1447,25 +1447,25 @@
         """
         returns supersingularities.
         """
         if self.order() % self.ch == 1:
             return True
         else:
             return False
-    
+
 def EC(coefficient, basefield=None):
     """
     generate new elliptic curve class.
     """
     try:
         character = basefield.getCharacteristic()
         field = basefield
     except:
         # backward compatiblity
-        if isinstance(basefield, (int, long)):
+        if isinstance(basefield, int):
             field = finitefield.FinitePrimeField(basefield)
             character = basefield
         elif isinstance(basefield, rational.RationalField) or not basefield:
             character = 0 # necessary to be defined
         else:
             raise ValueError("basefield must be RationalFieid or FiniteField.")
```

### Comparing `NZMATH-1.1.0/nzmath/prime.py` & `nzmath-3.0.0/src/prime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """
 A module for generating primes and testing primality.
 """
 
 import logging
+import warnings
 import nzmath.arith1 as arith1
 import nzmath.gcd as gcd
 import nzmath.bigrandom as bigrandom
 import nzmath.bigrange as bigrange
+import nzmath.poly.array as array_poly
 from nzmath.config import GRH
+from nzmath.plugins import MATHMODULE as math
 
 _log = logging.getLogger('nzmath.prime')
 _log.setLevel(logging.DEBUG)
 
 
+PRIMES_LE_31 = (2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31)
+PRIMONIAL_31 = arith1.product(PRIMES_LE_31)
+
+
 def trialDivision(n, bound=0):
     """
     Trial division primality test for an odd natural number.
     Optional second argument is a search bound of primes.
     If the bound is given and less than the sqaure root of n
     and True is returned, it only means there is no prime factor
     less than the bound.
@@ -33,15 +40,15 @@
 
 
 def spsp(n, base, s=None, t=None):
     """
     Strong Pseudo-Prime test.  Optional third and fourth argument
     s and t are the numbers such that n-1 = 2**s * t and t is odd.
     """
-    if not s or not t:
+    if s is None or t is None:
         s, t = arith1.vp(n-1, 2)
     z = pow(base, t, n)
     if z != 1 and z != n-1:
         j = 0
         while j < s:
             j += 1
             z = pow(z, 2, n)
@@ -56,24 +63,23 @@
     """
     Miller's primality test.
 
     This test is valid under GRH.
     """
     s, t = arith1.vp(n - 1, 2)
     # The O-constant 2 by E.Bach
-    ## 2 log(n) = 2 log_2(n)/log_2(e) = 2 log(2) log_2(n)
-    ## 2 log(2) <= 1.3862943611198906
-    bound = min(n - 2, 13862943611198906 * arith1.log(n) // 10 ** 16) + 1
+    ## ln(n) = log_2(n)/log_2(e) = ln(2) * log_2(n)
+    ## 2 * ln(2) ** 2 <= 0.960906027836404
+    bound = min(n - 1, 960906027836404 * (arith1.log(n) + 1) ** 2 // 10 ** 15 + 1)
     _log.info("bound: %d" % bound)
     for b in range(2, bound):
         if not spsp(n, b, s, t):
             return False
     return True
 
-
 def millerRabin(n, times=20):
     """
     Miller-Rabin pseudo-primality test.  Optional second argument
     times (default to 20) is the number of repetition.  The error
     probability is at most 4**(-times).
     """
     s, t = arith1.vp(n - 1, 2)
@@ -89,16 +95,16 @@
     Giving up rigorous proof of primality, return True for a probable
     prime.
     """
     if int(z) != z:
         raise ValueError("non-integer for primeq()")
     elif z <= 1:
         return False
-    elif gcd.gcd(z, 510510) > 1:
-        return (z in (2, 3, 5, 7, 11, 13, 17))
+    elif gcd.gcd(z, PRIMONIAL_31) > 1:
+        return (z in PRIMES_LE_31)
     return millerRabin(z)
 
 
 def Lucas_chain(n, f, g, x_0, x_1):
     """
     Given an integer n, two functions f and g, and initial value (x_0, x_1),
     compute (x_n, x_{n+1}), where the sequence {x_i} is defined as:
@@ -115,15 +121,15 @@
             u, v = f(u), g(u, v)
     return u, v
 
 
 def _lucas_test_sequence(n, a, b):
     """
     Return x_0, x_1, x_m, x_{m+1} of Lucas sequence of parameter a, b,
-    where m = (n - (a**2 - 4*b / n)) // 2.
+    where m = (n - (a**2 - 4*b / n)) >> 1.
     """
     d = a**2 - 4*b
     if (d >= 0 and arith1.floorsqrt(d) ** 2 == d) \
     or not(gcd.coprime(n, 2*a*b*d)):
         raise ValueError("Choose another parameters.")
 
     x_0 = 2
@@ -139,15 +145,15 @@
 
     def odd_step(u, v):
         """
         'add' u and v.
         """
         return (u*v - x_1) % n
 
-    m = (n - arith1.legendre(d, n)) // 2
+    m = (n - arith1.legendre(d, n)) >> 1
     x_m, x_mplus1 = Lucas_chain(m, even_step, odd_step, x_0, x_1)
 
     return x_0, x_1, x_m, x_mplus1
 
 
 def lpsp(n, a, b):
     """
@@ -165,20 +171,75 @@
     Frobenius test.
     Return True if n is a Frobenius pseudoprime of parameters a, b,
     i.e. with respect to x**2-a*x+b.
     """
     x_0, x_1, x_m, x_mplus1 = _lucas_test_sequence(n, a, b)
 
     if (x_1 * x_m - x_0 * x_mplus1) % n == 0:
-        euler_pow = pow(b, (n-1)//2, n)
+        euler_pow = pow(b, (n-1) >> 1, n)
         return (euler_pow * x_m) % n == 2
     else:
         return False
 
 
+def by_primitive_root(n, divisors):
+    """
+    Return True iff n is prime.
+
+    The method proves the primality of n by existence of a primitive
+    root.  It requires a sequence of all prime divisors of n - 1.
+
+    Lehmer,D.H., Tests for primality by the converse of Fermat's
+    theorem, Bull.Amer.Math.Soc, Vol.33, pp.327-340, 1927.
+    """
+    m_order = n - 1
+    primes = tuple(p for p in divisors if p > 2)
+    for g in bigrange.range(2, n):
+        jacobi = arith1.legendre(g, n)
+        if jacobi == 0:
+            return False
+        elif jacobi == 1:
+            continue
+        if pow(g, m_order, n) != 1:
+            return False
+        if all(pow(g, m_order // p, n) != 1 for p in primes):
+            return True
+    return True # only when n=2, flow reaches this line
+
+
+def full_euler(n, divisors):
+    """
+    Return True iff n is prime.
+
+    The method proves the primality of n by the equality
+    phi(n) = n - 1, where phi denotes the Euler totient.
+    It requires a sequence of all prime divisors of n - 1.
+
+    Brillhart,J. & Selfridge,J.L., Some Factorizations of $2^n\pm 1$
+    and Related Results, Math.Comp., Vol.21, 87-96, 1967
+    """
+    m_order = n - 1
+    primes = set(divisors)
+    for g in bigrange.range(2, n):
+        if pow(g, m_order, n) != 1:
+            return False
+        if 2 in primes:
+            jacobi = arith1.legendre(g, n)
+            if jacobi == 0:
+                return False
+            elif jacobi == -1:
+                primes.remove(2)
+        satisfied = [p for p in primes if p > 2 and pow(g, m_order // p, n) != 1]
+        if satisfied:
+            primes.difference_update(satisfied)
+        if not primes:
+            return True
+    return True # only when n=2, flow reaches this line
+
+
 def prime(s):
     """
     prime(n) returns the n-th prime number.
     """
     if s != int(s):
         raise ValueError("non-integer for prime()")
     elif s <= 0:
@@ -209,51 +270,63 @@
 
 
 def generator_eratosthenes(n):
     """
     Generate primes up to n (inclusive) using Eratosthenes sieve.
     """
     if n < 2:
-        raise StopIteration
+        return # raise StopIteration (RuntimeError by PEP479)
+
     yield 2
+    if n <= 2:
+        return
 
-    sieve_len_max = (n+1)//2
-    if n < 400:
-        # simple init is faster below 400, on my machine :-)
-        sieve = [1] * sieve_len_max
-        k = 3
-        i = 1
-    else:
-        yield 3
-        sieve = [1, 0, 1]
-        k = 5
-        i = 2
-        sieve_len = 3
-        while sieve_len < sieve_len_max:
-            if sieve[i]:
-                yield k
+    yield 3
+
+    # make list for sieve
+    sieve_len_max = (n+1) >> 1
+    sieve = [True, False, True]
+    sieve_len = 3
+    k = 5
+    i = 2
+    while sieve_len < sieve_len_max:
+        if sieve[i]:
+            yield k
+            sieve_len *= k
+            if sieve_len_max < sieve_len:
+                sieve_len //= k
+                # adjust sieve list length
+                sieve *= sieve_len_max // sieve_len
+                sieve += sieve[:(sieve_len_max - len(sieve))]
+                sieve_len = sieve_len_max
+            else:
                 sieve = sieve * k
-                sieve_len *= k
-                for j in range(i, sieve_len, k):
-                    sieve[j] = 0
-            k, i = k+2, i+1
-        sieve = sieve[:sieve_len_max]
+            for j in range(i, sieve_len, k):
+                sieve[j] = False
+        k += 2
+        i += 1
 
-    while k*k <= n:
+    # sieve
+    limit = arith1.floorsqrt(n)
+    while k <= limit:
         if sieve[i]:
             yield k
-            j = i + k
+            j = (k ** 2 - 1) >> 1
             while j < sieve_len_max:
-                sieve[j] = 0
+                sieve[j] = False
                 j += k
-        k, i = k+2, i+1
-    while k <= n:
+        k += 2
+        i += 1
+
+    # output result
+    limit = (n - 1) >> 1
+    while i <= limit:
         if sieve[i]:
-            yield k
-        k, i = k+2, i+1
+            yield 2 * i + 1
+        i += 1
 
 
 def nextPrime(n):
     """
     Return the smallest prime bigger than the given integer.
     """
     if n <= 1:
@@ -286,37 +359,40 @@
     # search continues from the lower bound.
     p = 10**(n-1) + 1
     while not primeq(p):
         p += 2
     return p
 
 
-def smallSpsp(n):
+def smallSpsp(n, s=None, t=None):
     """
     4 spsp tests are sufficient to determine whether an integer less
-    than 10**12 is prime or not.
+    than 10**12 is prime or not.  Optional third and fourth argument
+    s and t are the numbers such that n - 1 = 2**s * t and t is odd.
     """
-    for p in [2, 13, 23, 1662803]:
-        if not spsp(n, p):
+    if s is None or t is None:
+        s, t = arith1.vp(n - 1, 2)
+    for p in (2, 13, 23, 1662803):
+        if not spsp(n, p, s, t):
             return False
     return True
 
 
 def primeq(n):
     """
-    A convinient function for primatilty test. It uses one of
+    A convenient function for primatilty test. It uses one of
     trialDivision, smallSpsp or apr depending on the size of n.
     """
     if int(n) != n:
         raise ValueError("non-integer for primeq()")
     if n <= 1:
         return False
 
-    if gcd.gcd(n, 510510) > 1:
-        return (n in (2, 3, 5, 7, 11, 13, 17))
+    if gcd.gcd(n, PRIMONIAL_31) > 1:
+        return (n in PRIMES_LE_31)
     if n < 2000000:
         return trialDivision(n)
     if not smallSpsp(n):
         return False
     if n < 10 ** 12:
         return True
     if not GRH:
@@ -330,27 +406,44 @@
     Return 2*3*...*p for given prime p.
     """
     return arith1.product(generator_eratosthenes(p))
 
 
 # defs for APR algorithm
 
-def _isprime(n):
-    if gcd.gcd(n, 510510) > 1:
-        return (n in (2, 3, 5, 7, 11, 13, 17))
-    return smallSpsp(n)
+def _isprime(n, pdivisors=None):
+    """
+    Return True iff n is prime.
+
+    The check is done without APR.
+    Assume that n is very small (less than 10**12) or
+    prime factorization of n - 1 is known (prime divisors are passed to
+    the optional argument pdivisors as a sequence).
+    """
+    if gcd.gcd(n, PRIMONIAL_31) > 1:
+        return (n in PRIMES_LE_31)
+    elif n < 10 ** 12:
+        # 1369 == 37**2
+        # 1662803 is the only prime base in smallSpsp which has not checked
+        return n < 1369 or n == 1662803 or smallSpsp(n)
+    else:
+        return full_euler(n, pdivisors)
 
 def properDivisors(n):
     """
     Return proper divisors of n (divisors of n excluding 1 and n).
 
     It is only useful for a product of small primes.
     One can use FactoredInteger.proper_divisors() as well.
+
+    DEPRECATION: this function will be removed in version 1.3.
     """
-    if n in (2, 3, 5, 7, 11, 13, 17, 19, 23):
+    warnings.warn(DeprecationWarning("properDivisor is deprecated"))
+
+    if n in (1, 2, 3, 5, 7, 11, 13, 17, 19, 23):
         return []
     else:
         l = [1]
         for p, e in _factor(n):
             for j in range(1, e + 1):
                 l += [k*pow(p, j) for k in l if k % p != 0]
         l.remove(1)
@@ -362,15 +455,15 @@
     """
     Trial division factorization for a natural number.
     Optional second argument is a search bound of primes.
     If the bound is given and less than the sqaure root of n,
     result is not proved to be a prime factorization.
     """
     factors = []
-    if not (n % 2):
+    if not (n & 1):
         v2, n = arith1.vp(n, 2)
         factors.append((2, v2))
     m = _calc_bound(n, bound)
     p = 3
     while p <= m:
         if not (n % p):
             v, n = arith1.vp(n, p)
@@ -403,15 +496,15 @@
 
 class Zeta(object):
     """
     Represent linear combinations of roots of unity.
     """
     def __init__(self, size, pos=None, val=1):
         self.size = size
-        self.z = [0]*self.size
+        self.z = [0] * self.size
         if pos is not None:
             self.z[pos % self.size] = val
 
     def __add__(self, other):
         if self.size == other.size:
             m = self.size
             zr_a = Zeta(m)
@@ -435,15 +528,15 @@
                     continue
                 elif other.z[k] == 1:
                     zr_m = zr_m + (self<<k)
                 else:
                     zr_m = zr_m + (self<<k)*other.z[k]
             return zr_m
         else:
-            m = gcd.lcm(self.size,other.size)
+            m = gcd.lcm(self.size, other.size)
             return self.promote(m)*other.promote(m)
 
     __rmul__ = __mul__
 
     def __lshift__(self, offset):
         """
         The name is shift but the meaning of function is rotation.
@@ -486,38 +579,44 @@
 
     def _square_mod(self, mod):
         return self * self % mod
 
     def __pos__(self):
         m = self.size
         z_p = Zeta(m)
-        if m % 2 == 0:
-            mp = m//2
+        if m & 1 == 0:
+            mp = m >> 1
             for i in range(mp):
                 if self.z[i] > self.z[i+mp]:
                     z_p.z[i] = self.z[i] - self.z[i+mp]
                 else:
                     z_p.z[i+mp] = self.z[i+mp] - self.z[i]
         else:
             p = 3
             while m % p:
                 p += 2
-            mp = m//p
+            mp = m // p
             for i in range(mp):
-                min = self.z[i]
+                mini = self.z[i]
                 for j in range(mp + i, m, mp):
-                    if min > self.z[j]:
-                        min = self.z[j]
+                    if mini > self.z[j]:
+                        mini = self.z[j]
                 for j in range(i, m, mp):
-                    z_p.z[j] = self.z[j] - min
+                    z_p.z[j] = self.z[j] - mini
         return z_p
 
     def __mod__(self, mod):
+        """
+        Return a new Zeta instance modulo 'mod'.
+
+        All entries are reduced to the least absolute residues.
+        """
         new = Zeta(self.size)
-        new.z = [x%mod for x in self.z]
+        half = (mod - 1) >> 1 # -1 to make 1 (mod 2) be 1, not -1.
+        new.z = [(x + half) % mod - half for x in self.z]
         return new
 
     def __setitem__(self, position, value):
         self.z[position % self.size] = value
 
     def __getitem__(self, position):
         return self.z[position % self.size]
@@ -536,18 +635,27 @@
 
     def __eq__(self, other):
         for i in range(self.size):
             if self.z[i] != other.z[i]:
                 return False
         return True
 
+    def __hash__(self):
+        return sum([hash(self.z[i]) for i in range(1, self.size)])
+
     def weight(self):
-        return len(filter(None,self.z))
+        """
+        Return the number of nonzero entries.
+        """
+        return len([_f for _f in self.z if _f])
 
     def mass(self):
+        """
+        Return the sum of all entries.
+        """
         return sum(self.z)
 
 
 class FactoredInteger(object):
     """
     Integers with factorization information.
     """
@@ -569,24 +677,24 @@
     def from_partial_factorization(cls, integer, partial):
         """
         Construct a new FactoredInteger object from partial
         factorization information given as dict of type
         {prime:exponent}.
         """
         partial_factor = 1
-        for p, e in partial.iteritems():
+        for p, e in partial.items():
             partial_factor *= p**e
         assert not integer % partial_factor, "wrong factorization"
         return cls(integer // partial_factor) * cls(partial_factor, partial)
 
     def __iter__(self):
         """
         Default iterator
         """
-        return self.factors.iteritems()
+        return iter(self.factors.items())
 
     def __mul__(self, other):
         if isinstance(other, FactoredInteger):
             integer = self.integer * other.integer
             new_factors = self.factors.copy()
             for p in other.factors:
                 new_factors[p] = new_factors.get(p, 0) + other.factors[p]
@@ -600,50 +708,77 @@
         new_integer = self.integer**other
         new_factors = {}
         for p in self.factors:
             new_factors[p] = self.factors[p] * other
         return self.__class__(new_integer, new_factors)
 
     def __pos__(self):
-        return self.copy(self)
+        return self.copy()
 
     def __str__(self):
         return str(self.integer)
 
     def __eq__(self, other):
-        return self.integer == int(other)
+        try:
+            return self.integer == other.integer
+        except AttributeError:
+            return self.integer == int(other)
+
+    def __hash__(self):
+        return hash(self.integer)
 
     def __ne__(self, other):
-        return self.integer != int(other)
+        return not self.__eq__(other)
 
     def __le__(self, other):
-        return self.integer <= int(other)
+        try:
+            return self.integer <= other.integer
+        except AttributeError:
+            return self.integer <= int(other)
 
     def __lt__(self, other):
-        return self.integer < int(other)
+        try:
+            return self.integer < other.integer
+        except AttributeError:
+            return self.integer < int(other)
 
     def __gt__(self, other):
-        return self.integer > int(other)
+        try:
+            return self.integer > other.integer
+        except AttributeError:
+            return self.integer > int(other)
 
     def __ge__(self, other):
-        return self.integer >= int(other)
+        try:
+            return self.integer >= other.integer
+        except AttributeError:
+            return self.integer >= int(other)
 
     def __long__(self):
         return int(self.integer)
 
     __int__ = __long__
 
-    def copy(self):
-        return self.__class__(self.integer, self.factors.copy())
-
     def __mod__(self, other):
         # maybe you want self.is_divisible_by(other)
-        if int(other) in self.factors:
-            return 0
-        return self.integer % int(other)
+        try:
+            if other.integer in self.factors:
+                return 0
+            return self.integer % other.integer
+        except AttributeError:
+            if int(other) in self.factors:
+                return 0
+            return self.integer % int(other)
+
+    def __rfloordiv__(self, other):
+        # assume other is an integer.
+        return other // self.integer
+
+    def copy(self):
+        return self.__class__(self.integer, self.factors.copy())
 
     def is_divisible_by(self, other):
         """
         Return True if other divides self.
         """
         if int(other) in self.factors:
             # other is prime and divides
@@ -659,27 +794,27 @@
         if divisor in quotient.factors:
             if quotient.factors[divisor] == 1:
                 del quotient.factors[divisor]
             else:
                 quotient.factors[divisor] -= 1
         elif not isinstance(other, FactoredInteger):
             dividing = divisor
-            for p, e in self.factors.iteritems():
+            for p, e in self.factors.items():
                 while not dividing % p:
                     dividing //= p
                     if quotient.factors[p] == 1:
                         del quotient.factors[p]
                         assert dividing % p, dividing
                     else:
                         quotient.factors[p] -= 1
                 if dividing == 1:
                     break
             assert dividing == 1
         else:
-            for p, e in other.factors.iteritems():
+            for p, e in other.factors.items():
                 assert p in quotient.factors and quotient.factors[p] >= e
                 if quotient.factors[p] == e:
                     del quotient.factors[p]
                 else:
                     quotient.factors[p] -= e
         quotient.integer //= divisor
         return quotient
@@ -687,61 +822,68 @@
     # maybe this is what you want, isn't it?
     __floordiv__ = exact_division
 
     def divisors(self):
         """
         Return all divisors.
         """
-        l = [1]
-        for p, e in self.factors.iteritems():
+        divs = [FactoredInteger(1)]
+        for p, e in self.factors.items():
+            q = FactoredInteger(1)
+            pcoprimes = list(divs)
             for j in range(1, e + 1):
-                l += [k*pow(p, j) for k in l if k % p]
-        l.sort()
-        return l
+                q *= FactoredInteger(p, {p:1})
+                divs += [k * q for k in pcoprimes]
+        return divs
 
     def proper_divisors(self):
         """
         Return the proper divisors (divisors of n excluding 1 and n).
         """
         return self.divisors()[1:-1]
 
     def prime_divisors(self):
         """
         Return the list of primes that divides the number.
         """
-        return self.factors.keys()
+        return list(self.factors.keys())
 
 
 class TestPrime(object):
-    primes = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31]
+    primes = PRIMES_LE_31
+    primecache = set(primes)
 
     def __init__(self, t=12):
-        if isinstance(t, (int, long)):
+        if isinstance(t, int):
             self.t = FactoredInteger(t)
         else:
             assert isinstance(t, FactoredInteger)
             self.t = t
         powerof2 = self.t.factors[2] + 2
         self.et = FactoredInteger(2 ** powerof2, {2:powerof2})
         for d in self.t.divisors():
-            p = d + 1
-            if p & 1 and _isprime(p):
+            # d is an instance of FactoredInteger
+            p = d.integer + 1
+            if p & 1 and (p in self.primecache or _isprime(p, d.factors)):
                 self.et = self.et * FactoredInteger(p, {p:1})
                 if p in self.t.factors:
                     e = self.t.factors[p]
                     self.et = self.et * FactoredInteger(p**e, {p:e})
+                self.primecache.add(p)
 
-    def next(self):
+    def __next__(self):
         eu = []
         for p in self.primes:
             if p in self.t.factors:
-                eu.append((p - 1) * (p**(self.t.factors[p] - 1)))
+                eu.append((p - 1) * p**(self.t.factors[p] - 1))
             else:
                 eu.append(p - 1)
-        return self.__class__(self.t * self.primes[eu.index(min(eu))])
+                break
+        p = self.primes[eu.index(min(eu))]
+        return self.__class__(self.t * FactoredInteger(p, {p:1}))
 
 
 class Status:
     """
     status collector for apr.
     """
     def __init__(self):
@@ -846,47 +988,47 @@
         x = 3
         while m > x:
             c = r*x
             if c > m:
                 s = pow(sx_z[x], c//m, n) * s
             step = 8 - step
             x += step
-        r = r % 8
+        r = r & 7
         if r == 5 or r == 7:
             s = J.get(2, q).promote(m) * s
         s = +(s % n)
 
         if s.weight() == 1 and s.mass() == 1:
-            if gcd.gcd(m, s.z.index(1)) == 1 and pow(q, (n-1)//2, n) == n-1:
+            if gcd.gcd(m, s.z.index(1)) == 1 and pow(q, (n-1) >> 1, n) == n-1:
                 self.done(2)
             return True
         elif s.weight() == 1 and s.mass() == n-1:
-            if gcd.gcd(m, s.z.index(n-1)) == 1 and pow(q, (n-1)//2, n) == n-1:
+            if gcd.gcd(m, s.z.index(n-1)) == 1 and pow(q, (n-1) >> 1, n) == n-1:
                 self.done(2)
             return True
         return False
 
     def sub4(self, q, n, J):
         j2 = J.get(1, 2, q)**2
         s = q*j2 % n
-        s = pow(s, n//4, n)
-        if n%4 == 3:
+        s = pow(s, n >> 2, n)
+        if n & 3 == 3:
             s = s*j2 % n
         s = +(s % n)
         if s.weight() == 1 and s.mass() == 1:
             i = s.z.index(1)
-            if (i == 1 or i == 3) and pow(q, (n-1)//2, n) == n-1:
+            if (i == 1 or i == 3) and pow(q, (n-1) >> 1, n) == n-1:
                 self.done(2)
             return True
         return False
 
     def sub2(self, q, n):
-        s = pow(n-q, (n-1)//2, n)
+        s = pow(n-q, (n-1) >> 1, n)
         if s == n-1:
-            if n % 4 == 1:
+            if n & 3 == 1:
                 self.done(2)
         elif s != 1:
             return False
         return True
 
     def subrest(self, p, n, et, J, ub=200):
         if p == 2:
@@ -896,15 +1038,15 @@
                 if not _isprime(q) or et % q == 0:
                     continue
                 if n % q == 0:
                     _log.info("%s divides %s.\n" % (q, n))
                     return False
                 k = arith1.vp(q-1, 2)[0]
                 if k == 1:
-                    if n % 4 == 1 and not self.sub2(q, n):
+                    if n & 3 == 1 and not self.sub2(q, n):
                         return False
                 elif k == 2:
                     if not self.sub4(q, n, J):
                         return False
                 else:
                     if not self.sub8(q, k, n, J):
                         return False
@@ -976,24 +1118,25 @@
             pk = p**k
             Jpq = Zeta(pk, 1 + fx[1])
             for j in range(2, qpred):
                 Jpq[j + fx[j]] = Jpq[j + fx[j]] + 1
             self.shelve[1, p, q] = +Jpq
         del fx
 
-    def makefx(self, q):
+    @staticmethod
+    def makefx(q):
         """
         Return a dict called 'fx'.
         The dict stores the information that fx[i] == j iff
           g**i + g**j = 1 mod q
         for g, a primitive root of the prime q.
         """
         g = primitive_root(q)
         qpred = q - 1
-        qd2 = qpred//2
+        qd2 = qpred >> 1
         g_mf = [0, g]
         for _ in range(2, qpred):
             g_mf.append((g_mf[-1]*g) % q)
         fx = {}
         for i in range(1, qd2):
             if i in fx:
                 continue
@@ -1016,25 +1159,25 @@
     Assuming n is spsp for several bases.
     """
     L = Status()
 
     rb = arith1.floorsqrt(n) + 1
     el = TestPrime()
     while el.et <= rb:
-        el = el.next()
+        el = next(el)
 
-    plist = el.t.factors.keys()
+    plist = list(el.t.factors.keys())
     plist.remove(2)
     L.yet(2)
     for p in plist:
         if pow(n, p-1, p*p) != 1:
             L.done(p)
         else:
             L.yet(p)
-    qlist = el.et.factors.keys()
+    qlist = list(el.et.factors.keys())
     qlist.remove(2)
     J = JacobiSum()
     for q in qlist:
         for p in plist:
             if (q-1) % p != 0:
                 continue
             if not L.subodd(p, q, n, J):
@@ -1062,7 +1205,80 @@
 
 
 class ImplementLimit (Exception):
     """
     Exception throwed when the execution hits the implementation limit.
     """
     pass
+
+
+# AKS
+def aks(n):
+    """
+    AKS ( Cyclotomic Congruence Test ) primality test for a natural number.
+    
+    Input: a natural number n ( n > 1 ).
+    Output: n is prime => return True
+            n is not prime => return False.
+    """
+    import nzmath.multiplicative as multiplicative
+
+    if arith1.powerDetection(n)[1] != 1: #Power Detection
+        return False
+
+    lg = math.log(n, 2)
+    k = int(lg * lg)
+
+    start = 3
+    while 1:
+        d = gcd.gcd(start, n)
+        if 1 < d < n:
+            return False
+        x = n % start
+        N = x
+        for i in range(1, k + 1):
+            if N == 1:
+                break
+            N = (N * x) % start
+        if i == k:
+            r = start
+            break
+        start += 1
+    d = gcd.gcd(r, n)
+    if 1 < d < n:
+        return False
+    if n <= r:
+        return True
+
+    e = multiplicative.euler(r) #Cyclotomic Conguence
+    e = math.sqrt(e)
+    e = int(e * lg)
+    for b in range(1, e + 1):
+        f = array_poly.ArrayPolyMod([b, 1], n)
+        total = array_poly.ArrayPolyMod([1], n)
+        count = n
+        while count > 0:
+            if count & 1:
+                total = total * f
+                total = _aks_mod(total, r)
+            f = f.power()
+            f = _aks_mod(f, r)
+            count = count >> 1
+        total_poly = total.coefficients_to_dict()
+        if total_poly != {0:b, n % r:1}:
+            return False
+    return True
+
+def _aks_mod(polynomial, r):
+    """
+    This function is used in aks.
+    polynomial modulo (x^r - 1)
+    """
+    total = polynomial.coefficients[:r]
+    aks_mod = polynomial.coefficients[r:]
+    while len(aks_mod) - 1 >= r:
+        for i in range(r):
+            total[i] += aks_mod[i]
+        aks_mod = aks_mod[r:]
+    for i in range(len(aks_mod)):
+        total[i] += aks_mod[i]
+    return array_poly.ArrayPolyMod(total, polynomial.mod)
```

### Comparing `NZMATH-1.1.0/nzmath/arygcd.py` & `nzmath-3.0.0/src/arygcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         y = y1
     return x, y
 
 def _FormAdj_i(a, b):
     """
     transform gaussInteger a+b*i ->  form 1+2(1+i)*(x+y*i)
     """
-    if a % 2 == 0:
+    if a & 1 == 0:
         a, b = -b, a
-    if (b - a + 1) % 4 == 0:
+    if (b - a + 1) & 3 == 0:
         return a, b
     else:
         return -a, -b
 
 
 def arygcd_w(a1, a2, b1, b2):
     """
```

### Comparing `NZMATH-1.1.0/nzmath/rational.py` & `nzmath-3.0.0/src/rational.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,32 +20,32 @@
           * Rational.
         Other objects can be converted if they have toRational
         methods.  Otherwise raise TypeError.
         """
         if not denominator:
             raise ZeroDivisionError
         # numerator
-        integer = (int, long)
+        integer = (int, int)
         initDispatcher = {
             (Rational, Rational): Rational._init_by_Rational_Rational,
             (float, Rational): Rational._init_by_float_Rational,
             (integer, Rational): Rational._init_by_int_Rational,
             (Rational, float): Rational._init_by_Rational_float,
             (float, float): Rational._init_by_float_float,
             (integer, float): Rational._init_by_int_float,
             (Rational, integer): Rational._init_by_Rational_int,
             (float, integer): Rational._init_by_float_int,
             (integer, integer): Rational._init_by_int_int,
             }
-        if not isinstance(numerator, (Rational, float, int, long)):
+        if not isinstance(numerator, (Rational, float, int)):
             if hasattr(numerator, "toRational"):
                 numerator = numerator.toRational()
             elif hasattr(numerator, "__pos__"):
                 numerator = +numerator
-        if not isinstance(denominator, (Rational, float, int, long)):
+        if not isinstance(denominator, (Rational, float, int)):
             if hasattr(denominator, "toRational"):
                 denominator = denominator.toRational()
             elif hasattr(numerator, "__pos__"):
                 denominator = +denominator
         for (t1, t2) in initDispatcher:
             if isinstance(numerator, t1) and isinstance(denominator, t2):
                 initDispatcher[(t1, t2)](self, numerator, denominator)
@@ -309,15 +309,15 @@
 
     def __str__(self):
         return str(self.numerator) + "/" + str(self.denominator)
 
     def __repr__(self):
         return "%s(%d, %d)" % (self.__class__.__name__, self.numerator, self.denominator)
 
-    def __nonzero__(self):
+    def __bool__(self):
         if self.numerator:
             return True
         else:
             return False
 
     def __hash__(self):
         """
@@ -632,15 +632,15 @@
         if self._zero is None:
             self._zero = Rational(0, 1)
         return self._zero
 
     zero = property(_getZero, None, None, "additive unit.")
 
 
-class Integer(long, ring.CommutativeRingElement):
+class Integer(int, ring.CommutativeRingElement):
     """
     Integer is a class of integer.  Since 'int' and 'long' do not
     return rational for division, it is needed to create a new class.
     """
     def __init__(self, value):
         ring.CommutativeRingElement.__init__(self)
 
@@ -657,90 +657,93 @@
             return NotImplemented
 
     __truediv__ = __div__
 
     __rtruediv__ = __rdiv__
 
     def __floordiv__(self, other):
-        return Integer(long(self)//other)
+        return Integer(int(self)//other)
 
     def __rfloordiv__(self, other):
         try:
-            return Integer(other//long(self))
+            return Integer(other//int(self))
         except:
             return NotImplemented
 
     def __mod__(self, other):
-        if isinstance(other, (int, long)):
-            return Integer(long(self)%long(other))
+        if isinstance(other, int):
+            return Integer(int(self)%int(other))
         return NotImplemented
 
     def __rmod__(self, other):
-        return Integer(other%long(self))
+        return Integer(other%int(self))
 
     def __divmod__(self, other):
-        return tuple([Integer(x) for x in divmod(long(self), other)])
+        return tuple([Integer(x) for x in divmod(int(self), other)])
 
     def __rdivmod__(self, other):
-        return tuple([Integer(x) for x in divmod(other, long(self))])
+        return tuple([Integer(x) for x in divmod(other, int(self))])
 
     def __add__(self, other):
         if isIntegerObject(other):
-            return Integer(long(self)+other)
+            return Integer(int(self)+other)
         else:
             return NotImplemented
 
     __radd__ = __add__
 
     def __sub__(self, other):
         if isIntegerObject(other):
-            return Integer(long(self)-other)
+            return Integer(int(self)-other)
         else:
             return NotImplemented
 
     def __rsub__(self, other):
-        return Integer(other-long(self))
+        return Integer(other-int(self))
 
     def __mul__(self, other):
-        if isinstance(other, (int, long)):
-            return self.__class__(long(self) * other)
+        if isinstance(other, int):
+            return self.__class__(int(self) * other)
         try:
             retval = other.__rmul__(self)
             if retval is not NotImplemented:
                 return retval
         except Exception:
             pass
         return self.actAdditive(other)
 
     def __rmul__(self, other):
-        if isinstance(other, (int, long)):
-            return self.__class__(other * long(self))
-        elif other.__class__ in __builtins__.values():
-            return other.__mul__(long(self))
+        if isinstance(other, int):
+            return self.__class__(other * int(self))
+        elif other.__class__ in list(__builtins__.values()):
+            return other.__mul__(int(self))
         return self.actAdditive(other)
 
     def __pow__(self, index, modulo=None):
         """
         If index is negative, result may be a rational number.
         """
         if modulo is None and index < 0:
-            return Rational(1, long(self) ** (-index))
-        return Integer(pow(long(self), index, modulo))
+            return Rational(1, int(self) ** (-index))
+        return Integer(pow(int(self), index, modulo))
 
     def __pos__(self):
         return Integer(self)
 
     def __neg__(self):
-        return Integer(-long(self))
+        return Integer(-int(self))
 
     def __abs__(self):
-        return Integer(abs(long(self)))
+        return Integer(abs(int(self)))
 
     def __eq__(self, other):
-        return long(self) == long(other)
+        return int(self) == int(other)
+
+    def __hash__(self):
+        return hash(int(self))
 
     def getRing(self):
         return theIntegerRing
 
     def inverse(self):
         return Rational(1, self)
 
@@ -926,23 +929,23 @@
 
 
 def isIntegerObject(anObject):
     """
     True if the given object is instance of int or long,
     False otherwise.
     """
-    return isinstance(anObject, (int, long))
+    return isinstance(anObject, int)
 
 def IntegerIfIntOrLong(anObject):
     """
     Cast int or long objects to Integer.
     The objects in list or tuple can be casted also.
     """
     objectClass = anObject.__class__
-    if objectClass == int or objectClass == long:
+    if objectClass == int or objectClass == int:
         return Integer(anObject)
     elif isinstance(anObject, (list,tuple)):
         return objectClass([IntegerIfIntOrLong(i) for i in anObject])
     return anObject
 
 ##
 def continued_fraction_expansion(target, terms):
```

### Comparing `NZMATH-1.1.0/nzmath/compatibility.py` & `nzmath-3.0.0/src/compatibility.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,22 @@
     set, frozenset
 except NameError:
     import sets
     __builtins__["set"] = sets.Set
     __builtins__["frozenset"] = sets.ImmutableSet
     del sets
 
+# __builtins__.cmp is only in <3.0.
+# Be careful that the compatibility is not perfect.
+try:
+    cmp
+except NameError:
+    cmp = lambda x,y: (x>y) - (x<y)
+    __builtins__["cmp"] = cmp
+    del cmp
 
 # builtin len() raises OverflowError when the result > sys.maxint.
 # I'm not sure this restriction will go away in the future.
 # The following function card() ought to be used instead of len()
 # for obtaining cardinality of sets or set-like objects.
 def card(virtualset):
     """
```

### Comparing `NZMATH-1.1.0/nzmath/matrix.py` & `nzmath-3.0.0/src/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from __future__ import division
+
 
 import nzmath.ring as ring
 import nzmath.vector as vector
+from functools import reduce
 
 
 class Matrix(object):
     """
     Matrix is a class for matrices.
     """
 
@@ -16,16 +17,16 @@
         self._initialize(row, column, compo, coeff_ring)
         self._selectMatrix()
 
     def _initialize(self, row, column, compo=0, coeff_ring=0):
         """
         initialize matrix.
         """
-        if (isinstance(row, (int, long))
-            and isinstance(column, (int, long))
+        if (isinstance(row, int)
+            and isinstance(column, int)
             and row > 0
             and column > 0 ): # row and column check
             self.row = row
             self.column = column
             self.compo = []
             if isinstance(compo, (ring.Ring, int)):
                 coeff_ring = compo
@@ -83,15 +84,15 @@
             if coeff_ring == 0:
                 self.coeff_ring = ring.getRing(self.compo[0][0])
             else:
                 self.coeff_ring = coeff_ring = _getRing(coeff_ring)
                 if not(isinstance(ring.getRing(self.compo[0][0]), coeff_ring.__class__)):
                     compos = []
                     for i in range(self.row):
-                        compos.append(map(coeff_ring.createElement, self.compo[i]))
+                        compos.append(list(map(coeff_ring.createElement, self.compo[i])))
                     self.compo = compos
         else:
             raise ValueError("invalid value for matrix size")
 
     def _selectMatrix(self):
         """
         Select Matrix class.
@@ -110,27 +111,27 @@
     def __getitem__(self, index):
         """
         M[i,j] : Return (i,j)-component of M.
         M[i] <==> M.getColumn(i)
         """
         if isinstance(index, tuple):
             return self.compo[index[0] - 1][index[1] - 1]
-        elif isinstance(index, (int, long)):
+        elif isinstance(index, int):
             return self.getColumn(index)
         else:
             raise IndexError("Matrix invalid index: %s" % index)
 
     def __setitem__(self, key, value):
         """
         M[i,j] = a   :   Substitute a for (i,j)-component of M.
         M[i] = V <==> M.setColumn(i, V)
         """
         if isinstance(key, tuple):
             self.compo[key[0] - 1][key[1] - 1] = value
-        elif isinstance(key, (int, long)):
+        elif isinstance(key, int):
             self.setColumn(key, value)
         else:
             raise TypeError(self.__setitem__.__doc__)
 
     def __eq__(self, other):
         """
         Check self == other.
@@ -145,22 +146,29 @@
                         return False
             return True
         elif isinstance(other, int) and other == 0: # zero matrix ?
             return not bool(self)
         else:
             return False
 
+    def __hash__(self):
+        val = 0
+        for i in range(self.row):
+            for j in range(self.column):
+                val += hash(self.compo[i][j])
+        return val
+
     def __ne__(self, other):
         """
         Check self != other.
         self != 0 means whether self != zeromatrix or not.
         """
         return not (self == other)
 
-    def __nonzero__(self):
+    def __bool__(self):
         """
         Check self != zeromatrix
         """
         for i in range(self.row):
             for j in range(self.column):
                 if self.compo[i][j]:
                     return True
@@ -213,15 +221,15 @@
 
     def map(self, function):
         """
         Return matrix applied function to all self elements.
         """
         compos = []
         for i in range(self.row):
-            compos = compos + (map(function, self.compo[i]))
+            compos = compos + (list(map(function, self.compo[i])))
         return createMatrix(self.row, self.column, compos)
 
     def reduce(self, function, initializer=None):
         """
         Return value applied binomial function to all self elements.
         """
         if initializer:
@@ -427,15 +435,15 @@
         """
         Return submatrix whose element is self[i, j] for i in I and j in J.
         If I, J is not index(list or tuple) but integer,
          return submatrix which deleted I-th row and J-th column from self.
         """
         if J == None:
             J = I
-        if isinstance(I, (int, long)) and isinstance(J, (int, long)):
+        if isinstance(I, int) and isinstance(J, int):
             mat = self.copy()
             mat.deleteRow(I)
             mat.deleteColumn(J)
             return mat
         else:
             mat = []
             for i in I:
@@ -863,15 +871,15 @@
         self._initialize(row, column, compo, coeff_ring)
 
     def __pow__(self, other):
         """
         powering self to integer.
         """
         n = +other
-        if not isinstance(n, (int, long)):
+        if not isinstance(n, int):
             raise TypeError("index must be an integer")
         power = unitMatrix(self.row, self.coeff_ring)
         # check n
         if n == 0:
             return power
         if n > 0:
             z = self.copy()
@@ -1598,14 +1606,17 @@
         """
         self == other
         """
         return (self.__class__ == other.__class__ and
                 self.size == other.size and
                 self.scalars == other.scalars)
 
+    def __hash__(self):
+        return self.scalars ** self.size
+
     def __repr__(self):
         return "MatrixRing(%d, %s)" % (self.size, self.scalars)
 
     def __str__(self):
         return "M_%d(%s)" % (self.size, str(self.scalars))
 
     @classmethod
@@ -1766,15 +1777,15 @@
         """
         self.toBasis()
         if self.row < self.column:
             raise MatrixSizeError()
         n = self.row
         k = self.column
         M = self.copy()
-        pnt = range(1, self.row + 1)
+        pnt = list(range(1, self.row + 1))
         for s in range(1, k + 1):
             for t in range(s, n + 1):
                 if M[t, s]:
                     break
             else: # zero space
                 return unitMatrix(self.row, self.coeff_ring)
             d = ring.inverse(M[t, s])
@@ -1887,15 +1898,15 @@
     """
     return zero matrix.
     coeff is subclass for ring.Ring or ring.Ring.zero.
     """
     if column == 0:
         coeff = 0
         column = row
-    if not(isinstance(column, (int, long))):
+    if not(isinstance(column, int)):
         if column == None:
             column = row
         else:
             coeff = column
             column = row
     if isinstance(coeff, ring.Ring):
         zero = coeff.zero
```

### Comparing `NZMATH-1.1.0/nzmath/squarefree.py` & `nzmath-3.0.0/src/squarefree.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     """
     if n == 1 or n == 2:
         return True
     if arith1.issquare(n):
         return False
     if n & 1:
         return lenstra(n)
-    elif not (n % 4):
+    elif not (n & 3):
         return False
     raise Undetermined("trivial test can't determine squarefreeness")
 
 
 def viafactor(n):
     """
     Test whether n is squarefree or not.
@@ -147,15 +147,15 @@
     """
     if n == 1 or n == 2:
         return True
     if arith1.issquare(n):
         return False
     if n & 1:
         return lenstra_ternary(n)
-    elif not (n % 4):
+    elif not (n & 3):
         return False
     return None
 
 
 def trial_division_ternary(n):
     """
     Test the squarefreeness of n.
```

### Comparing `NZMATH-1.1.0/nzmath/lattice.py` & `nzmath-3.0.0/src/lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 from math import floor
 from nzmath.matrix import Matrix
 from nzmath.matrix import VectorsNotIndependent
 from nzmath.vector import *
 from nzmath.arith1 import *
 from nzmath.gcd import *
 #import nzmath.matrix as matrix
```

### Comparing `NZMATH-1.1.0/nzmath/algfield.py` & `nzmath-3.0.0/src/algfield.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 
 import math
 import nzmath.arith1 as arith1
 import nzmath.equation as equation
 import nzmath.gcd as gcd
 import nzmath.lattice as lattice
 import nzmath.vector as vector
@@ -68,15 +68,15 @@
         (The output is not field disc of self but disc of self.polynomial.)
         """
         """
         Obasis, disc = round2.round2(self)
         A = [algfield.MatAlgNumber(obasis[0][i]) for i in range(degree)]
         return disc(A) <--- real disc of self field.
         """
-   
+
         if not hasattr(self, "poldisc"):
             degree = self.degree
             traces = []
             for i in range(degree):
                 for j in range(degree):
                     s = self.basis(i)*self.basis(j)
                     traces.append(s.trace())
@@ -104,15 +104,15 @@
             self.integer_basis = matrix.createMatrix(
                 self.degree, [vector.Vector(int_basis[j]) for j in range(
                 len(int_basis))])
         return self.discriminant
 
     def basis(self, j):
         """
-        Return the j-th basis of self. 
+        Return the j-th basis of self.
         """
         base = [0] * self.degree
         base[j] = 1
         return BasicAlgNumber([base, 1], self.polynomial)
 
     def signature(self):
         """
@@ -121,49 +121,49 @@
         """
         if not hasattr(self, "sign"):
             degree = self.degree
             #Step 1.
             if degree == 0:
                 return (0, 0)
             # no check for degree 1?
-    
+
             minpoly = zpoly(self.polynomial)
             d_minpoly = minpoly.differentiate()
             A = minpoly.primitive_part()
             B = d_minpoly.primitive_part()
             g = 1
             h = 1
             pos_at_inf = A.leading_coefficient() > 0
-            pos_at_neg = pos_at_inf == (degree % 2)
+            pos_at_neg = pos_at_inf == (degree & 1)
             r_1 = 1
-    
+
             #Step 2.
             while True:
                 deg = A.degree() - B.degree()
                 residue = A.pseudo_mod(B)
                 if not residue:
                     raise ValueError("not squarefree")
-                if B.leading_coefficient() > 0 or deg % 2:
+                if B.leading_coefficient() > 0 or deg & 1:
                     residue = - residue
                 #Step 3.
                 degree_res = residue.degree()
                 pos_at_inf_of_res = residue.leading_coefficient() > 0
-    
+
                 if pos_at_inf_of_res != pos_at_inf:
                     pos_at_inf = not pos_at_inf
                     r_1 -= 1
-    
-                if pos_at_inf_of_res != (pos_at_neg == (degree_res % 2 == 0)):
+
+                if pos_at_inf_of_res != (pos_at_neg == (degree_res & 1 == 0)):
                     pos_at_neg = not pos_at_neg
                     r_1 += 1
-    
+
                 #Step 4.
                 if degree_res == 0:
-                    return (r_1, (degree - r_1)//2)
-    
+                    return (r_1, (degree - r_1) >> 1)
+
                 A, B = B, residue.scalar_exact_division(g*(h**deg))
                 g = abs(A.leading_coefficient())
                 if deg == 1:
                     h = g
                 elif deg > 1:
                     h = g**deg // h**(deg - 1)
         return self.sign
@@ -179,15 +179,15 @@
 
         #Step 1.
         Basis = self.integer_ring()
         BaseList = []
         for i in range(n):
             AlgInt = MatAlgNumber(Basis[i].compo, self.polynomial)
             BaseList.append(AlgInt)
-        
+
         #Step 2.
         traces = []
         if self.signature()[1] == 0:
             for i in range(n):
                 for j in range(n):
                     s = BaseList[i]*BaseList[j]
                     traces.append(s.trace())
@@ -203,30 +203,30 @@
                         m += f[i](sigma[k])*f[j](sigma[k].conjugate())
                     traces.append(m.real)
 
         #Step 3.
         M = matrix.createMatrix(n, n, traces)
         S = matrix.unitMatrix(n)
         L = lattice.LLL(S, M)[0]
-        
+
 
         #Step 4.
         Ch_Basis = []
         for i in range(n):
             base_cor = changetype(0, self.polynomial).ch_matrix()
             for v in range(n):
                 base_cor += BaseList[v]*L.compo[v][i]
             Ch_Basis.append(base_cor)
 
         C = []
         a = Ch_Basis[0]
         for i in range(n):
             coeff = Ch_Basis[i].ch_basic().getCharPoly()
             C.append(zpoly(coeff))
-            
+
         #Step 5.
         P = []
         for i in range(n):
             diff_C = C[i].differentiate()
             gcd_C = C[i].subresultant_gcd(diff_C)
             P.append(C[i].exact_division(gcd_C))
 
@@ -236,16 +236,16 @@
         """
         Determine whether self.basis is integral basis of self field.
         """
         D = self.disc()
         if squarefree.trial_division(abs(D)):
             return True
         else:
-            if D % 4 == 0:
-                if squarefree.trial_division(abs(D)//4) and (D//4) % 4 != 1:
+            if D & 3 == 0:
+                if squarefree.trial_division(abs(D) >> 2) and (D >> 2) & 3 != 1:
                     return True
         # compare with real integer ring
         return abs(self.integer_ring().determinant()) == 1
 
     def isGaloisField(self, other = None):
         """
         Determine whether self/other is Galois field.
@@ -253,15 +253,15 @@
         if self.signature[0] == 0 or self.signature[1] == 0:
             return "Can not determined"
         else:
             return False
 
     def isFieldElement(self, A):
         """
-        Determine whether A is field element of self field or not.  
+        Determine whether A is field element of self field or not.
         """
         poly = A.polynomial
         if poly == self.polynomial:
             return True
         else:
             if poly == self.POLRED():
                 return True
@@ -311,14 +311,17 @@
         """
         Equality test.
         """
         if self.issubring(other) and self.issuperring(other):
             return True
         return False
 
+    def __hash__(self):
+        raise NotImplementedError
+
     # properties
     def _getOne(self):
         "getter for one"
         if self._one is None:
             self._one = BasicAlgNumber([[1] + [0] * (self.degree - 1), 1],
                               self.polynomial)
         return self._one
@@ -345,27 +348,27 @@
         self.value = valuelist
         self.coeff = valuelist[0]
         self.denom = valuelist[1]
         self.degree = len(polynomial) - 1
         self.polynomial = polynomial
         self.field = NumberField(self.polynomial)
         Gcd = gcd.gcd_of_list(self.coeff)
-        GCD = gcd.gcd(Gcd[0], self.denom) 
+        GCD = gcd.gcd(Gcd[0], self.denom)
         if GCD != 1:
             self.coeff = [i//GCD for i in self.coeff]
             self.denom = self.denom//GCD
         if precompute:
             self.getConj()
             self.getApprox()
             self.getCharPoly()
-    
+
     def __repr__(self):
         return_str = '%s(%s, %s)' % (self.__class__.__name__, [self.coeff, self.denom], self.polynomial)
         return return_str
-    
+
     def __neg__(self):
         coeff = []
         for i in range(len(self.coeff)):
             coeff.append(-self.coeff[i])
         return BasicAlgNumber([coeff, self.denom], self.polynomial)
 
     def _int_to_algnumber(self, other):
@@ -386,15 +389,15 @@
         if isinstance(other, BasicAlgNumber):
             d = self.denom*other.denom
             coeff = []
             for i in range(len(self.coeff)):
                 coeff.append(
                     other.denom*self.coeff[i] + self.denom*other.coeff[i])
             return BasicAlgNumber([coeff, d], self.polynomial)
-        elif isinstance(other, (int, long)):
+        elif isinstance(other, int):
             return self + self._int_to_algnumber(other)
         elif isinstance(other, rational.Rational):
             return self + self._rational_to_algnumber(other)
         else:
             return NotImplemented
 
     __radd__ = __add__
@@ -407,16 +410,16 @@
             d = self.denom*other.denom
             f = zpoly(self.polynomial)
             g = zpoly(self.coeff)
             h = zpoly(other.coeff)
             j = (g * h).pseudo_mod(f)
             jcoeff = [j[i] for i in range(self.degree)]
             return BasicAlgNumber([jcoeff, d], self.polynomial)
-        elif isinstance(other, (int, long)):
-            Coeff = [i*other for i in self.coeff] 
+        elif isinstance(other, int):
+            Coeff = [i*other for i in self.coeff]
             return BasicAlgNumber([Coeff, self.denom], self.polynomial)
         elif isinstance(other, rational.Rational):
             GCD = gcd.gcd(other.numerator, self.denom)
             denom = self.denom * other.denominator
             mul = other.numerator
             if GCD != 1:
                 denom //= GCD
@@ -494,22 +497,22 @@
                     Approx += self.coeff[j]*(self.getConj()[i]**j)
                 APP.append(Approx)
             self.approx = APP
         return self.approx
 
     def getCharPoly(self):
         """
-        Return the characteristic polynomial of self 
+        Return the characteristic polynomial of self
         by compute products of (x-self^{(i)}).
         """
         if not hasattr(self, "charpoly"):
             Conj = self.getApprox()
             P = uniutil.polynomial({0:-Conj[0], 1:1}, ring.getRing(Conj[0]))
             for i in range(1, self.degree):
-                P *= uniutil.polynomial({0:-Conj[i], 1:1}, 
+                P *= uniutil.polynomial({0:-Conj[i], 1:1},
                     ring.getRing(Conj[i]))
             charcoeff = []
             for i in range(self.degree + 1):
                 if hasattr(P[i], "real"):
                     charcoeff.append(int(math.floor(P[i].real + 0.5)))
                 else:
                     charcoeff.append(int(math.floor(P[i] + 0.5)))
@@ -517,22 +520,22 @@
         return self.charpoly
 
     def getRing(self):
         """
         Return the algebraic number field contained self.
         """
         return NumberField(self.polynomial)
-    
+
     def trace(self):
         """
         Compute the trace of self in K.
         """
         denom = self.denom
         n = len(self.polynomial) - 1
-        
+
         tlist = [n]
         for k in range(1, n):
             s = 0
             for i in range(1, k):
                 s += tlist[k - i] * self.polynomial[n - i]
             tlist.append(-k * self.polynomial[n - k] - s)
 
@@ -565,15 +568,15 @@
                 else:
                     return rational.Rational(R, denom)
             else:
                 return R / denom
 
     def isAlgInteger(self):
         """
-        Determine whether self is an algebraic integer or not. 
+        Determine whether self is an algebraic integer or not.
         """
         Norm = self.norm()
         if isinstance(Norm, int):
             return True
         else:
             return False
 
@@ -625,15 +628,15 @@
                 basis3.append([self.coeff[j] * k for k in List[j+flag]])
             for l in range(self.degree):
                 t = 0
                 for m in range(self.degree):
                     t += basis3[m][l]
                 Matrix.append(t)
             flag += 1
-        
+
         self.matrix = matrix.createMatrix(self.degree, self.degree, Matrix)
         self.polynomial = polynomial
         self.field = NumberField(self.polynomial)
 
     def __repr__(self):
         return_str = '%s(%s, %s)' % (self.__class__.__name__, self.matrix.__repr__(), self.polynomial)
         return return_str
@@ -642,55 +645,55 @@
         mat = - self.matrix
         coeff = []
         for i in range(mat.row):
             coeff.append(mat[0][i])
         return MatAlgNumber(coeff, self.polynomial)
 
     def __add__(self, other):
-        if isinstance(other, (int, long, rational.Rational)):
+        if isinstance(other, (int, rational.Rational)):
             other = MatAlgNumber(
                 [other] + [0] * (self.degree -1), self.polynomial)
         elif not isinstance(other, MatAlgNumber):
             return NotImplemented
         mat = self.matrix + other.matrix
         coeff = []
         for i in range(mat.row):
             coeff.append(mat[i+1][1])
         return MatAlgNumber(coeff, self.polynomial)
 
     __radd__ = __add__
 
     def __sub__(self, other):
-        if isinstance(other, (int, long, rational.Rational)):
+        if isinstance(other, (int, rational.Rational)):
             other = MatAlgNumber(
                 [other] + [0] * (self.degree -1), self.polynomial)
         elif not isinstance(other, MatAlgNumber):
             return NotImplemented
         mat = self.matrix - other.matrix
         coeff = []
         for i in range(mat.row):
             coeff.append(mat[i+1][1])
         return MatAlgNumber(coeff, self.polynomial)
 
     def __mul__(self, other):
         if isinstance(other, MatAlgNumber):
             mat = self.matrix * other.matrix
-        elif isinstance(other, (int, long, rational.Rational)):
+        elif isinstance(other, (int, rational.Rational)):
             mat = other * self.matrix
         else:
             return NotImplemented
         coeff = []
         for i in range(mat.row):
             coeff.append(mat[i+1][1])
         return MatAlgNumber(coeff, self.polynomial)
 
     __rmul__ = __mul__
 
     def __truediv__(self, other):
-        if isinstance(other, (int, long, rational.Rational)):
+        if isinstance(other, (int, rational.Rational)):
             return self * (rational.Rational(other) ** -1)
         elif not isinstance(other, MatAlgNumber):
             return NotImplemented
         other_mat = other.matrix.copy()
         other_mat.toFieldMatrix()
         mat = other_mat.inverse(self.matrix)
         coeff = []
@@ -703,23 +706,23 @@
 
     def __pow__(self, other):
         mat = self.matrix ** other
         coeff = []
         for i in range(mat.row):
             coeff.append(mat[i+1][1])
         return MatAlgNumber(coeff, self.polynomial)
-        
+
     def inverse(self):
         (self.matrix).toFieldMatrix()
         inv = (self.matrix).inverse()
         coeff = []
         for i in range(inv.row):
             coeff.append(inv[i+1][1])
         return MatAlgNumber(coeff, self.polynomial)
-    
+
     def norm(self):
         return (self.matrix).determinant()
 
     def trace(self):
         return (self.matrix).trace()
 
     def getRing(self):
@@ -783,15 +786,15 @@
     # import nzmath.module as module
     raise NotImplementedError
 
 def changetype(a, polynomial=[0, 1]):
     """
     Change 'a' to be an element of field K defined polynomial
     """
-    if isinstance(a, (int, long)):
+    if isinstance(a, int):
         coeff = [a] + [0] * (len(polynomial) - 2)
         return BasicAlgNumber([coeff, 1], polynomial)
     elif isinstance(a, rational.Rational):
         coeff = [a.numerator] + [0] * (len(polynomial) - 2)
         return BasicAlgNumber([coeff, a.denominator], polynomial)
     else:
         deg = len(a) - 1
```

### Comparing `NZMATH-1.1.0/nzmath/ecpp.py` & `nzmath-3.0.0/src/ecpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 import os
 import csv
 import logging
 import nzmath.arith1 as arith1
 import nzmath.bigrandom as bigrandom
 import nzmath.bigrange as bigrange
 import nzmath.equation as equation
@@ -38,20 +38,20 @@
 
 
 _log = logging.getLogger('nzmath.ecpp')
 
 # mapping from disc to list of order functions.
 default_orders = [lambda n, u, v: n + 1 + u,
                   lambda n, u, v: n + 1 - u]
-orders = {-3: default_orders + [lambda n, u, v: n + 1 - (u + 3*v)//2,
-                                lambda n, u, v: n + 1 + (u + 3*v)//2,
-                                lambda n, u, v: n + 1 - (u - 3*v)//2,
-                                lambda n, u, v: n + 1 + (u - 3*v)//2],
-          -4: default_orders + [lambda n, u, v: n + 1 + 2*v,
-                                lambda n, u, v: n + 1 - 2*v]}
+orders = {-3: default_orders + [lambda n, u, v: n + 1 - ((u + 3*v) >> 1),
+                                lambda n, u, v: n + 1 + ((u + 3*v) >> 1),
+                                lambda n, u, v: n + 1 - ((u - 3*v) >> 1),
+                                lambda n, u, v: n + 1 + ((u - 3*v) >> 1)],
+          -4: default_orders + [lambda n, u, v: n + 1 + (v << 1),
+                                lambda n, u, v: n + 1 - (v << 1)]}
 # default absolute value bound of discriminant
 DEFAULT_ABS_BOUND = 200000
 
 def dedekind(tau, floatpre):
     """
     Algorithm 22 (Dedekind eta)
     Input : tau in the upper half-plane, k in N
@@ -131,22 +131,25 @@
     return h, T
 
 def hilbert(D):
     """
     wrapper to split mpmath part and others.
     """
     if HAVE_NET:
-        import urllib2
-        url = 'http://hilbert-class-polynomial.appspot.com/%d/' % D
-        result = urllib2.urlopen(url).read()
-        if result == 'null':
+        try:
+            import urllib.request, urllib.error, urllib.parse
+            url = 'http://hilbert-class-polynomial.appspot.com/%d/' % D
+            result = urllib.request.urlopen(url).read()
+            if result == 'null':
+                pass
+            else:
+                hcp = eval(result)
+                return len(hcp) - 1, hcp
+        except Exception:
             pass
-        else:
-            hcp = eval(result)
-            return len(hcp) - 1, hcp
 
     if HAVE_MPMATH:
         return hilbert_mpmath(D)
 
     raise prime.ImplementLimit("impliment limit")
 
 
@@ -297,15 +300,15 @@
         if b:
             return (b, 1)
         else:
             raise ValueError("no solution")
     if arith1.legendre(d, p) == -1:
         raise ValueError("no solution")
     x0 = arith1.modsqrt(d, p)
-    if (x0 - d) % 2 != 0:
+    if (x0 - d) & 1:
         x0 = p - x0
     a = 2 * p
     b = x0
     l = arith1.floorsqrt(q)
     while b > l:
         a, b = b, a % b
     c, r = divmod(q - b * b, -d)
@@ -499,17 +502,17 @@
     """
     Return fundamental discriminant D, such that D < d.
     If there is no D with |d| < |D| < absbound, return False
     """
     # -disc % 16
     negdisc_mod16 = (3, 4, 7, 8, 11, 15)
     for negdisc in bigrange.range(-d + 1, absbound):
-        if negdisc % 16 not in negdisc_mod16:
+        if negdisc & 15 not in negdisc_mod16:
             continue
-        if negdisc % 2 == 1 and not squarefree.trial_division(negdisc):
+        if negdisc & 1 and not squarefree.trial_division(negdisc):
             continue
         if arith1.issquare(negdisc):
             continue
         return -negdisc
     return False
 
 def disc_gen(absbound=DEFAULT_ABS_BOUND):
```

### Comparing `NZMATH-1.1.0/nzmath/group.py` & `nzmath-3.0.0/src/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
                 baby_e = GroupElement(g_gen[j - 1])
                 giant_e = GroupElement(g_gen[j - 1])
                 flag = False
                 while not flag:
                     for (g_g, v) in giant_s:
                         for (g_b, w) in baby_s:
                             if g_g.ope(giant_e) == g_b:
-                                b[j] = v + w + (e * (e + 1) // 2) * e_vec[j - 1]
+                                b[j] = v + w + (e * (e + 1) >> 1) * e_vec[j - 1]
                                 flag = True
                                 break
                         if flag:
                             break
                     if flag:
                         break
                     for (g_a, v_a) in a_baby_s:
```

### Comparing `NZMATH-1.1.0/nzmath/factor/methods.py` & `nzmath-3.0.0/src/factor/methods.py`

 * *Files identical despite different names*

### Comparing `NZMATH-1.1.0/nzmath/factor/find.py` & `nzmath-3.0.0/src/factor/find.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         _silence()
 
     if n <= 3:
         return 1
 
     g = n
     while g == n:
+        # x^2 + a is iterated. Starting value x = u.
         a = bigrandom.randrange(1, n-2)
         u = v = bigrandom.randrange(0, n-1)
         _log.info("%d %d" % (a, u))
         g = gcd.gcd((v**2 + v + a) % n - u, n)
         while g == 1:
             u = (u**2 + a) % n
             v = ((pow(v, 2, n) + a)**2 + a) % n
@@ -51,29 +52,32 @@
     """
     # verbosity
     verbose = options.get('verbose', False)
     if not verbose:
         _silence()
 
     # initialize
-    x , B = 2 , 10000001
-    y = x
+    x = y = 2
     primes = []
+    if 'B' in options:
+        B = options['B']
+    else:
+        B = 10000
 
     for q in prime.generator():
         primes.append(q)
         if q > B:
             if gcd.gcd(x-1, n) == 1:
                 if not verbose:
                     _verbose()
                 return 1
             x = y
             break
         q1 = q
-        l = B//q
+        l = B // q
         while q1 <= l:
             q1 *= q
         x = pow(x, q1, n)
         if len(primes) >= 20:
             if gcd.gcd(x-1, n) == 1:
                 primes, y = [], x
             else:
@@ -106,31 +110,32 @@
     # verbosity
     verbose = options.get('verbose', False)
     if not verbose:
         _silence()
 
     if 'start' in options and 'stop' in options:
         if 'step' in options:
-            trials = range(options['start'], options['stop'], options['step'])
+            trials = list(range(options['start'], options['stop'], options['step']))
         else:
-            trials = range(options['start'], options['stop'])
+            trials = list(range(options['start'], options['stop']))
     elif 'iterator' in options:
         trials = options['iterator']
     elif n < 1000000:
         trials = prime.generator_eratosthenes(arith1.floorsqrt(n))
     else:
         trials = prime.generator()
 
+    limit = arith1.floorsqrt(n)
     for p in trials:
-        if not (n % p):
+        if limit < p:
+            break
+        if 0 == n % p:
             if not verbose:
                 _verbose()
             return p
-        if p ** 2 > n:
-            break
     if not verbose:
         _verbose()
     return 1
 
 def _silence():
     """
     Stop verbose outputs.
```

### Comparing `NZMATH-1.1.0/nzmath/factor/mpqs.py` & `nzmath-3.0.0/src/factor/mpqs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,37 @@
 import math
 import time
 import logging
 import nzmath.arith1 as arith1
 import nzmath.gcd as gcd
 import nzmath.prime as prime
-import nzmath.factor.find as find
 
-# TODO: add psyco to config entry
-##         try:
-##             import psyco
-##             psyco.full()
-##         except ImportError:
-##             pass
+
+SCALE = 30
 
 _log = logging.getLogger('nzmath.factor.mpqs')
 
+
 class QS(object):
     def __init__(self, n, sieverange, factorbase):
         self.number = n
         self.sqrt_n = int(math.sqrt(n))
-        for i in [2,3,5,7,11,17,19]:
-            if n % i == 0:
-                raise ValueError("This number is divided by %d" % i)
+        for p in (2, 3, 5, 7, 11, 13, 17, 19):
+            if n % p == 0:
+                raise ValueError("This number is divided by %d" % p)
 
         self.digit = arith1.log(self.number, 10) + 1
         self.Srange = sieverange
         self.FBN = factorbase
 
-        self.move_range = range(self.sqrt_n-self.Srange, self.sqrt_n+self.Srange+1)
-
-        i = 0
-        k = 0
-        factor_base = [-1]
-        FB_log = [0]
-        while True:
-            ii = primes_table[i]
-            if arith1.legendre(self.number, ii) == 1:
-                factor_base.append(ii)
-                FB_log.append(primes_log_table[i])
-                k += 1
-                i += 1
-                if k == self.FBN:
-                    break
-            else:
-                i += 1
-
-        self.FB = factor_base
-        self.FB_log = FB_log
-        self.maxFB = factor_base[-1]
+        self.move_range = list(range(self.sqrt_n-self.Srange, self.sqrt_n+self.Srange+1))
+        self.FB = [-1]
+        self.FB_log = [0]
+        self.set_factor_base(factorbase)
+        self.maxFB = self.FB[-1]
         N_sqrt_list = []
         for i in self.FB:
             if i != 2 and i != -1:
                 e = int(math.log(2*self.Srange, i))
                 N_sqrt_modp = sqroot_power(self.number, i, e)
                 N_sqrt_list.append(N_sqrt_modp)
         self.solution = N_sqrt_list  #This is square roots of N on Z/pZ, p in factor base.
@@ -69,53 +49,62 @@
             lj = int((math.log(jj)*30)*0.97)  # 0.97 is an erroe
             poly_table.append(jj)
             log_poly.append(lj)
         self.poly_table = poly_table  # This is Q(x) value , x in [-M+sqrt_n,M+sqrt_n].
         self.log_poly = log_poly      # This is log(Q(x)) value.
         self.minus_check = minus_val # This is "x" that Q(x) is minus value.
 
+    def set_factor_base(self, factorbase_size):
+        for p, log_p in zip(PRIMES_TABLE, PRIMES_LOG_TABLE):
+            if arith1.legendre(self.number, p) == 1:
+                self.FB.append(p)
+                self.FB_log.append(log_p)
+                if len(self.FB) == factorbase_size:
+                    return
+
     def run_sieve(self):
         T = time.time()
         M = self.Srange
         start_location = []
         logp = [0]*(2*M+1)
         j = 2
         for i in self.solution:
             k = 0
             start_p = []
             while k < len(i):
-                q = int((self.sqrt_n)/(self.FB[j]**(k+1)))
-                s_1 = q*(self.FB[j]**(k+1))+i[k][0]
-                s_2 = q*(self.FB[j]**(k+1))+i[k][1]
+                ppow = self.FB[j]**(k+1)
+                q = self.sqrt_n // ppow
+                s_1 = q*ppow + i[k]
+                s_2 = q*ppow + (ppow - i[k])
                 while True:
                     if s_1 < self.sqrt_n-M:
-                        s_1 = s_1+(self.FB[j]**(k+1))
+                        s_1 = s_1 + ppow
                         break
                     else:
-                        s_1 = s_1-(self.FB[j]**(k+1))
+                        s_1 = s_1 - ppow
                 while True:
                     if s_2 < self.sqrt_n-M:
-                        s_2 = s_2+(self.FB[j]**(k+1))
+                        s_2 = s_2 + ppow
                         break
                     else:
-                        s_2 = s_2-(self.FB[j]**(k+1))
+                        s_2 = s_2 - ppow
                 start_p.append([s_1-self.sqrt_n+M,s_2-self.sqrt_n+M])
 
                 k += 1
             start_location.append(start_p)
             j += 1
         self.start_location = start_location
 
-        if self.poly_table[0] % 2 == 0:
+        if self.poly_table[0] & 1 == 0:
             i = 0
             while i <= 2*M:
                 j = 1
                 while True:
                     if self.poly_table[i] % (2**(j+1)) == 0:
-                        j+=1
+                        j += 1
                     else:
                         break
                 logp[i] += self.FB_log[1]*j
                 i += 2
         else:
             i = 1
             while i <= 2*M:
@@ -145,444 +134,493 @@
             L += 1
 
         self.logp = logp
         smooth = []
         for t in range(2*M+1):
             if logp[t] >= self.log_poly[t]:
                 poly_val = self.poly_table[t]
-                index_vector = []
-                for p in self.FB:
+                index_set = set()
+                for i, p in enumerate(self.FB):
                     if p == -1:
                         if t in self.minus_check:
-                            index_vector.append(1)
-                        else:
-                            index_vector.append(0)
+                            index_set.add(0)
                     else:
                         r = 0
-                        while poly_val % (p**(r+1)) == 0:
-                            r += 1
-                        v = r % 2
-                        index_vector.append(v)
-                smooth.append([index_vector, (poly_val, t+self.sqrt_n-M)])
+                        if arith1.vp(poly_val, p)[0] & 1:
+                            index_set.add(i)
+                smooth.append([index_set, (poly_val, t+self.sqrt_n-M)])
         _log.info(" Sieve time is %f sec" % (time.time()-T))
         _log.info(" Found smooth numbers are %d / %d" % (len(smooth), len(self.FB)))
         self.smooth = smooth
         return smooth
 
 
 class MPQS(object):
     def __init__(self, n, sieverange=0, factorbase=0, multiplier=0):
-        self.number = n
-        _log.info("The number is %d MPQS starting" % n)
+        _log.info("%d; MPQS starting", n)
 
-        if prime.primeq(self.number):
+        if prime.primeq(n):
             raise ValueError("This number is Prime Number")
-        for i in [2,3,5,7,11,13]:
-            if n % i == 0:
-                raise ValueError("This number is divided by %d" % i)
+        for p in (2, 3, 5, 7, 11, 13):
+            if n % p == 0:
+                raise ValueError("This number is divided by %d" % p)
 
+        self.number = n
+        self.multiplier = 1
+        self.last_poly = None
+        self.sieve_range = 0
+        self.FBN = 0
+        self.FB = [-1]
+        self.FB_log = [0]
+        self.n_sqrt_p = []
+        self.smooth = []
         self.sievingtime = 0
         self.coefficienttime = 0
-        self.d_list = []
-        self.a_list = []
-        self.b_list = []
 
         #Decide prameters for each digits
-        self.digit = arith1.log(self.number, 10) + 1
+        digit = arith1.log(self.number, 10) + 1
+
+        self._init_srange(sieverange, digit)
+        self._init_fbn(factorbase, digit)
+
+        self._init_multiplier(multiplier)
+        self.number = self.multiplier * self.number
+
+        _log.info("%d - digits Number", digit)
+        _log.info("Multiplier is %d", self.multiplier)
+
+        # Table of (log p) , p in FB
+        self._init_fb()
+
+        # Solve x^2 = n (mod p^e)
+        self._init_nsqrt()
 
+    def _init_srange(self, sieverange, digit):
         if sieverange != 0:
-            self.Srange = sieverange
-            if factorbase != 0:
-                self.FBN = factorbase
-            elif self.digit < 9:
-                self.FBN = parameters_for_mpqs[0][1]
-            else:
-                self.FBN = parameters_for_mpqs[self.digit-9][1]
-        elif factorbase != 0:
-            self.FBN = factorbase
-            if self.digit < 9:
-                self.Srange = parameters_for_mpqs[0][0]
-            else:
-                self.Srange = parameters_for_mpqs[self.digit-9][0]
-        elif self.digit < 9:
-            self.Srange = parameters_for_mpqs[0][0]
-            self.FBN = parameters_for_mpqs[0][1]
-        elif self.digit > 53:
-            self.Srange = parameters_for_mpqs[44][0]
-            self.FBN = parameters_for_mpqs[44][1]
+            self.sieve_range = sieverange
+        elif digit < min(PARAMETERS_FOR_MPQS):
+            self.sieve_range = PARAMETERS_FOR_MPQS[min(PARAMETERS_FOR_MPQS)][0]
+        elif digit > max(PARAMETERS_FOR_MPQS):
+            self.sieve_range = PARAMETERS_FOR_MPQS[max(PARAMETERS_FOR_MPQS)][0]
         else:
-            self.Srange = parameters_for_mpqs[self.digit-9][0]
-            self.FBN = parameters_for_mpqs[self.digit-9][1]
+            self.sieve_range = PARAMETERS_FOR_MPQS[digit][0]
 
-        self.move_range = range(-self.Srange, self.Srange+1)
+    def _init_fbn(self, factorbase, digit):
+        if factorbase != 0:
+            self.FBN = factorbase
+        elif digit < min(PARAMETERS_FOR_MPQS):
+            self.FBN = PARAMETERS_FOR_MPQS[min(PARAMETERS_FOR_MPQS)][1]
+        elif digit > max(PARAMETERS_FOR_MPQS):
+            self.FBN = PARAMETERS_FOR_MPQS[max(PARAMETERS_FOR_MPQS)][1]
+        else:
+            self.FBN = PARAMETERS_FOR_MPQS[digit][1]
 
-        # Decide k such that k*n = 1 (mod4) and k*n has many factor base
+    def _init_multiplier(self, multiplier):
+        """
+        Decide k such that k*n = 1 (mod4) and k*n has many factor base
+        """
         if multiplier == 0:
-            self.sqrt_state = []
-            for i in [3,5,7,11,13]:
-                s = arith1.legendre(self.number, i)
-                self.sqrt_state.append(s)
-            index8 = (self.number % 8) // 2
-            j = 0
-            while self.sqrt_state != prime_8[index8][j][1]:
-                j += 1
-            k = prime_8[index8][j][0]
+            sqrt_state = []
+            for p in (3, 5, 7, 11, 13):
+                sqrt_state.append(arith1.legendre(self.number, p))
+
+            if self.number % 8 == 1 and sqrt_state == [1, 1, 1, 1, 1]:
+                self.multiplier = 1
+            else:
+                index8 = (self.number & 7) >> 1
+                j = 0
+                while sqrt_state != PRIME_8[index8][j][1]:
+                    j += 1
+                self.multiplier = PRIME_8[index8][j][0]
         else:
-            if n % 4 == 1:
-                k = 1
+            if self.number & 3 == 1:
+                self.multiplier = 1
             else:
                 if multiplier == 1:
                     raise ValueError("This number is 3 mod 4 ")
                 else:
-                    k = multiplier
-        self.number = k*self.number
-        self.multiplier = k
-
-        _log.info("%d - digits Number" % self.digit)
-        _log.info("Multiplier is %d" % self.multiplier)
+                    self.multiplier = multiplier
 
-        # Table of (log p) , p in FB
+    def _init_fb(self):
+        """
+        Table of (log p) , p in FB
+        """
         i = 0
-        k = 0
-        factor_base = [-1]
-        FB_log = [0]
-        while k < self.FBN:
-            ii = primes_table[i]
-            if arith1.legendre(self.number,ii) == 1:
-                factor_base.append(ii)
-                FB_log.append(primes_log_table[i])
-                k += 1
+        while len(self.FB) < self.FBN:
+            p = PRIMES_TABLE[i]
+            if arith1.legendre(self.number, p) == 1:
+                self.FB.append(p)
+                self.FB_log.append(PRIMES_LOG_TABLE[i])
             i += 1
 
-        self.FB = factor_base
-        self.FB_log = FB_log
-        self.maxFB = factor_base[-1]
-
-        # Solve x^2 = n (mod p^e)
-        N_sqrt_list = []
-        for i in self.FB:
-            if i != 2 and i != -1:
-                e = int(math.log(2*self.Srange, i))
-                N_sqrt_modp = sqroot_power(self.number, i, e)
-                N_sqrt_list.append(N_sqrt_modp)
-        self.Nsqrt = N_sqrt_list
+    def _init_nsqrt(self):
+        """
+        Solve x^2 = n (mod p^e)
+        """
+        assert self.FB[1] == 2
+        for p in self.FB[2:]:
+            e = int(math.log(2*self.sieve_range, p))
+            self.n_sqrt_p.append(sqroot_power(self.number, p, e))
 
     def make_poly(self):
         """
         Make coefficients of f(x)= ax^2+b*x+c
         """
         T = time.time()
-        if self.d_list == []:
-            d = int(math.sqrt((math.sqrt(self.number)/(math.sqrt(2)*self.Srange))))
-            if d%2 == 0:
-                if (d+1)%4 == 1: #case d=0 mod4
-                    d += 3
-                else:
-                    d += 1       #case d=2 mod4
-            elif d%4 == 1:       #case d=1 mod4
-                d += 2
-                                 #case d=3 mod4
+        self._make_next_coefficients()
+
+        # Get solution of  F(x) = 0 (mod p^i)
+        solutions = self._get_solutions(self.last_poly.f_2, self.last_poly.f_1)
+        self.coefficienttime += time.time() - T
+        return solutions
+
+    def _make_next_coefficients(self):
+        """
+        Make new quadratic polynomial ax^2 + b*x + c with next bigger a.
+        """
+        if self.last_poly is None:
+            self.last_poly = QuadraticPolynomial.next_polynomial(self.number, sieve_range=self.sieve_range)
         else:
-            d = self.d_list[-1]
+            self.last_poly = QuadraticPolynomial.next_polynomial(self.number, init_param=self.last_poly.param)
 
-        while d in self.d_list or not prime.primeq(d) or \
-              arith1.legendre(self.number,d) != 1 or d in self.FB:
-            d += 4
-        a = d**2
-        h_0 = pow(self.number, (d-3)//4, d)
-        h_1 = (h_0*self.number) % d
-        h_2 = ((arith1.inverse(2,d)*h_0*(self.number - h_1**2))/d) % d
-        b = (h_1 + h_2*d) % a
-        if b%2 == 0:
-            b = b - a
-
-        self.d_list.append(d)
-        self.a_list.append(a)
-        self.b_list.append(b)
+        while self.last_poly.param in self.FB:
+            self.last_poly = QuadraticPolynomial.next_polynomial(self.number, init_param=self.last_poly.param)
 
-        # Get solution of  F(x) = 0 (mod p^i)
+    def _get_solutions(self, a, b):
+        """
+        Get solution of  F(x) = 0 (mod p^i)
+        """
         solution = []
-        i = 0
-        for s in self.Nsqrt:
+        for p, s in zip(self.FB[2:], self.n_sqrt_p):
             k = 0
             p_solution = []
             ppow = 1
             while k < len(s):
-                ppow *= self.FB[i+2]
-                a_inverse = arith1.inverse(2*self.a_list[-1], ppow)
-                x_1 = ((-b + s[k][0])*a_inverse) % ppow
-                x_2 = ((-b + s[k][1])*a_inverse) % ppow
-                p_solution.append([x_1, x_2])
+                ppow *= p
+                a_inverse = arith1.inverse(2*a, ppow)
+                x_1 = ((-b + s[k])*a_inverse) % ppow
+                x_2 = ((-b + (ppow - s[k]))*a_inverse) % ppow
+                p_solution.append((x_1, x_2))
                 k += 1
-            i += 1
             solution.append(p_solution)
-        self.solution = solution
-        self.coefficienttime += time.time() - T
+        return solution
 
     def run_sieve(self):
-        self.make_poly()
+        solutions = self.make_poly()
         T = time.time()
-        M = self.Srange
-        a = self.a_list[-1]            #
-        b = self.b_list[-1]            # These are coefficients of F(x)
-        c = (b**2-self.number)/(4*a)   #
-        d = self.d_list[-1]            #
-
-        self.poly_table = []  # This is F(x) value , x in [-M,M].
-        self.log_poly = []    # This is log(F(x)) value.
-        self.minus_check = [] # This is "x" that F(x) is minus value.
-        for j in self.move_range:
-            jj = (a * j + b) * j + c
-            if jj < 0:
-                jj = -jj
-                self.minus_check.append(j + M)
-            elif jj == 0:
-                jj = 1
-            lj = int((math.log(jj)*30)*0.95)  # 0.95 is an erroe
-            self.poly_table.append(jj)
-            self.log_poly.append(lj)
 
-        y = arith1.inverse(2*d, self.number)
+        poly_table = []  # This is F(x) value , x in [-M,M].
+        log_poly = []    # This is log(F(x)) value.
+        minus_check = self._make_value_tables(poly_table, log_poly)
+
+        start_location = self._prepare_start_location(solutions)
+
+        logp = [0] * (2 * self.sieve_range + 1)
+
+        # sieve by 2 & its powers
+        self._sieve_2(logp, poly_table)
+
+        for p, log_p, start_p in zip(self.FB[2:], self.FB_log[2:], start_location):
+            # sieve by p
+            self._sieve_p(logp, p, log_p, start_p)
+
+        smooth = self._collect_smooth_vectors(logp, log_poly, poly_table, minus_check)
+        self.sievingtime += time.time() - T
+        _log.debug("Sieving Time = %f sec", self.sievingtime)
+        return smooth
+
+    def _make_value_tables(self, poly_table, log_poly):
+        """
+        Make tables poly_table and log_poly, which will be sieved.
+        """
+        diminished_scale = SCALE * 0.95  # 0.95 is an error
+        rho = math.exp(1 / diminished_scale)
+        rough_lower = 0
+        rough_upper = 0
+        minus_check = set()  # set of x where F(x) is negative.
+        q_j = self.last_poly(-self.sieve_range - 1)
+        for j in range(-self.sieve_range, self.sieve_range + 1):
+            q_j += self.last_poly.delta(j)
+            f_j = q_j
+            if f_j < 0:
+                f_j = -f_j
+                minus_check.add(j + self.sieve_range)
+            elif f_j == 0:
+                f_j = 1
+            if not (rough_lower <= f_j <= rough_upper):
+                l_j = int(math.log(f_j) * diminished_scale)
+                rough_lower = int(f_j / rho) + 1
+                rough_upper = int(f_j * rho)
+            poly_table.append(f_j)
+            log_poly.append(l_j)
+        return minus_check
+
+    def _prepare_start_location(self, solutions):
+        """
+        For each odd prime in the factor base, find start location of
+        sieve process.
+        """
         start_location = []
-        logp = [0]*(2*M+1)
-        j = 2
-        for i in self.solution:
+        for p, solution in zip(self.FB[2:], solutions):
             start_p = []
             ppow = 1
-            for k in range(len(i)):
-                ppow *= self.FB[j]
-                q = -M // ppow
-                s_1 = (q + 1) * ppow + i[k][0]
-                s_2 = (q + 1) * ppow + i[k][1]
-                while s_1 + M >= ppow:
-                    s_1 = s_1 - ppow
-                while s_2 + M >= ppow:
-                    s_2 = s_2 - ppow
-                start_p.append([s_1+M, s_2+M])
+            for s_k in solution:
+                ppow *= p
+                q = -self.sieve_range // ppow
+                s_1 = (q + 1) * ppow + s_k[0] + self.sieve_range
+                s_2 = (q + 1) * ppow + s_k[1] + self.sieve_range
+                while s_1 >= ppow:
+                    s_1 -= ppow
+                while s_2 >= ppow:
+                    s_2 -= ppow
+                start_p.append((s_1, s_2))
             start_location.append(start_p)
-            j += 1
-        self.start_location = start_location
+        return start_location
 
-        i = self.poly_table[0] % 2
-        while i <= 2*M:
-            j = 1
-            while self.poly_table[i] % (2**(j+1)) == 0:
-                j += 1
-            logp[i] += self.FB_log[1]*j
-            i += 2
-        L = 2
-        for plocation in self.start_location:
-            for k in range(len(plocation)):
-                s_1 = plocation[k][0]
-                s_2 = plocation[k][1]
-                ppow = self.FB[L]**(k+1)
-                while s_1 <= 2*M:
-                    logp[s_1] += self.FB_log[L]
-                    s_1 += ppow
-                while s_2 <= 2*M:
-                    logp[s_2] += self.FB_log[L]
-                    s_2 += ppow
-            L += 1
+    def _sieve_2(self, logp, poly_table):
+        """
+        Sieve by 2; update logp.
+        """
+        log_2 = self.FB_log[1]
+        fullrange = 2 * self.sieve_range + 1
+        ppow = 1
+        solutions = []
+        for pos in (0, 1):
+            if poly_table[pos] & 1 == 0:
+                solutions.append(pos)
+        for i in range(12):
+            ppow *= 2
+            new_solutions = []
+            for pos in solutions:
+                for j in range(pos, fullrange, ppow):
+                    logp[j] += log_2
+                if poly_table[pos] % (ppow * 2) == 0:
+                    new_solutions.append(pos)
+                elif pos + ppow < fullrange and poly_table[pos + ppow] % (ppow * 2) == 0:
+                    new_solutions.append(pos + ppow)
+            if not new_solutions:
+                break
+            solutions = tuple(new_solutions)
 
-        self.logp = logp
+    def _sieve_p(self, logp, p, log_p, start_p):
+        """
+        Sieve by p; update logp.
+        """
+        fullrange = 2 * self.sieve_range + 1
+        ppow = 1
+        for starts in start_p:
+            ppow *= p
+            for divisible in starts:
+                for index in range(divisible, fullrange, ppow):
+                    logp[index] += log_p
+
+    def _collect_smooth_vectors(self, logp, log_poly, poly_table, minus_check):
+        """
+        Return smooth vectors collected from sieved tables.
+        """
+        a = self.last_poly.f_2
+        b = self.last_poly.f_1
+        d = self.last_poly.param
         smooth = []
-        for t in range(2*M+1):
-            if logp[t] >= self.log_poly[t]:
-                poly_val = self.poly_table[t]
-                index_vector = []
-                H = (y*(2*a*(t-self.Srange)+b))%self.number
-                for p in self.FB:
-                    if p == -1:
-                        if t in self.minus_check:
-                            index_vector.append(1)
-                        else:
-                            index_vector.append(0)
-                    else:
-                        r = 0
-                        while poly_val % (p**(r+1)) == 0:
-                            r += 1
-                        v = r % 2
-                        index_vector.append(v)
-                smooth.append([index_vector, (poly_val, H)])
-        self.sievingtime += time.time() - T
+        y = arith1.inverse(2 * d, self.number)
+        for t in range(2 * self.sieve_range + 1):
+            if logp[t] >= log_poly[t]:
+                poly_val = poly_table[t]
+                index_set = set()
+                # -1
+                if t in minus_check:
+                    index_set.add(0)
+                # p
+                for i, p in enumerate(self.FB[1:], 1):
+                    if arith1.vp(poly_val, p)[0] & 1:
+                        index_set.add(i)
+                H = y*(2*a*(t - self.sieve_range) + b) % self.number
+                smooth.append([index_set, (poly_val, H)])
         return smooth
 
     def get_vector(self):
-        T = time.time()
-        P = len(self.FB)
-        if P < 100:
-            V = -5
+        _start = time.time()
+        necessary = len(self.FB)
+        if necessary < 100:
+            necessary += 5
         else:
-            V = 0
-        smooth = []
-        i = 0
-        while P*1 > V:
-            n = self.run_sieve()
-            V += len(n)
-            smooth += n
-            i += 1
-            if i % 50 == 0:
-                if i == 50:
-                    _log.info("*/ Per 50 times changing poly report /* ")
-                _log.info("Time of deciding coefficient = %f sec" % self.coefficienttime)
-                _log.info("Sieving Time = %f sec" % self.sievingtime)
-                _log.info("Find smooth numbers are %d / %d" % (V, P))
-        if P < 100:
-            V += 5
-        self.smooth = smooth
-        _log.info("*/ Total %d times changing poly report /*" % i)
-        _log.info("Time of deciding coefficient = %f sec" % self.coefficienttime)
-        _log.info("Sieving Time = %f sec" % self.sievingtime)
-        _log.info("Found smooth numbers are %d / %d" % (V, P))
-        _log.info("Total time of getting enough smooth numbers = %f sec" % (time.time()-T))
-        return smooth
+            necessary += 1
+        self.smooth = []
+        while len(self.smooth) < necessary:
+            self.smooth.extend(self.run_sieve())
+        _log.info("Found smooth numbers are %d / %d", len(self.smooth), len(self.FB))
+        _log.info("Sieving Time = %f sec", self.sievingtime)
+        _log.info("Total time of getting enough smooth numbers = %f sec", time.time() - _start)
+        return self.smooth
+
+
+class QuadraticPolynomial(object):
+    """
+    A quadratic polynomial to use in MPQS.
+    """
+    def __init__(self, number, init_param):
+        self.number = number
+        self.param = init_param
+        # coefficents: f_0 + f_1 * x + f_2 * x^2, later initialized
+        self.f_0 = self.f_1 = self.f_2 = None
+        # coefficents: d_0 + d_1 * x = F(x) - F(x - 1)
+        self.d_0 = self.d_1 = None
+        self.init_coefficients()
+
+    @classmethod
+    def next_polynomial(cls, number, sieve_range=None, init_param=None):
+        """
+        Return the next polynomial.
+
+        If init_param optional argument is given, start searching the
+        parameter from init_param + 4.  The argument should be 3 mod 4,
+        otherwise factorization does not work.
+
+        If sieve_range optional argument is given and init_param is not
+        given, the parameter will be the smallest one.
+        """
+        if init_param is None:
+            param = int(math.sqrt((math.sqrt(number)/(math.sqrt(2)*sieve_range)))) | 3
+        else:
+            param = init_param + 4
+
+        while not prime.primeq(param) or arith1.legendre(number, param) != 1:
+            param += 4
+
+        return cls(number, param)
+
+    def init_coefficients(self):
+        """
+        Initialize the coefficients f_0, f_1 & f_2 of the quadratic
+        polynomial, determined from the parameter.
+        """
+        self.f_2 = self.param**2
+        h_0 = pow(self.number, (self.param - 3) >> 2, self.param)
+        h_1 = h_0 * self.number % self.param
+        h_2 = (arith1.inverse(2, self.param) * h_0 * (self.number - h_1 ** 2) // self.param) % self.param
+        self.f_1 = (h_1 + h_2 * self.param) % self.f_2
+        if self.f_1 & 1 == 0:
+            self.f_1 -= self.f_2
+        self.f_0 = (self.f_1 * self.f_1 - self.number) // (4 * self.f_2)
+
+        self.d_0 = self.f_1 - self.f_2
+        self.d_1 = 2 * self.f_2
+
+    def __call__(self, num):
+        """
+        Return the value as quadratic polynomial function.
+        """
+        return (self.f_2 * num + self.f_1) * num + self.f_0
+ 
+    def delta(self, num):
+        """
+        Return f(num) - f(num - 1)
+        """
+        return self.d_0 + self.d_1 * num
 
 
 class Elimination(object):
-    def __init__(self, smooth):
+    def __init__(self, smooth, fb_size):
         self.vector = []
         self.history = []
-        i = 0
-        for vec in smooth:
+        for i, vec in enumerate(smooth):
             self.vector.append(vec[0])
-            self.history.append({i:1})
-            i += 1
-        self.FB_number = len(self.vector[0])
+            self.history.append(set((i,)))
+        self.FB_number = fb_size
         self.row_size = len(self.vector)
-        self.historytime = 0
 
     def vector_add(self, i, j):
-        V_i = self.vector[i]
-        V_j = self.vector[j]
-        k = 0
-        while k < len(V_i):
-            if V_i[k] == 1:
-                if V_j[k] == 1:
-                    V_j[k] = 0
-                else:
-                    V_j[k] = 1
-            k += 1
-
-    def transpose(self):
-        Transe_vector = []
-        i = 0
-        while i < self.FB_number:
-            j = 0
-            vector = []
-            while j < self.row_size:
-                vector.append(self.vector[j][i])
-                j += 1
-            Transe_vector.append(vector)
-            i += 1
-        self.Transe = Transe_vector
+        self.vector[j] = self.vector[i] ^ self.vector[j]
 
     def history_add(self, i, j):
-        T = time.time()
-        H_i = self.history[i].keys()
-        H_j = self.history[j].keys()
-        for k in H_i:
-            if k in H_j:
-                del self.history[j][k]
-            else:
-                self.history[j][k] = 1
-        self.historytime += time.time() - T
+        self.history[j] = self.history[i] ^ self.history[j]
 
     def gaussian(self):
         T = time.time()
-        pivot = []
-        FBnum = self.FB_number
+        pivot = set()
         Smooth = len(self.vector)
         for j in range(self.FB_number):
-            for k in range(Smooth):
-                if k in pivot or not self.vector[k][j]:
+            for k, V_k in enumerate(self.vector):
+                if k in pivot or j not in V_k:
                     continue
-                pivot.append(k)
-                V_k = self.vector[k]
-                for h in range(Smooth):
-                    if h in pivot or not self.vector[h][j]:
+                pivot.add(k)
+                for h in range(k + 1, Smooth):
+                    if h in pivot or j not in self.vector[h]:
                         continue
                     self.history_add(k, h)
-                    V_h = self.vector[h]
-                    for q in range(j, FBnum):
-                        if V_k[q]:
-                            V_h[q] = not V_h[q]
+                    self.vector_add(k, h)
                 break
-        self.pivot = pivot
 
         zero_vector = []
         for check in range(Smooth):
-            if check not in pivot:
-                g = 0
-                while g < FBnum:
-                    if self.vector[check][g] == 1:
-                        break
-                    g += 1
-                if g == FBnum:
-                    zero_vector.append(check)
-        _log.info("Time of Gaussian Elimination = %f sec" % (time.time() - T))
+            if check not in pivot and not self.vector[check]:
+                zero_vector.append(check)
+        _log.info("Time of Gaussian Elimination = %f sec", time.time() - T)
         return zero_vector
 
+
+# qs, mpqs factors n completely
 def qs(n, s, f):
     """
     This is main function of QS
     Arguments are (composite_number, sieve_range, factorbase_size)
     You must input these 3 arguments.
     """
     a = time.time()
     Q = QS(n, s, f)
     _log.info("Sieve range is [ %d , %d ] , Factorbase size = %d , Max Factorbase %d" % (Q.move_range[0], Q.move_range[-1], len(Q.FB), Q.maxFB))
     Q.run_sieve()
-    V = Elimination(Q.smooth)
+    V = Elimination(Q.smooth, len(Q.FB))
     A = V.gaussian()
     _log.info("Found %d linearly dependent relations" % len(A))
     answerX_Y = []
     N_factors = []
     for i in A:
-        B = V.history[i].keys()
         X = 1
         Y = 1
-        for j in B:
+        for j in V.history[i]:
             X *= Q.smooth[j][1][0]
             Y *= Q.smooth[j][1][1]
             Y = Y % Q.number
         X = sqrt_modn(X, Q.number)
         answerX_Y.append(X-Y)
     for k in answerX_Y:
         if k != 0:
             factor = gcd.gcd(k, Q.number)
             if factor not in N_factors and factor != 1 and \
                factor != Q.number and prime.primeq(factor) == 1:
                 N_factors.append(factor)
     N_factors.sort()
     _log.info("Total time = %f sec" % (time.time()-a))
     _log.info(str(N_factors))
+    return N_factors
+
 
 def mpqs(n, s=0, f=0, m=0):
     """
     This is main function of MPQS.
     Arguments are (composite_number, sieve_range, factorbase_size, multiplier)
     You must input composite_number at least.
     """
     T = time.time()
     M = MPQS(n, s, f, m)
-    _log.info("Sieve range is [ %d , %d ] , Factorbase size = %d , Max Factorbase %d" % (M.move_range[0], M.move_range[-1], len(M.FB), M.maxFB))
+    _log.info("Sieve range is [ %d , %d ] , Factorbase size = %d , Max Factorbase %d" % (-M.sieve_range, M.sieve_range, len(M.FB), max(M.FB)))
     M.get_vector()
     N = M.number // M.multiplier
-    V = Elimination(M.smooth)
+    V = Elimination(M.smooth, len(M.FB))
     A = V.gaussian()
     _log.info("Found %d linerly dependent relations" % len(A))
     answerX_Y = []
     N_prime_factors = []
     N_factors = []
     output = []
     for i in A:
-        B = V.history[i].keys()
         X = 1
         Y = 1
-        for j in B:
+        for j in V.history[i]:
             X *= M.smooth[j][1][0]
             Y *= M.smooth[j][1][1]
             Y = Y % M.number
         X = sqrt_modn(X, M.number)
         if X != Y:
             answerX_Y.append(X-Y)
     NN = 1
@@ -651,191 +689,154 @@
         return output
     else:
         N_factors.sort()
         _log.error("Sorry, not factored completely")
         return output, N_factors
 
 
-
 ########################################################
 #                                                      #
 # Following functions are subfunction for main program #
 #                                                      #
 ########################################################
 
 def eratosthenes(n):
-    if n < 2:
-        raise ValueError("Input value must be bigger than 1")
-    else:
-        primes = [2]
-        sieves = [1]*(((n+1)//2)-1)
-        k = 3
-        i = 0
-        sieves_len = len(sieves)
-        while k <= math.sqrt(n):
-            if sieves[i] == 1:
-                j = 1
-                while i+j*k <= sieves_len-1:
-                    sieves[i+j*k] = 0
-                    j = j+1
-                k, i = k+2, i+1
-            else:
-                k, i = k+2, i+1
-        y = 3
-        for x in sieves:
-            if x == 1:
-                primes.append(y)
-            y = y+2
-        return primes
+    return list(prime.generator_eratosthenes(n))
 
-def prime_mod8(n):
+def prime_mod8():
     """
-    This is table for choosing multiplier which makes N to have
+    Make a table for choosing multiplier which makes N to have
     factorbase(2,3,5,7,11,13)
     """
-    primes = eratosthenes(n)
+    primes = eratosthenes(8090)
     PrimeList = {1:[], 3:[], 5:[], 7:[]}
-    LegendreList = {1:[], 3:[], 5:[], 7:[]}
-    sp = [2, 3, 5, 7, 11, 13]
-    for p in primes:
-        if p not in sp:
-            leg = [arith1.legendre(p, q) for q in sp[1:]]
-            if leg not in PrimeList[p % 8]:
-                LegendreList[p % 8].append(leg)
-                PrimeList[p % 8].append([p, leg])
+    sp = (3, 5, 7, 11, 13)
+    for p in primes[6:]:
+        leg = [arith1.legendre(p, q) for q in sp]
+        if leg not in PrimeList[p & 7]:
+            PrimeList[p & 7].append([p, leg])
     return [PrimeList[1], PrimeList[3], PrimeList[5], PrimeList[7]]
 
-def eratosthenes_log(n):
-    primes = eratosthenes(n)
-    primes_log = []
-    for i in primes:
-        l = int(math.log(i)*30) #30 is scale
-        primes_log.append(l)
+def eratosthenes_log():
+    primes = PRIMES_TABLE
+    primes_log = [int(math.log(p) * SCALE) for p in primes]
     return primes_log
 
 def sqrt_modn(n, modulo):
     import nzmath.factor.methods as methods
     factorOfN = methods.trialDivision(n)
     prod = 1
     for p, e in factorOfN:
-        prod = (prod * pow(p, e//2, modulo)) % modulo
+        prod = (prod * pow(p, e >> 1, modulo)) % modulo
     return prod
 
 def sqroot_power(a, p, n):
     """
-    return squareroot of a mod p^k for k = 2,3,...,n
+    return a square root of a mod p^k for k = 2,3,...,n for each k
     """
-    r = arith1.modsqrt(a, p)
-    x = (r, p-r)
-    i = 2
+    x = arith1.modsqrt(a, p)
     answer = [x]
     ppower = p
-    while i <= n:
-        b_1 = (x[0]**2-a) // ppower
-        b_2 = (x[1]**2-a) // ppower
-        x_1 = -b_1 * arith1.inverse(2*x[0], p)
-        x_2 = -b_2 * arith1.inverse(2*x[1], p)
-        X_1 = x[0] + x_1*ppower % (p*ppower)
-        X_2 = x[1] + x_2*ppower % (p*ppower)
-        x = [X_1, X_2]
-        answer.append(x)
-        i += 1
+    inverse = arith1.inverse(x << 1, p)
+    for i in range(n - 1):
+        x += (a - x ** 2) // ppower * inverse % p * ppower
         ppower *= p
+        answer.append(x)
     return answer
 
 #################
 # Initial items #
 #################
-primes_table = eratosthenes(10**5)
-primes_log_table = eratosthenes_log(10**5)
-prime_8 = prime_mod8(8090)
-parameters_for_mpqs = [[100,20], #9 -digits
-                      [100,21], #10
-                      [100,22], #11
-                      [100,24], #12
-                      [100,26], #13
-                      [100,29], #14
-                      [100,32], #15
-                      [200,35], #16
-                      [300,40], #17
-                      [300,60], #18
-                      [300,80], #19
-                      [300,100], #20
-                      [300,100], #21
-                      [300,120], #22
-                      [300,140], #23
-                      [600,160], #24
-                      [900,180], #25
-                      [1200,200], #26
-                      [1000,220], #27
-                      [2000,240], #28
-                      [2000,260], #29
-                      [2000,325], #30
-                      [2000,355], #31
-                      [2000,375], #32
-                      [3000,400], #33
-                      [2000,425], #34
-                      [2000,550], #35
-                      [3000,650], #36
-                      [5000,750], #37
-                      [4000,850], #38
-                      [4000,950], #39
-                      [5000,1000], #40
-                      [14000,1150], #41
-                      [15000,1300], #42
-                      [15000,1600], #43
-                      [15000,1900], #44
-                      [15000,2200], #45
-                      [20000,2500], #46
-                      [25000,2500], #47
-                      [27500,2700], #48
-                      [30000,2800], #49
-                      [35000,2900], #50
-                      [40000,3000], #51
-                      [50000,3200], #52
-                      [50000,3500]] #53
-
+PRIMES_TABLE = eratosthenes(10**5)
+PRIMES_LOG_TABLE = eratosthenes_log()
+PRIME_8 = prime_mod8()
+# {#digits: (sieve_range, factorbase_size)}
+PARAMETERS_FOR_MPQS = {
+    9: (100, 20),
+    10: (100, 21),
+    11: (100, 22),
+    12: (100, 24),
+    13: (100, 26),
+    14: (100, 29),
+    15: (100, 32),
+    16: (200, 35),
+    17: (300, 40),
+    18: (300, 60),
+    19: (300, 80),
+    20: (300, 90),
+    21: (300, 100),
+    22: (300, 120),
+    23: (300, 140),
+    24: (600, 160),
+    25: (900, 180),
+    26: (1000, 200),
+    27: (1200, 220),
+    28: (1600, 240),
+    29: (2000, 260),
+    30: (2400, 350),
+    31: (2700, 370),
+    32: (3000, 390),
+    33: (4000, 410),
+    34: (5000, 500),
+    35: (6000, 600),
+    36: (6500, 700),
+    37: (7000, 8500),
+    38: (8000, 1000),
+    39: (9000, 1200),
+    40: (10000, 1500),
+    41: (12000, 1600),
+    42: (14000, 1700),
+    43: (15000, 1800),
+    44: (15000, 1900),
+    45: (15000, 2200),
+    46: (20000, 2400),
+    47: (25000, 2500),
+    48: (27500, 2700),
+    49: (30000, 2800),
+    50: (35000, 2900),
+    51: (40000, 3000),
+    52: (50000, 3200),
+    53: (50000, 3500),
+    54: (55000, 3800),
+    55: (60000, 4000),
+}
 
 ###
 ### only find a factor
 ###
 
 def mpqsfind(n, s=0, f=0, m=0, verbose=False):
     """
-    This is main function of MPQS.
-    Arguments are (composite_number, sieve_range, factorbase_size, multiplier)
-    You must input composite_number at least.
+    This is the main function of MPQS.
+    The main argument is the composite_number to be factored.
+    Parameters are s=sieve_range, f=factorbase_size, m=multiplier
+    and verbose.
     """
     # verbosity
     if verbose:
         _log.setLevel(logging.DEBUG)
         _log.debug("verbose")
     else:
         _log.setLevel(logging.NOTSET)
 
     starttime = time.time()
     M = MPQS(n, s, f, m)
-    _log.info("Sieve range is [%d, %d]" % (M.move_range[0], M.move_range[-1]))
-    _log.info("Factorbase size = %d, Max Factorbase %d" % (len(M.FB), M.maxFB))
+    _log.info("Sieve range is [%d, %d]", -M.sieve_range, M.sieve_range)
+    _log.info("Factorbase size = %d, Max Factorbase %d", len(M.FB), M.FB[-1])
     M.get_vector()
     N = M.number // M.multiplier
-    V = Elimination(M.smooth)
+    V = Elimination(M.smooth, len(M.FB))
     A = V.gaussian()
-    _log.info("Found %d linearly dependent relations" % len(A))
-    differences = []
+    _log.info("Found %d linearly dependent relations", len(A))
     for i in A:
-        B = V.history[i].keys()
         X = 1
         Y = 1
-        for j in B:
+        for j in V.history[i]:
             X *= M.smooth[j][1][0]
             Y *= M.smooth[j][1][1]
             Y = Y % M.number
         X = arith1.floorsqrt(X) % M.number
         if X != Y:
-            differences.append(X-Y)
-
-    for diff in differences:
-        divisor = gcd.gcd(diff, N)
-        if 1 < divisor < N:
-            _log.info("Total time = %f sec" % (time.time() - starttime))
-            return divisor
+            divisor = gcd.gcd(X - Y, N)
+            if 1 < divisor < N:
+                _log.info("Total time = %f sec", time.time() - starttime)
+                return divisor
```

### Comparing `NZMATH-1.1.0/nzmath/factor/ecm.py` & `nzmath-3.0.0/src/factor/ecm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Elliptic Curve Method Factorization
 
 It's using Montgomery's parametrization.
 """
 
-from __future__ import division
+
 import logging
 import random
 import nzmath.arith1 as _arith1
 import nzmath.gcd as _gcd
 import nzmath.prime as _prime
 
 _log = logging.getLogger('nzmath.factor.ecm')
@@ -18,22 +18,22 @@
 S = SUYAMA = 1
 B = BERNSTEIN = 2
 A1 = ASUNCION1 = 5
 A2 = ASUNCION2 = 6
 A3 = ASUNCION3 = 8
 A4 = ASUNCION4 = 9
 A5 = ASUNCION5 = 10
-
+N3 = NAKAMURA3 = 13
 
 class Curve (object):
     """
     Elliptic curves for factorization.
     """
 
-    _CURVE_TYPES = (S, B, A1, A2, A3, A4, A5)
+    _CURVE_TYPES = (S, B, A1, A2, A3, A4, A5, N3)
     
     def __init__(self, c):
         """
         Initialize a Curve object with Montgomery's parameter c.
         """
         self.c = c
         self.c2 = (c + 2)//4
@@ -50,16 +50,16 @@
           S: Suyama's parameter selection strategy
           B: Bernstein's [2:1], [16,18,4,2]
           A1: Asuncion's [2:1], [4,14,1,1]
           A2: Asuncion's [2:1], [16,174,4,41]
           A3: Asuncion's [3:1], [9,48,1,2]
           A4: Asuncion's [3:1], [9,39,1,1]
           A5: Asuncion's [4:1], [16,84,1,1]
-
-        This is a class method.
+          N3: Nakamura's [2:1], [28,22,7,3]
+          This is a class method.
         """
         bound = bounds.first
         if curve_type not in cls._CURVE_TYPES:
             raise ValueError("Input curve_type is wrong.")
         if curve_type == SUYAMA:
             t = n
             while _gcd.gcd(t, n) != 1:
@@ -89,14 +89,18 @@
             d = random.randrange(1, bound + 1)
             start_point = Point(3, 1)
             curve = cls((d + 1) % n)
         elif curve_type == ASUNCION5:
             d = random.randrange(1, bound + 1)
             start_point = Point(4, 1)
             curve = cls((d + 1) % n)
+        elif curve_type == NAKAMURA3:
+            d = random.randrange(1, bound + 1)
+            start_point = Point(2, 1)
+            curve = cls((7*d + 3) % n)
         return curve, start_point
 
 
 class Point (tuple):
     """
     x and z projective coordinates of elliptic curves.
     """
```

### Comparing `NZMATH-1.1.0/nzmath/factor/misc.py` & `nzmath-3.0.0/src/factor/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 def primePowerTest(n):
     """
     This program using Algo. 1.7.5 in Cohen's book judges whether
     n is of the form p**k with prime p or not.
     If it is True, then (p,k) will be returned,
     otherwise (n,0).
     """
-    if n % 2 == 1:
+    if n & 1:
         q = n
         while True:
             if not prime.primeq(q):
                 a = 2
                 while prime.spsp(n, a):
                     a += 1
                 d = gcd.gcd(pow(a,q,q) - a, q)
                 if d == 1 or d == q:
                     return (n, 0)
-                else:
-                    q = d
+                q = d
             else:
                 p = q
                 break
     else:
         p = 2
 
     k, q = arith1.vp(n, p)
@@ -48,38 +47,38 @@
         """
         FactoredInteger(integer [, factors])
 
         If factors is given, it is a dict of type {prime:exponent}
         and the product of prime**exponent is equal to the integer.
         Otherwise, factorization is carried out in initialization.
         """
-        self.integer = long(integer)
+        self.integer = int(integer)
         if factors is None:
             self.factors = dict(methods.factor(self.integer))
         else:
             self.factors = dict(factors)
 
     @classmethod
     def from_partial_factorization(cls, integer, partial):
         """
         Construct a new FactoredInteger object from partial
         factorization information given as dict of type
         {prime:exponent}.
         """
         partial_factor = 1
-        for p, e in partial.iteritems():
+        for p, e in partial.items():
             partial_factor *= p**e
         assert not integer % partial_factor, "wrong factorization"
         return cls(integer // partial_factor) * cls(partial_factor, partial)
 
     def __iter__(self):
         """
         Default iterator
         """
-        return self.factors.iteritems()
+        return iter(self.factors.items())
 
     def __mul__(self, other):
         if isinstance(other, FactoredInteger):
             integer = self.integer * other.integer
             new_factors = self.factors.copy()
             for p in other.factors:
                 new_factors[p] = new_factors.get(p, 0) + other.factors[p]
@@ -101,14 +100,17 @@
 
     def __str__(self):
         return str(self.integer)
 
     def __eq__(self, other):
         return self.integer == int(other)
 
+    def __hash__(self):
+        return hash(self.integer)
+
     def __ne__(self, other):
         return self.integer != int(other)
 
     def __long__(self):
         return self.integer
 
     __int__ = __long__
@@ -140,27 +142,27 @@
         if divisor in quotient.factors:
             if quotient.factors[divisor] == 1:
                 del quotient.factors[divisor]
             else:
                 quotient.factors[divisor] -= 1
         elif not isinstance(other, FactoredInteger):
             dividing = divisor
-            for p, e in self.factors.iteritems():
+            for p, e in self.factors.items():
                 while not dividing % p:
                     dividing //= p
                     if quotient.factors[p] == 1:
                         del quotient.factors[p]
                         assert dividing % p, dividing
                     else:
                         quotient.factors[p] -= 1
                 if dividing == 1:
                     break
             assert dividing == 1
         else:
-            for p, e in other.factors.iteritems():
+            for p, e in other.factors.items():
                 assert p in quotient.factors and quotient.factors[p] >= e
                 if quotient.factors[p] == e:
                     del quotient.factors[p]
                 else:
                     quotient.factors[p] -= e
         quotient.integer //= divisor
         return quotient
@@ -169,15 +171,15 @@
     __floordiv__ = exact_division
 
     def divisors(self):
         """
         Return all divisors.
         """
         l = [1]
-        for p, e in self.factors.iteritems():
+        for p, e in self.factors.items():
             for j in range(1, e + 1):
                 l += [k*pow(p, j) for k in l if k % p]
         l.sort()
         return l
 
     def proper_divisors(self):
         """
@@ -185,42 +187,42 @@
         """
         return self.divisors()[1:-1]
 
     def prime_divisors(self):
         """
         Return the list of primes that divides the number.
         """
-        return self.factors.keys()
+        return list(self.factors.keys())
 
     def square_part(self, asfactored=False):
         """
         Return the largest integer whose square divides the number.
 
         If an optional argument asfactored is true, then the result is
         also a FactoredInteger object. (default is False)
         """
         result = FactoredInteger(1, {})
-        for d, e in self.factors.iteritems():
+        for d, e in self.factors.items():
             if e >= 2:
-                result *= FactoredInteger(d ** (e//2), {d:e//2})
+                result *= FactoredInteger(d ** (e >> 1), {d:e>>1})
         if asfactored:
             return result
         else:
             return result.integer
 
     def squarefree_part(self, asfactored=False):
         """
         Return the largest divisor of the number which is squarefree.
 
         If an optional argument asfactored is true, then the result is
         also a FactoredInteger object. (default is False)
         """
         result = FactoredInteger(1, {})
-        for d, e in self.factors.iteritems():
-            if e % 2:
+        for d, e in self.factors.items():
+            if e & 1:
                 result *= FactoredInteger(d, {d:1})
         if asfactored:
             return result
         else:
             return result.integer
```

### Comparing `NZMATH-1.1.0/nzmath/factor/util.py` & `nzmath-3.0.0/src/factor/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     @staticmethod
     def _validate_input_number(number):
         """
         Return True if the given number is an integer greater than one.
         Return False if the given number is equal to one.
         Otherwise, raise ValueError.
         """
-        if isinstance(number, (int, long)):
+        if isinstance(number, int):
             if number == 1:
                 return False
             if number > 1:
                 return True
         raise ValueError("number must be a positive integer.")
 
     def find(self, target, **options):
```

### Comparing `NZMATH-1.1.0/nzmath/bigrandom.py` & `nzmath-3.0.0/src/bigrandom.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     """
     Choose a random item from range([start,] stop[, step]).
     (Return long integer.)
 
     see random.randrange
     """
     if stop is None:
-        if abs(start) < sys.maxint:
+        if abs(start) < sys.maxsize:
             return _random.randrange(start)
-    elif abs(stop - start) < sys.maxint:
+    elif abs(stop - start) < sys.maxsize:
         return _random.randrange(start, stop, step)
 
     negative_step = False
     if stop is None:
         start, stop = 0, start
     if step < 0:
         start, stop, step = -start, -stop, -step
@@ -48,19 +48,19 @@
 
 def _validate_for_randrange(start, stop, step):
     """
     Check validity of arguments for randrange.
     """
     if step == 0:
         raise ValueError("zero step for randrange()")
-    elif start != long(start):
+    elif start != int(start):
         raise ValueError("non-integer arg 1 for randrange()")
-    elif stop != long(stop):
+    elif stop != int(stop):
         raise ValueError("non-integer stop for randrange()")
-    elif step != long(step):
+    elif step != int(step):
         raise ValueError("non-integer step for randrange()")
     if start >= stop:
         raise ValueError("empty range for randrange()")
 
 random = _random.random
 seed = _random.seed
```

### Comparing `NZMATH-1.1.0/nzmath/quad.py` & `nzmath-3.0.0/src/quad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 import math
 import copy
 import warnings
 import nzmath.gcd as gcd
 import nzmath.arith1 as arith1
 import nzmath.prime as prime
 import nzmath.factor.misc as misc
@@ -28,15 +28,15 @@
     def __mul__(self, other):
         if not isinstance(other, ReducedQuadraticForm):
             return NotImplemented
         composition = compositePDF(self.element, other.element)
         return self.__class__(composition, self.unit)
 
     def __pow__(self, exp):
-        if not isinstance(exp, (int, long)):
+        if not isinstance(exp, int):
             raise TypeError("powering index must be an integer.")
         powered_form = powPDF(self.element, exp, self.unit)
         return self.__class__(powered_form, self.unit)
 
     def __truediv__(self, other):
         invel = other.inverse()
         composition = compositePDF(self.element, invel.element)
@@ -56,14 +56,19 @@
         if self.__class__ != other.__class__:
             return False
         if self.element == other.element and self.unit == other.unit:
             return True
         else:
             return False
 
+    def __hash__(self):
+        val = sum([hash(ele) for ele in self.element])
+        val += sum([hash(ele) for ele in self.unit])
+        return val
+
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def disc(self):
         """
         Return discriminant of the form.
         """
@@ -191,27 +196,27 @@
     return int(ht * ml + 0.5)
 
 def class_number(disc, limit_of_disc=100000000):
     """
     Return class number with the given discriminant by counting reduced forms.
     Not only fundamental discriminant.
     """
-    if disc % 4 not in (0, 1):
+    if disc & 3 not in (0, 1):
         raise ValueError("a discriminant must be 0 or 1 mod 4")
     if disc >= 0:
         raise ValueError("a discriminant must be negative")
     if -disc >= limit_of_disc:
         warnings.warn("the discriminant seems to have too big absolute value")
 
     h = 1
-    b = disc % 2
+    b = disc & 1
     c_b = int(math.sqrt(-disc / 3))
 
     while b <= c_b:
-        q = (b**2 - disc) // 4
+        q = (b**2 - disc) >> 2
         a = b
         if a <= 1:
             a = 2
         while a**2 <= q:
             if q % a == 0 and gcd.gcd_of_list([a, b, q//a])[0] == 1:
                 if a == b or a**2 == q or b == 0:
                     h += 1
@@ -222,38 +227,38 @@
     return h
 
 def class_group(disc, limit_of_disc=100000000):
     """
     Return the class number and the class group with the given discriminant
     by counting reduced forms. Not only fundamental discriminant.
     """
-    if disc % 4 not in (0, 1):
+    if disc & 3 not in (0, 1):
         raise ValueError("a discriminant must be 0 or 1 mod 4")
     if disc >= 0:
         raise ValueError("a discriminant must be negative")
     if -disc >= limit_of_disc:
         warnings.warn("the discriminant seems to have too big absolute value")
 
     h = 1
-    b = disc % 2
+    b = disc & 1
     c_b = int(math.sqrt(-disc / 3))
 
     ret_list = []
     f_a = 1
-    if disc % 4 == 0:
+    if disc & 3 == 0:
         f_b = 0
-        f_c = -(disc // 4)
+        f_c = -(disc >> 2)
     else:
         f_b = 1
-        f_c = -((disc - 1) // 4)
+        f_c = -((disc - 1) >> 2)
     unit = (f_a, f_b, f_c)
     ret_list.append(ReducedQuadraticForm(unit, unit))
 
     while b <= c_b:
-        q = (b**2 - disc) // 4
+        q = (b**2 - disc) >> 2
         a = b
         if a <= 1:
             a = 2
         while a**2 <= q:
             if q % a == 0 and gcd.gcd_of_list([a, b, q//a])[0] == 1:
                 f_c = (b**2 - disc) // (4 * a)
                 if a == b or a**2 == q or b == 0:
@@ -282,23 +287,23 @@
         self.g_parent = 0
 
 
 def class_number_bsgs(disc):
     """
     Return the class number with the given discriminant.
     """
-    if disc % 4 not in (0, 1):
+    if disc & 3 not in (0, 1):
         raise ValueError("a discriminant must be 0 or 1 mod 4")
 
     if disc >= 0:
         raise ValueError("a discriminant must be negative")
 
     lx = max(arith1.floorpowerroot(abs(disc), 5), 500 * (math.log(abs(disc)))**2)
     uprbd = int(class_formula(disc, int(lx)) * 3 / 2)
-    lwrbd = uprbd // 2 + 1
+    lwrbd = (uprbd >> 1) + 1
     bounds = [lwrbd, uprbd]
 
     # get the unit
     element = RetNext(disc)
     ut = element.unit()
 
     # append the unit to subset of G
@@ -335,27 +340,27 @@
 
     return h
 
 def class_group_bsgs(disc, classnum, qin):
     """
     Return the construction of the class group with the given discriminant.
     """
-    if disc % 4 not in (0, 1):
+    if disc & 3 not in (0, 1):
         raise ValueError("a discriminant must be 0 or 1 mod 4")
     if disc >= 0:
         raise ValueError("a discriminant must be negative")
 
     matla = []
     lstofelg = []
     lpt = []
 
     # compute bounds
     qpt = qin[0] ** qin[1]
     uprbd = qpt + 1
-    lwrbd = uprbd // 2 + 1
+    lwrbd = (uprbd >> 1) + 1
     if lwrbd > uprbd:
         raise TypeError("lower bound needs to be less than upper bound")
     if lwrbd <= (uprbd / 2):
         raise TypeError("upper bound / 2 needs to be more than lower bound")
     bounds = [lwrbd, uprbd]
 
     # get the unit
@@ -400,15 +405,15 @@
     """
     def __init__(self, disc):
         self.disc = disc
         self.utroot = unit_form(disc)
         self._unit = ReducedQuadraticForm(self.utroot, self.utroot)
         self.cnt = 1
         self.previous = []
-        self.elhash = range(int(math.sqrt(abs(disc) // 3)) + 2)
+        self.elhash = list(range(int(math.sqrt(abs(disc) // 3)) + 2))
 
     def unit(self):
         """
         Return reduced quadratic unit form.
         """
         return self._unit
 
@@ -436,38 +441,38 @@
                     return nxtfm
 
     def add_to_hash(self, form):
         """
         Add a form to hash
         """
         key = form.element[0]
-        if isinstance(self.elhash[key], (int, long)):
+        if isinstance(self.elhash[key], int):
             self.elhash[key] = [form]
         else:
             self.elhash[key].append(form)
 
     def has_in_hash(self, form):
         """
         check hash
         """
         key = form.element[0]
-        if isinstance(self.elhash[key], (int, long)):
+        if isinstance(self.elhash[key], int):
             return False
         return form in self.elhash[key]
 
 
 def disc(f):
     """
     Return the discriminant of the given quadratic form 'f'.
     f = [a, b, c]
     """
     if len(f) != 3:
         raise TypeError("form must be composed of 3 integers")
     for i in f:
-        if not isinstance(i, (int, long)):
+        if not isinstance(i, int):
             raise TypeError("all components must be integers")
     return (f[1]*f[1] - 4*f[0]*f[2])
 
 def reducePDF(f):
     """
     Return the reduced form of the given positive definite form 'f'.
     f = (f_1, f_2, f_3)
@@ -485,17 +490,17 @@
             if (f_1 == f_3) and (f_2 < 0):
                 f_2 = -f_2
             return (f_1, f_2, f_3)
     while 1:
         q = f_2 // (2*f_1)
         r = f_2 - q*(2*f_1)
         if r > f_1:
-            r = r - 2*f_1
-            q = q + 1
-        f_3 = f_3 - ((f_2 + r)//2)*q
+            r -= 2*f_1
+            q += 1
+        f_3 -= ((f_2 + r)>>1)*q
         f_2 = r
         if f_1 > f_3:
             f_2 = -f_2
             f_1, f_3 = f_3, f_1
             continue
         else:
             if (f_1 == f_3) and (f_2 < 0):
@@ -519,15 +524,15 @@
         lc = -c_1
 
     # partial reduction
     v_2, v_3, z, d, v = parteucl(la, lc, sogsp)
 
     if z == 0:
         g = (lb * v_3 + f[2]) // d
-        a_2 = d**2
+        a_2 = d ** 2
         c_2 = v_3 ** 2
         b_2 = f[1] + (d + v_3)**2 - a_2 - c_2
         c_2 = c_2 + g * d_1
         return reducePDF((a_2, b_2, c_2))
 
     e = (f[2] * v + lb * d) // la
     g = (e * v_2 - lb) // v
@@ -563,17 +568,17 @@
         sz = (f[0], -f[1], f[2])
     else:
         lexp = exp
         sz = f
     # Right-Left Binary algorithm
     sy = ut
     while True:
-        if (lexp % 2) == 1:
+        if (lexp & 1) == 1:
             sy = compositePDF(sz, sy)
-        lexp = lexp // 2
+        lexp >>= 1
         if lexp == 0:
             return sy
         else:
             sz = sqrPDF(sz)
 
 def compositePDF(f_1, f_2):
     """
@@ -586,15 +591,15 @@
         raise ValueError("coefficients of a quadratic form must be relatively prime")
     if disc(f_1) != disc(f_2):
         raise ValueError("two quadratic forms must have same discriminant")
 
     if f_1[0] > f_2[0]:
         f_1, f_2 = f_2, f_1
 
-    s = (f_1[1] + f_2[1]) // 2
+    s = (f_1[1] + f_2[1]) >> 1
     n = f_2[1] - s
 
     if f_2[0] % f_1[0] == 0:
         y_1 = 0
         d = f_1[0]
     else:
         u, v, d = euclid_exd(f_2[0], f_1[0])
@@ -619,19 +624,19 @@
 
     return reducePDF((a_3, b_3, c_3))
 
 def unit_form(disc):
     """
     Return generated quadratic form with the given discriminant.
     """
-    if disc % 4 == 0:
+    if disc & 3 == 0:
         a = 1
         b = 0
         c = disc // -4
-    elif disc % 4 == 1:
+    elif disc & 3 == 1:
         a = 1
         b = 1
         c = (disc - 1) // -4
     else:
         raise ValueError("discriminant is not 0 or 1 mod 4.")
     return (a, b, c)
 
@@ -641,29 +646,29 @@
     """
     tab2 = (0, 1, 0, -1, 0, -1, 0, 1)
     if b == 0:
         if abs(a) != 1:
             return 0
         if abs(a) == 1:
             return 1
-    if a % 2 == 0 and b % 2 == 0:
+    if a & 1 == 0 and b & 1 == 0:
         return 0
 
     v, b = arith1.vp(b, 2)
-    if v % 2 == 0:
+    if v & 1 == 0:
         k = 1
     else:
         k = tab2[a & 7]
     if b < 0:
         b = -b
         if a < 0:
             k = -k
     while a:
         v, a = arith1.vp(a, 2)
-        if v % 2 == 1:
+        if v & 1:
             k *= tab2[b & 7]
         if a & b & 2:
             # both a and b are 3 mod 4
             k = -k
         r = abs(a)
         a = b % r
         b = r
@@ -730,22 +735,22 @@
 
 def sqroot(disc, p):
     """
     Return a reduced quadratic form with the given discriminant.
     'disc' is a quadratic residue mod 'p'.
     """
     if p == 2: # if 8 | disc => (disc / 8) = 0, 8 not | disc but 4 | disc => 2
-        if (disc % 8) == 0:
+        if (disc & 7) == 0:
             bp = disc
-        elif (disc % 4) == 0: # 4 - 4 * odd % 8 => 0
+        elif (disc & 3) == 0: # 4 - 4 * odd % 8 => 0
             bp = 2
-        elif (disc % 8) == 1: # disc is odd and disc % 8 is 1
+        elif (disc & 7) == 1: # disc is odd and disc % 8 is 1
             bp = disc
-        else: # disc is odd and disc % 4 is 1 => impossible (-5 / 2) = -1
-            raise ValueError("disc is odd and disc % 4 is 1 => impossible (-5 / 2) = -1")
+        else: # disc is odd and disc & 3 is 1 => impossible (-5 / 2) = -1
+            raise ValueError("disc is odd and disc & 3 is 1 => impossible (-5 / 2) = -1")
     else:
         bpf1 = arith1.modsqrt(disc, p)
         bpf2 = disc
         bp = crt([(bpf1, p), (bpf2, 4)])
     if bp > p:
         bp = 2 * p - bp
 
@@ -779,30 +784,30 @@
 def isfundamental(disc):
     """
     Determine whether the given discriminant is fundamental or not.
     """
     if disc == 1:
         return False
     spt = misc.squarePart(abs(disc))
-    if (disc % 4) == 1:
+    if (disc & 3) == 1:
         return spt == 1
-    elif (disc % 4) == 0:
+    elif (disc & 3) == 0:
         spt //= 2
         if spt != 1:
             return False
-        discof = (disc // 4) % 4
+        discof = (disc >> 2) & 3
         return discof == 2 or discof == 3
     return False
 
 def euclid_exd(a, b):
     """
     Return a tuple (u, v, d); they are the greatest common divisor d
     of two integers a and b and u, v such that d = a * u + b * v.
     """
-    if not isinstance(a, (int, long)) or not isinstance(b, (int, long)):
+    if not isinstance(a, int) or not isinstance(b, int):
         raise TypeError
     u = 1
     d = a
     if b == 0:
         v = 0
         return (u, v, d)
     else:
@@ -839,15 +844,15 @@
             t_2 = v - (q * v_2)
             v = v_2
             d = v_3
             v_2 = t_2
             v_3 = t_3
             z = z + 1
         else:
-            if z % 2 != 0:
+            if z & 1:
                 v_2 = -v_2
                 v_3 = -v_3
             return (v_2, v_3, z, d, v)
 
 def isfinished_bsgscv(n, sossp, sogsp, nt, lpt, qpt, disc, classnum, indofg):
     """
     Determine whether the bsgs algorithm is finished or not yet.
@@ -862,15 +867,15 @@
     elif sumn > qpt:
         raise ValueError
 
     if n == 1:
         return False, sossp, sogsp
     else:
         tpsq = misc.primePowerTest(n)
-        if (tpsq[1] != 0) and ((tpsq[1] % 2) == 0):
+        if (tpsq[1] != 0) and ((tpsq[1] & 1) == 0):
             q = arith1.floorsqrt(n)
         else:
             q = arith1.floorsqrt(n) + 1
 
     ss = sossp.retel()
     new_sossp = ClassGroup(disc, classnum, [])
     tnt = copy.deepcopy(nt)
@@ -963,15 +968,15 @@
     """
     mstp1 = bounds[1] - bounds[0]
     if (mstp1 == 0) or (mstp1 == 1):
         q = 1
     else:
         tppm = misc.primePowerTest(mstp1)
         q = arith1.floorsqrt(mstp1)
-        if (tppm[1] == 0) or (tppm[1] % 2):
+        if (tppm[1] == 0) or (tppm[1] & 1):
             q += 1
 
     n_should_be_set = True
     # initialize
     c_s1 = ClassGroup(disc, classnum, []) # a subset of G
 
     # extracting i = 0 case of main loop
```

### Comparing `NZMATH-1.1.0/nzmath/gcd.py` & `nzmath-3.0.0/src/gcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,13 +87,13 @@
     >>> pairwise_coprime([1, 2, 3])
     True
     >>> pairwise_coprime([1, 2, 3, 4])
     False
     >>>
     """
     int_iter = iter(int_list)
-    product = int_iter.next()
+    product = next(int_iter)
     for n in int_iter:
         if not coprime(product, n):
             return False
         product *= n
     return True
```

### Comparing `NZMATH-1.1.0/nzmath/config.py` & `nzmath-3.0.0/src/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 import warnings
 
 WINDOWS_PLATFORMS = ('win32', 'win64', 'cli', )
 
 def nzmath_info():
-	print("NZMATH [Version 1.1.0]")
+    print("NZMATH [Version 3.0.0]")
 
 # ----------------
 # Default Settings
 # ----------------
 #
 # Dependencies
 # ============
@@ -60,23 +60,23 @@
 # net availability
 # ----------------
 #
 # Some functions will connect to the Net.
 # Desktop machines are usually connected to the Net, but notebooks
 # may have connectivity only occasionally.
 #
-# If you have net connectivity now, set as the following:
-#HAVE_NET = True
-#CHECK_NET = False
+# If sometimes you have net connectivity, set as the following:
+HAVE_NET = True
+CHECK_NET = False
 # Or, if your machine is not connected, set as the following:
 #HAVE_NET = False
 #CHECK_NET = False
-# The default values mean "I don't know; check it later":
-HAVE_NET = None
-CHECK_NET = True
+# Or you can let NZMATH check connectivity every time, set as the following:
+#HAVE_NET = None
+#CHECK_NET = True
 
 #
 # psyco
 # -----
 #
 # psyco is a package providing JIT compiler for Python.
 # http://psyco.sourceforge.net/
@@ -244,22 +244,22 @@
 # net availability
 # ----------------
 #
 def check_net():
     """
     Check the net connection by http call.
     """
-    import urllib2
+    import urllib.request, urllib.error, urllib.parse
     try:
-        urllib2.urlopen('http://sourceforge.net/projects/nzmath/')
+        urllib.request.urlopen('http://sourceforge.net/projects/nzmath/')
         return True
-    except urllib2.HTTPError:
+    except urllib.error.HTTPError:
         # the problem is on server side, thus connected anyway
         return True
-    except urllib2.URLError:
+    except urllib.error.URLError:
         # no dns, thus no connection
         return False
     except Exception:
         # I don't know the reason, but something wrong
         return False
 
 if CHECK_NET:
@@ -300,14 +300,18 @@
 
 #
 # data directory
 # --------------
 #
 def default_datadir():
     candidates = []
+    
+    # developing environment
+    candidates.append(os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), 'dist', 'data'))
+
     if DATADIR is not None:
         candidates.append(DATADIR)
     if sys.platform in WINDOWS_PLATFORMS:
         candidates.append(os.path.join(sys.prefix, 'Data', 'nzmath'))
     else:
         candidates.append(os.path.join(sys.prefix, 'share', 'nzmath'))
     # default install script will install here ...hmm
```

### Comparing `NZMATH-1.1.0/nzmath/equation.py` & `nzmath-3.0.0/src/equation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nzmath.plugins import SETPRECISION
 SETPRECISION(200)
 
 Then, the following computations will be done in such precision, if
 plugins.PRECISION_CHANGEABLE is true.
 """
 
-from __future__ import division
+
 import logging
 
 import nzmath.arith1 as arith1
 import nzmath.bigrandom as bigrandom
 import nzmath.bigrange as bigrange
 import nzmath.finitefield as finitefield
 import nzmath.imaginary as imaginary
@@ -50,15 +50,15 @@
         raise ValueError("No Solution")
 
 def e2(x):
     """
     0 = x[0] + x[1]*t + x[2]*t**2
     """
     c, b, a = x
-    d = b**2 - 4*a*c 
+    d = b**2 - 4*a*c
     if d >= 0:
         sqrtd = math.sqrt(d)
     else:
         sqrtd = cmath.sqrt(d)
     return ((-b + sqrtd)/(2*a), (-b - sqrtd)/(2*a))
 
 def e2_Fp(x, p):
@@ -67,17 +67,17 @@
     f = x[0] + x[1]*t + x[2]*t**2
     """
     c, b, a = [_x % p for _x in x]
     if a == 0:
         return [e1_ZnZ([c, b], p)]
     if p == 2:
         solutions = []
-        if x[0] % 2 == 0:
+        if x[0] & 1 == 0:
             solutions.append(0)
-        if (x[0] + x[1] + x[2]) % 2 == 0:
+        if (x[0] + x[1] + x[2]) & 1 == 0:
             solutions.append(1)
         if len(solutions) == 1:
             return solutions * 2
         return solutions
     d = b**2 - 4*a*c
     if arith1.legendre(d, p) == -1:
         return []
@@ -237,46 +237,46 @@
 
     return z
 
 def _upper_bound_of_roots(g):
     """
     Return an upper bound of roots.
     """
-    weight = len(filter(None, g))
+    weight = len([_f for _f in g if _f])
     assert g[-1]
     return max([pow(weight*abs(c/g[-1]), 1/len(g)) for c in g])
 
 def root_Fp(g, p, flag=True):
     """
     Return a root over F_p of nonzero polynomial g.
     p must be prime.
     If flag = False, return a root randomly
     """
     if isinstance(g, list):
         if not isinstance(g[0], tuple):
-            g = zip(range(len(g)), g)
+            g = list(zip(list(range(len(g))), g))
     Fp = finitefield.FinitePrimeField(p)
     g = uniutil.FinitePrimeFieldPolynomial(g, Fp)
     h = uniutil.FinitePrimeFieldPolynomial({1:-1, p:1}, Fp)
     g = g.gcd(h)
     deg_g = g.degree()
     if g[0] == 0:
         deg_g = deg_g - 1
-        g = g.shift_degree_to(deg_g) 
+        g = g.shift_degree_to(deg_g)
     while True:
         if deg_g == 0:
             return None
         if deg_g == 1:
             return (-g[0]/g[1]).toInteger()
         elif deg_g == 2:
             d = g[1]*g[1] - 4*g[0]
             e = arith1.modsqrt(d.toInteger(), p)
             return ((-g[1]-e)/(2*g[2])).toInteger()
         deg_h = 0
-        x = uniutil.FinitePrimeFieldPolynomial({0:-1, (p-1)//2:1}, Fp)
+        x = uniutil.FinitePrimeFieldPolynomial({0:-1, (p-1)>>1:1}, Fp)
         if flag:
             a = 0
             while deg_h == 0 or deg_h == deg_g:
                 b = uniutil.FinitePrimeFieldPolynomial({0:-a, 1:1}, Fp)
                 v = g(b)
                 h = x.gcd(v)
                 a = a + 1
@@ -296,15 +296,15 @@
 def allroots_Fp(g, p):
     """
     Return roots over F_p of nonzero polynomial g.
     p must be prime.
     """
     if isinstance(g, list):
         if not isinstance(g[0], tuple):
-            g = zip(range(len(g)), g)
+            g = list(zip(list(range(len(g))), g))
     Fp = finitefield.FinitePrimeField(p)
     g = uniutil.FinitePrimeFieldPolynomial(g, Fp)
     h = uniutil.FinitePrimeFieldPolynomial({1:-1, p:1}, Fp)
     g = g.gcd(h)
     deg_g = g.degree()
     roots = []
     if g[0] == 0:
@@ -321,15 +321,15 @@
     elif deg_g == 2:
         d = g[1]*g[1]-4*g[0]
         e = arith1.modsqrt(d.toInteger(), p)
         g1 = -g[1]
         g2 = 2*g[2]
         return [((g1 - e) / g2).toInteger(), ((g1 + e) / g2).toInteger()]
     deg_h = 0
-    x = uniutil.FinitePrimeFieldPolynomial({0:-1, (p-1)//2:1}, Fp)
+    x = uniutil.FinitePrimeFieldPolynomial({0:-1, (p-1)>>1:1}, Fp)
     a = 0
     while deg_h == 0 or deg_h == deg_g:
         b = uniutil.FinitePrimeFieldPolynomial({0:-a, 1:1}, Fp)
         v = g(b)
         h = x.gcd(v)
         a = a + 1
         deg_h = h.degree()
```

### Comparing `NZMATH-1.1.0/nzmath/ring.py` & `nzmath-3.0.0/src/ring.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 base classes for rings.
 """
 
-from __future__ import division
+
 
 
 class Ring (object):
     """
     Ring is an abstract class which expresses that
     the derived classes are (in mathematical meaning) rings.
 
@@ -17,15 +17,15 @@
     """
 
     def __init__(self):
         """
         Initialize _one and _zero for later use for properties 'one'
         and 'zero'.
         """
-        # This class is abstract and cannot be instanciated.
+        # This class is abstract and cannot be instantiated.
         if type(self) is Ring:
             raise NotImplementedError("class Ring is abstract")
         self._one = None
         self._zero = None
 
     def createElement(self, seed):
         """
@@ -71,14 +71,17 @@
 
     def __eq__(self, other):
         """
         Equality test.
         """
         raise NotImplementedError("derived class should override")
 
+    def __hash__(self):
+        raise NotImplementedError("derived class should override")
+
     def __ne__(self, other):
         """
         Inequality test.
         """
         return not self.__eq__(other)
 
 
@@ -89,15 +92,15 @@
     """
 
     def __init__(self):
         """
         Initialize 'properties' attribute by an object of
         CommutativeRingProperties.
         """
-        # This class is abstract and cannot be instanciated.
+        # This class is abstract and cannot be instantiated.
         if type(self) is CommutativeRing:
             raise NotImplementedError("class CommutativeRing is abstract")
         Ring.__init__(self)
         self.properties = CommutativeRingProperties()
         self._actions = {}
         self._actions_order = []
 
@@ -190,15 +193,15 @@
     the derived classes are (in mathematical meaning) fields.
     """
 
     def __init__(self):
         """
         Set field flag True of 'properties' attribute.
         """
-        # This class is abstract and cannot be instanciated.
+        # This class is abstract and cannot be instantiated.
         if type(self) is Field:
             raise NotImplementedError
         CommutativeRing.__init__(self)
         self.properties.setIsfield(True)
 
     def createElement(self, *args):
         """
@@ -234,15 +237,15 @@
     """
 
     def __init__(self, domain):
         """
         Create quotient field from given domain.
         Initialize 'basedomain' attribute by the given 'domain'.
         """
-        # This class is abstract and cannot be instanciated.
+        # This class is abstract and cannot be instantiated.
         if type(self) is QuotientField:
             raise NotImplementedError("QuotientField is an abstract class")
         Field.__init__(self)
         self.basedomain = domain
 
         def baseaction(baseelement, quotient):
             return quotient.__class__(baseelement * quotient.numerator, quotient.denominator)
@@ -253,15 +256,15 @@
 class RingElement (object):
     """
     RingElement is an abstract class for elements of rings.
     """
 
     def __init__(self, *args, **kwd):
         """
-        This class is abstract and cannot be instanciated.
+        This class is abstract and cannot be instantiated.
         """
         if type(self) is RingElement:
             raise NotImplementedError("RingElement is an abstract class.")
 
     def getRing(self):
         """
         getRing returns an object of a subclass of Ring,
@@ -271,14 +274,17 @@
 
     def __eq__(self, other):
         """
         Equality test.
         """
         raise NotImplementedError
 
+    def __hash__(self):
+        raise NotImplementedError
+
     def __ne__(self, other):
         """
         Inequality test.
         """
         return not (self == other)
 
 
@@ -286,15 +292,15 @@
     """
     CommutativeRingElement is an abstract class for elements of
     commutative rings.
     """
 
     def __init__(self):
         """
-        This class is abstract and cannot be instanciated.
+        This class is abstract and cannot be instantiated.
         """
         if type(self) is CommutativeRingElement:
             raise NotImplementedError("CommutativeRingElement is an abstract class.")
         RingElement.__init__(self)
 
     def mul_module_action(self, other):
         """
@@ -302,15 +308,15 @@
         other must be in one of the action rings of self's ring.
         """
         try:
             self_ring = self.getRing()
             other_ring = getRing(other)
             if self_ring.hasaction(other_ring):
                 return self_ring.getaction(other_ring)(other, self)
-        except RuntimeError, e:
+        except RuntimeError as e:
             #print "mul_module_action", e
             raise
         raise TypeError("no module action with %s" % str(other_ring))
 
     def exact_division(self, other):
         """
         In UFD, if other divides self, return the quotient as a UFD
@@ -336,15 +342,15 @@
 
 class FieldElement (CommutativeRingElement):
     """
     FieldElement is an abstract class for elements of fields.
     """
     def __init__(self):
         """
-        This class is abstract and cannot be instanciated.
+        This class is abstract and cannot be instantiated.
         """
         if type(self) is FieldElement:
             raise NotImplementedError("FieldElement is an abstract class.")
         CommutativeRingElement.__init__(self)
 
     def exact_division(self, other):
         """
@@ -444,14 +450,16 @@
         if hasattr(other, "numerator") and hasattr(other, "denominator"):
             return self.numerator*other.denominator == self.denominator*other.numerator
         try:
             return self == self.getRing().one.mul_module_action(other)
         except TypeError:
             return NotImplemented
 
+    def __hash__(self):
+        return hash(self.numerator * self.denominator)
 
 class Ideal (object):
     """
     Ideal class is an abstract class to represent the finitely
     generated ideals.  Because the finitely-generatedness is not a
     restriction for Noetherian rings and in the most cases only
     Noetherian rings are used, it is general enough.
@@ -504,14 +512,17 @@
         assert type(self) is type(other)
         if self is other:
             return True
         if self.ring is not other.ring:
             return False
         return self.issubset(other) and self.issuperset(other)
 
+    def __hash__(self):
+        raise NotImplementedError
+
     def __ne__(self, other):
         """
         I != J <=> I.__ne__(J)
         """
         return not self.__eq__(other)
 
     def __contains__(self, element):
@@ -570,14 +581,17 @@
         return False
 
     def __eq__(self, other):
         if isinstance(other, ResidueClassRing):
             return self.ideal == other.ideal
         return False
 
+    def __hash__(self):
+        return hash(self.ideal)
+
     # properties
     def _getOne(self):
         "getter for one"
         if self._one is None:
             seed = self.ring.one
             if seed is not None:
                 self._one = ResidueClass(seed, self.ideal)
@@ -624,14 +638,17 @@
 
     def __eq__(self, other):
         if isinstance(other, ResidueClass):
             if self.ideal == other.ideal:
                 return (self.x - other.x) in self.ideal
         return False
 
+    def __hash__(self):
+        raise NotImplementedError 
+
     def getRing(self):
         """
         Return a ResidueClassRing object.
         This overrides the method inherited from CommutativeRingElement.
         """
         return ResidueClassRing(self.ideal.ring, self.ideal)
 
@@ -774,15 +791,15 @@
     """
     Return a RingElement instance which eqauls 'obj'.
 
     Mainly for python built-in objects such as int or float.
     """
     if isinstance(obj, RingElement):
         return obj
-    elif isinstance(obj, (int, long)):
+    elif isinstance(obj, int):
         import nzmath.rational as rational
         return rational.Integer(obj)
     elif isinstance(obj, float):
         import nzmath.real as real
         return real.Real(obj)
     elif isinstance(obj, complex):
         import nzmath.imaginary as imaginary
@@ -795,15 +812,15 @@
 
     Mainly for python built-in objects such as int or float.
     """
     try:
         # if obj has its getRing method, use it.
         return obj.getRing()
     except AttributeError:
-        if isinstance(obj, (int, long)):
+        if isinstance(obj, int):
             import nzmath.rational as rational
             return rational.theIntegerRing
         if isinstance(obj, float):
             import nzmath.real as real
             return real.theRealField
         if isinstance(obj, complex):
             import nzmath.imaginary as imaginary
@@ -816,15 +833,15 @@
     field, if the 'obj' is an element of non-field domain.
 
     Mainly for python built-in objects such as int or float.
     """
     if hasattr(obj, "inverse"):
         return obj.inverse()
     # special cases
-    if isinstance(obj, (int, long)):
+    if isinstance(obj, int):
         import nzmath.rational as rational
         return rational.Rational(1, obj)
     elif isinstance(obj, (float, complex)):
         return 1 / obj
     # final trial
     try:
         # if true division does not fail, it should return the inverse
```

### Comparing `NZMATH-1.1.0/nzmath/permute.py` & `nzmath-3.0.0/src/permute.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import nzmath.gcd as gcd
 import nzmath.matrix as matrix
 import nzmath.rational as rational
 
 class Permute:
 
     """
-    This is a class for 'normal' type element of permutation group.
+    This is a class for 'normal' type element in the permutation group.
     Example, [2,3,1,5,4]
     This means [1 2 3 4 5]
                [2 3 1 5 4]
     (It is 1:1 onto mapping, 1->2, 2->3, 3->1, 4->5, 5->4)
     """
 
     def __init__(self, value, key=None, flag=False):
@@ -23,93 +23,95 @@
         Permute(['b','c','d','e','a'], 1) -> [2,3,4,5,1]-normal type(identity is ascending order)
         Permute(['b','c','d','e','a'], -1) -> [4,3,2,1,5]-normal type(identity is descending order)
         Permute(['b','c','d','e','a'], ['b','a', 'c','d','e']) -> [1,3,4,5,2]-normal type(identity=key)
         Permute({'a':'b','b':'c','c':'d','d':'e','e':'a'}) -> [2,3,4,5,1]-normal type
         """
         if isinstance(value, dict):
             if key:
-                raise TypeError("key isn't need when dict type is used")
-            data = value.values()
-            key = value.keys()
+                raise TypeError("cannot convert Permute. I think `key` should be None.")
+            data = list(value.values())
+            key = list(value.keys())
         elif isinstance(value, (list, tuple)):
             data = list(value)
         else:
-            raise TypeError("Not normal form")
+            raise TypeError("cannot convert Permute. `value` should be a list or a dict.")
         if key == 0:
             self.data = [i + 1 for i in data]
-            self.key = range(len(data))
+            self.key = list(range(len(data)))
         elif key:
             if isinstance(key, (list, tuple)):
                 self.key = list(key)
                 if len(value) != len(key):
-                    raise TypeError("Length error")
+                    raise TypeError("cannot convert Permute. The length of `key` should be equal to that of `value`.")
             elif key == 1:
                 p_key = list(data)
                 p_key.sort()
                 self.key = p_key
             elif key == -1:
                 p_key = list(data)
                 p_key.sort()
                 p_key.reverse()
                 self.key = p_key
             else:
-                raise TypeError("Input sequence type")
+                raise TypeError("cannot convert Permute. `key` should be a list.")
             key = self.key
             if flag:
                 self.data = data
             else:
                 self.data = [key.index(x) + 1 for x in data]
         else:
             self.data = data
-            self.key = range(1, len(data) + 1)
+            self.key = list(range(1, len(data) + 1))
         data = self.data
-        p_data = range(len(data))
+        p_data = list(range(len(data)))
         for x in data:
             if not rational.isIntegerObject(x):
-                raise TypeError("This number should be integer list")
+                raise TypeError("cannot convert Permute. `flag` should be False.")
             elif x <= 0 or x > len(data):
-                raise TypeError("This isn't onto")
+                raise TypeError("cannot convert Permute. The map should be onto.")
             elif p_data[x-1] == -1:
-                raise ValueError("This isn't one-to-one")
+                raise ValueError("cannot convert Permute. The map should be one-to-one.")
             else:
                 p_data[x-1] = -1
 
     def __getitem__(self, other):
         try:
             idx = self.key.index(other)
         except ValueError:
-            raise ValueError("Input key element")
+            raise ValueError("The indices must be elements of self.key.")
         return self.key[self.data[idx]  - 1]
 
     def __mul__(self, other):
         """
-        Multiplication is with composite mapping way.
-        Self is calculated after other
+        Compute the multiplication, that is, the composite of two maps self \circ other.
+        The map is the application of `self` to the result of `other`.
         """
         s_data = self.data
         o_data = other.data
         lth = len(s_data)
         if self.key != other.key or lth != len(o_data):
-            raise TypeError("This can't multiply")
+            raise TypeError("cannot multiply a Permute by a Permute which has a different type.")
         sol = [s_data[o_data[i] - 1] for i in range(lth)]
         return Permute(sol, self.key, flag=True)
 
     def __rmul__(self, other):
         return other * self
 
     def __div__(self, other):
         return self * (other.inverse())
 
+    __truediv__ = __div__
+
     def __rdiv__(self, other):
         return other * (self.inverse())
 
     def __pow__(self, other):
         sol = self.__class__(self.data, self.key, flag=True)
         if not rational.isIntegerObject(other):
-            raise TypeError("This can't calculate")
+            raise TypeError("cannot pow operation with %s" % other)
         if other > 0:
             for i in range(other - 1):
                 sol = self * sol
         else:
             inv = self.inverse()
             for i in range(abs(other) + 1):
                 sol = inv * sol
@@ -117,40 +119,40 @@
 
     def __call__(self, other):
         return self.permute(other)
 
     def setKey(self, key=None):
         """
         Set other key.
-        this is used when you want to permute different sequence by
-        same permutation.
+        The function may be used if you want to permute a different sequence with
+        the same permutation.
         """
         if key == 0:
-            self.key = range(len(data))
+            self.key = list(range(len(data)))
         elif key:
             if len(key) != len(self.key):
-                raise TypeError, "Invalid length"
+                raise TypeError("The length of `key` should be equal to that of self.key.")
             else:
                 if key[0] in self.key: # key transformation
                     data = list(self.data)
                     keys = self.key
                     sol = [0] * len(data)
                     try:
                         for i in range(len(data)):
                             sol[key.index(keys[i])] = key.index(keys[data[i]-1]) + 1
                         self.data = sol
                     except ValueError:
                         pass
                 self.key = key
         else:
-            self.key = range(1, len(data) + 1)
+            self.key = list(range(1, len(data) + 1))
 
     def getValue(self):
         """
-        Get value expressed by key
+        Return value of self.
         """
         return [self.key[self.data[i] - 1] for i in range(len(self.data))]
 
     def inverse(self):
         s_data = self.data
         sol = [0] * len(s_data)
         for i in range(len(s_data)):
@@ -158,17 +160,19 @@
         return Permute(sol, self.key, flag=True)
 
     def getGroup(self):
         return PermGroup(self.key)
 
     def numbering(self):
         """
-        Return number of permutation element.
+        Return the number of self by the following numbering.
+
+        This is the inductive definition on the dimension.
         It is symmetrical arranging.
-        This is inductive definition for dimension.
+
         Example,
         2-dimension [1,2], [2,1]
         3-dimension [1,2,3], [2,1,3], [1,3,2], [2,3,1], [3,1,2], [3,2,1]
         4-dimension [1,2,3,4], [2,1,3,4], [1,3,2,4], [2,3,1,4], [3,1,2,4],
                     [3,2,1,4], ..., [4,3,2,1]
         """
         s_data = self.data
@@ -190,15 +194,16 @@
         """
         return self.ToCyclic().order()
 
     def ToTranspose(self):
         """
         This method returns
          2-dimensional cyclic type element of permutation group.
-        It is recursive program.
+
+        The method uses recursion.
         """
         s_data = list(self.data)
         lth = len(s_data)
         if lth == 1:
             return ExPermute(1, [])
         else:
             sol = []
@@ -226,48 +231,53 @@
                     box[j] = '*'
                 if len(p_sol) != 1:
                     sol.append(tuple(p_sol))
         return ExPermute(len(s_data), sol, self.key, flag=True)
 
     def sgn(self):
         """
-        This method returns sign for permutation element.
+        This method returns sign.
+        
+        If self is even permutation, that is, self can be written as a composition
+        of an even number of transpositions, it returns 1. Otherwise,that is, for odd
+        permutation, it returns -1.
         """
         return self.ToCyclic().sgn()
 
     def types(self):
         """
         This method returns 'type' defined by each cyclic element length.
         """
         c_data = self.ToCyclic().data
         sol = [len(c_data[i]) for i in range(len(c_data))]
         sol.sort()
-        return repr(sol) + ' type'
+        return sol
 
     def ToMatrix(self):
         """
-        This method returns permutation matrix
+        This method returns the permutation matrix.
         """
         lth = len(self.data)
         A = matrix.SquareMatrix(lth)
         for j in range(lth):
             A[j+1, self.data[j]] = 1
         return A
 
     def permute(self, lists):
         """
-        permute list following with self permutation
-        Warning: this permutation is independent on key (except dict type)
+        permute list following with self permutation.
+
+        Warning: The method do not check the compatibility of `lists` and self.key (except dict type).
         """
         if len(lists) != len(self.data):
-            raise TypeError, "invalid data size"
+            raise TypeError("The length of `lists` should be equal to that of self.key.")
         if isinstance(lists, dict):
             sol = {}
             key = self.key
-            for x in lists.keys():
+            for x in list(lists.keys()):
                 sol[key[self.data[key.index(x)] - 1]] = lists[x]
         elif isinstance(lists, (list, tuple)):
             sol = [0] * len(lists)
             for i in range(len(lists)):
                 sol[self.data[i] - 1] = lists[i]
         return sol
 
@@ -298,87 +308,89 @@
     This is a class for cyclic type element of permutation group.
     Example, (5, [(1, 2), (3, 4)])
     This means (1, 2)(3, 4)=[2, 1, 4, 3, 5]
     """
 
     def __init__(self, dim, value, key=None, flag=False):
         if not (rational.isIntegerObject(dim) and isinstance(value, list)):
-            raise TypeError("This isn't cyclic form")
+            raise TypeError("cannot convert ExPermute. `dim` should be an integer and `value` should be a list.")
         self.dim = dim
         data = value
         self.data = []
         if key == 0:
-            self.key = range(dim)
+            self.key = list(range(dim))
             for x in data:
                 ele = [ y + 1 for y in x ]
                 self.data.append(tuple(ele))
         elif key:
             if isinstance(key, (list, tuple)):
                 self.key = list(key)
                 if dim != len(key):
-                    raise TypeError("Length error")
+                    raise TypeError("cannot convert ExPermute. The length of `key` should be equal to dim.")
             else:
-                raise TypeError("Input sequence type")
+                raise TypeError("cannot convert ExPermute. `key` should be a list or a tuple.")
             key = self.key
             if flag:
                 self.data = data
             else:
                 for x in data:
                     ele = [key.index(x[i]) + 1 for i in range(len(x))]
                     self.data.append(tuple(ele))
         else:
             self.data = data
-            self.key = range(1, dim + 1)
+            self.key = list(range(1, dim + 1))
         data = self.data
         for x in data:
             if not isinstance(x, tuple):
-                raise TypeError("This isn't cyclic form")
-            box = range(dim)
+                raise TypeError("cannot convert ExPermute. `flag` should be False.")
+            box = list(range(dim))
             for y in x:
                 if (y > dim) or (y <= 0):
-                    raise TypeError("This is out of range")
+                    raise TypeError("cannot convert ExPermute. The map should be onto.")
                 elif box[y-1] == -1:
-                    raise ValueError("This isn't one-to-one")
+                    raise ValueError("cannot convert ExPermute. The map should be one-to-one.")
                 else:
                     box[y-1] = -1
 
     def __getitem__(self, other):
         try:
             idx = self.key.index(other)
         except ValueError:
-            raise ValueError("Input key element")
+            raise ValueError("The indices must be elements of self.key.")
         val = idx + 1
         for i in range(len(self.data) - 1, -1, -1):
             data_i = list(self.data[i])
             try:
                 pla = data_i.index(val)
                 val = data_i[(pla+1) % len(data_i)]
             except ValueError:
                 pass
         return self.key[val - 1]
 
     def __mul__(self, other):
         if self.key != other.key or self.dim != other.dim:
-            raise TypeError("This can't multiply")
+            raise TypeError("cannot multiply an ExPermute by an ExPermute which has a different type.")
         sol = [x for x in self.data] + [x for x in other.data]
         return ExPermute(self.dim, sol, self.key, flag=True)
 
     def __rmul__(self, other):
         return other * self
 
     def __div__(self, other):
         return self * other.inverse()
 
+    __truediv__ = __div__
+
     def __rdiv__(self, other):
         return other * self.inverse()
 
     def __pow__(self, other):
         sol = ExPermute(self.dim, self.data, self.key, flag=True)  # other instance
         if not rational.isIntegerObject(other):
-            raise TypeError("This can't calculate")
+            raise TypeError("cannot pow operation with %s" % other)
         if other > 0:
             for i in range(other - 1):
                 sol = self * sol
         else:
             inv = self.inverse()
             for i in range(abs(other) + 1):
                 sol = inv * sol
@@ -386,22 +398,22 @@
 
     def __call__(self, other):
         return self.permute(other)
 
     def setKey(self, key=None):
         """
         Set other key.
-        this is used when you want to permute different sequence by
-        same permutation.
+        The function may be used if you want to permute a different sequence with 
+        the same permutation.
         """
         if key == 0:
-            self.key = range(self.dim)
+            self.key = list(range(self.dim))
         elif key:
             if len(key) != self.dim:
-                raise TypeError, "Invalid length"
+                raise TypeError("The lenght of `key` should be equal to that of self.key.")
             else:
                 if key[0] in self.key: # key transformation
                     data = list(self.data)
                     keys = self.key
                     sol = []
                     try:
                         for x in data:
@@ -410,19 +422,19 @@
                                 p_ele.append(key.index(keys[x[i]-1])+1)
                             sol.append(tuple(p_ele))
                         self.data = sol
                     except ValueError:
                         pass
                 self.key = key
         else:
-            self.key = range(1, self.dim + 1)
+            self.key = list(range(1, self.dim + 1))
 
     def getValue(self):
         """
-        Get data expressed by key
+        Return value of self.
         """
         out = []
         for x in self.data:
             out.append(tuple([self.key[x[i] - 1] for i in range(len(x))]))
         return out
 
     def inverse(self):
@@ -479,28 +491,33 @@
         This method returns more simple element.
         """
         return self.ToNormal().ToCyclic()
 
     def sgn(self):
         """
         This method returns sign for permutation element.
+
+        If self is even permutation, that is, self can be written as a composition
+        of an even number of transpositions, it returns 1. Otherwise,that is, for odd
+        permutation, it returns -1.
         """
         sol = 1
         for x in self.data:
-            if len(x) % 2 == 0:
+            if len(x) & 1 == 0:
                 sol = -sol
         return sol
 
     def permute(self, lists):
         """
         permute list following with self permutation
-        Warning: this permutation is independent on key (except dict type)
+        
+        Warning: The method do not check the compatibility of `lists` and self.key (except dict type).
         """
         if len(lists) != self.dim:
-            raise TypeError, "invalid data size"
+            raise TypeError("The length of `lists` should be equal to self.dim.")
         if isinstance(lists, dict):
             sol = dict(lists)
             key = self.key
             data = self.data
             for i in range(len(data) - 1, -1, -1):
                 data_i = data[i]
                 first = key[data_i[0] - 1]
@@ -542,22 +559,22 @@
         return str(self.getValue()) + " <" + str(self.key) + ">"
 
 class PermGroup:
     """
     This is a class for permutation group.
     """
     def __init__(self, key):
-        if isinstance(key, (int, long)):
-            self.key = range(1, key + 1)
+        if isinstance(key, int):
+            self.key = list(range(1, key + 1))
         elif isinstance(key, (list, tuple)):
             self.key = list(key)
         elif isinstance(key, dict):
-            self.key = dict.keys()
+            self.key = list(dict.keys())
         else:
-            raise TypeError, "input int or sequence"
+            raise TypeError("cannot convert PermGroup. `key` should be an integer or a list/tuple/dict.")
 
     def __repr__(self):
         return repr(self.key)
 
     def __str__(self):
         return str(self.key)
 
@@ -581,23 +598,23 @@
         createElement(key_element_list) -> Permute(key_element_list, self.key)
         createElement([cyclic_tuple,...]) -> ExPermute(len(self.key), [cyclic_tuple,...], self.key)
         """
         if isinstance(seed, dict):
             if set(self.key) == set(dict.keys()):
                 return Permute(seed)
             else:
-                raise TypeError, "key type is contradict"
+                raise TypeError("`seed`.key should be equal to self.key.")
         elif isinstance(seed, tuple):
             return Permute(list(seed). self.key)
         elif isinstance(seed, list):
             if seed[0] in self.key:
                 return Permute(seed, self.key)
             elif isinstance(seed[0], tuple):
                 return ExPermute(len(self.key), seed, self.key)
-        raise TypeError, "input Normal type or Cyclic type seed."
+        raise TypeError("`seed` should be a dict/tuple/list.")
 
     def identity(self):
         return Permute(self.key, self.key)
 
     def identity_c(self):
         """
         Return identity for cyclic type.
```

### Comparing `NZMATH-1.1.0/nzmath/multiplicative.py` & `nzmath-3.0.0/src/multiplicative.py`

 * *Files identical despite different names*

### Comparing `NZMATH-1.1.0/nzmath/intresidue.py` & `nzmath-3.0.0/src/intresidue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 import logging
 import nzmath.gcd as gcd
 import nzmath.rational as rational
 import nzmath.ring as ring
 import nzmath.prime as prime
 
 
@@ -17,15 +17,15 @@
         ring.CommutativeRingElement.__init__(self)
         if modulus == 0:
             raise ValueError("modulus can not be zero")
         elif modulus < 0:
             modulus = -modulus
         self.m = modulus
 
-        if isinstance(representative, (int, long)):
+        if isinstance(representative, int):
             self.n = representative % self.m
         elif all(hasattr(representative, attr) for attr in ("m", "n")):
             assert representative.m == modulus
             self.n = representative.n
         elif isinstance(representative, rational.Rational):
             t = IntegerResidueClass(representative.denominator, self.m).inverse().getResidue()
             self.n = representative.numerator * t % self.m
@@ -43,40 +43,40 @@
                 return IntegerResidueClass(self.n * other.n, other.m)
             elif other.m % self.m == 0:
                 return IntegerResidueClass(self.n * other.n, self.m)
             else:
                 raise ValueError("incompatible modulus: %d and %d" % (self.m, other.m))
         try:
             return self.mul_module_action(other)
-        except TypeError, e:
+        except TypeError as e:
             #trial may fail with TypeError.
             #_log.debug("no action for %s * %s" % (str(self), str(other)))
             pass
-        except AttributeError, e:
+        except AttributeError as e:
             #trial may fail with AttributeError because other may lack ring.
             #_log.debug("no action for %s * %s" % (str(self), str(other)))
             pass
-        except RuntimeError, e:
+        except RuntimeError as e:
             # maximum recursion depth may exceed
             #_log.debug("recursion limit for %s * %s" % (str(self), str(other)))
             pass
         return NotImplemented
 
     def __rmul__(self, other):
         try:
             return self.mul_module_action(other)
-        except TypeError, e:
+        except TypeError as e:
             #trial may fail with TypeError.
             #_log.debug("no action for %s * %s" % (str(other), str(self)))
             pass
-        except AttributeError, e:
+        except AttributeError as e:
             #trial may fail with AttributeError because other may lack ring.
             #_log.debug("no action for %s * %s" % (str(other), str(self)))
             pass
-        except RuntimeError, e:
+        except RuntimeError as e:
             # maximum recursion depth may exceed
             #_log.debug("recursion limit for %s * %s" % (str(other), str(self)))
             pass
         return NotImplemented
 
     def __div__(self, other):
         try:
@@ -154,15 +154,15 @@
 
     def __neg__(self):
         return self.__class__(-self.n, self.m)
 
     def __pos__(self):
         return self.__class__(+self.n, self.m)
 
-    def __nonzero__(self):
+    def __bool__(self):
         return bool(self.n)
 
     def __eq__(self, other):
         if not other and self.n == 0:
             return True
         if isinstance(other, IntegerResidueClass):
             if other.m == self.m and other.n == self.n:
@@ -203,15 +203,15 @@
 
     def minimumAbsolute(self):
         """
         Return the minimum absolute representative integer of the
         residue class.
         """
         result = self.n % self.m
-        if result > self.m // 2:
+        if result > (self.m >> 1):
             result -= self.m
         return rational.Integer(result)
 
     def getRing(self):
         return IntegerResidueClassRing.getInstance(self.m)
```

### Comparing `NZMATH-1.1.0/nzmath/imaginary.py` & `nzmath-3.0.0/src/imaginary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import division
+
 # standard modules
 import itertools
 # NZMATH modules
 import nzmath.real as real
 import nzmath.rational as rational
 import nzmath.ring as ring
 
@@ -127,14 +127,17 @@
             return self.real == other.real and self.imag == other.imag
         except AttributeError:
             if other in real.theRealField:
                 return self.imag == 0 and self.real == other
             else:
                 return NotImplemented
 
+    def __hash__(self):
+        return hash(self.real**2 + self.imag**2)
+
     def __ne__(self, other):
         try:
             return self.real != other.real or self.imag != other.imag
         except AttributeError:
             if other in real.theRealField:
                 return self.imag != 0 or self.real != other
             else:
@@ -151,15 +154,15 @@
         if self.imag == 0:
             return +self.real
         return self.__class__(+self.real, +self.imag)
 
     def __neg__(self):
         return self.__class__(-self.real, -self.imag)
 
-    def __nonzero__(self):
+    def __bool__(self):
         return bool(self.real or self.imag)
 
     def __repr__(self):
         return "Complex(" + repr(self.real) + ", " + repr(self.imag) + ")"
 
     def __str__(self):
         return str(self.real) + " + " + str(self.imag) + "j"
```

### Comparing `NZMATH-1.1.0/nzmath/round2.py` & `nzmath-3.0.0/src/round2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The method is for obtaining the maximal order of a number field from a
 subring generated by a root of a defining polynomial of the field.
 
 - H.Cohen CCANT Algorithm 6.1.8
 - Kida Y. LN Chapter 3
 """
 
-from __future__ import division
+
 import logging
 import nzmath.arith1 as arith1
 import nzmath.finitefield as finitefield
 import nzmath.factor.misc as factor_misc
 import nzmath.gcd as gcd
 import nzmath.intresidue as intresidue
 import nzmath.matrix as matrix
@@ -71,27 +71,27 @@
             if e > 1:
                 squareness, oddity = divmod(e, 2)
                 squarefactors.append((p, squareness))
                 if oddity:
                     fund_disc *= p
             else:
                 fund_disc *= p
-    if fund_disc % 4 == 1:
-        if v2 % 2:
+    if fund_disc & 3 == 1:
+        if v2 & 1:
             squareness, oddity = divmod(v2, 2)
             squarefactors.append((2, squareness))
             if oddity:
                 fund_disc *= 2
         else:
-            squarefactors.append((2, v2 // 2))
-    else: # fund_disc % 4 == 3
+            squarefactors.append((2, v2 >> 1))
+    else: # fund_disc & 3 == 3
         assert v2 >= 2
         fund_disc *= 4
         if v2 > 2:
-            squarefactors.append((2, (v2 - 2) // 2))
+            squarefactors.append((2, (v2 - 2) >> 1))
     return squarefactors
 
 def _p_maximal(p, e, minpoly_coeff):
     """
     Return p-maximal basis with some related informations.
 
     The arguments:
@@ -235,15 +235,15 @@
 
 def _null_linear_combination(zeta, alpha, j, p, theminpoly):
     """
     Return linear combination coefficients of tau_i = z_i * alpha[j],
     which is congruent to 0 modulo theminpoly and pIp.
 
     alpha is a module.
-    
+
     zeta_{j+1} = {z in zeta_j | z * alpha[j] (mod theminpoly) = 0 (mod pIp)}
     """
     n = theminpoly.degree()
     l = len(zeta)
     assert n == len(alpha.basis)
     alpha_basis = [tuple(b) for b in alpha.get_rationals()]
     alpha_mat = matrix.createMatrix(n, alpha_basis, coeff_ring=Q)
@@ -347,24 +347,24 @@
             # expecting Z/(p^2 Z)
             result = finitefield.FinitePrimeFieldElement(elem.n, p).n
         else:
             # expecting Z or Q
             result = finitefield.FinitePrimeFieldElement(elem, p).n
     else:
         result = elem.n
-    if result > p // 2: # minimum absolute
+    if result > (p >> 1): # minimum absolute
         result -= p
     return result
 
 def _normalize_int(elem):
     """
     Return integer object, which is equal to given elem, whose type is
     either integer or rational number.
     """
-    if isinstance(elem, (int, long)):
+    if isinstance(elem, int):
         return elem
     elif elem.denominator == 1:
         return elem.numerator
     else:
         raise ValueError("non integer: %s" % str(elem))
 
 def _default_omega(degree):
```

### Comparing `NZMATH-1.1.0/nzmath/prime_decomp.py` & `nzmath-3.0.0/src/prime_decomp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-prime ideal decomposion over an (absolute) number field
+prime ideal decomposition over an (absolute) number field
 """
 
 import nzmath.arith1 as arith1
 import nzmath.rational as rational
 import nzmath.matrix as matrix
 import nzmath.vector as vector
 import nzmath.algfield as algfield
@@ -154,15 +154,15 @@
     # if r > m, raise NoInverseImage error
     X = matrix.Subspace.fromMatrix(other.inverseImage(self_new))
     B = X.supplementBasis()
     other_self = other * B # first r columns are self, others are supplement
     other_self.toFieldMatrix()
 
     gamma_part = other_self.subMatrix(
-        range(1, n + 1), range(r + 1, m + 1))
+        list(range(1, n + 1)), list(range(r + 1, m + 1)))
     omega_gamma = other_self.inverseImage(_matrix_mul_by_base_mul(
         matrix.unitMatrix(n, F_p), gamma_part, base_multiply))
     vect_list = []
     for k in range(1, n + 1):
         vect = vector.Vector([F_p.zero] * ((m - r) ** 2))
         for i in range(1, m - r + 1):
             for j in range(1, m - r + 1):
@@ -190,19 +190,19 @@
         raise ValueError
     H_add_one.extendColumn(vector.Vector([F_p.one] + [F_p.zero] * (n - 1)))
     H_add_one.toSubspace(True)
     full_base = H_add_one.supplementBasis()
     full_base.toFieldMatrix()
     # step 9
     A = full_base.subMatrix(
-        range(1, n + 1), range(r + 1, n + 1))
+        list(range(1, n + 1)), list(range(r + 1, n + 1)))
     gamma_mul = full_base.inverseImage(
         _matrix_mul_by_base_mul(A, A, base_multiply))
     gamma_mul = gamma_mul.subMatrix(
-        range(r + 1, n + 1), range(1, gamma_mul.column + 1))
+        list(range(r + 1, n + 1)), list(range(1, gamma_mul.column + 1)))
     return A, gamma_mul
 
 def _check_H(p, H, field, gamma_mul):
     """
     If H express the prime ideal, return (H, f),
     where f: residual degree.
     Else return some column of M_1 (not (1,0,..,0)^t).
@@ -241,15 +241,15 @@
     # assume that first basis of the integral basis equals 1
     int_basis = field.integer_ring()
     
     # step 1
     n = field.degree
     Z = rational.theIntegerRing
     beta = (p * matrix.unitMatrix(n, Z).subMatrix(
-        range(1, n + 1), range(2, n + 1))).copy()
+        list(range(1, n + 1)), list(range(2, n + 1)))).copy()
     beta.extendColumn(hnf)
     m = beta.column
     # step 2
     R = 0
     P_norm = p ** f
     while True:
         R += 1
```

### Comparing `NZMATH-1.1.0/nzmath/plugin/math/_mpmath.py` & `nzmath-3.0.0/src/plugin/math/_mpmath.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     Return 1 if testee is a real number, 0 if complex.
     If testee is not a complex number, raise an exception.
     """
     try:
         COMPLEXTYPE(testee)
     except TypeError:
-	# not a complex number
+        # not a complex number
         raise
     try:
         FLOATTYPE(testee)
         return 1
     except TypeError:
         return 0
```

### Comparing `NZMATH-1.1.0/nzmath/plugin/math/default.py` & `nzmath-3.0.0/src/plugin/math/default.py`

 * *Files identical despite different names*

### Comparing `NZMATH-1.1.0/nzmath/plugin/math/__init__.py` & `nzmath-3.0.0/src/plugin/math/__init__.py`

 * *Files identical despite different names*

### Comparing `NZMATH-1.1.0/nzmath/__init__.py` & `nzmath-3.0.0/src/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 NZMATH is a Python based number theory oriented calculation system.
 It is developed at Tokyo Metropolitan University.
 
 NZMATH is distributed under the BSD license.  See LICENSE.txt for
 detail.
 
-Copyright (c) 2003-2010, NZMATH development group, all right reserved.
+Copyright (c) 2003-2022, NZMATH development group, all right reserved.
 """
 
 __all__ = [
     "algfield",
     "arith1",
     "arygcd",
     "bigrandom",
@@ -37,7 +37,9 @@
     "rational",
     "real",
     "ring",
     "round2",
     "squarefree",
     "vector"
     ]
+
+__all__.append("all")
```

### Comparing `NZMATH-1.1.0/nzmath/plugins.py` & `nzmath-3.0.0/src/plugins.py`

 * *Files identical despite different names*

### Comparing `NZMATH-1.1.0/README.txt` & `nzmath-3.0.0/README.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-NZMATH 1.1.0
-=============
+NZMATH 3.0.0 (Python 3 calculator on number theory)
+===================================================
 
 Introduction
 ------------
 
 NZMATH is a Python based number theory oriented calculation system.
-The centre of development in origin is Tokyo Metropolitan University.
-Today it is developed at SourceForge.net. 
+Its development started at Nakamula laboratory, Tokyo Metropolitan
+University.  Today it is developed at SourceForge.net .
 
-This version 1.1.0 contains several new features, bug fixes.
+This version 3.0.0 is based on Python 3, while former versions are all
+based on Python 2.  Most features are equal to those of version 1.2.0.
 The API can still be changed with versions.
 
 Installation
 ------------
 
-To install NZMATH on your computer, you must have Python 2.5 or
-better.  If you don't have a copy of Python, please install it first.
-Python is available from http://www.python.org/ .
+To install NZMATH on your computer, you must have Python 3.8 or later.
+If you don't have a copy of Python, please install it first.
+Python is available from https://www.python.org/ .
 
-The next step is to expand the NZMATH-1.1.0.tar.gz.  The way to do it
+The next step is to expand the NZMATH-3.0.0.tar.gz.  The way to do it
 depends on your operating system.  On the systems with recent GNU tar,
 you can do it with a single command::
 
- % tar xf NZMATH-1.1.0.tar.gz
+ % tar xf NZMATH-3.0.0.tar.gz
 
 where, % is the command line prompt.  Or with standard tar, you can do
 it as::
 
- % gzip -cd NZMATH-1.1.0.tar.gz | tar xf -
+ % gzip -cd NZMATH-3.0.0.tar.gz | tar xf -
 
-Then, you have a child directory named NZMATH-1.1.0.
+Then, you have a child directory named NZMATH-3.0.0.
 
 The third step is the last step, to install NZMATH to the standard
-python path. Usually, this means to write files to somewhere under
+python path.  Usually, this means to write files to somewhere under
 /usr/lib or /usr/local/lib, and thus you have to have appropriate
 write permission.  Typically, do as the following::
 
- % cd NZMATH-1.1.0
+ % cd NZMATH-3.0.0
  % su
  # python setup.py install
 
-
 Usage
 -----
 
 NZMATH is provided as a Python library package named 'nzmath', so
 please use it as a usual package.  For more information please refer
 Tutorial_.
 
 .. _Tutorial: tutorial.html
 
 Feedback
 --------
 
 Your feedbacks are always welcomed.  Please consider to join the
-mailing list nzmath-user@tnt.math.se.tmu.ac.jp.  You can join the
-list with writing a mail containing a line of "subscribe" in the body
-to nzmath-user-request@tnt.math.se.tmu.ac.jp.  *Be careful* not to
-send it to nzmath-user.
-
+mailing list nzmath-user@lists.sourceforge.net .  You can join the list
+by visiting the web page
+https://lists.sourceforge.net/lists/listinfo/nzmath-user .
 
 Copyright
 ---------
-NZMATH is distributed under the BSD license.  See LICENSE.txt_ for
-detail.
+
+NZMATH is distributed under the BSD license.  Please read LICENSE.txt_
+in the distribution tar ball for detail.
 
 .. _LICENSE.txt: LICENSE.txt
 
-Copyright (c) 2003-2011, NZMATH development group, all right reserved.
+
+AddressObject
```

