# Comparing `tmp/smartnoise-sql-1.0.0.tar.gz` & `tmp/smartnoise-sql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartnoise-sql-1.0.0.tar", max compression
+gzip compressed data, was "smartnoise-sql-1.0.1.tar", max compression
```

## Comparing `smartnoise-sql-1.0.0.tar` & `smartnoise-sql-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     8241 2023-02-18 22:13:33.740254 smartnoise-sql-1.0.0/README.md
--rw-r--r--   0        0        0      638 2023-04-26 04:03:19.514431 smartnoise-sql-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      182 2023-02-18 22:13:33.767421 smartnoise-sql-1.0.0/snsql/__init__.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.767476 smartnoise-sql-1.0.0/snsql/_ast/__init__.py
--rw-r--r--   0        0        0    21496 2023-04-26 04:00:06.105916 smartnoise-sql-1.0.0/snsql/_ast/ast.py
--rw-r--r--   0        0        0     2878 2023-02-18 22:13:33.767948 smartnoise-sql-1.0.0/snsql/_ast/expression.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.768000 smartnoise-sql-1.0.0/snsql/_ast/expressions/__init__.py
--rw-r--r--   0        0        0     4485 2023-04-13 02:01:02.698944 smartnoise-sql-1.0.0/snsql/_ast/expressions/date.py
--rw-r--r--   0        0        0    12150 2023-02-18 22:13:33.768330 smartnoise-sql-1.0.0/snsql/_ast/expressions/logical.py
--rw-r--r--   0        0        0     7007 2023-02-18 22:13:33.768402 smartnoise-sql-1.0.0/snsql/_ast/expressions/numeric.py
--rw-r--r--   0        0        0     6510 2023-04-17 21:31:42.310775 smartnoise-sql-1.0.0/snsql/_ast/expressions/sql.py
--rw-r--r--   0        0        0     5258 2023-02-18 22:13:33.768711 smartnoise-sql-1.0.0/snsql/_ast/expressions/string.py
--rw-r--r--   0        0        0     1613 2023-02-18 22:13:33.768761 smartnoise-sql-1.0.0/snsql/_ast/expressions/types.py
--rw-r--r--   0        0        0    13833 2023-02-18 22:13:33.769141 smartnoise-sql-1.0.0/snsql/_ast/tokens.py
--rw-r--r--   0        0        0     5484 2023-02-18 22:13:33.769240 smartnoise-sql-1.0.0/snsql/_ast/validate.py
--rw-r--r--   0        0        0     2400 2023-02-18 22:13:33.769301 smartnoise-sql-1.0.0/snsql/connect.py
--rw-r--r--   0        0        0    20665 2023-04-23 02:41:53.046121 smartnoise-sql-1.0.0/snsql/metadata.py
--rw-r--r--   0        0        0       48 2023-02-18 22:13:33.769924 smartnoise-sql-1.0.0/snsql/reader/__init__.py
--rw-r--r--   0        0        0     2096 2023-02-18 22:13:33.769990 smartnoise-sql-1.0.0/snsql/reader/base.py
--rw-r--r--   0        0        0       41 2023-02-18 22:13:33.770057 smartnoise-sql-1.0.0/snsql/sql/__init__.py
--rw-r--r--   0        0        0      251 2023-02-18 22:13:33.770458 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/__init__.py
--rw-r--r--   0        0        0     3487 2023-04-12 02:24:35.798160 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/approx_bounds.py
--rw-r--r--   0        0        0     2990 2023-02-18 22:13:33.771151 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/base.py
--rw-r--r--   0        0        0     3495 2023-02-18 22:13:33.771319 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_gaussian.py
--rw-r--r--   0        0        0     3106 2023-02-18 22:13:33.771572 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_laplace.py
--rw-r--r--   0        0        0     2921 2023-02-18 22:13:33.771721 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/laplace.py
--rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.771936 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/normal.py
--rw-r--r--   0        0        0      328 2023-02-18 22:13:33.771985 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/rand.py
--rw-r--r--   0        0        0     3739 2023-02-18 22:13:33.772068 smartnoise-sql-1.0.0/snsql/sql/dpsu.py
--rw-r--r--   0        0        0     3026 2023-02-18 22:13:33.772125 smartnoise-sql-1.0.0/snsql/sql/odometer.py
--rw-r--r--   0        0        0    18985 2023-02-18 22:13:33.772385 smartnoise-sql-1.0.0/snsql/sql/parse.py
--rw-r--r--   0        0        0       60 2023-02-18 22:13:33.772479 smartnoise-sql-1.0.0/snsql/sql/parser/.gitignore
--rw-r--r--   0        0        0      679 2023-02-18 22:13:33.773049 smartnoise-sql-1.0.0/snsql/sql/parser/Makefile
--rw-r--r--   0        0        0      441 2023-02-18 22:13:33.773104 smartnoise-sql-1.0.0/snsql/sql/parser/README.md
--rw-r--r--   0        0        0    12171 2023-02-18 22:13:33.773544 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmall.g4
--rw-r--r--   0        0        0     1612 2023-02-18 22:13:33.773610 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallErrorListener.py
--rw-r--r--   0        0        0    71022 2023-02-18 22:13:33.774105 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallLexer.py
--rw-r--r--   0        0        0   275434 2023-02-18 22:13:33.774968 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallParser.py
--rw-r--r--   0        0        0    19760 2023-02-18 22:13:33.775115 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallVisitor.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.775145 smartnoise-sql-1.0.0/snsql/sql/parser/__init__.py
--rw-r--r--   0        0        0     3374 2023-02-18 22:13:33.775515 smartnoise-sql-1.0.0/snsql/sql/privacy.py
--rw-r--r--   0        0        0    35627 2023-04-26 04:00:06.106219 smartnoise-sql-1.0.0/snsql/sql/private_reader.py
--rw-r--r--   0        0        0    15548 2023-04-17 21:31:42.310975 smartnoise-sql-1.0.0/snsql/sql/private_rewriter.py
--rw-r--r--   0        0        0      325 2023-02-18 22:13:33.776273 smartnoise-sql-1.0.0/snsql/sql/reader/__init__.py
--rw-r--r--   0        0        0     9029 2023-02-18 22:13:33.776459 smartnoise-sql-1.0.0/snsql/sql/reader/base.py
--rw-r--r--   0        0        0     3918 2023-02-18 22:13:33.776828 smartnoise-sql-1.0.0/snsql/sql/reader/bigquery.py
--rw-r--r--   0        0        0      465 2023-02-18 22:13:33.777016 smartnoise-sql-1.0.0/snsql/sql/reader/engine.py
--rw-r--r--   0        0        0     2417 2023-02-18 22:13:33.777431 smartnoise-sql-1.0.0/snsql/sql/reader/mysql.py
--rw-r--r--   0        0        0     7024 2023-04-26 04:00:06.106399 smartnoise-sql-1.0.0/snsql/sql/reader/pandas.py
--rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.777743 smartnoise-sql-1.0.0/snsql/sql/reader/postgres.py
--rw-r--r--   0        0        0     2966 2023-02-18 22:13:33.777984 smartnoise-sql-1.0.0/snsql/sql/reader/presto.py
--rw-r--r--   0        0        0     3698 2023-04-26 04:00:06.106547 smartnoise-sql-1.0.0/snsql/sql/reader/probe.py
--rw-r--r--   0        0        0     1902 2023-02-18 22:13:33.778268 smartnoise-sql-1.0.0/snsql/sql/reader/spark.py
--rw-r--r--   0        0        0     4389 2023-02-18 22:13:33.778451 smartnoise-sql-1.0.0/snsql/sql/reader/sql_server.py
--rw-r--r--   0        0        0     2044 2023-02-18 22:13:33.778680 smartnoise-sql-1.0.0/snsql/sql/reader/sqlite.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.778740 smartnoise-sql-1.0.0/snsql/xpath/__init__.py
--rw-r--r--   0        0        0     8951 2023-02-18 22:13:33.778827 smartnoise-sql-1.0.0/snsql/xpath/ast.py
--rw-r--r--   0        0        0     4783 2023-02-18 22:13:33.778888 smartnoise-sql-1.0.0/snsql/xpath/parse.py
--rw-r--r--   0        0        0       57 2023-02-18 22:13:33.778962 smartnoise-sql-1.0.0/snsql/xpath/parser/.gitignore
--rw-r--r--   0        0        0      661 2023-02-18 22:13:33.779272 smartnoise-sql-1.0.0/snsql/xpath/parser/Makefile
--rw-r--r--   0        0        0     2790 2023-02-18 22:13:33.779339 smartnoise-sql-1.0.0/snsql/xpath/parser/XPath.g4
--rw-r--r--   0        0        0     1362 2023-02-18 22:13:33.779393 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathErrorListener.py
--rw-r--r--   0        0        0    14203 2023-02-18 22:13:33.779671 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathLexer.py
--rw-r--r--   0        0        0    53099 2023-02-18 22:13:33.780085 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathParser.py
--rw-r--r--   0        0        0     4070 2023-02-18 22:13:33.780237 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathVisitor.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.780267 smartnoise-sql-1.0.0/snsql/xpath/parser/__init__.py
--rw-r--r--   0        0        0     9417 2023-04-26 04:03:28.741811 smartnoise-sql-1.0.0/setup.py
--rw-r--r--   0        0        0     9134 2023-04-26 04:03:28.742243 smartnoise-sql-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8241 2023-02-18 22:13:33.740254 smartnoise-sql-1.0.1/README.md
+-rw-r--r--   0        0        0      638 2023-07-27 01:25:12.842115 smartnoise-sql-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-02-18 22:13:33.767421 smartnoise-sql-1.0.1/snsql/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.767476 smartnoise-sql-1.0.1/snsql/_ast/__init__.py
+-rw-r--r--   0        0        0    21496 2023-04-26 04:00:06.105916 smartnoise-sql-1.0.1/snsql/_ast/ast.py
+-rw-r--r--   0        0        0     2878 2023-02-18 22:13:33.767948 smartnoise-sql-1.0.1/snsql/_ast/expression.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.768000 smartnoise-sql-1.0.1/snsql/_ast/expressions/__init__.py
+-rw-r--r--   0        0        0     4485 2023-04-13 02:01:02.698944 smartnoise-sql-1.0.1/snsql/_ast/expressions/date.py
+-rw-r--r--   0        0        0    12150 2023-02-18 22:13:33.768330 smartnoise-sql-1.0.1/snsql/_ast/expressions/logical.py
+-rw-r--r--   0        0        0     7007 2023-02-18 22:13:33.768402 smartnoise-sql-1.0.1/snsql/_ast/expressions/numeric.py
+-rw-r--r--   0        0        0     6510 2023-04-17 21:31:42.310775 smartnoise-sql-1.0.1/snsql/_ast/expressions/sql.py
+-rw-r--r--   0        0        0     5258 2023-02-18 22:13:33.768711 smartnoise-sql-1.0.1/snsql/_ast/expressions/string.py
+-rw-r--r--   0        0        0     1613 2023-02-18 22:13:33.768761 smartnoise-sql-1.0.1/snsql/_ast/expressions/types.py
+-rw-r--r--   0        0        0    13833 2023-02-18 22:13:33.769141 smartnoise-sql-1.0.1/snsql/_ast/tokens.py
+-rw-r--r--   0        0        0     5484 2023-02-18 22:13:33.769240 smartnoise-sql-1.0.1/snsql/_ast/validate.py
+-rw-r--r--   0        0        0     2400 2023-02-18 22:13:33.769301 smartnoise-sql-1.0.1/snsql/connect.py
+-rw-r--r--   0        0        0    20665 2023-04-23 02:41:53.046121 smartnoise-sql-1.0.1/snsql/metadata.py
+-rw-r--r--   0        0        0       48 2023-02-18 22:13:33.769924 smartnoise-sql-1.0.1/snsql/reader/__init__.py
+-rw-r--r--   0        0        0     2096 2023-02-18 22:13:33.769990 smartnoise-sql-1.0.1/snsql/reader/base.py
+-rw-r--r--   0        0        0       41 2023-02-18 22:13:33.770057 smartnoise-sql-1.0.1/snsql/sql/__init__.py
+-rw-r--r--   0        0        0      251 2023-02-18 22:13:33.770458 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/__init__.py
+-rw-r--r--   0        0        0     3487 2023-04-12 02:24:35.798160 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/approx_bounds.py
+-rw-r--r--   0        0        0     2990 2023-02-18 22:13:33.771151 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/base.py
+-rw-r--r--   0        0        0     3495 2023-02-18 22:13:33.771319 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/discrete_gaussian.py
+-rw-r--r--   0        0        0     3106 2023-02-18 22:13:33.771572 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/discrete_laplace.py
+-rw-r--r--   0        0        0     2921 2023-02-18 22:13:33.771721 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/laplace.py
+-rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.771936 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/normal.py
+-rw-r--r--   0        0        0      328 2023-02-18 22:13:33.771985 smartnoise-sql-1.0.1/snsql/sql/_mechanisms/rand.py
+-rw-r--r--   0        0        0     3739 2023-02-18 22:13:33.772068 smartnoise-sql-1.0.1/snsql/sql/dpsu.py
+-rw-r--r--   0        0        0     3026 2023-02-18 22:13:33.772125 smartnoise-sql-1.0.1/snsql/sql/odometer.py
+-rw-r--r--   0        0        0    18985 2023-02-18 22:13:33.772385 smartnoise-sql-1.0.1/snsql/sql/parse.py
+-rw-r--r--   0        0        0       60 2023-02-18 22:13:33.772479 smartnoise-sql-1.0.1/snsql/sql/parser/.gitignore
+-rw-r--r--   0        0        0      679 2023-02-18 22:13:33.773049 smartnoise-sql-1.0.1/snsql/sql/parser/Makefile
+-rw-r--r--   0        0        0      441 2023-02-18 22:13:33.773104 smartnoise-sql-1.0.1/snsql/sql/parser/README.md
+-rw-r--r--   0        0        0    12171 2023-02-18 22:13:33.773544 smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmall.g4
+-rw-r--r--   0        0        0     1612 2023-02-18 22:13:33.773610 smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallErrorListener.py
+-rw-r--r--   0        0        0    71022 2023-02-18 22:13:33.774105 smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallLexer.py
+-rw-r--r--   0        0        0   275434 2023-02-18 22:13:33.774968 smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallParser.py
+-rw-r--r--   0        0        0    19760 2023-02-18 22:13:33.775115 smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallVisitor.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.775145 smartnoise-sql-1.0.1/snsql/sql/parser/__init__.py
+-rw-r--r--   0        0        0     3374 2023-02-18 22:13:33.775515 smartnoise-sql-1.0.1/snsql/sql/privacy.py
+-rw-r--r--   0        0        0    35627 2023-04-26 04:00:06.106219 smartnoise-sql-1.0.1/snsql/sql/private_reader.py
+-rw-r--r--   0        0        0    15548 2023-04-17 21:31:42.310975 smartnoise-sql-1.0.1/snsql/sql/private_rewriter.py
+-rw-r--r--   0        0        0      325 2023-02-18 22:13:33.776273 smartnoise-sql-1.0.1/snsql/sql/reader/__init__.py
+-rw-r--r--   0        0        0     9029 2023-02-18 22:13:33.776459 smartnoise-sql-1.0.1/snsql/sql/reader/base.py
+-rw-r--r--   0        0        0     3918 2023-02-18 22:13:33.776828 smartnoise-sql-1.0.1/snsql/sql/reader/bigquery.py
+-rw-r--r--   0        0        0      465 2023-02-18 22:13:33.777016 smartnoise-sql-1.0.1/snsql/sql/reader/engine.py
+-rw-r--r--   0        0        0     2417 2023-02-18 22:13:33.777431 smartnoise-sql-1.0.1/snsql/sql/reader/mysql.py
+-rw-r--r--   0        0        0     7024 2023-04-26 04:00:06.106399 smartnoise-sql-1.0.1/snsql/sql/reader/pandas.py
+-rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.777743 smartnoise-sql-1.0.1/snsql/sql/reader/postgres.py
+-rw-r--r--   0        0        0     2966 2023-02-18 22:13:33.777984 smartnoise-sql-1.0.1/snsql/sql/reader/presto.py
+-rw-r--r--   0        0        0     3698 2023-04-26 04:00:06.106547 smartnoise-sql-1.0.1/snsql/sql/reader/probe.py
+-rw-r--r--   0        0        0     1902 2023-02-18 22:13:33.778268 smartnoise-sql-1.0.1/snsql/sql/reader/spark.py
+-rw-r--r--   0        0        0     4389 2023-02-18 22:13:33.778451 smartnoise-sql-1.0.1/snsql/sql/reader/sql_server.py
+-rw-r--r--   0        0        0     2044 2023-02-18 22:13:33.778680 smartnoise-sql-1.0.1/snsql/sql/reader/sqlite.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.778740 smartnoise-sql-1.0.1/snsql/xpath/__init__.py
+-rw-r--r--   0        0        0     8951 2023-02-18 22:13:33.778827 smartnoise-sql-1.0.1/snsql/xpath/ast.py
+-rw-r--r--   0        0        0     4783 2023-02-18 22:13:33.778888 smartnoise-sql-1.0.1/snsql/xpath/parse.py
+-rw-r--r--   0        0        0       57 2023-02-18 22:13:33.778962 smartnoise-sql-1.0.1/snsql/xpath/parser/.gitignore
+-rw-r--r--   0        0        0      661 2023-02-18 22:13:33.779272 smartnoise-sql-1.0.1/snsql/xpath/parser/Makefile
+-rw-r--r--   0        0        0     2790 2023-02-18 22:13:33.779339 smartnoise-sql-1.0.1/snsql/xpath/parser/XPath.g4
+-rw-r--r--   0        0        0     1362 2023-02-18 22:13:33.779393 smartnoise-sql-1.0.1/snsql/xpath/parser/XPathErrorListener.py
+-rw-r--r--   0        0        0    14203 2023-02-18 22:13:33.779671 smartnoise-sql-1.0.1/snsql/xpath/parser/XPathLexer.py
+-rw-r--r--   0        0        0    53099 2023-02-18 22:13:33.780085 smartnoise-sql-1.0.1/snsql/xpath/parser/XPathParser.py
+-rw-r--r--   0        0        0     4070 2023-02-18 22:13:33.780237 smartnoise-sql-1.0.1/snsql/xpath/parser/XPathVisitor.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.780267 smartnoise-sql-1.0.1/snsql/xpath/parser/__init__.py
+-rw-r--r--   0        0        0     9417 2023-07-27 01:28:24.819586 smartnoise-sql-1.0.1/setup.py
+-rw-r--r--   0        0        0     9134 2023-07-27 01:28:24.820010 smartnoise-sql-1.0.1/PKG-INFO
```

### Comparing `smartnoise-sql-1.0.0/README.md` & `smartnoise-sql-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/pyproject.toml` & `smartnoise-sql-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "smartnoise-sql"
-version = "1.0.0"
+version = "1.0.1"
 description = "Differentially Private SQL Queries"
 authors = ["SmartNoise Team <smartnoise@opendp.org>"]
 license = "MIT"
 packages = [{include="snsql"}]
 homepage = "https://smartnoise.org"
 repository = "https://github.com/opendp/smartnoise-sdk"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
