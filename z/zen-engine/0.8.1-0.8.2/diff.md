# Comparing `tmp/zen_engine-0.8.1.tar.gz` & `tmp/zen_engine-0.8.2.tar.gz`

## Comparing `zen_engine-0.8.1.tar` & `zen_engine-0.8.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.1/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    19250 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6816 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      783 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6339 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     4010 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     5318 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4286 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    14053 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2604 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9905 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    51034 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    23163 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.1/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123      972 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     5478 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3160 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.1/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-07-20 20:44:12.000000 zen_engine-0.8.1/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-07-20 20:44:12.000000 zen_engine-0.8.1/.gitignore
--rw-r--r--   0     1001      123     1057 2023-07-20 20:44:12.000000 zen_engine-0.8.1/LICENSE
--rw-r--r--   0     1001      123     5965 2023-07-20 20:44:12.000000 zen_engine-0.8.1/README.md
--rw-r--r--   0     1001      123     1578 2023-07-20 20:44:12.000000 zen_engine-0.8.1/index.py
--rw-r--r--   0     1001      123      966 2023-07-20 20:44:12.000000 zen_engine-0.8.1/pyproject.toml
--rw-r--r--   0     1001      123     1429 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/decision.rs
--rw-r--r--   0     1001      123     3012 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/value.rs
--rw-r--r--   0     1001      123    48279 2023-07-20 20:44:19.000000 zen_engine-0.8.1/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.2/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    19250 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6816 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      783 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6339 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     4010 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     5318 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4286 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    14053 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2604 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9905 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    51034 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    23163 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9097 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5185 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.2/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123     2222 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     5632 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3160 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.2/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-07-27 20:02:57.000000 zen_engine-0.8.2/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-07-27 20:02:57.000000 zen_engine-0.8.2/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-07-27 20:02:57.000000 zen_engine-0.8.2/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-07-27 20:02:57.000000 zen_engine-0.8.2/README.md
+-rw-r--r--   0     1001      123     1578 2023-07-27 20:02:57.000000 zen_engine-0.8.2/index.py
+-rw-r--r--   0     1001      123      966 2023-07-27 20:02:57.000000 zen_engine-0.8.2/pyproject.toml
+-rw-r--r--   0     1001      123     1517 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/decision.rs
+-rw-r--r--   0     1001      123     3100 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/value.rs
+-rw-r--r--   0     1001      123    48279 2023-07-27 20:03:04.000000 zen_engine-0.8.2/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.2/PKG-INFO
```

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.8.2/local_dependencies/zen-expression/Cargo.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/README.md` & `zen_engine-0.8.2/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/src/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/tests/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.8.2/local_dependencies/zen-expression/tests/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.8.2/local_dependencies/zen-engine/Cargo.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/README.md` & `zen_engine-0.8.2/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,19 @@
         let rule_id = match rule.get("_id") {
             Some(rid) => rid.clone(),
             None => "".to_string(),
         };
 
         let mut expressions: HashMap<String, String> = Default::default();
         let mut reference_map: HashMap<String, Value> = Default::default();
+
         expressions.insert("_id".to_string(), rule_id.clone());
+        if let Some(description) = rule.get("_description") {
+            expressions.insert("_description".to_string(), description.clone());
+        }
 
         for input in &content.inputs {
             let rule_value = rule.get(input.id.as_str())?;
             let mut input_identifier = input.id.clone();
             if let Some(input_field) = &input.field {
                 input_identifier = format!("{input_field}[{input_identifier}]");
             }
```

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.8.2/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/.gitignore` & `zen_engine-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/LICENSE` & `zen_engine-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/README.md` & `zen_engine-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/index.py` & `zen_engine-0.8.2/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/pyproject.toml` & `zen_engine-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/src/decision.rs` & `zen_engine-0.8.2/src/decision.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::engine::PyZenEvaluateOptions;
 use crate::loader::PyDecisionLoader;
 use crate::value::PyValue;
-use anyhow::Context;
+use anyhow::{anyhow, Context};
 use pyo3::types::PyDict;
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python, ToPyObject};
 use pythonize::depythonize;
 use std::sync::Arc;
 use zen_engine::{Decision, EvaluationOptions};
 
 #[pyclass]
@@ -32,13 +32,15 @@
         let result = futures::executor::block_on(decision.evaluate_with_opts(
             &context,
             EvaluationOptions {
                 max_depth: options.max_depth,
                 trace: options.trace,
             },
         ))
