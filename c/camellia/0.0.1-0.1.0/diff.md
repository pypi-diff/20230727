# Comparing `tmp/camellia-0.0.1.tar.gz` & `tmp/camellia-0.1.0.tar.gz`

## Comparing `camellia-0.0.1.tar` & `camellia-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 camellia-0.0.1/src/camellia/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 camellia-0.0.1/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 camellia-0.0.1/LICENSE
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 camellia-0.0.1/README.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 camellia-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 camellia-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/__init__.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/block.py
+-rw-r--r--   0        0        0    12011 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/bundle.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/exception.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/instance.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/module.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 camellia-0.1.0/camellia/verilog/rawcode.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 camellia-0.1.0/tests/hello.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 camellia-0.1.0/tests/test_block.py
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 camellia-0.1.0/tests/test_bundle.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 camellia-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 camellia-0.1.0/LICENSE
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 camellia-0.1.0/README.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 camellia-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 camellia-0.1.0/PKG-INFO
```

### Comparing `camellia-0.0.1/LICENSE` & `camellia-0.1.0/LICENSE`

 * *Files identical despite different names*