-opendp = "^0.6.0"
+opendp = "^0.7.0"
 antlr4-python3-runtime = "4.9.3"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 graphviz = "^0.17"
 sqlalchemy = "^2.0.0"
 pandas = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/ast.py` & `smartnoise-sql-1.0.1/snsql/_ast/ast.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expression.py` & `smartnoise-sql-1.0.1/snsql/_ast/expression.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/date.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/date.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/logical.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/logical.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/numeric.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/numeric.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/sql.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/sql.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/string.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/string.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/expressions/types.py` & `smartnoise-sql-1.0.1/snsql/_ast/expressions/types.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/tokens.py` & `smartnoise-sql-1.0.1/snsql/_ast/tokens.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/_ast/validate.py` & `smartnoise-sql-1.0.1/snsql/_ast/validate.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/connect.py` & `smartnoise-sql-1.0.1/snsql/connect.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/metadata.py` & `smartnoise-sql-1.0.1/snsql/metadata.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/reader/base.py` & `smartnoise-sql-1.0.1/snsql/reader/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/approx_bounds.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/approx_bounds.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/base.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_gaussian.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_laplace.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/discrete_laplace.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/laplace.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/normal.py` & `smartnoise-sql-1.0.1/snsql/sql/_mechanisms/normal.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/dpsu.py` & `smartnoise-sql-1.0.1/snsql/sql/dpsu.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/odometer.py` & `smartnoise-sql-1.0.1/snsql/sql/odometer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parse.py` & `smartnoise-sql-1.0.1/snsql/sql/parse.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/Makefile` & `smartnoise-sql-1.0.1/snsql/sql/parser/Makefile`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmall.g4` & `smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmall.g4`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallErrorListener.py` & `smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallErrorListener.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallLexer.py` & `smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallLexer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallParser.py` & `smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallParser.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallVisitor.py` & `smartnoise-sql-1.0.1/snsql/sql/parser/SqlSmallVisitor.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/privacy.py` & `smartnoise-sql-1.0.1/snsql/sql/privacy.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/private_reader.py` & `smartnoise-sql-1.0.1/snsql/sql/private_reader.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/private_rewriter.py` & `smartnoise-sql-1.0.1/snsql/sql/private_rewriter.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/base.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/bigquery.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/bigquery.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/mysql.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/mysql.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/pandas.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/pandas.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/postgres.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/postgres.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/presto.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/presto.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/probe.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/probe.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/spark.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/spark.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/sql_server.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/sql_server.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/sql/reader/sqlite.py` & `smartnoise-sql-1.0.1/snsql/sql/reader/sqlite.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/ast.py` & `smartnoise-sql-1.0.1/snsql/xpath/ast.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parse.py` & `smartnoise-sql-1.0.1/snsql/xpath/parse.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/Makefile` & `smartnoise-sql-1.0.1/snsql/xpath/parser/Makefile`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/XPath.g4` & `smartnoise-sql-1.0.1/snsql/xpath/parser/XPath.g4`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathErrorListener.py` & `smartnoise-sql-1.0.1/snsql/xpath/parser/XPathErrorListener.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathLexer.py` & `smartnoise-sql-1.0.1/snsql/xpath/parser/XPathLexer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathParser.py` & `smartnoise-sql-1.0.1/snsql/xpath/parser/XPathParser.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathVisitor.py` & `smartnoise-sql-1.0.1/snsql/xpath/parser/XPathVisitor.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-1.0.0/setup.py` & `smartnoise-sql-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
  'snsql.xpath',
  'snsql.xpath.parser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