-        .context("Failed to evaluate graph")?;
+        .map_err(|e| {
+            anyhow!(serde_json::to_string(e.as_ref()).unwrap_or_else(|_| e.to_string()))
+        })?;
 
         let value = serde_json::to_value(&result).context("Fail")?;
         Ok(PyValue(value).to_object(py))
     }
 }
```

### Comparing `zen_engine-0.8.1/src/engine.rs` & `zen_engine-0.8.2/src/engine.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::decision::PyZenDecision;
 use crate::loader::PyDecisionLoader;
 use crate::value::PyValue;
-use anyhow::Context;
+use anyhow::{anyhow, Context};
 use pyo3::types::PyDict;
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python, ToPyObject};
 use pythonize::depythonize;
 use serde::{Deserialize, Serialize};
 use std::sync::Arc;
 use zen_engine::model::DecisionContent;
 use zen_engine::{DecisionEngine, EvaluationOptions};
@@ -76,15 +76,17 @@
             key,
             &context,
             EvaluationOptions {
                 max_depth: options.max_depth,
                 trace: options.trace,
             },
         ))
-        .context("Failed to evaluate graph")?;
+        .map_err(|e| {
+            anyhow!(serde_json::to_string(e.as_ref()).unwrap_or_else(|_| e.to_string()))
+        })?;
 
         let value = serde_json::to_value(&result).context("Failed to serialize result")?;
         Ok(PyValue(value).to_object(py))
     }
 
     pub fn create_decision(&self, content: String) -> PyResult<PyZenDecision> {
         let decision_content: DecisionContent =
```

### Comparing `zen_engine-0.8.1/src/loader.rs` & `zen_engine-0.8.2/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/src/value.rs` & `zen_engine-0.8.2/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.1/Cargo.lock` & `zen_engine-0.8.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -92,26 +92,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.71"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -317,26 +317,26 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.17"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b0827b011f6f8ab38590295339817b0d26f344aa4932c3ced71b45b0c54b4a9"
+checksum = "5fd304a20bff958a57f04c4e96a2e7594cc4490a0e809cbd48bb6437edaa452d"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.17"
+version = "4.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9441b403be87be858db6a23edb493e7f694761acdc3343d5a0fcaafd304cbc9e"
+checksum = "01c6a3f08f1fe5662a35cfe393aec09c4df95f60ee93b7556505260f75eee9e1"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -448,15 +448,15 @@
 [[package]]
 name = "ctor"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f34ba9a9bcb8645379e9de8cb3ecfcf4d1c85ba66d90deb3259206fa5aa193b"
 dependencies = [
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -466,17 +466,17 @@
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
@@ -572,15 +572,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -888,17 +888,17 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -979,15 +979,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
@@ -1149,17 +1149,17 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1380,17 +1380,17 @@
 name = "semver"
 version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.173"
+version = "1.0.177"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e91f70896d6720bc714a4a57d22fc91f1db634680e65c8efe13323f1fa38d53f"
+checksum = "63ba2516aa6bf82e0b19ca8b50019d52df58455d3cf9bdaf6315225fdd0c560a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.12"
@@ -1398,28 +1398,28 @@
 checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.173"
+version = "1.0.177"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6250dde8342e0232232be9ca3db7aa40aceb5a3e5dd9bddbc00d99a007cde49"
+checksum = "401797fe7833d72109fedec6bfcbe67c0eed9b99772f26eb8afd261f0abc6fd3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.103"
+version = "1.0.104"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
+checksum = "076066c5f1078eac5b722a31827a8832fe108bed65dfa75e233c89f8206e976c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1474,17 +1474,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.26"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1497,30 +1497,30 @@
 name = "target-lexicon"
 version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1572,15 +1572,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
@@ -1610,17 +1610,17 @@
 name = "uuid"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
 
 [[package]]
 name = "v8"
-version = "0.74.2"
+version = "0.74.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7568bf38565bd5b350d96abbf3d09417e8c9dd74fbb38860e91b759e46f9009c"
+checksum = "2eedac634b8dd39b889c5b62349cbc55913780226239166435c5cf66771792ea"
 dependencies = [
  "bitflags 1.3.2",
  "fslock",
  "once_cell",
  "which",
 ]
 
@@ -1675,15 +1675,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1697,15 +1697,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -1899,15 +1899,15 @@
  "napi-derive",
  "serde_json",
  "zen-engine",
 ]
 
 [[package]]
 name = "zen-python"
-version = "0.8.1"
+version = "0.8.2"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.8.1/PKG-INFO` & `zen_engine-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.8.1
+Version: 0.8.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