+['PyYAML>=6.0.1,<7.0.0',
  'antlr4-python3-runtime==4.9.3',
  'graphviz>=0.17,<0.18',
- 'opendp>=0.6.0,<0.7.0',
+ 'opendp>=0.7.0,<0.8.0',
  'pandas>=2.0.1,<3.0.0',
  'sqlalchemy>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'smartnoise-sql',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Differentially Private SQL Queries',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)\n\n<a href="https://smartnoise.org"><img src="https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg" align="left" height="65" vspace="8" hspace="18"></a>\n\n## SmartNoise SQL\n\nDifferentially private SQL queries.  Tested with:\n* PostgreSQL\n* SQL Server\n* Spark\n* Pandas (SQLite)\n* PrestoDB\n* BigQuery\n\nSmartNoise is intended for scenarios where the analyst is trusted by the data owner.  SmartNoise uses the [OpenDP](https://github.com/opendp/opendp) library of differential privacy algorithms.\n\n## Installation\n\n```\npip install smartnoise-sql\n```\n\n## Querying a Pandas DataFrame\n\nUse the `from_df` method to create a private reader that can issue queries against a pandas dataframe.\n\n```python\nimport snsql\nfrom snsql import Privacy\nimport pandas as pd\nprivacy = Privacy(epsilon=1.0, delta=0.01)\n\ncsv_path = \'PUMS.csv\'\nmeta_path = \'PUMS.yaml\'\n\npums = pd.read_csv(csv_path)\nreader = snsql.from_df(pums, privacy=privacy, metadata=meta_path)\n\nresult = reader.execute(\'SELECT sex, AVG(age) AS age FROM PUMS.PUMS GROUP BY sex\')\n```\n\n## Querying a SQL Database\n\nUse `from_connection` to wrap an existing database connection.\n\n```python\nimport snsql\nfrom snsql import Privacy\nimport psycopg2\n\nprivacy = Privacy(epsilon=1.0, delta=0.01)\nmeta_path = \'PUMS.yaml\'\n\npumsdb = psycopg2.connect(user=\'postgres\', host=\'localhost\', database=\'PUMS\')\nreader = snsql.from_connection(pumsdb, privacy=privacy, metadata=meta_path)\n\nresult = reader.execute(\'SELECT sex, AVG(age) AS age FROM PUMS.PUMS GROUP BY sex\')\n```\n\n## Querying a Spark DataFrame\n\nUse `from_connection` to wrap a spark session.\n\n```python\nimport pyspark\nfrom pyspark.sql import SparkSession\nspark = SparkSession.builder.getOrCreate()\nfrom snsql import *\n\npums = spark.read.load(...)  # load a Spark DataFrame\npums.createOrReplaceTempView("PUMS_large")\n\nmetadata = \'PUMS_large.yaml\'\n\nprivate_reader = from_connection(\n    spark, \n    metadata=metadata, \n    privacy=Privacy(epsilon=3.0, delta=1/1_000_000)\n)\nprivate_reader.reader.compare.search_path = ["PUMS"]\n\n\nres = private_reader.execute(\'SELECT COUNT(*) FROM PUMS_large\')\nres.show()\n```\n\n## Privacy Cost\n\nThe privacy parameters epsilon and delta are passed in to the private connection at instantiation time, and apply to each computed column during the life of the session.  Privacy cost accrues indefinitely as new queries are executed, with the total accumulated privacy cost being available via the `spent` property of the connection\'s `odometer`:\n\n```python\nprivacy = Privacy(epsilon=0.1, delta=10e-7)\n\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nresult = reader.execute(\'SELECT COUNT(*) FROM PUMS.PUMS\')\nprint(reader.odometer.spent)  # approximately (0.1, 10e-7)\n```\n\nThe privacy cost increases with the number of columns:\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nresult = reader.execute(\'SELECT AVG(age), AVG(income) FROM PUMS.PUMS\')\nprint(reader.odometer.spent)  # approximately (0.4, 10e-6)\n```\n\nThe odometer is advanced immediately before the differentially private query result is returned to the caller.  If the caller wishes to estimate the privacy cost of a query without running it, `get_privacy_cost` can be used:\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\ncost = reader.get_privacy_cost(\'SELECT AVG(age), AVG(income) FROM PUMS.PUMS\')\nprint(cost)  # approximately (0.4, 10e-6)\n\nprint(reader.odometer.spent)  # (0.0, 0.0)\n```\n\nNote that the total privacy cost of a session accrues at a slower rate than the sum of the individual query costs obtained by `get_privacy_cost`.  The odometer accrues all invocations of mechanisms for the life of a session, and uses them to compute total spend.\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nquery = \'SELECT COUNT(*) FROM PUMS.PUMS\'\nepsilon_single, _ = reader.get_privacy_cost(query)\nprint(epsilon_single)  # 0.1\n\n# no queries executed yet\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nfor _ in range(100):\n    reader.execute(query)\n\nepsilon_many, _ = reader.odometer.spent\nprint(f\'{epsilon_many} < {epsilon_single * 100}\')\n```\n\n## Histograms\n\nSQL `group by` queries represent histograms binned by grouping key.  Queries over a grouping key with unbounded or non-public dimensions expose privacy risk. For example:\n\n```sql\nSELECT last_name, COUNT(*) FROM Sales GROUP BY last_name\n```\n\nIn the above query, if someone with a distinctive last name is included in the database, that person\'s record might accidentally be revealed, even if the noisy count returns 0 or negative.  To prevent this from happening, the system will automatically censor dimensions which would violate differential privacy.\n\n## Private Synopsis\n\nA private synopsis is a pre-computed set of differentially private aggregates that can be filtered and aggregated in various ways to produce new reports.  Because the private synopsis is differentially private, reports generated from the synopsis do not need to have additional privacy applied, and the synopsis can be distributed without risk of additional privacy loss.  Reports over the synopsis can be generated with non-private SQL, within an Excel Pivot Table, or through other common reporting tools.\n\nYou can see a sample [notebook for creating private synopsis](samples/Synopsis.ipynb) suitable for consumption in Excel or SQL.\n\n## Limitations\n\nYou can think of the data access layer as simple middleware that allows composition of `opendp` computations using the SQL language.  The SQL language provides a limited subset of what can be expressed through the full `opendp` library.  For example, the SQL language does not provide a way to set per-field privacy budget.\n\nBecause we delegate the computation of exact aggregates to the underlying database engines, execution through the SQL layer can be considerably faster, particularly with database engines optimized for precomputed aggregates.  However, this design choice means that analysis graphs composed with SQL language do not access data in the engine on a per-row basis.  Therefore, SQL queries do not currently support algorithms that require per-row access, such as quantile algorithms that use underlying values.  This is a limitation that future releases will relax for database engines that support row-based access, such as Spark.\n\nThe SQL processing layer has limited support for bounding contributions when individuals can appear more than once in the data.  This includes ability to perform reservoir sampling to bound contributions of an individual, and to scale the sensitivity parameter.  These parameters are important when querying reporting tables that might be produced from subqueries and joins, but require caution to use safely.\n\nFor this release, we recommend using the SQL functionality while bounding user contribution to 1 row.  The platform defaults to this option by setting `max_contrib` to 1, and should only be overridden if you know what you are doing.  Future releases will focus on making these options easier for non-experts to use safely.\n\n\n## Communication\n\n- You are encouraged to join us on [GitHub Discussions](https://github.com/opendp/opendp/discussions/categories/smartnoise)\n- Please use [GitHub Issues](https://github.com/opendp/smartnoise-sdk/issues) for bug reports and feature requests.\n- For other requests, including security issues, please contact us at [smartnoise@opendp.org](mailto:smartnoise@opendp.org).\n\n## Releases and Contributing\n\nPlease let us know if you encounter a bug by [creating an issue](https://github.com/opendp/smartnoise-sdk/issues).\n\nWe appreciate all contributions. Please review the [contributors guide](../contributing.rst). We welcome pull requests with bug-fixes without prior discussion.\n\nIf you plan to contribute new features, utility functions or extensions, please first open an issue and discuss the feature with us.\n',
     'author': 'SmartNoise Team',
     'author_email': 'smartnoise@opendp.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://smartnoise.org',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['snsql',
 'snsql._ast', 'snsql._ast.expressions', 'snsql.reader', 'snsql.sql',
 'snsql.sql._mechanisms', 'snsql.sql.parser', 'snsql.sql.reader', 'snsql.xpath',
 'snsql.xpath.parser'] package_data = \ {'': ['*']} install_requires = \
-['PyYAML>=5.4.1,<6.0.0', 'antlr4-python3-runtime==4.9.3',
-'graphviz>=0.17,<0.18', 'opendp>=0.6.0,<0.7.0', 'pandas>=2.0.1,<3.0.0',
+['PyYAML>=6.0.1,<7.0.0', 'antlr4-python3-runtime==4.9.3',
+'graphviz>=0.17,<0.18', 'opendp>=0.7.0,<0.8.0', 'pandas>=2.0.1,<3.0.0',
 'sqlalchemy>=2.0.0,<3.0.0'] setup_kwargs = { 'name': 'smartnoise-sql',
-'version': '1.0.0', 'description': 'Differentially Private SQL Queries',
+'version': '1.0.1', 'description': 'Differentially Private SQL Queries',
 'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://
 img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)\n\n
 [https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/
 Logo%20Mark_grey.svg]\n\n## SmartNoise SQL\n\nDifferentially private SQL
 queries. Tested with:\n* PostgreSQL\n* SQL Server\n* Spark\n* Pandas
 (SQLite)\n* PrestoDB\n* BigQuery\n\nSmartNoise is intended for scenarios where
```

### Comparing `smartnoise-sql-1.0.0/PKG-INFO` & `smartnoise-sql-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: smartnoise-sql
-Version: 1.0.0
+Version: 1.0.1
 Summary: Differentially Private SQL Queries
 Home-page: https://smartnoise.org
 License: MIT
 Author: SmartNoise Team
 Author-email: smartnoise@opendp.org
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: antlr4-python3-runtime (==4.9.3)
 Requires-Dist: graphviz (>=0.17,<0.18)
-Requires-Dist: opendp (>=0.6.0,<0.7.0)
+Requires-Dist: opendp (>=0.7.0,<0.8.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/opendp/smartnoise-sdk
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: smartnoise-sql Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: smartnoise-sql Version: 1.0.1 Summary:
 Differentially Private SQL Queries Home-page: https://smartnoise.org License:
 MIT Author: SmartNoise Team Author-email: smartnoise@opendp.org Requires-
 Python: >=3.7,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: PyYAML (>=5.4.1,<6.0.0) Requires-Dist:
+Language :: Python :: 3.9 Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 antlr4-python3-runtime (==4.9.3) Requires-Dist: graphviz (>=0.17,<0.18)
-Requires-Dist: opendp (>=0.6.0,<0.7.0) Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: opendp (>=0.7.0,<0.8.0) Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0) Project-URL: Repository, https://
 github.com/opendp/smartnoise-sdk Description-Content-Type: text/markdown [!
 [License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-
 3.7%20%7C%203.8-blue)](https://www.python.org/) [https://github.com/opendp/
 smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg] ##
 SmartNoise SQL Differentially private SQL queries. Tested with: * PostgreSQL *
```

