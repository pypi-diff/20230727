# Comparing `tmp/magma-lang-2.2.9.tar.gz` & `tmp/magma-lang-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma-lang-2.2.9.tar", last modified: Mon Mar  7 19:34:19 2022, max compression
+gzip compressed data, was "magma-lang-2.3.0.tar", last modified: Thu Jul 27 20:29:13 2023, max compression
```

## Comparing `magma-lang-2.2.9.tar` & `magma-lang-2.3.0.tar`

### file list

```diff
@@ -1,175 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-03-07 19:26:09.000000 magma-lang-2.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-07 19:34:19.116249 magma-lang-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8418 2022-03-07 19:26:09.000000 magma-lang-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.076248 magma-lang-2.2.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2538 2022-03-07 19:26:09.000000 magma-lang-2.2.9/bin/magma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.092248 magma-lang-2.2.9/magma/
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36614 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ast_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.092248 magma-lang-2.2.9/magma/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/blif.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/check_wiring_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.096248 magma-lang-2.2.9/magma/backend/coreir/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)    22238 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/coreir_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/insert_coreir_wires.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/coreir/insert_wrap_casts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/dot.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/firrtl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.100248 magma-lang-2.2.9/magma/backend/mlir/
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/build_magma_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/comb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/compile_to_mlir.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/graph_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    28234 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/hardware_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/hw.py
--rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/magma_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/magma_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_printer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_to_verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/mlir_to_verilog_main.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/printer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/scoped_name_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/sv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/mlir/translation_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     9056 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/backend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bfloat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bind.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bit_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)    26367 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bits.py
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/bitutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11289 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/braid.py
--rw-r--r--   0 runner    (1001) docker     (121)    32492 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/clock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/clock_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5240 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     8363 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compile_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11644 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/definition_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/digital.py
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/family.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.104248 magma-lang-2.2.9/magma/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/coreir.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/coreir_.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/dummy_verilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/pyverilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/frontend/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/if_def.py
--rw-r--r--   0 runner    (1001) docker     (121)    10060 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/inline_verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)    17236 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ir.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/is_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/is_primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/linking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/math.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/operator_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.104248 magma-lang-2.2.9/magma/passes/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7146 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/clock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/debug_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/drive_undriven.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/find_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/ir.py
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/passes.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/terminate_unused.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/passes/tsort.py
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/placer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/lut.py
--rw-r--r--   0 runner    (1001) docker     (121)     6933 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     7197 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/mux.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/register.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/set_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/primitives/wire.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/protocol_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ref.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/set_name.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/simulator/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11159 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/coreir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21013 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/mdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    13858 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/python_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/simulator/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/smart/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17619 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/smart/smart_bits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.108249 magma-lang-2.2.9/magma/ssa/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ssa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6757 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/ssa/ssa.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/symbol_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/syntax/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10787 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/combinational.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/combinational2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10970 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/inline_combinational.py
--rw-r--r--   0 runner    (1001) docker     (121)    15172 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/sequential2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/syntax/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/inline_yield_from.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/transforms/replace_symbols.py
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14406 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/verilog.py
--rw-r--r--   0 runner    (1001) docker     (121)    14548 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/syntax/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5229 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/t.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.112249 magma-lang-2.2.9/magma/testing/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9924 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    18653 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/magma/types/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/bit_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)    11623 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/ready_valid.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/types/valid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/uniquification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/value_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/view.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/waveform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/wire.py
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-03-07 19:26:09.000000 magma-lang-2.2.9/magma/wire_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:34:19.116249 magma-lang-2.2.9/magma_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-07 19:34:18.000000 magma-lang-2.2.9/magma_lang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-03-07 19:34:19.116249 magma-lang-2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-03-07 19:26:09.000000 magma-lang-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-27 20:21:18.000000 magma-lang-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-27 20:29:13.504423 magma-lang-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-27 20:21:18.000000 magma-lang-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.488422 magma-lang-2.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2538 2023-07-27 20:21:18.000000 magma-lang-2.3.0/bin/magma
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.492423 magma-lang-2.3.0/magma/
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37390 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/ast_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.492423 magma-lang-2.3.0/magma/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/blif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/check_wiring_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.492423 magma-lang-2.3.0/magma/backend/coreir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/coreir_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/coreir_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/coreir_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22466 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/coreir_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/coreir_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/insert_coreir_wires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/coreir/insert_wrap_casts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/firrtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.496423 magma-lang-2.3.0/magma/backend/mlir/
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/build_magma_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/comb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/compile_to_mlir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/compile_to_mlir_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/graph_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52142 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/hardware_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/magma_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/magma_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/mem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/mlir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/mlir_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/mlir_printer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/mlir_to_verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/print_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/printer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/scoped_name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/translation_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/when_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/mlir/xmr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/backend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bfloat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bind2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bit_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28340 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/bitutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/braid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37457 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/clock_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/compile_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/compile_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/definition_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/digital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/find_unconnected_ports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.496423 magma-lang-2.3.0/magma/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/coreir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/coreir_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/dummy_verilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/pyverilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/verilog_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/frontend/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/if_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/inline_verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/inline_verilog2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/inline_verilog_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/is_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/is_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/operator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.496423 magma-lang-2.3.0/magma/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/debug_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/drive_undriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/elaborate_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/elaborate_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/finalize_whens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/instance_callback_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/raise_logs_as_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/terminate_unused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/passes/tsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/placer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/lut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/multiport_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/mux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/set_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/wire.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/primitives/xmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/protocol_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/set_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/simulator/coreir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/simulator/mdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/simulator/python_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/simulator/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/smart/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/smart/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/smart/make_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/smart/smart_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/ssa/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/ssa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/ssa/ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/stubify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/symbol_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/combinational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/combinational2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/inline_combinational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/sequential2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/syntax/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/transforms/inline_yield_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/transforms/replace_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/syntax/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/t.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/types/bit_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/types/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/types/valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/uniquification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/value_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/wire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/wire_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-27 20:21:18.000000 magma-lang-2.3.0/magma/wire_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:29:13.500423 magma-lang-2.3.0/magma_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-27 20:29:13.000000 magma-lang-2.3.0/magma_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-27 20:29:13.000000 magma-lang-2.3.0/magma_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:29:13.000000 magma-lang-2.3.0/magma_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 20:29:13.000000 magma-lang-2.3.0/magma_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 20:29:13.000000 magma-lang-2.3.0/magma_lang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 20:29:13.504423 magma-lang-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 20:21:18.000000 magma-lang-2.3.0/setup.py
```

### Comparing `magma-lang-2.2.9/LICENSE.txt` & `magma-lang-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/PKG-INFO` & `magma-lang-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: magma-lang
-Version: 2.2.9
+Version: 2.3.0
 Summary: An embedded DSL for constructing hardware circuits
 Home-page: https://github.com/phanrahan/magma
 Maintainer: Lenny Truong
 Maintainer-email: lenny@cs.stanford.edu
 License: MIT
 Description: # Magma
         [![Documentation Status](https://readthedocs.org/projects/magma/badge/?version=latest)](https://magma.readthedocs.io/en/latest/?badge=latest)
         [![Linux Test](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml/badge.svg)](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml)
         [![codecov](https://codecov.io/gh/phanrahan/magma/branch/master/graph/badge.svg)](https://codecov.io/gh/phanrahan/magma)
         [![Join the chat at https://gitter.im/Magma-HDL/community](https://badges.gitter.im/Magma-HDL/community.svg)](https://gitter.im/Magma-HDL/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         
-        [CHANGELOG](https://github.com/phanrahan/magma/blob/master/CHANGELOG.md)
-        
         [CHEAT SHEET](https://github.com/phanrahan/magma/blob/master/docs/cheat_sheet.md)
         
         Magma is a hardware design language embedded in python.
         
         The central abstraction in Magma is a circuit.
         A circuit is a set of functional units that are wired together.
         Magma circuits are analagous to verilog modules.
@@ -56,15 +54,15 @@
         [magmathon](https://github.com/phanrahan/magmathon) repository contains
         a set of [Jupyter
         Notebooks](https://github.com/phanrahan/magmathon/tree/master/notebooks/tutorial)
         that introduce the system. There's also
         [magma_examples](https://github.com/leonardt/magma_examples) and
         [magma_tutorial](https://github.com/leonardt/magma_tutorial) which contain a
         set of basic circuits and tests, providing an example templates for a magma
-        projects.  Finally there is [magma_riscv_mini](https://github.com/leonardt/magma_riscv_mini)
+        projects.  Finally there is [magma_riscv_mini](./examples/riscv_mini)
         which provides an example of a simple RISCV processor. Please also refer to the
         [documentation](http://magma.readthedocs.io/).
         
         The design of Magma was heavily influenced by 
         [Chisel](https://chisel.eecs.berkeley.edu/),
         so Magma should be easy to learn if you know Chisel.
         Some examples from the Chisel tutorial have been ported to
```

### Comparing `magma-lang-2.2.9/README.md` & `magma-lang-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Magma
 [![Documentation Status](https://readthedocs.org/projects/magma/badge/?version=latest)](https://magma.readthedocs.io/en/latest/?badge=latest)
 [![Linux Test](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml/badge.svg)](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml)
 [![codecov](https://codecov.io/gh/phanrahan/magma/branch/master/graph/badge.svg)](https://codecov.io/gh/phanrahan/magma)
 [![Join the chat at https://gitter.im/Magma-HDL/community](https://badges.gitter.im/Magma-HDL/community.svg)](https://gitter.im/Magma-HDL/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
-[CHANGELOG](https://github.com/phanrahan/magma/blob/master/CHANGELOG.md)
-
 [CHEAT SHEET](https://github.com/phanrahan/magma/blob/master/docs/cheat_sheet.md)
 
 Magma is a hardware design language embedded in python.
 
 The central abstraction in Magma is a circuit.
 A circuit is a set of functional units that are wired together.
 Magma circuits are analagous to verilog modules.
@@ -48,15 +46,15 @@
 [magmathon](https://github.com/phanrahan/magmathon) repository contains
 a set of [Jupyter
 Notebooks](https://github.com/phanrahan/magmathon/tree/master/notebooks/tutorial)
 that introduce the system. There's also
 [magma_examples](https://github.com/leonardt/magma_examples) and
 [magma_tutorial](https://github.com/leonardt/magma_tutorial) which contain a
 set of basic circuits and tests, providing an example templates for a magma
-projects.  Finally there is [magma_riscv_mini](https://github.com/leonardt/magma_riscv_mini)
+projects.  Finally there is [magma_riscv_mini](./examples/riscv_mini)
 which provides an example of a simple RISCV processor. Please also refer to the
 [documentation](http://magma.readthedocs.io/).
 
 The design of Magma was heavily influenced by 
 [Chisel](https://chisel.eecs.berkeley.edu/),
 so Magma should be easy to learn if you know Chisel.
 Some examples from the Chisel tutorial have been ported to
```

### Comparing `magma-lang-2.2.9/bin/magma` & `magma-lang-2.3.0/bin/magma`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/array.py` & `magma-lang-2.3.0/magma/array.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import weakref
 from functools import reduce, lru_cache
 import operator
 from abc import ABCMeta
-from hwtypes import BitVector
-from .common import deprecated
-from .ref import AnonRef, ArrayRef
-from .t import Type, Kind, Direction, In, Out
+from hwtypes import BitVector, AbstractBitVector
+from .ref import ArrayRef
+from .t import Type, Kind, Direction
 from .compatibility import IntegerTypes
 from .digital import Digital
 from .bit import Bit
-from .bitutils import int2seq, seq2int
-from .debug import debug_wire, get_callee_frame_info
+from .bitutils import int2seq
+from .debug import debug_wire, get_debug_info, debug_unwire
 from .logging import root_logger
 from .protocol_type import magma_type, magma_value
 
 from magma.operator_utils import output_only
-from magma.wire_container import WiringLog, Wire, Wireable
 from magma.protocol_type import MagmaProtocol
+from magma.when import no_when, temp_when
+from magma.wire_container import (
+    WiringLog,
+    AggregateWireable,
+    aggregate_wireable_method
+)
 
 
 _logger = root_logger()
 
 
 class ArrayMeta(ABCMeta, Kind):
     # BitVectorType, size :  BitVectorType[size]
@@ -148,15 +152,14 @@
         if t is not None:
             return t
         else:
             raise AttributeError('type {} has no abstract_t'.format(cls))
 
     @property
     def undirected_t(cls) -> 'ArrayMeta':
-        T = cls.T
         if cls.is_concrete:
             return cls[cls.N, cls.T.qualify(Direction.Undirected)]
         else:
             raise AttributeError('type {} has no undirected_t'.format(cls))
 
     @property
     def N(cls) -> int:
@@ -282,15 +285,15 @@
                          "with list equal to array length")
     return [elem if not isinstance(elem, int) else T(elem)
             for elem in arg]
 
 
 def _make_array_from_array(N, arg):
     if len(arg) != N:
-        raise TypeError(f"Will not do implicit conversion of arrays")
+        raise TypeError("Will not do implicit conversion of arrays")
     return arg.ts[:]
 
 
 def _make_array_from_bv(N, T, arg):
     if not issubclass(T, Bit):
         raise TypeError(f"Can only instantiate Array[N, Bit] "
                         f"with int/bv, not Array[N, {T}]")
@@ -354,47 +357,51 @@
     return _make_array_no_args(array)
 
 
 def _is_slice_child(child):
     return isinstance(child, Array) and child._is_slice()
 
 
-class Array(Type, Wireable, metaclass=ArrayMeta):
+class Array(Type, AggregateWireable, metaclass=ArrayMeta):
     """
-    Wireable class allows Array values to be "bulk wired" like a Digital value
+    AggregateWireable class allows Array values to be "bulk wired" like a
+    Digital value
 
     The `self._ts` attribute contains a lazily constructed mapping from index
     to child value.
 
     The `self._slices` attribute contains a list of slice objects that
     reference an array value.  Slices are lazily expanded in order to optimize
     performance in the commons case.  Slices are expanded by constructing the
     child objects and populating the corresponding entries in the `._ts`
     dictionary of both the slice object the parent array object.
 
-    A large portion of the Array logic for the Wireable interface must dispatch
-    on `self._ts` and `self._slices` to see if the Array has been expanded
-    (requiring the logic to be implemented recursively over the children),
-    otherwise the logic will treat the Array as a "bulk wired" value.
+    A large portion of the Array logic for the AggregateWireable interface
+    must dispatch on `self._ts` and `self._slices` to see if the Array has been
+    expanded (requiring the logic to be implemented recursively over the
+    children), otherwise the logic will treat the Array as a "bulk wired"
+    value.
     """
+
     def __init__(self, *args, **kwargs):
         # Pass name= kwarg to Type constructor
         Type.__init__(self, **kwargs)
-        Wireable.__init__(self)
+        AggregateWireable.__init__(self)
         if args:
             # If args is not empty, that means this array is being constructed
             # with existing values, so populate the `_ts` dictionary eagerly
             self._ts = {i: t for i, t in enumerate(_make_array(self, args))}
+            self._resolved = True
         else:
             self._ts = {}
 
         self._slices = {}
         self._unresolved_slices = {}
-        # Store mapping from slice start index to object for faster lookup when
-        # checking overlapping indicies/slices
+        # Store mapping from slice start index to slice key and object for
+        # faster lookup when checking overlapping indicies/slices
         self._slices_by_start_index = {}
 
     @classmethod
     def is_oriented(cls, direction):
         if cls.T is None:
             return False
         return cls.T.is_oriented(direction)
@@ -429,19 +436,19 @@
 
     @classmethod
     def flat_length(cls):
         return cls.N * cls.T.flat_length()
 
     def _is_whole_slice(self, key):
         # check if it's any of `x[:], x[0:], x[:len(x)], x[0:len(x)]`
-        return (isinstance(key[-1], slice) and
-                (key[-1] == slice(None) or
-                 key[-1] == slice(0, None) or
-                 key[-1] == slice(None, len(self)) or
-                 key[-1] == slice(0, len(self))))
+        return (isinstance(key, slice) and
+                (key == slice(None) or
+                 key == slice(0, None) or
+                 key == slice(None, len(self)) or
+                 key == slice(0, len(self))))
 
     def __setitem__(self, key, val):
         """
         Validate when the user attempts to mutate the array.  This is done by
         default by using the @= operator, so the simplest check is to validate
         val is self[key] since this should return the same value except in one
         case (the ndarray slicing logic will return a new array).
@@ -493,15 +500,15 @@
         total = self.N + other_len
         res_bits = []
         for i in range(total):
             res_bits.append(self[i] if i < self.N else other[i - self.N])
         return type(self)[len(res_bits), self.T](res_bits)
 
     def __call__(self, o):
-        return self.wire(o, get_callee_frame_info())
+        return self.wire(o, get_debug_info(3))
 
     def as_list(self):
         return [self[i] for i in range(len(self))]
 
     def _check_wireable(self, o, debug_info):
         if not isinstance(o, ArrayType):
             if isinstance(o, IntegerTypes):
@@ -509,15 +516,14 @@
                     WiringLog(f"Cannot wire {o} (type={type(o)}) to {{}} "
                               f"(type={type(self)}) because conversions from "
                               f"IntegerTypes are only defined for Bits, not "
                               f"general Arrays", self),
                     debug_info=debug_info
                 )
             else:
-                o_str = getattr(o, "debug_name", str(o))
                 _logger.error(
                     WiringLog(f"Cannot wire {{}} (type={type(o)}) to {{}} "
                               f"(type={type(self)}) because {{}} is not an "
                               "Array", o, self, o),
                     debug_info=debug_info
                 )
             return False
@@ -528,23 +534,21 @@
                           f"(type={type(self)}) because the arrays do not have "
                           f"the same length", o, self),
                 debug_info=debug_info
             )
             return False
         return True
 
+    @aggregate_wireable_method
     def driving(self):
-        if self._has_elaborated_children():
-            return [t.driving() for t in self]
-        return Wireable.driving(self)
+        return [t.driving() for t in self]
 
+    @aggregate_wireable_method
     def wired(self):
-        if self._has_elaborated_children():
-            return all(t.wired() for t in self)
-        return Wireable.wired(self)
+        return all(t.wired() for t in self)
 
     # test whether the values refer a whole array
     @staticmethod
     def _iswhole(ts):
 
         n = len(ts)
 
@@ -578,103 +582,94 @@
         size_T = cls.T.flat_length()
         if len(value) != size_T * cls.N:
             raise TypeError("Width mismatch")
         ts = [cls.T.unflatten(value[i:i + size_T])
               for i in range(0, size_T * cls.N, size_T)]
         return cls(ts)
 
-    def concat(self, other) -> 'AbstractBitVector':
+    def concat(self, other) -> AbstractBitVector:
         return type(self)[len(self) + len(other), self.T](self.ts + other.ts)
 
     def undriven(self):
         for elem in self:
             elem.undriven()
 
     def unused(self):
         for elem in self:
             elem.unused()
 
     @classmethod
     def is_mixed(cls):
         return cls.T.is_mixed()
 
-    def _wire_children(self, o):
+    def _wire_children(self, o, debug_info):
         for i, child in self._enumerate_children():
-            curr_value = child.value()
-            new_value = o[i]
-            if curr_value is not new_value:
-                # Skip updating wire in the case that it's the same value
-                # (avoids an error message)
-                child.wire(new_value)
+            child.wire(o[i], debug_info)
 
     @debug_wire
     def wire(self, o, debug_info):
         o = magma_value(o)
         if not self._check_wireable(o, debug_info):
             return
-        if self._has_elaborated_children() or o._has_elaborated_children():
+        if self._should_wire_children(o):
             # Ensure the children maintain consistency with the bulk wire
-            self._wire_children(o)
+            self._wire_children(o, debug_info)
         else:
             # Perform a bulk wire
-            Wireable.wire(self, o, debug_info)
+            AggregateWireable.wire(self, o, debug_info)
 
-    def unwire(self, o):
-        if self._has_elaborated_children():
-            for i, child in self._enumerate_children():
-                child.unwire(o[i])
-        else:
-            Wireable.unwire(self, o)
+    @debug_unwire
+    @aggregate_wireable_method
+    def unwire(self, o=None, debug_info=None, keep_wired_when_contexts=False):
+        for i, child in self._enumerate_children():
+            o_i = None if o is None else o[i]
+            child.unwire(o_i, debug_info=debug_info,
+                         keep_wired_when_contexts=keep_wired_when_contexts)
 
     def iswhole(self):
-        if self._has_elaborated_children():
+        if self.has_elaborated_children():
             return Array._iswhole(self._collect_children(lambda x: x))
         return True
 
     def const(self):
-        if self._has_elaborated_children():
+        if self.has_elaborated_children():
             return all(child.const()
                        for _, child in self._enumerate_children())
         return False
 
-    def _resolve_bulk_wire(self):
-        """
-        If a child reference is made, we "expand" a bulk wire into the
-        constiuent children to maintain consistency
-        """
-        if not self._wire.driven():
-            return
-        # Remove bulk wire since children will now track the wiring
-        value = self._wire.value()
-        Wireable.unwire(self, value)
-
-        # Update children
-        for i, child in self._enumerate_children():
-            child.wire(value[i])
+    def __int__(self):
+        if not self.const():
+            raise TypeError("Can't call __int__ on a non-constant")
+        if not issubclass(self.T, Digital):
+            raise TypeError("Can only call __int__ on array of bit values")
+        bits = [bool(v) for _, v in self._enumerate_children()]
+        return BitVector[len(self)](bits).as_uint()
 
     def _make_t(self, index):
         if issubclass(self.T, MagmaProtocol):
-            return self.T._from_magma_value_(
-                self.T._to_magma_()(name=ArrayRef(self, index)))
-        return self.T(name=ArrayRef(self, index))
+            value = self.T._to_magma_()(name=ArrayRef(self, index))
+            value.set_enclosing_when_context(self._enclosing_when_context)
+            return self.T._from_magma_value_(value)
+        value = self.T(name=ArrayRef(self, index))
+        value.set_enclosing_when_context(self._enclosing_when_context)
+        return value
 
     def _resolve_slice_children(self, start, stop, slice_value):
         for i in range(start, stop):
-            slice_value._ts[i - start] = self._get_t(i)
+            if (not isinstance(slice_value.name, ArrayRef) or
+                    slice_value.name.array is not self):
+                self._ts[i] = slice_value[i - start]
+            else:
+                slice_value._ts[i - start] = self._get_t(i)
 
     def _resolve_slice_driver(self, start, stop, value):
         # When we encounter an overlapping slice that is already bulk driven,
         # we ensure the corresponding children are updated to their current
         # values
-        if not value._wire.driven():
-            return
-        driver = value._wire.value()
-        Wireable.unwire(value, driver)
-        for i in range(start, stop):
-            self._ts[i] @= driver[i - start]
+        value._resolve_bulk_wire()
 
     def _remove_slice(self, key):
         """
         Remove slice since we don't need to track it anymore (handled by child
         logic) to optimize other slice iteration logic This avoids having to
         iterate over slices when we are just using their children instead
 
@@ -684,35 +679,41 @@
         here) since we are trying to resolve/remove a slice more than once.
         """
         assert key in self._unresolved_slices
         assert key[0] in self._slices_by_start_index
         del self._unresolved_slices[key]
         del self._slices_by_start_index[key[0]]
 
-    def _update_overlapping_slices(self, t, index):
+    def _check_slice_overlap(self, index):
         # Update existing slices to have matching child references
         def _filter(item):
             (start, stop), _ = item
             return start <= index < stop
         overlaps = list(filter(_filter, self._unresolved_slices.items()))
-        for k, v in overlaps:
-            self._remove_slice(k)
-            assert v._ts.get(index - k[0], t) is t
-            v._ts[index - k[0]] = t
-            self._resolve_slice_children(k[0], k[1], v)
-            self._resolve_slice_driver(k[0], k[1], v)
+        if not len(overlaps):
+            return False
+        # Because overlapping slices are expanded, we only ever expect one
+        # slice to overlap a _get_t index
+        assert len(overlaps) == 1
+        key, value = overlaps[0]
+        self._remove_slice(key)
+        self._resolve_slice_children(key[0], key[1], value)
+        self._resolve_slice_driver(key[0], key[1], value)
+        return True
 
     def _get_t(self, index):
         if index not in self._ts:
             if self._is_slice():
                 # Maintain consistency by always fetching child object from top
                 # level array
-                return self.name.array._get_t(self.name.index.start + index)
-            self._ts[index] = t = self._make_t(index)
-            self._update_overlapping_slices(t, index)
+                self._ts[index] = self.name.array._get_t(self.name.index.start
+                                                         + index)
+            elif not self._check_slice_overlap(index):
+                self._ts[index] = self._make_t(index)
+            self._ts[index].parent = self
         return self._ts[index]
 
     def _resolve_overlapping_indices(self, slice_, value):
         """
         If there's any overlapping children or slices, collect the total range
         of the children and realize them so slices are "expanded" and maintain
         consistency
@@ -727,26 +728,30 @@
 
         overlapping |= any(range_overlapping(k, (start, stop))
                            for k, v in self._unresolved_slices.items())
         if overlapping:
             for i in range(start, stop):
                 # _get_t to populate slice children and resolve any overlaps
                 value._ts[i - start] = self._get_t(i)
+            value._resolved = True
         return overlapping
 
     def _get_slice(self, slice_):
         key = (slice_.start, slice_.stop)
         slice_value = self._slices.get(key, None)
         if slice_value is None:
             slice_T = type(self)[slice_.stop - slice_.start, self.T]
             slice_value = slice_T(name=ArrayRef(self, slice_))
+            slice_value.set_enclosing_when_context(self._enclosing_when_context)
             self._slices[key] = slice_value
-            if not self._resolve_overlapping_indices(slice_, slice_value):
-                self._slices_by_start_index[key[0]] = slice_value
-                self._unresolved_slices[key] = slice_value
+            slice_value.parent = self
+            if self._resolve_overlapping_indices(slice_, slice_value):
+                return slice_value
+            self._slices_by_start_index[key[0]] = (slice_, slice_value)
+            self._unresolved_slices[key] = slice_value
         return slice_value
 
     def _normalize_slice_key(self, key):
         # Normalize slice by mapping None to concrete int values
         start = key.start if key.start is not None else 0
         if start < 0:
             start = self.N + start
@@ -764,15 +769,15 @@
     def _ndarray_getitem(self, key: tuple):
         # tuple -> ND Array key
 
         if len(key) == 1:
             return self[key[0]]
         if not isinstance(key[-1], slice):
             return self[key[-1]][key[:-1]]
-        if not self._is_whole_slice(key):
+        if not self._is_whole_slice(key[-1]):
             # If it's not a slice of the whole array, first slice the
             # current array (self), then replace with a slice of the whole
             # array (this is how we determine that we're ready to traverse
             # into the children)
             this_key = key[-1]
             result = self[this_key][key[:-1] + (slice(None), )]
             return result
@@ -811,14 +816,16 @@
             # indexed using a dynamic magma value, generate mux circuit
             return self.dynamic_mux_select(key)
         if isinstance(key, tuple):
             return self._ndarray_getitem(key)
         if isinstance(key, int) and key > self.N - 1:
             raise IndexError()
         if isinstance(key, slice):
+            if self._is_whole_slice(key):
+                return self
             if key.step is not None:
                 return self._variable_step_slice_getitem(key)
             if not _is_valid_slice(self.N, key):
                 raise IndexError(f"array index out of range "
                                  f"(type={type(self)}, key={key})")
             key = self._normalize_slice_key(key)
 
@@ -827,25 +834,24 @@
         if isinstance(key, (int, BitVector)):
             result = arr._get_t(offset + self._normalize_int_key(key))
         elif isinstance(key, slice):
             result = arr._get_slice(slice(offset + key.start,
                                           offset + key.stop))
         else:
             raise NotImplementedError(key, type(key))
-        self._resolve_bulk_wire()
         return result
 
     def flatten(self):
         ts = []
         for _, child in self._enumerate_children():
             ts.extend(child.flatten())
         return ts
 
     def __repr__(self):
-        if self.name.anon():
+        if self.name.anon() and self.has_elaborated_children():
             t_strs = ', '.join(repr(t) for t in self.ts)
             return f'array([{t_strs}])'
         return Type.__repr__(self)
 
     @property
     def ts(self):
         return [elem for elem in self]
@@ -857,41 +863,45 @@
 
         `func` is called on the child
             e.g. to fetch the value of the children, use lambda x: x.value()
 
         Returns None if func(child) returns None
             e.g. the value is None if any of the children have a value None
         """
-        ts = []
-        for _, child in self._enumerate_children():
+        T = type(self).flip()()
+        for i, child in self._enumerate_children():
             result = func(child)
             if result is None:
                 return None
             if _is_slice_child(child) and child.name.array is self:
-                ts.extend(result.ts)
+                key = (i.start, i.stop)
+                T._slices[key] = result
+                T._slices_by_start_index[key[0]] = (i, result)
+                T._unresolved_slices[key] = result
             else:
-                ts.append(result)
+                T._ts[i] = result
+        T._resolved = True
 
-        # Pack whole array together for readability
-        if Array._iswhole(ts):
-            return ts[0].name.array
+        if len(T._ts) == self.N:
+            if Array._iswhole(T.ts):
+                # Pack whole array together for readability
+                return T.ts[0].name.array
 
-        # Pack into Bits const if possible for readability
-        if all(t.const() for t in ts):
-            return type(self).flip()(ts)
+            if all(t.const() for t in T.ts):
+                # Pack into Bits const if possible for readability
+                return type(self).flip()(T.ts)
 
-        return type(self)[self.N, self.T.flip()](ts)
+        return T
 
-    def _has_elaborated_children(self):
+    def has_elaborated_children(self):
         return bool(self._ts) or bool(self._slices)
 
+    @aggregate_wireable_method
     def value(self):
-        if self._has_elaborated_children():
-            return self._collect_children(lambda x: x.value())
-        return super().value()
+        return self._collect_children(lambda x: x.value())
 
     def _make_trace_child(self, skip_self):
         def _trace_child(t):
             """
             This handles the case where certain children trace further than
             others.
 
@@ -910,29 +920,24 @@
             if result is not None:
                 return result
             if not skip_self and (t.is_output() or t.is_inout()):
                 return t
             return None
         return _trace_child
 
+    @aggregate_wireable_method
     def trace(self, skip_self=True):
-        if self._has_elaborated_children():
-            result = self._collect_children(self._make_trace_child(skip_self))
-            return result
-        return Wireable.trace(self)
+        return self._collect_children(self._make_trace_child(skip_self))
 
+    @aggregate_wireable_method
     def driven(self):
-        if not self._has_elaborated_children():
-            return Wireable.driven(self)
-        for _, child in self._enumerate_children():
-            if child is None:
-                return False
-            if not child.driven():
-                return False
-        return True
+        return all(
+            child is not None and child.driven()
+            for _, child in self._enumerate_children()
+        )
 
     def _is_slice(self):
         return (isinstance(self.name, ArrayRef) and
                 isinstance(self.name.index, slice))
 
     def _enumerate_children(self):
         i = 0
@@ -940,16 +945,15 @@
             if i in self._ts:
                 yield i, self._ts[i]
                 i += 1
             elif i in self._slices_by_start_index:
                 # We only need to lookup one slice by start index because if
                 # multiple slices overlap, they're children will be realized
                 # and in self._ts
-                value = self._slices_by_start_index[i]
-                slice_ = value.name.index
+                slice_, value = self._slices_by_start_index[i]
                 yield slice_, value
                 i = slice_.stop
             else:
                 # Create the child using default getitem logic
                 yield i, self[i]
                 i += 1
 
@@ -992,9 +996,18 @@
                 yield from ((t, t.trace()) for t in self)
             else:
                 yield from _yield_curr_slice_or_elem(curr_slice_or_elem)
 
     def has_children(self):
         return True
 
+    def set_enclosing_when_context(self, ctx):
+        # This code assumes set_enclosing_when_context is called when a child
+        # of a lazy value is created, so it should not have any children
+        # elaborated yet (and any future elaborations will inherit this
+        # context).
+        assert not self._ts
+        assert not self._slices
+        super().set_enclosing_when_context(ctx)
+
 
 ArrayType = Array
```

### Comparing `magma-lang-2.2.9/magma/ast_utils.py` & `magma-lang-2.3.0/magma/ast_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/blif.py` & `magma-lang-2.3.0/magma/backend/blif.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/check_wiring_context.py` & `magma-lang-2.3.0/magma/backend/check_wiring_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     return get_ref_defn(value.name)
 
 
 def check_wiring_context(i, o):
     """
     Ensures that i and o come from the same definition context
     """
+    orig_i, orig_o = i, o
     if isinstance(o, Slice):
         o = o.value
     if isinstance(i, Slice):
         i = i.value
     i, o = magma_value(i), magma_value(o)
     if is_temp_ref(o.name) or is_temp_ref(i.name):
         # Will be handled recursively by the get_source logic for the coreir
@@ -49,9 +50,9 @@
         return
     if o_inst is not None and i_defn is not None and o_inst.defn is i_defn:
         return
     if (o_inst is not None and i_inst is not None and
             o_inst.defn is i_inst.defn):
         return
     raise MagmaCompileException(
-        f"Cannot wire {o.debug_name} to {i.debug_name} because they are"
-        " not from the same definition context")
+        f"Cannot wire {orig_o.debug_name} to {orig_i.debug_name} because they "
+        "are not from the same definition context")
```

### Comparing `magma-lang-2.2.9/magma/backend/coreir/coreir_backend.py` & `magma-lang-2.3.0/magma/backend/coreir/coreir_backend.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/coreir/coreir_compiler.py` & `magma-lang-2.3.0/magma/backend/coreir/coreir_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from magma.config import EnvConfig, config
 from magma.backend.coreir.insert_coreir_wires import insert_coreir_wires
 from magma.backend.coreir.insert_wrap_casts import insert_wrap_casts
 from magma.frontend import coreir_ as coreir_frontend
 from magma.is_definition import isdefinition
 from magma.logging import root_logger
 from magma.passes import InstanceGraphPass
-from magma.passes.find_errors import find_errors_pass
+from magma.passes.elaborate_circuit import elaborate_all_pass
+from magma.passes.raise_logs_as_exceptions import raise_logs_as_exceptions_pass
+from magma.primitives.mux import Mux
 from magma.symbol_table import SymbolTable
 from magma.symbol_table_utils import MasterSymbolTable
 
 
 _logger = root_logger()
 config._register(
     fast_coreir_verilog_compile=EnvConfig(
@@ -48,14 +50,16 @@
         cmd += " --verilator_compat"
     if opts.get("verilog_prefix", ""):
         cmd += f" --verilog-prefix {opts['verilog_prefix']}"
     if opts.get("verilog_prefix_extern", False):
         cmd += " --verilog-prefix-extern"
     if opts.get("generate_symbols", False):
         cmd += f" --symbols {basename}_symbol_table.json"
+    if opts.get("use_packed_arrays", False):
+        cmd += " --use-packed-arrays"
     return cmd
 
 
 def _make_opts(backend, opts):
     new_opts = {}
     user_namespace = opts.get("user_namespace", None)
     if user_namespace is not None:
@@ -71,23 +75,26 @@
 class CoreIRCompiler(Compiler):
     def __init__(self, main, basename, opts):
         super().__init__(main, basename, opts)
         self.namespaces = self.opts.get("namespaces", ["global"])
         self.passes = opts.get("passes", [])
         if "markdirty" not in self.passes:
             self.passes.append("markdirty")
-        self.deps = self._deps()
         self.backend = coreir_frontend.GetCoreIRBackend()
 
     def compile(self):
         result = {}
         result["symbol_table"] = symbol_table = SymbolTable()
+        elaborate_all_pass(self.main, generators=(Mux,))
         insert_coreir_wires(self.main)
         insert_wrap_casts(self.main)
-        find_errors_pass(self.main)
+        raise_logs_as_exceptions_pass(self.main)
+        # NOTE(rsetaluri): We can compute deps only after all the passes have
+        # been run, as they can possibly introduce new circuits with new deps.
+        self.deps = self._deps()
         backend = self.backend
         opts = _make_opts(backend, self.opts)
         opts["symbol_table"] = symbol_table
         backend.compile(self.main, opts)
         backend.context.run_passes(self.passes, self.namespaces)
         if isdefinition(self.main):
             result["coreir_module"] = backend.get_module(self.main)
@@ -136,14 +143,16 @@
             split=self.opts.get("split", ""),
             inline=self.opts.get("inline", False),
             verilator_debug=self.opts.get("verilator_debug", False),
             disable_width_cast=self.opts.get("disable_width_cast", False),
         )
         if self.opts.get("verilog_prefix", False):
             raise NotImplementedError()
+        if self.opts.get("use_packed_arrays", False):
+            raise NotImplementedError()
         ret = self.backend.context.compile_to_verilog(top, filename, **opts)
         if not ret:
             raise RuntimeError(f"CoreIR compilation to verilog failed")
 
     def _compile_verilog_epilogue(self):
         self._process_header_footer()
```

### Comparing `magma-lang-2.2.9/magma/backend/coreir/coreir_runtime.py` & `magma-lang-2.3.0/magma/backend/coreir/coreir_runtime.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/coreir/coreir_transformer.py` & `magma-lang-2.3.0/magma/backend/coreir/coreir_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from magma.backend.check_wiring_context import check_wiring_context
 from magma.backend.coreir.coreir_utils import (
     attach_debug_info, check_magma_interface, constant_to_value, get_inst_args,
     get_module_of_inst, magma_interface_to_coreir_module_type,
     magma_port_to_coreir_port, make_cparams, map_genarg,
     magma_name_to_coreir_select, Slice)
 from magma.compile_exception import UnconnectedPortException
+from magma.inline_verilog_expression import InlineVerilogExpression
 from magma.interface import InterfaceKind
 from magma.is_definition import isdefinition
 from magma.linking import (
     get_linked_modules, has_default_linked_module, get_default_linked_module)
 from magma.logging import root_logger
 from magma.passes import dependencies
 from magma.tuple import Tuple
@@ -483,16 +484,19 @@
         coreir_names = list(k for k, _ in self.coreir_module.type.items())
         assert len(magma_names) == len(coreir_names)
         for magma_name, coreir_name in zip(magma_names, coreir_names):
             self.opts.get("symbol_table").set_port_name(
                 self.decl.name, magma_name, coreir_name)
 
     def _run_self_impl(self):
-        self.decl = self.decl
         _logger.debug(f"Compiling declaration {self.decl}")
+        if isinstance(self.decl, InlineVerilogExpression):
+            raise NotImplementedError(
+                "Can not compile InlineVerilogExpression generator to CoreIR"
+            )
         if self.decl.coreir_lib is not None:
             self.backend.include_lib_or_libs(self.decl.coreir_lib)
         # These libraries are already available by default in coreir, so we
         # don't need declarations.
         if self.decl.coreir_lib in ["coreir", "corebit", "commonlib",
                                     "memory"]:
             lib = self.backend.get_lib(self.decl.coreir_lib)
```

### Comparing `magma-lang-2.2.9/magma/backend/coreir/coreir_utils.py` & `magma-lang-2.3.0/magma/backend/coreir/coreir_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/coreir/insert_coreir_wires.py` & `magma-lang-2.3.0/magma/backend/coreir/insert_coreir_wires.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from magma.array import Array
+from magma.bits import Bits
+from magma.digital import Digital
 from magma.clock import AsyncReset, AsyncResetN, Clock, _ClockType
-from magma.conversions import as_bits, from_bits, bit, convertbit
+from magma.conversions import as_bits, from_bits, bit, convertbit, convertbits
+from magma.debug import maybe_get_debug_info
 from magma.digital import Digital
 from magma.generator import Generator2
 from magma.passes.passes import DefinitionPass, pass_lambda
 from magma.primitives.wire import Wire
 from magma.ref import NamedRef, ArrayRef, PortViewRef, InstRef
 from magma.t import In, Out
 from magma.tuple import Tuple
@@ -13,18 +16,19 @@
 def _sanitize_name(name):
     return name.replace("[", "_").replace("]", "")\
                .replace("(", "").replace(")", "")\
                .replace(",", "").replace(" ", "_")
 
 
 class InsertCoreIRWires(DefinitionPass):
-    def __init__(self, main):
+    def __init__(self, main, flatten: bool = True):
         super().__init__(main)
         self.seen = set()
         self.wire_map = {}
+        self._flatten = flatten
 
     def _make_wire(self, driver, value, definition):
         is_bits = (isinstance(driver.name, ArrayRef) and
                    isinstance(driver, Digital) and not driver.name.anon())
 
         # If this is a member of a bits, emit only one wire for the parent
         # Bits, since it shouldn't be flattened
@@ -38,45 +42,47 @@
             driver_name = _sanitize_name(driver_name)
 
             # Rename driver so it doesn't conflict with new wire instance name
             if isinstance(driver.name, NamedRef):
                 driver.name.name = "_" + driver.name.name
 
             name = f"{driver_name}"
-            wire_inst = Wire(T)(name=name)
+            wire_inst = Wire(T, flatten=self._flatten)(name=name)
+            wire_inst.debug_info = maybe_get_debug_info(value)
             self.wire_map[driver] = wire_inst
         wire_inst = self.wire_map[driver]
         wire_input = wire_inst.I
         wire_output = wire_inst.O
 
         if is_bits:
             # Select the index off the parent bits wire
             wire_output = wire_output[index]
             # NOTE(leonardt): We don't select off the input and instead wire up
             # the entire bits (this avoids an "undriven" error when only one
             # index of the bits is used)
 
-        if not is_bits and not isinstance(driver, Digital):
+        if self._flatten and not is_bits and not isinstance(driver, Digital):
             driver = as_bits(driver)
             wire_output = from_bits(T, wire_output)
 
         # Could be already wired for fanout cases
         if not wire_input.driven():
-            if isinstance(wire_input, Array):
-                for d, w in zip(driver, wire_input):
-                    # Could have wired up child elements already
-                    if not w.driven():
-                        w @= d
-            else:
-                wire_input @= driver
-        if (isinstance(value, _ClockType) and
-                not isinstance(wire_output, type(value))):
+            wire_input @= driver
+
+        value_T = type(value)
+        if not isinstance(wire_output, value_T):
             # This mean it was cast by the user (e.g. m.clock(value)), so we
             # need to "recast" the wire output
-            wire_output = convertbit(wire_output, type(value))
+            if isinstance(value, Digital):
+                wire_output = convertbit(wire_output, value_T)
+            elif isinstance(value, Array):
+                wire_output = convertbits(
+                    wire_output, len(value_T), value_T,
+                    issubclass(value_T, Bits)
+                )
         value @= wire_output
 
     def _insert_wire(self, value, definition):
         if value.is_mixed():  # mixed children
             for child, _ in value.connection_iter():
                 if not child.is_output():
                     self._insert_wire(child, definition)
@@ -121,13 +127,24 @@
         definition._coreir_wires_inserted_ = True
         # Copy instances because inserting wire will append to instances.
         instances_copy = definition.instances.copy()
         for instance in instances_copy:
             for value in instance.interface.ports.values():
                 if not value.is_output():
                     self._insert_wire(value, definition)
+
+        # See https://github.com/phanrahan/magma/pull/1157 for more context, we
+        # need to run this on specifically the when builder instance, since
+        # this hasn't been finalized yet and may trace back to temporary
+        # values.
+        for builder in definition._context_._builders:
+            if builder._finalized:
+                continue
+            for value in builder._io.inst_ports.values():
+                if not value.is_output():
+                    self._insert_wire(value, definition)
         for value in definition.interface.ports.values():
             if not value.is_output():
                 self._insert_wire(value, definition)
 
 
 insert_coreir_wires = pass_lambda(InsertCoreIRWires)
```

### Comparing `magma-lang-2.2.9/magma/backend/coreir/insert_wrap_casts.py` & `magma-lang-2.3.0/magma/backend/coreir/insert_wrap_casts.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from magma.clock import AsyncReset, AsyncResetN, Clock, is_clock_or_nested_clock
 from magma.conversions import convertbit
 from magma.interface import IO
 from magma.passes import DefinitionPass, pass_lambda
 from magma.t import In, Out, Direction
 from magma.tuple import Tuple
 from magma.wire import wire
+from magma.wire_container import AggregateWireable
 
 
 _NAMED_TYPES = (AsyncReset, AsyncResetN, Clock)
 
 
 class InsertWrapCasts(DefinitionPass):
     def define_wrap(self, wrap_type, in_type, out_type):
@@ -44,17 +45,23 @@
         if isinstance(port, Array):
             # Avoid recursion when possible (for Array2) by checking the nested
             # array type and only descending if necessary
             # Note(leonardt): If value is anon, we need to check the children
             # via recursion in case the children are named types (since
             # .value() will return Array[N, T.flip()], the anon value may not
             # have the namedtypes in its type)
-            if (is_clock_or_nested_clock(type(port), _NAMED_TYPES) or
-                    is_clock_or_nested_clock(type(value), _NAMED_TYPES) or
-                    value.anon()):
+            if (
+                is_clock_or_nested_clock(type(port), _NAMED_TYPES) or
+                is_clock_or_nested_clock(type(value), _NAMED_TYPES) or
+                (
+                    value.anon() and
+                    isinstance(value, AggregateWireable) and
+                    value.has_elaborated_children()
+                )
+            ):
                 for child, _ in port.connection_iter():
                     if not self.wrap_if_named_type(child, definition):
                         return False
                 return True
             else:
                 return self.wrap_if_named_type(value, definition)
         if not (isinstance(port, _NAMED_TYPES) or
```

### Comparing `magma-lang-2.2.9/magma/backend/dot.py` & `magma-lang-2.3.0/magma/backend/dot.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/firrtl.py` & `magma-lang-2.3.0/magma/backend/firrtl.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/mlir/comb.py` & `magma-lang-2.3.0/magma/backend/mlir/comb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import dataclasses
 from typing import List
 
 from magma.backend.mlir.mlir import MlirDialect, begin_dialect, end_dialect
 from magma.backend.mlir.mlir_printer_utils import print_names, print_types
 from magma.backend.mlir.mlir import MlirValue, MlirOp
+from magma.backend.mlir.print_opts import PrintOpts
 from magma.backend.mlir.printer_base import PrinterBase
 
 
 comb = MlirDialect("comb")
 begin_dialect(comb)
 
 
 @dataclasses.dataclass
 class BaseOp(MlirOp):
     operands: List[MlirValue]
     results: List[MlirValue]
     op_name: str
 
-    def print_op(self, printer: PrinterBase):
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
         print_names(self.results, printer)
         printer.print(f" = comb.{self.op_name} ")
         print_names(self.operands, printer)
         printer.print(" : ")
         print_types(self.results, printer)
 
 
 @dataclasses.dataclass
 class ConcatOp(MlirOp):
     operands: List[MlirValue]
     results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
         print_names(self.results, printer)
         printer.print(f" = comb.concat ")
         print_names(self.operands, printer)
         printer.print(" : ")
         print_types(self.operands, printer)
 
 
 @dataclasses.dataclass
 class ExtractOp(MlirOp):
     operands: List[MlirValue]
     results: List[MlirValue]
     lo: int
 
-    def print_op(self, printer: PrinterBase):
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
         print_names(self.results, printer)
         printer.print(" = comb.extract ")
         print_names(self.operands, printer)
         printer.print(f" from {self.lo} : (")
         print_types(self.operands, printer)
         printer.print(") -> ")
         print_types(self.results, printer)
@@ -56,28 +57,28 @@
 
 @dataclasses.dataclass
 class ICmpOp(MlirOp):
     operands: List[MlirValue]
     results: List[MlirValue]
     predicate: str
 
-    def print_op(self, printer: PrinterBase):
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
         print_names(self.results, printer)
         printer.print(f" = comb.icmp {self.predicate} ")
         print_names(self.operands, printer)
         printer.print(f" : ")
         print_types(self.operands[0], printer)
 
 
 @dataclasses.dataclass
 class ParityOp(MlirOp):
     operands: List[MlirValue]
     results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
         print_names(self.results, printer)
         printer.print(f" = comb.parity ")
         print_names(self.operands, printer)
         printer.print(" : ")
         print_types(self.operands, printer)
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/common.py` & `magma-lang-2.3.0/magma/backend/mlir/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,26 +31,9 @@
 
 
 @dataclasses.dataclass
 class WithId:
     id: str = dataclasses.field(default_factory=make_unique_name, init=False)
 
 
-def replace_all(s: str, replacements: Dict[str, str]) -> str:
-    for old, new in replacements.items():
-        s = s.replace(old, new)
-    return s
-
-
 def constant(value: Any):
     return lambda: value
-
-
-def try_call(fn: Callable[[], Any], ExceptionType: Optional[Any]):
-    if ExceptionType is None:
-        ExceptionType = BaseException
-    try:
-        ret = fn()
-    except ExceptionType:
-        pass
-    else:
-        return ret
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/hardware_module.py` & `magma-lang-2.3.0/magma/backend/mlir/hardware_module.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,123 @@
+import abc
 import contextlib
 import dataclasses
 import functools
+import itertools
+import pathlib
 from typing import Any, List, Mapping, Optional, Tuple, Union
 import weakref
 
 from magma.array import Array, ArrayMeta
-from magma.backend.mlir.build_magma_graph import build_magma_graph
+from magma.backend.mlir.build_magma_graph import (
+    BuildMagmaGrahOpts, build_magma_graph
+)
 from magma.backend.mlir.builtin import builtin
 from magma.backend.mlir.comb import comb
 from magma.backend.mlir.common import wrap_with_not_implemented_error
+from magma.backend.mlir.compile_to_mlir_opts import CompileToMlirOpts
+from magma.backend.mlir.errors import MlirCompilerInternalError
 from magma.backend.mlir.graph_lib import Graph
 from magma.backend.mlir.hw import hw
 from magma.backend.mlir.magma_common import (
     ModuleLike as MagmaModuleLike,
     ValueWrapper as MagmaValueWrapper,
     InstanceWrapper as MagmaInstanceWrapper,
     value_or_type_to_string as magma_value_or_type_to_string,
     visit_value_or_value_wrapper_by_direction as
-    visit_magma_value_or_value_wrapper_by_direction
+    visit_magma_value_or_value_wrapper_by_direction,
+    tuple_key_to_str as magma_tuple_key_to_str,
+)
+from magma.backend.mlir.mem_utils import (
+    make_mem_reg,
+    make_mem_read,
+    emit_conditional_assign,
+    emit_conditional_assigns,
+    make_index_op,
+    collect_multiport_memory_operands,
+    make_multiport_memory_index_ops,
+    make_multiport_memory_read_ops,
+)
+from magma.backend.mlir.mlir import (
+    MlirType, MlirValue, MlirSymbol, MlirAttribute, MlirBlock, push_block,
+    push_location
 )
-from magma.backend.mlir.mlir import MlirType, MlirValue, MlirSymbol, push_block
-from magma.backend.mlir.printer_base import PrinterBase
 from magma.backend.mlir.scoped_name_generator import ScopedNameGenerator
 from magma.backend.mlir.sv import sv
+from magma.backend.mlir.when_utils import WhenCompiler
+from magma.backend.mlir.xmr_utils import get_xmr_paths
+from magma.bind2 import is_bound_instance
 from magma.bit import Bit
 from magma.bits import Bits, BitsMeta
 from magma.bitutils import clog2
 from magma.circuit import AnonymousCircuitType, CircuitKind, DefineCircuitKind
 from magma.clock import Reset, ResetN, AsyncReset, AsyncResetN
+from magma.common import filter_by_key, assert_false
+from magma.compile_guard import get_compile_guard_data
 from magma.digital import Digital, DigitalMeta
+from magma.inline_verilog_expression import InlineVerilogExpression
+from magma.inline_verilog2 import InlineVerilog2
 from magma.is_definition import isdefinition
 from magma.is_primitive import isprimitive
+from magma.linking import (
+    has_any_linked_modules,
+    get_linked_modules,
+    has_default_linked_module,
+    get_default_linked_module,
+)
+from magma.primitives.multiport_memory import MultiportMemory
 from magma.primitives.mux import Mux
 from magma.primitives.register import Register
+from magma.primitives.when import iswhen
+from magma.primitives.wire import Wire
+from magma.primitives.xmr import XMRSink, XMRSource
+from magma.protocol_type import magma_value as get_magma_value
 from magma.t import Kind, Type
 from magma.tuple import TupleMeta, Tuple as m_Tuple
+from magma.value_utils import make_selector, TupleSelector, ArraySelector
+from magma.view import PortView
 
 
 MlirValueList = List[MlirValue]
 
 
-def _get_defn_or_decl_output_name(defn_or_decl: CircuitKind) -> str:
+def _get_defn_or_decl_output_name(
+        ctx: 'HardwareModule', defn_or_decl: CircuitKind) -> str:
     metadata = defn_or_decl.coreir_metadata
     try:
         return metadata["verilog_name"]
     except KeyError:
         pass
-    return defn_or_decl.name
+    name = defn_or_decl.name
+    if ctx.opts.user_namespace is not None:
+        name = ctx.opts.user_namespace + f"_{name}"
+    if ctx.opts.verilog_prefix is not None:
+        name = ctx.opts.verilog_prefix + f"{name}"
+    return name
+
+
+def _make_compile_guard_block(compile_guard: Mapping) -> MlirBlock:
+    if_def = sv.IfDefOp(compile_guard["condition_str"])
+    if compile_guard["type"] == "defined":
+        return if_def.then_block
+    assert compile_guard["type"] == "undefined"
+    return if_def.else_block
+
+
+def _maybe_set_location_info(op, debug_info):
+    if debug_info is None:
+        return
+    loc = builtin.FileLineColLoc(debug_info.filename, debug_info.lineno, 0)
+    op.location = loc
+
+
+def _make_location_info(debug_info):
+    if debug_info is None:
+        return builtin.UnknownLoc()
+    return builtin.FileLineColLoc(debug_info.filename, debug_info.lineno, 0)
 
 
 @wrap_with_not_implemented_error
 def parse_reset_type(T: Kind) -> Tuple[str, str]:
     if T is Reset:
         return "syncreset", "posedge"
     if T is ResetN:
@@ -70,98 +137,287 @@
     if issubclass(type, Bits):
         return builtin.IntegerType(type.N)
     if issubclass(type, Array):
         if issubclass(type.T, Bit):
             return magma_type_to_mlir_type(Bits[type.N])
         return hw.ArrayType((type.N,), magma_type_to_mlir_type(type.T))
     if issubclass(type, m_Tuple):
-        fields = {str(k): magma_type_to_mlir_type(t)
-                  for k, t in type.field_dict.items()}
-        return hw.StructType(tuple(fields.items()))
+        fields = (
+            (magma_tuple_key_to_str(k, type), magma_type_to_mlir_type(t))
+            for k, t in type.field_dict.items()
+        )
+        return hw.StructType(tuple(fields))
+
+
+@wrap_with_not_implemented_error
+@functools.lru_cache()
+def python_type_to_mlir_type(type_: type) -> MlirType:
+    # NOTE(rsetaluri): We only support integer attribtue types right now. All
+    # integer parameter types are assumed to be int32's.
+    if type_ is int:
+        return builtin.IntegerType(32)
+
+
+@wrap_with_not_implemented_error
+def python_value_to_mlir_attribtue(value: Any) -> MlirAttribute:
+    # NOTE(rsetaluri): We only support integer attribute types right now.
+    if isinstance(value, int):
+        return builtin.IntegerAttr(value)
 
 
 def get_module_interface(
         module: MagmaModuleLike, ctx) -> Tuple[MlirValueList, MlirValueList]:
     operands = []
     results = []
     for port in module.interface.ports.values():
+        port = get_magma_value(port)
         visit_magma_value_or_value_wrapper_by_direction(
             port,
             lambda p: operands.append(ctx.get_or_make_mapped_value(p)),
-            lambda p: results.append(ctx.get_or_make_mapped_value(p))
+            lambda p: results.append(ctx.get_or_make_mapped_value(p)),
+            flatten_all_tuples=ctx.opts.flatten_all_tuples,
         )
     return operands, results
 
 
+def make_mux(
+        ctx: 'HardwareModule',
+        data: List[MlirValue],
+        select: MlirValue,
+        result: MlirValue):
+    if ctx.opts.extend_non_power_of_two_muxes:
+        closest_power_of_two_size = 2 ** clog2(len(data))
+        if closest_power_of_two_size != len(data):
+            extension = [data[0]] * (closest_power_of_two_size - len(data))
+            data = extension + data
+    mlir_type = hw.ArrayType((len(data),), data[0].type)
+    array = ctx.new_value(mlir_type)
+    hw.ArrayCreateOp(
+        operands=data,
+        results=[array])
+    hw.ArrayGetOp(
+        operands=[array, select],
+        results=[result])
+
+
+def get_register_data_and_init(
+        ctx: 'HardwareModule', I: Type, operands: List[MlirValue], init: Type):
+    T_out, data_out, init_out = [], [], []
+
+    def _visit_input(i):
+        T_out.append(type(i))
+        data_out.append(operands.pop(0))
+        init_out.append(make_selector(i).select(init))
+
+    visit_magma_value_or_value_wrapper_by_direction(
+        I,
+        _visit_input,
+        _visit_input,
+        flatten_all_tuples=ctx.opts.flatten_all_tuples
+    )
+    return T_out, data_out, init_out
+
+
+def make_hw_param_decl(name: str, value: Any):
+    type_ = python_type_to_mlir_type(type(value))
+    value = python_value_to_mlir_attribtue(value)
+    return hw.ParamDeclAttr(name, type_, value)
+
+
 def make_hw_instance_op(
         operands: MlirValueList,
         results: MlirValueList,
         name: str,
         module: hw.ModuleOp,
+        parameters: Mapping[str, Any] = dict(),
         sym: Optional[MlirSymbol] = None,
-        compile_guard: Optional[Mapping] = None) -> hw.InstanceOp:
+        compile_guard: Optional[Mapping] = None,
+        attrs: Optional[Mapping] = None,
+) -> hw.InstanceOp:
     if compile_guard is not None:
-        if_def = sv.IfDefOp(compile_guard["condition_str"])
-        block = (
-            if_def.then_block
-            if compile_guard["type"] == "defined"
-            else if_def.else_block
-        )
-        ctx = push_block(block)
+        ctx = push_block(_make_compile_guard_block(compile_guard))
     else:
         ctx = contextlib.nullcontext()
+    parameters = [
+        make_hw_param_decl(name, value) for name, value in parameters.items()
+    ]
     with ctx:
         op = hw.InstanceOp(
             name=name,
             module=module,
             operands=operands,
             results=results,
+            parameters=parameters,
             sym=sym)
+    if attrs is not None:
+        op.attr_dict.update(attrs)
     return op
 
 
+def resolve_xmr(ctx: 'HardwareModule', xmr: PortView):
+    assert isinstance(xmr, PortView)
+    mlir_type = magma_type_to_mlir_type(type(xmr)._to_magma_())
+    in_out = ctx.new_value(hw.InOutType(mlir_type))
+    sv.XMROp(is_rooted=False, path=list(xmr.path()), results=[in_out])
+    value = ctx.new_value(mlir_type)
+    sv.ReadInOutOp(operands=[in_out], results=[value])
+    return value
+
+
 @dataclasses.dataclass(frozen=True)
 class ModuleWrapper:
     module: MagmaModuleLike
     operands: MlirValueList
     results: MlirValueList
 
     @staticmethod
     def make(module: MagmaModuleLike, ctx) -> 'ModuleWrapper':
         operands, results = get_module_interface(module, ctx)
         return ModuleWrapper(module, operands, results)
 
 
 class ModuleVisitor:
+
+    class VisitError(RuntimeError):
+        pass
+
+    class RevisitedModuleError(VisitError):
+        pass
+
     def __init__(self, graph: Graph, ctx):
         self._graph = graph
         self._ctx = ctx
         self._visited = set()
 
+    @property
+    def ctx(self):
+        return self._ctx
+
     @functools.lru_cache()
     def make_constant(
             self, T: Kind, value: Optional[Any] = None) -> MlirValue:
-        result = self._ctx.new_value(T)
+        result = self.ctx.new_value(T)
         if isinstance(T, (DigitalMeta, BitsMeta)):
             value = value if value is not None else 0
             hw.ConstantOp(value=int(value), results=[result])
             return result
         if isinstance(T, ArrayMeta):
+            if isinstance(T.T, DigitalMeta):
+                return self.make_constant(Bits[T.N], value)
             value = value if value is not None else (None for _ in range(T.N))
             operands = [self.make_constant(T.T, v) for v in value]
             hw.ArrayCreateOp(operands=operands, results=[result])
             return result
         if isinstance(T, TupleMeta):
             fields = T.field_dict.items()
             value = value if value is not None else {k: None for k, _ in fields}
             operands = [self.make_constant(t, value[k]) for k, t in fields]
             hw.StructCreateOp(operands=operands, results=[result])
             return result
         raise TypeError(T)
 
+    @functools.lru_cache()
+    def make_array_ref(self, arr: MlirValue, i: Union[int, tuple]) -> MlirValue:
+        if isinstance(i, tuple):  # slice
+            start, stop, step = i
+            assert step in [1, None], "Expected step 1 slice"
+            n = stop - start
+        else:
+            start = i
+            n = 1
+
+        if isinstance(arr.type, builtin.IntegerType):
+            operand = self.ctx.new_value(builtin.IntegerType(n))
+            comb.ExtractOp(operands=[arr], results=[operand], lo=start)
+            return operand
+
+        num_sel_bits = clog2(arr.type.dims[0])
+        start = self.make_constant(Bits[num_sel_bits], start)
+
+        if isinstance(i, tuple):
+            operand = self.ctx.new_value(hw.ArrayType((n, ), arr.type.T))
+            hw.ArraySliceOp(operands=[arr, start], results=[operand])
+            return operand
+
+        operand = self.ctx.new_value(arr.type.T)
+        hw.ArrayGetOp(operands=[arr, start], results=[operand])
+        return operand
+
+    def make_concat(self, operands, result):
+        """Collect single elements and put them into an array create op,
+        this allows slices to be concatenated with the surround elements.
+        """
+        T = result.type
+        if isinstance(T, builtin.IntegerType):
+            # comb concat supports single elem/slices
+            return comb.ConcatOp(operands=operands, results=[result])
+        new_operands = []  # packed single elements
+        i = 0
+        while i < len(operands):
+            if i == len(operands):
+                break
+            if operands[i].type != T.T:
+                # Found slice
+                new_operands.append(operands[i])
+                i += 1
+                continue
+
+            # Collect elements until we encounter a slice or the end.
+            elems = []
+            while i < len(operands) and operands[i].type == T.T:
+                elems.append(operands[i])
+                i += 1
+
+            if len(elems) == len(operands):
+                # Found a whole create op
+                return hw.ArrayCreateOp(operands=elems, results=[result])
+
+            # Add create for current elements
+            elems_T = hw.ArrayType((len(elems),), T.T)
+            curr_result = self.ctx.new_value(elems_T)
+            hw.ArrayCreateOp(operands=elems, results=[curr_result])
+            new_operands.append(curr_result)
+
+        hw.ArrayConcatOp(operands=new_operands, results=[result])
+
+    @wrap_with_not_implemented_error
+    def visit_coreir_mem(self, module: ModuleWrapper) -> bool:
+        inst = module.module
+        defn = type(inst)
+        assert (
+            defn.coreir_name == "mem"
+            or defn.coreir_name == "sync_read_mem"
+        )
+        # TODO(rsetaluri): Add support for initialization.
+        if defn.coreir_genargs["has_init"]:
+            raise NotImplementedError("coreir.mem init not supported")
+        width = defn.coreir_genargs["width"]
+        depth = defn.coreir_genargs["depth"]
+        is_sync_read_mem = (defn.coreir_name == "sync_read_mem")
+        raddr, waddr, wdata, clk, wen = module.operands[:5]
+        rdata = module.results[0]
+        mem = make_mem_reg(
+            self._ctx, inst.name, depth, builtin.IntegerType(width)
+        )
+        # Register read logic.
+        read = make_index_op(self._ctx, mem, raddr)
+        read_reg, read_temp = make_mem_read(
+            self._ctx, read, rdata, is_sync_read_mem
+        )
+        # Register write logic.
+        write = make_index_op(self._ctx, mem, waddr)
+        # Always logic.
+        always = sv.AlwaysFFOp(operands=[clk], clock_edge="posedge").body_block
+        with push_block(always):
+            emit_conditional_assign(write, wdata, wen)
+            if is_sync_read_mem:
+                ren = module.operands[-1]
+                emit_conditional_assign(read_reg, read_temp, ren)
+        return True
+
     @wrap_with_not_implemented_error
     def visit_coreir_not(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert defn.coreir_name == "not"
         neg_one = self.make_constant(type(inst.I), -1)
         comb.BaseOp(
@@ -171,15 +427,15 @@
         return True
 
     @wrap_with_not_implemented_error
     def visit_coreir_reg(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert defn.coreir_name == "reg" or defn.coreir_name == "reg_arst"
-        reg = self._ctx.new_value(
+        reg = self.ctx.new_value(
             hw.InOutType(magma_type_to_mlir_type(type(defn.O))))
         sv.RegOp(name=inst.name, results=[reg])
         clock_edge = "posedge"
         has_reset = (defn.coreir_name == "reg_arst")
         operands = [module.operands[1]]
         attrs = dict(clock_edge=clock_edge)
         if has_reset:
@@ -193,16 +449,17 @@
         const = self.make_constant(type(defn.I), init)
         with push_block(always.body_block):
             sv.PAssignOp(operands=[reg, module.operands[0]])
         if has_reset:
             always.operands.append(module.operands[1])
             with push_block(always.reset_block):
                 sv.PAssignOp(operands=[reg, const])
-        with push_block(sv.InitialOp()):
-            sv.BPAssignOp(operands=[reg, const])
+        if not self._ctx.opts.disable_initial_blocks:
+            with push_block(sv.InitialOp()):
+                sv.BPAssignOp(operands=[reg, const])
         sv.ReadInOutOp(operands=[reg], results=module.results.copy())
         return True
 
     @wrap_with_not_implemented_error
     def visit_coreir_reduce(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
@@ -225,28 +482,59 @@
                 operands=module.operands,
                 results=module.results)
         return True
 
     @wrap_with_not_implemented_error
     def visit_coreir_wire(self, module: ModuleWrapper) -> bool:
         inst = module.module
-        mlir_type = hw.InOutType(module.operands[0].type)
-        wire = self._ctx.new_value(mlir_type)
-        sym = self._ctx.parent.get_or_make_mapped_symbol(
-            inst, name=f"{self._ctx.name}.{inst.name}", force=True)
-        sv.WireOp(results=[wire], name=inst.name, sym=sym)
-        sv.AssignOp(operands=[wire, module.operands[0]])
-        sv.ReadInOutOp(operands=[wire], results=module.results)
+
+        def _visit(value, counter):
+            index = next(counter)
+            mlir_type = hw.InOutType(module.operands[index].type)
+            wire = self.ctx.new_value(mlir_type)
+            name = inst.name
+            # TODO(rsetaluri): Making a selector and inspecting it in order to
+            # find the name is a kind of hacky way to get the qualified name of
+            # the sub-field of the value. Instead we should have a common API
+            # (what "qualifiedname" really should be...) to obtain this name.
+            selector = make_selector(value)
+            if isinstance(selector, (TupleSelector, ArraySelector)):
+                name += str(selector).replace(".", "_")
+            else:
+                assert index == 0
+            sym = self._ctx.parent.get_or_make_mapped_symbol(
+                value, name=f"{self._ctx.name}.{name}", force=True
+            )
+            sv.WireOp(results=[wire], name=name, sym=sym)
+            sv.AssignOp(operands=[wire, module.operands[index]])
+            sv.ReadInOutOp(operands=[wire], results=[module.results[index]])
+
+        counter = itertools.count()
+        visit_magma_value_or_value_wrapper_by_direction(
+            inst.I,
+            lambda v: _visit(v, counter),
+            assert_false,
+            flatten_all_tuples=self._ctx.opts.flatten_all_tuples,
+        )
         return True
 
     @wrap_with_not_implemented_error
     def visit_coreir_primitive(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
-        assert (defn.coreir_lib == "coreir" or defn.coreir_lib == "corebit")
+        assert (
+            defn.coreir_lib == "coreir"
+            or defn.coreir_lib == "corebit"
+            or defn.coreir_lib == "memory"
+        )
+        if (
+            defn.coreir_name == "mem"
+            or defn.coreir_name == "sync_read_mem"
+        ):
+            return self.visit_coreir_mem(module)
         if defn.coreir_name == "not":
             return self.visit_coreir_not(module)
         if defn.coreir_name in (
                 "eq", "ult", "eq", "ne", "slt", "sle", "sgt", "sge", "ult",
                 "ule", "ugt", "uge",
         ):
             comb.ICmpOp(
@@ -260,32 +548,58 @@
             return self.visit_coreir_reduce(module)
         if defn.coreir_name == "wire":
             return self.visit_coreir_wire(module)
         if defn.coreir_name == "wrap":
             return self.visit_coreir_wire(module)
         if defn.coreir_name == "term":
             return True
+        if defn.coreir_name == "undriven":
+            mlir_type = hw.InOutType(module.results[0].type)
+            wire = self.ctx.new_value(mlir_type)
+            sym = self._ctx.parent.get_or_make_mapped_symbol(
+                inst, name=f"{self._ctx.name}.{inst.name}", force=True)
+            sv.WireOp(results=[wire], sym=sym)
+            sv.ReadInOutOp(operands=[wire], results=module.results)
+            return True
+        if defn.coreir_name == "neg":
+            zero = self.make_constant(type(inst.I), 0)
+            comb.BaseOp(
+                op_name="sub",
+                operands=[zero, module.operands[0]],
+                results=module.results)
+            return True
         op_name = defn.coreir_name
         if op_name == "ashr":
             op_name = "shrs"
         if op_name == "lshr":
             op_name = "shru"
+        if op_name == "udiv":
+            op_name = "divu"
+        if op_name == "sdiv":
+            op_name = "divs"
         comb.BaseOp(
             op_name=op_name,
             operands=module.operands,
             results=module.results)
         return True
 
     @wrap_with_not_implemented_error
     def visit_muxn(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert defn.coreir_name == "muxn"
-        data = self._ctx.new_value(defn.I.data)
-        sel = self._ctx.new_value(defn.I.sel)
+        data = self.ctx.new_value(defn.I.data)
+        sel = self.ctx.new_value(defn.I.sel)
+        # NOTE(rsetaluri): This is a specialized code path for the case where
+        # all tuples are flattened.
+        if self._ctx.opts.flatten_all_tuples:
+            hw.ArrayGetOp(
+                operands=module.operands.copy(),
+                results=module.results.copy())
+            return True
         hw.StructExtractOp(
             field="data",
             operands=module.operands.copy(),
             results=[data])
         hw.StructExtractOp(
             field="sel",
             operands=module.operands.copy(),
@@ -297,17 +611,17 @@
 
     @wrap_with_not_implemented_error
     def visit_lutN(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert defn.coreir_name == "lutN"
         init = defn.coreir_configargs["init"]
-        consts = [self.make_constant(Bit, b) for b in init]
+        consts = [self.make_constant(Bit, b) for b in reversed(init)]
         mlir_type = hw.ArrayType((len(init),), builtin.IntegerType(1))
-        array = self._ctx.new_value(mlir_type)
+        array = self.ctx.new_value(mlir_type)
         hw.ArrayCreateOp(
             operands=consts,
             results=array)
         hw.ArrayGetOp(
             operands=[array, module.operands[0]],
             results=module.results)
         return True
@@ -336,98 +650,238 @@
         # using an i1 constant.
         # TODO(rsetaluri): Figure out how to emit hw.array_get for
         # !hw.array_type<1x_> types.
         if size == 1:
             assert index == 0
             other = self.make_constant(T)
             concat_type = hw.ArrayType((2,), operands[0].type.T)
-            concat = self._ctx.new_value(concat_type)
+            concat = self.ctx.new_value(concat_type)
             hw.ArrayConcatOp(
-                operands=[operands[0], other],
+                operands=[other, operands[0]],
                 results=[concat])
             operands = [concat]
             size = 2
         num_sel_bits = clog2(size)
         index = self.make_constant(Bits[num_sel_bits], index)
         hw.ArrayGetOp(
             operands=(operands + [index]),
             results=module.results)
         return True
 
     @wrap_with_not_implemented_error
+    def visit_array_slice(self, module: ModuleWrapper) -> bool:
+        inst_wrapper = module.module
+        T = inst_wrapper.attrs["T"]
+        size = T.N
+        operands = module.operands
+        lo = inst_wrapper.attrs["lo"]
+        num_sel_bits = clog2(size)
+        lo = self.make_constant(Bits[num_sel_bits], lo)
+        hw.ArraySliceOp(
+            operands=(operands + [lo]),
+            results=module.results)
+        return True
+
+    @wrap_with_not_implemented_error
+    def visit_when(self, module: ModuleWrapper) -> bool:
+        return WhenCompiler(self, module).compile()
+
+    @wrap_with_not_implemented_error
+    def visit_multiport_memory(self, module: ModuleWrapper) -> bool:
+        inst = module.module
+        defn = type(inst)
+        clk = module.operands[0]
+        read_ports_out = module.results
+        read_port_len = 1 + defn.has_read_enable
+        read_ports = collect_multiport_memory_operands(
+            module.operands, 1, defn.num_read_ports, read_port_len
+        )
+        write_ports = collect_multiport_memory_operands(
+            module.operands,
+            1 + defn.num_read_ports * read_port_len,
+            defn.num_write_ports,
+            3
+        )
+        elt_type = hw.InOutType(magma_type_to_mlir_type(defn.T))
+        mem = make_mem_reg(self._ctx, inst.name, defn.height, elt_type.T)
+        read_results = make_multiport_memory_index_ops(
+            self._ctx, read_ports, mem
+        )
+        read_targets = make_multiport_memory_read_ops(
+            self._ctx, read_results, read_ports, read_ports_out
+        )
+        write_results = make_multiport_memory_index_ops(
+            self._ctx, write_ports, mem
+        )
+        write_targets = (
+            (write_results[i], *write_ports[i][1:3])
+            for i in range(len(write_results))
+        )
+        always = sv.AlwaysFFOp(operands=[clk], clock_edge="posedge").body_block
+        with push_block(always):
+            emit_conditional_assigns(write_targets)
+            if len(read_targets):
+                emit_conditional_assigns(read_targets)
+        return True
+
+    @wrap_with_not_implemented_error
     def visit_primitive(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert isprimitive(defn)
-        if defn.coreir_lib == "coreir" or defn.coreir_lib == "corebit":
+        if (
+            defn.coreir_lib == "coreir"
+            or defn.coreir_lib == "corebit"
+            or defn.coreir_lib == "memory"
+        ):
             return self.visit_coreir_primitive(module)
         if defn.coreir_lib == "commonlib":
             return self.visit_commonlib_primitive(module)
+        if isinstance(defn, MultiportMemory):
+            return self.visit_multiport_memory(module)
+        if isinstance(defn, InlineVerilogExpression):
+            assert len(module.operands) == 0
+            assert len(module.results) > 0
+            sv.VerbatimExprOp(
+                operands=list(),
+                results=module.results,
+                expr=defn.expr,
+            )
+            return True
+        if isinstance(defn, InlineVerilog2):
+            sv.VerbatimOp(string=defn.expr, operands=module.operands)
+            return True
+        if iswhen(defn):
+            return self.visit_when(module)
+
+    @wrap_with_not_implemented_error
+    def visit_magma_wire(self, module: ModuleWrapper) -> bool:
+        inst = module.module
+        defn = type(inst)
+        assert isinstance(defn, Wire) and not defn.flattened
+        return self.visit_coreir_wire(module)
 
     @wrap_with_not_implemented_error
     def visit_magma_mux(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         assert isinstance(defn, Mux)
         # NOTE(rsetaluri): This is a round-about way to get the height while
         # magma.Mux does not store those parameters. That should be fixed in
         # magma/primitives/mux.py.
         height = len(list(filter(
             lambda p: "I" in p.name.name, defn.interface.outputs())))
-        T = type(defn.I0)
-        mlir_type = hw.ArrayType((height,), magma_type_to_mlir_type(T))
-        array = self._ctx.new_value(mlir_type)
-        hw.ArrayCreateOp(
-            operands=module.operands[:-1],
-            results=[array])
-        hw.ArrayGetOp(
-            operands=[array, module.operands[-1]],
-            results=module.results)
+        data, select = module.operands[:-1], module.operands[-1]
+        # NOTE(rsetaluri): This is a specialized code path for the case where
+        # all tuples are flattened.
+        if self._ctx.opts.flatten_all_tuples and len(data) != height:
+            assert len(data) % height == 0
+            stride = len(data) // height
+            assert len(module.results) == stride
+            for i in range(stride):
+                inputs = list(reversed(data[i::stride]))
+                make_mux(self._ctx, inputs, select, module.results[i])
+            return True
+        # NOTE(rsetaluri): Reversing data needs to be done *after* we check for
+        # tuple flattening. Otherwise the tuple field ordering gets reversed as
+        # well.
+        data = list(reversed(data))
+        make_mux(self._ctx, data, select, module.results[0])
         return True
 
     @wrap_with_not_implemented_error
     def visit_magma_register(self, module: ModuleWrapper) -> bool:
+        # NOTE(rsetaluri): Refactoring this compilation into the make_register
+        # and get_register_data_and_init functions is necessary to support
+        # flatten_all_tuples=True. make_register works for arbitrary types of
+        # inputs, so we can either invoke it once for the top-level type or call
+        # it on all flattened parts. get_register_data_and_init associates the
+        # operands with init values (and magma type), so that flattened and
+        # unflattened tuples can be treated uniformly.
+
+        def make_register(T, data, init, result):
+            reg = self.ctx.new_value(hw.InOutType(data.type))
+            sv.RegOp(name=inst.name, results=[reg])
+            always = sv.AlwaysFFOp(operands=always_operands, **attrs)
+            const = self.make_constant(T, init)
+            with push_block(always.body_block):
+                ctx = contextlib.nullcontext()
+                if has_enable:
+                    ctx = push_block(sv.IfOp(operands=[enable]).then_block)
+                with ctx:
+                    sv.PAssignOp(operands=[reg, data])
+            if has_reset:
+                with push_block(always.reset_block):
+                    sv.PAssignOp(operands=[reg, const])
+            if not self._ctx.opts.disable_initial_blocks:
+                with push_block(sv.InitialOp()):
+                    sv.BPAssignOp(operands=[reg, const])
+            sv.ReadInOutOp(operands=[reg], results=[result])
+
         inst = module.module
         defn = type(inst)
-        reg = self._ctx.new_value(
-            hw.InOutType(magma_type_to_mlir_type(type(defn.O))))
-        sv.RegOp(name=inst.name, results=[reg])
         clock_edge = "posedge"
         has_reset = defn.reset_type is not None
         # NOTE(resetaluri): This is a hack until
         # magma/primitives/register.py:Register is updated to store this
         # generator parameter directly.
         has_enable = "CE" in defn.interface.ports
-        data = module.operands[0]
+        operands = module.operands.copy()
+        T, data, init = get_register_data_and_init(
+            self._ctx, defn.I, operands, defn.init)
+        assert len(data) == len(init)
+        assert len(data) == len(T)
+        assert len(data) == len(module.results)
         if has_enable:
-            enable = module.operands[1]
-            clk = module.operands[2]
+            enable = operands[0]
+            clk = operands[1]
         else:
-            clk = module.operands[1]
+            clk = operands[0]
         always_operands = [clk]
         attrs = dict(clock_edge=clock_edge)
         if has_reset:
-            reset = module.operands[-1]
+            reset = operands[-1]
             always_operands.append(reset)
             reset_type, reset_edge = parse_reset_type(defn.reset_type)
             attrs.update(dict(reset_type=reset_type, reset_edge=reset_edge))
-        always = sv.AlwaysFFOp(operands=always_operands, **attrs)
-        const = self.make_constant(type(defn.I), defn.init)
-        with push_block(always.body_block):
-            ctx = contextlib.nullcontext()
-            if has_enable:
-                ctx = push_block(sv.IfOp(operands=[enable]).then_block)
-            with ctx:
-                sv.PAssignOp(operands=[reg, data])
-        if has_reset:
-            with push_block(always.reset_block):
-                sv.PAssignOp(operands=[reg, const])
-        with push_block(sv.InitialOp()):
-            sv.BPAssignOp(operands=[reg, const])
-        sv.ReadInOutOp(operands=[reg], results=module.results.copy())
+        for T_i, data_i, init_i, result_i in zip(T, data, init, module.results):
+            make_register(T_i, data_i, init_i, result_i)
+        return True
+
+    @wrap_with_not_implemented_error
+    def visit_magma_xmr_sink(self, module: ModuleWrapper) -> bool:
+        inst = module.module
+        defn = type(inst)
+        assert isinstance(defn, XMRSink)
+        xmr = defn.value
+        try:
+            self._ctx.parent.xmr_paths[xmr]
+        except KeyError:
+            pass
+        else:
+            return True
+        paths = get_xmr_paths(self._ctx, xmr)
+        assert len(paths) == len(module.operands)
+        self._ctx.parent.xmr_paths[xmr] = paths
+        return True
+
+    @wrap_with_not_implemented_error
+    def visit_magma_xmr_source(self, module: ModuleWrapper) -> bool:
+        inst = module.module
+        defn = type(inst)
+        assert isinstance(defn, XMRSource)
+        xmr = defn.value
+        paths = self._ctx.parent.xmr_paths[xmr]
+        assert len(paths) == len(module.results)
+        base = defn.value.parent_view.path()
+        for result, path in zip(module.results, paths):
+            in_out = self.ctx.new_value(hw.InOutType(result.type))
+            path = base + path
+            sv.XMROp(is_rooted=False, path=path, results=[in_out])
+            sv.ReadInOutOp(operands=[in_out], results=[result])
         return True
 
     @wrap_with_not_implemented_error
     def visit_inline_verilog(self, module: ModuleWrapper) -> bool:
         inst = module.module
         defn = type(inst)
         inline_verilog_strs = defn.inline_verilog_strs
@@ -452,31 +906,51 @@
         return True
 
     @wrap_with_not_implemented_error
     def visit_instance(self, module: ModuleWrapper) -> bool:
         inst = module.module
         assert isinstance(inst, AnonymousCircuitType)
         defn = type(inst)
+        elaborate_magma_registers = self._ctx.opts.elaborate_magma_registers
+        if isinstance(defn, Wire) and not defn.flattened:
+            return self.visit_magma_wire(module)
         if isinstance(defn, Mux):
             return self.visit_magma_mux(module)
-        if isinstance(defn, Register):
+        if isinstance(defn, Register) and not elaborate_magma_registers:
             return self.visit_magma_register(module)
+        if isinstance(defn, XMRSink):
+            return self.visit_magma_xmr_sink(module)
+        if isinstance(defn, XMRSource):
+            return self.visit_magma_xmr_source(module)
         if getattr(defn, "inline_verilog_strs", []):
             return self.visit_inline_verilog(module)
         if isprimitive(defn):
             return self.visit_primitive(module)
         module_type = self._ctx.parent.get_hardware_module(defn).hw_module
-        metadata = getattr(inst, "coreir_metadata", {})
-        compile_guard = metadata.get("compile_guard", None)
+        parameters = filter_by_key(
+            lambda key: key not in ["name", "locl"],
+            inst.kwargs
+        )
+        compile_guard = get_compile_guard_data(inst)
+        sym = None
+        attrs = {}
+        if is_bound_instance(inst):
+            sym = self._ctx.parent.get_or_make_mapped_symbol(
+                inst, name=f"{inst.defn.name}.{inst.name}", force=True
+            )
+            attrs["doNotPrint"] = builtin.BoolAttr(True)
         make_hw_instance_op(
             name=inst.name,
             module=module_type,
             operands=module.operands,
             results=module.results,
-            compile_guard=compile_guard)
+            sym=sym,
+            parameters=parameters,
+            compile_guard=compile_guard,
+            attrs=attrs)
         return True
 
     @wrap_with_not_implemented_error
     def visit_instance_wrapper(self, module: ModuleWrapper) -> bool:
         inst_wrapper = module.module
         assert isinstance(inst_wrapper, MagmaInstanceWrapper)
         if inst_wrapper.name.startswith("magma_array_get_op_"):
@@ -484,27 +958,34 @@
             if isinstance(T, BitsMeta) or issubclass(T.T, Bit):
                 comb.ExtractOp(
                     operands=module.operands,
                     results=module.results,
                     lo=inst_wrapper.attrs["index"])
                 return True
             return self.visit_array_get(module)
-        if inst_wrapper.name.startswith("magma_array_create_op"):
+        if inst_wrapper.name.startswith("magma_array_slice_op_"):
             T = inst_wrapper.attrs["T"]
             if isinstance(T, BitsMeta) or issubclass(T.T, Bit):
-                comb.ConcatOp(
-                    operands=list(reversed(module.operands)),
-                    results=module.results)
+                comb.ExtractOp(
+                    operands=module.operands,
+                    results=module.results,
+                    lo=inst_wrapper.attrs["lo"])
                 return True
-            hw.ArrayCreateOp(
-                operands=list(reversed(module.operands)),
-                results=module.results)
+            return self.visit_array_slice(module)
+        if inst_wrapper.name.startswith("magma_array_create_op"):
+            self.make_concat(
+                list(reversed(module.operands)),
+                module.results[0]
+            )
             return True
         if inst_wrapper.name.startswith("magma_tuple_get_op"):
-            index = inst_wrapper.attrs["index"]
+            index = magma_tuple_key_to_str(
+                inst_wrapper.attrs["index"],
+                inst_wrapper.attrs["T"]
+            )
             hw.StructExtractOp(
                 field=index,
                 operands=module.operands,
                 results=module.results)
             return True
         if inst_wrapper.name.startswith("magma_tuple_create_op"):
             hw.StructCreateOp(
@@ -520,47 +1001,57 @@
             return True
 
     @wrap_with_not_implemented_error
     def visit_module(self, module: ModuleWrapper) -> bool:
         if isinstance(module.module, DefineCircuitKind):
             return True
         if isinstance(module.module, AnonymousCircuitType):
-            return self.visit_instance(module)
+            with push_location(_make_location_info(module.module.debug_info)):
+                return self.visit_instance(module)
         if isinstance(module.module, MagmaInstanceWrapper):
             return self.visit_instance_wrapper(module)
 
-    def visit(self, module: MagmaModuleLike):
-        if module in self._visited:
-            raise RuntimeError(f"Can not re-visit module")
-        self._visited.add(module)
-        for predecessor in self._graph.predecessors(module):
+    def _process_magma_module(self, magma_module: MagmaModuleLike):
+        if not self._graph.has_node(magma_module):
+            return
+        for predecessor in self._graph.predecessors(magma_module):
             if predecessor in self._visited:
                 continue
             self.visit(predecessor)
-        for src, _, data in self._graph.in_edges(module, data=True):
+        for src, _, data in self._graph.in_edges(magma_module, data=True):
             info = data["info"]
             src_port, dst_port = info["src"], info["dst"]
             src_value = self._ctx.get_or_make_mapped_value(src_port)
             self._ctx.set_mapped_value(dst_port, src_value)
-        assert self.visit_module(ModuleWrapper.make(module, self._ctx))
+
+    def visit(self, module: MagmaModuleLike):
+        if module in self._visited:
+            raise ModuleVisitor.RevisitedModuleError(module)
+        self._visited.add(module)
+        self._process_magma_module(module)
+        self.visit_module(ModuleWrapper.make(module, self._ctx))
         instances = getattr(module, "instances", [])
         for inst in instances:
             if inst in self._visited:
                 continue
             self.visit(inst)
 
 
-def treat_as_primitive(defn_or_decl: CircuitKind) -> bool:
+def treat_as_primitive(
+        defn_or_decl: CircuitKind,
+        ctx: 'HardwareModule'
+) -> bool:
     # NOTE(rsetaluri): This is a round-about way to mark new types as
     # primitives. These definitions should actually be marked as primitives.
+    elaborate_magma_registers = ctx.opts.elaborate_magma_registers
     if isprimitive(defn_or_decl):
         return True
     if isinstance(defn_or_decl, Mux):
         return True
-    if isinstance(defn_or_decl, Register):
+    if isinstance(defn_or_decl, Register) and not elaborate_magma_registers:
         return True
     if getattr(defn_or_decl, "inline_verilog_strs", []):
         return True
     return False
 
 
 def treat_as_definition(defn_or_decl: CircuitKind) -> bool:
@@ -569,82 +1060,182 @@
     if getattr(defn_or_decl, "verilog", ""):
         return False
     if getattr(defn_or_decl, "verilogFile", ""):
         return False
     return True
 
 
-class BindProcessor:
-    def __init__(self, ctx, defn: CircuitKind):
+class BindProcessorInterface(abc.ABC):
+    def __init__(self, ctx: 'HardwareModule', defn: CircuitKind):
         self._ctx = ctx
         self._defn = defn
 
+    @abc.abstractmethod
+    def preprocess(self):
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def process(self):
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def postprocess(self):
+        raise NotImplementedError()
+
+
+class NativeBindProcessor(BindProcessorInterface):
     def preprocess(self):
         for bind_module in self._defn.bind_modules:
             # TODO(rsetaluri): Here we should check if @bind_module has already
             # been compiled, in the case that the bound module is either used
             # multiple times or is also a "normal" module that was compiled
             # elsewhere. Currently, the `set_hardware_module` call will raise an
             # error if @bind_module has been compiled already.
             hardware_module = self._ctx.parent.new_hardware_module(bind_module)
             hardware_module.compile()
             assert hardware_module.hw_module is not None
-            self._ctx.parent.set_hardware_module(
-                bind_module, hardware_module.hw_module)
+            self._ctx.parent.set_hardware_module(bind_module, hardware_module)
+
+    @wrap_with_not_implemented_error
+    def _resolve_arg(self, arg) -> MlirValue:
+        if isinstance(arg, Type):
+            return self._ctx.get_mapped_value(arg)
+        if isinstance(arg, PortView):
+            return resolve_xmr(self._ctx, arg)
 
     def process(self):
         self._syms = []
         for bind_module, (args, _) in self._defn.bind_modules.items():
-            operands = [
-                self._ctx.get_mapped_value(p)
-                for p in self._defn.interface.ports.values()
-            ]
-            for arg in args:
-                operands.append(self._ctx.get_mapped_value(arg))
+            operands = []
+            for port in self._defn.interface.ports.values():
+                port = get_magma_value(port)
+                visit_magma_value_or_value_wrapper_by_direction(
+                    port,
+                    lambda p: operands.append(self._ctx.get_mapped_value(p)),
+                    lambda p: operands.append(self._ctx.get_mapped_value(p)),
+                    flatten_all_tuples=self._ctx.opts.flatten_all_tuples,
+                )
+            operands += list(map(self._resolve_arg, args))
             inst_name = f"{bind_module.name}_inst"
             sym = self._ctx.parent.get_or_make_mapped_symbol(
                 (self._defn, bind_module),
                 name=f"{self._defn.name}.{inst_name}",
                 force=True)
             module = self._ctx.parent.get_hardware_module(bind_module)
             inst = hw.InstanceOp(
                 name=inst_name,
-                module=module,
+                module=module.hw_module,
                 operands=operands,
                 results=[],
                 sym=sym)
-            inst.attr_dict["doNotPrint"] = 1
+            inst.attr_dict["doNotPrint"] = builtin.BoolAttr(True)
             self._syms.append(sym)
 
-    def post_process(self):
+    def postprocess(self):
         defn_sym = self._ctx.parent.get_mapped_symbol(self._defn)
         for sym in self._syms:
             instance = hw.InnerRefAttr(defn_sym, sym)
             sv.BindOp(instance=instance)
+        bound_instances = list(filter(is_bound_instance, self._defn.instances))
+        for bound_instance in bound_instances:
+            inst_sym = self._ctx.parent.get_mapped_symbol(bound_instance)
+            ref = hw.InnerRefAttr(defn_sym, inst_sym)
+            sv.BindOp(instance=ref)
+
+
+class CoreIRBindProcessor(BindProcessorInterface):
+    def preprocess(self):
+        return
+
+    def process(self):
+        for name, content in self._defn.compiled_bind_modules.items():
+            path = pathlib.Path(self._ctx.opts.basename).parent
+            filename = path / f"{name}.sv"
+            with open(filename, "w") as f:
+                f.write(content)
+            self._ctx.parent.add_external_bind_file(filename.name)
+
+    def postprocess(self):
+        return
+
+
+def _make_bind_processor(ctx: 'HardwareModule', defn: CircuitKind):
+    if ctx.opts.use_native_bind_processor:
+        return NativeBindProcessor(ctx, defn)
+    return CoreIRBindProcessor(ctx, defn)
+
+
+def _visit_linked_module(
+        ctx: 'HardwareModule', decl: CircuitKind, op: hw.ModuleOp):
+    # In order to emit a linked module, we perform the following steps:
+    #   (1) Declare a wire for each output of the module.
+    #   (2) For each linked module, first enter an `ifdef block.
+    #       (a) Instantiate the linked target.
+    #       (b) Assign the wires with the outputs of the instance.
+    #       (c) Enter the `else of the `ifdef block.
+    #   (3) If we have a default link target, perform (2a-b).
+    module = ModuleWrapper.make(decl, ctx)
+    wires = {
+        output: ctx.new_value(hw.InOutType(output.type))
+        for output in module.operands
+    }
+
+    def _process_target(defn):
+        hw_module = ctx.parent.get_hardware_module(defn).hw_module
+        results = [ctx.new_value(output.type) for output in module.operands]
+        make_hw_instance_op(
+            name=f"{defn.name}_inst",
+            module=hw_module,
+            operands=module.results,
+            results=results,
+        )
+        for result, wire in zip(results, wires.values()):
+            sv.AssignOp(operands=[wire, result])
+
+    with push_block(op):
+        for output, wire in wires.items():
+            sv.WireOp(results=[wire])
+            sv.ReadInOutOp(operands=[wire], results=[output])
+        with contextlib.ExitStack() as stack:
+            for key, linked_module in get_linked_modules(decl).items():
+                if_def = sv.IfDefOp(key)
+                stack.enter_context(push_block(if_def.then_block))
+                _process_target(linked_module)
+                stack.enter_context(push_block(if_def.else_block))
+            if has_default_linked_module(decl):
+                default_linked_module = get_default_linked_module(decl)
+                _process_target(default_linked_module)
+        hw.OutputOp(operands=module.operands)
+    return op
 
 
 class HardwareModule:
     def __init__(
             self, magma_defn_or_decl: CircuitKind,
-            parent: weakref.ReferenceType):
+            parent: weakref.ReferenceType, opts: CompileToMlirOpts):
         self._magma_defn_or_decl = magma_defn_or_decl
         self._parent = parent
+        self._opts = opts
         self._hw_module = None
-        self._name_gen = ScopedNameGenerator()
+        self._name_gen = ScopedNameGenerator(disallow_duplicates=False)
         self._value_map = {}
 
     @property
     def magma_defn_or_decl(self) -> CircuitKind:
         return self._magma_defn_or_decl
 
     @property
     def parent(self):
         return self._parent()
 
     @property
+    def opts(self) -> CompileToMlirOpts:
+        return self._opts
+
+    @property
     def hw_module(self) -> hw.ModuleOpBase:
         return self._hw_module
 
     @property
     def name(self) -> str:
         return self._magma_defn_or_decl.name
 
@@ -678,49 +1269,85 @@
         else:
             raise TypeError(value_or_type)
         name = self._name_gen(**kwargs)
         return MlirValue(mlir_type, name)
 
     def compile(self):
         self._hw_module = self._compile()
+        if self._hw_module is None:
+            return
+        self._add_module_parameters(self._hw_module)
+        _maybe_set_location_info(
+            self._hw_module,
+            self._magma_defn_or_decl.debug_info
+        )
 
     def _compile(self) -> hw.ModuleOpBase:
-        if treat_as_primitive(self._magma_defn_or_decl):
+        if treat_as_primitive(self._magma_defn_or_decl, self):
             return
 
         def new_values(fn, ports):
             namer = magma_value_or_type_to_string
-            return [fn(port, name=namer(port), force=True) for port in ports]
+            return [
+                fn(port, name=namer(port), force=True)
+                for port in map(get_magma_value, ports)
+            ]
 
         i, o = [], []
         for port in self._magma_defn_or_decl.interface.ports.values():
+            port = get_magma_value(port)
             visit_magma_value_or_value_wrapper_by_direction(
-                port, i.append, o.append
+                port, i.append, o.append,
+                flatten_all_tuples=self._opts.flatten_all_tuples,
             )
         inputs = new_values(self.get_or_make_mapped_value, o)
         named_outputs = new_values(self.new_value, i)
         defn_or_decl_output_name = _get_defn_or_decl_output_name(
-            self._magma_defn_or_decl)
+            self, self._magma_defn_or_decl)
         name = self.parent.get_or_make_mapped_symbol(
             self._magma_defn_or_decl,
             name=defn_or_decl_output_name, force=True)
+        if has_any_linked_modules(self._magma_defn_or_decl):
+            op = hw.ModuleOp(
+                name=name,
+                operands=inputs,
+                results=named_outputs,
+            )
+            return _visit_linked_module(self, self._magma_defn_or_decl, op)
         if not treat_as_definition(self._magma_defn_or_decl):
             return hw.ModuleExternOp(
                 name=name,
                 operands=inputs,
                 results=named_outputs)
-        bind_processor = BindProcessor(self, self._magma_defn_or_decl)
+        bind_processor = _make_bind_processor(self, self._magma_defn_or_decl)
         bind_processor.preprocess()
         op = hw.ModuleOp(
             name=name,
             operands=inputs,
             results=named_outputs)
-        graph = build_magma_graph(self._magma_defn_or_decl)
+        build_magma_graph_opts = BuildMagmaGrahOpts(
+            self._opts.flatten_all_tuples)
+        graph = build_magma_graph(
+            self._magma_defn_or_decl, build_magma_graph_opts)
         visitor = ModuleVisitor(graph, self)
         with push_block(op):
-            visitor.visit(self._magma_defn_or_decl)
+            try:
+                visitor.visit(self._magma_defn_or_decl)
+            except ModuleVisitor.VisitError:
+                raise MlirCompilerInternalError(visitor)
             bind_processor.process()
             output_values = new_values(self.get_or_make_mapped_value, i)
             if named_outputs:
                 hw.OutputOp(operands=output_values)
-        bind_processor.post_process()
+        bind_processor.postprocess()
         return op
+
+    def _add_module_parameters(self, hw_module: hw.ModuleOpBase):
+        defn_or_decl = self._magma_defn_or_decl
+        try:
+            param_types = defn_or_decl.coreir_config_param_types
+        except AttributeError:
+            return
+        for name, type in param_types.items():
+            type = python_type_to_mlir_type(type)
+            param = hw.ParamDeclAttr(name, type)
+            hw_module.parameters.append(param)
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/magma_common.py` & `magma-lang-2.3.0/magma/backend/mlir/magma_common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import dataclasses
 from typing import Any, Callable, Iterable, Mapping, Union
 
 from magma.array import Array, ArrayMeta
-from magma.backend.mlir.common import make_unique_name, replace_all
+from magma.backend.mlir.common import make_unique_name
+from magma.backend.mlir.graph_lib import Graph
 from magma.circuit import Circuit, DefineCircuitKind
+from magma.common import replace_all, Stack, SimpleCounter
 from magma.ref import Ref, ArrayRef, TupleRef
 from magma.t import Kind, Type
-from magma.tuple import TupleMeta, Tuple as m_Tuple
+from magma.tuple import TupleMeta, Tuple as m_Tuple, AnonProduct
 
 
 ModuleLike = Union[DefineCircuitKind, Circuit]
 
 
 _VALUE_OR_TYPE_TO_STRING_REPLACEMENTS = {
     "(": "_",
@@ -20,22 +22,39 @@
     " ": "",
     ",": "_",
     "=": "_",
     ".": "_",
 }
 
 
+def contains_tuple(T: Kind):
+    if isinstance(T, TupleMeta):
+        return True
+    if isinstance(T, ArrayMeta):
+        return contains_tuple(T.T)
+    return False
+
+
 def value_or_type_to_string(value_or_type: Union[Type, Kind]):
     if isinstance(value_or_type, Type):
         s = value_or_type.name.qualifiedname("_")
     else:
         s = str(value_or_type)
     return replace_all(s, _VALUE_OR_TYPE_TO_STRING_REPLACEMENTS)
 
 
+def tuple_key_to_str(key: Union[str, int], T: TupleMeta) -> str:
+    # NOTE(rsetaluri): If the type is Tuple (i.e. has integer keys), then the
+    # struct type we emit should prefix the field key with an underscore
+    # (e.g. "_0") to make it a valid keyword.
+    if issubclass(T, AnonProduct):
+        return str(key)
+    return f"_{key}"
+
+
 @dataclasses.dataclass(frozen=True)
 class ValueWrapper:
     id: str = dataclasses.field(default_factory=make_unique_name, init=False)
     name: str
     T: Kind
 
     def is_input(self) -> bool:
@@ -60,29 +79,80 @@
             )
         raise NotImplementedError(f"{self} is not iterable")
 
 
 ValueOrValueWrapper = Union[Type, ValueWrapper]
 
 
+def value_or_value_wrapper_to_tree(
+        value_or_value_wrapper: ValueOrValueWrapper,
+        flatten_all_tuples: bool = False) -> Graph:
+    tree = Graph()
+    state = Stack()
+    index = SimpleCounter()
+
+    def _visit_leaf(v):
+        tree.add_node(v, index=index.next())
+        if not state:
+            return
+        tree.add_edge(state.peek(), v)
+
+    def _pre_descend(v):
+        tree.add_node(v, index=index.next())
+        if state:
+            tree.add_edge(state.peek(), v)
+        state.push(v)
+
+    def _post_descend(v):
+        assert state.pop() is v
+
+    visit_value_or_value_wrapper_by_direction(
+        value_or_value_wrapper,
+        _visit_leaf,
+        _visit_leaf,
+        flatten_all_tuples=flatten_all_tuples,
+        pre_descend=_pre_descend,
+        post_descend=_post_descend,
+    )
+
+    return tree
+
+
 def visit_value_or_value_wrapper_by_direction(
         value_or_value_wrapper: ValueOrValueWrapper,
         input_visitor: Callable[[Type], Any],
-        output_visitor: Callable[[Type], Any]):
+        output_visitor: Callable[[Type], Any],
+        **kwargs):
+
+    pre_descend = kwargs.get("pre_descend", lambda _: None)
+    post_descend = kwargs.get("post_descend", lambda _: None)
+    inout_visitor = kwargs.get("inout_visitor", None)
+
+    def descend(v):
+        if not isinstance(v, (m_Tuple, Array)):
+            raise TypeError(v)
+        pre_descend(v)
+        for item in v:
+            visit_value_or_value_wrapper_by_direction(
+                item, input_visitor, output_visitor, **kwargs)
+        post_descend(v)
+
+    flatten_all_tuples = kwargs.get("flatten_all_tuples", False)
+
+    if flatten_all_tuples and contains_tuple(type(value_or_value_wrapper)):
+        return descend(value_or_value_wrapper)
     if value_or_value_wrapper.is_input():
         return input_visitor(value_or_value_wrapper)
     if value_or_value_wrapper.is_output():
         return output_visitor(value_or_value_wrapper)
     if value_or_value_wrapper.is_mixed():
-        if isinstance(value_or_value_wrapper, (m_Tuple, Array)):
-            for item in value_or_value_wrapper:
-                visit_value_or_value_wrapper_by_direction(
-                    item, input_visitor, output_visitor
-                )
-            return
+        return descend(value_or_value_wrapper)
+    if inout_visitor is not None:
+        return inout_visitor(value_or_value_wrapper)
+
     raise TypeError(value_or_value_wrapper)
 
 
 class InstanceWrapper:
 
     @dataclasses.dataclass(frozen=True)
     class _Interface:
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/magma_ops.py` & `magma-lang-2.3.0/magma/backend/mlir/magma_ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 from typing import Union
 
-from magma.array import ArrayMeta
+from magma.array import ArrayMeta, Array
 from magma.backend.mlir.magma_common import (
     InstanceWrapper, value_or_type_to_string)
 from magma.bits import BitsMeta
 from magma.digital import DigitalMeta
 from magma.generator import Generator2
 from magma.interface import IO
 from magma.t import In, Out
-from magma.tuple import TupleMeta, ProductMeta
+from magma.tuple import TupleMeta, AnonymousProductMeta
 
 
 def _get_tuple_field_type(T: TupleMeta, index: Union[int, str]):
-    if isinstance(T, ProductMeta):
+    if isinstance(T, AnonymousProductMeta):
         return T.field_dict[index]
     index = int(index)
     return T.field_dict[index]
 
 
-def MagmaArrayGetOp(T: ArrayMeta, index: str):
+def _resized_array(T: ArrayMeta, new_size: int):
+    if isinstance(T, BitsMeta):
+        return T.unsized_t[new_size]
+    return T[new_size, T.T]
+
+
+def MagmaArrayGetOp(T: ArrayMeta, index: int):
     assert isinstance(T, ArrayMeta)
     T = T.undirected_t
     name = f"magma_array_get_op_{value_or_type_to_string(T)}"
     T_out = T.T
     ports = dict(I=In(T), O=Out(T_out))
     attrs = dict(T=T, index=index)
     return InstanceWrapper(name, ports, attrs)
 
 
-class MagmaArraySliceOp(Generator2):
-    def __init__(self, T: ArrayMeta, lo: int, hi: int):
-        assert isinstance(T, ArrayMeta)
-        T = T.undirected_t
-        type_string = value_or_type_to_string(T)
-        self.name = f"magma_array_slice_op_{type_string}_{lo}_{hi}"
-        self.primitive = True
-
-        T_out = T.unsized_t[hi - lo]
-        self.io = IO(I=In(T), O=Out(T_out))
-
-        self.T = T
-        self.lo = lo
-        self.hi = hi
+def MagmaArraySliceOp(T: ArrayMeta, lo: int, hi: int):
+    assert isinstance(T, ArrayMeta)
+    T = T.undirected_t
+    type_string = value_or_type_to_string(T)
+    name = f"magma_array_slice_op_{type_string}_{lo}_{hi}"
+    T_out = _resized_array(T, hi - lo)
+    ports = dict(I=In(T), O=Out(T_out))
+    attrs = dict(T=T, lo=lo, hi=hi)
+    return InstanceWrapper(name, ports, attrs)
 
 
-def MagmaArrayCreateOp(T: ArrayMeta):
+def MagmaArrayCreateOp(value: Array):
+    T = type(value)
     assert isinstance(T, ArrayMeta)
     T = T.undirected_t
     name = f"magma_array_create_op_{value_or_type_to_string(T)}"
-    ports = {f"I{i}": In(T.T) for i in range(T.N)}
+    ports = {}
+    for i, _ in value._enumerate_children():
+        if isinstance(i, slice):
+            ports[f"I{i}"] = In(Array[i.stop - i.start, T.T])
+        else:
+            ports[f"I{i}"] = In(T.T)
     ports.update(dict(O=Out(T)))
     attrs = dict(T=T)
     return InstanceWrapper(name, ports, attrs)
 
 
 def MagmaTupleGetOp(T: TupleMeta, index: Union[int, str]):
     assert isinstance(T, TupleMeta)
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/mlir_printer_utils.py` & `magma-lang-2.3.0/magma/backend/mlir/mlir_printer_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Callable, List, Mapping, Union
+from typing import Any, Callable, List, Mapping, Union
 
-from magma.backend.mlir.mlir import MlirValue
+from magma.backend.mlir.mlir import MlirAttribute, MlirValue
+from magma.backend.mlir.print_opts import PrintOpts
 from magma.backend.mlir.printer_base import PrinterBase
 
 
 MlirValueList = List[MlirValue]
 MlirValueOrMlirValueList = Union[MlirValue, MlirValueList]
 
 
@@ -35,17 +36,33 @@
     value_list = _maybe_wrap_value_or_value_list(value_or_value_list)
     printer.print(", ".join(v.type.emit() for v in value_list))
 
 
 def print_signature(
         value_or_value_list: MlirValueOrMlirValueList,
         printer: PrinterBase,
-        raw_names: bool = False):
+        print_opts: PrintOpts,
+        raw_names: bool = False,
+):
     value_list = _maybe_wrap_value_or_value_list(value_or_value_list)
     get_name = get_name_fn(raw_names)
-    signatures = (f"{get_name(v)}: {v.type.emit()}" for v in value_list)
-    printer.print(", ".join(signatures))
+
+    def _make_signature(value: MlirValue) -> str:
+        signature = f"{get_name(value)}: {value.type.emit()}"
+        if print_opts.print_locations:
+            signature += f" {value.location.emit()}"
+        return signature
+
+    printer.print(", ".join(map(_make_signature, value_list)))
+
+
+def _attr_to_string(value: Any) -> str:
+    if isinstance(value, MlirAttribute):
+        return value.emit()
+    return str(value)
 
 
 def print_attr_dict(attr_dict: Mapping, printer: PrinterBase):
-    attr_dict_to_string = ", ".join(f"{k} = {v}" for k, v in attr_dict.items())
+    attr_dict_to_string = ", ".join(
+        f"{k} = {v.emit()}" for k, v in attr_dict.items()
+    )
     printer.print(f"{{{attr_dict_to_string}}}")
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/printer_base.py` & `magma-lang-2.3.0/magma/backend/mlir/printer_base.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/backend/mlir/scoped_name_generator.py` & `magma-lang-2.3.0/magma/backend/mlir/scoped_name_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 class ScopedNameGeneratorBase(abc.ABC):
     @abc.abstractmethod
     def __call__(self, name: Optional[str] = None, force: bool = False) -> str:
         raise NotImplementedError()
 
 
 class ScopedNameGenerator(ScopedNameGeneratorBase):
-    def __init__(self):
+    def __init__(self, disallow_duplicates: bool):
+        self._disallow_duplicates = disallow_duplicates
         self._indices = collections.Counter()
 
     def __call__(self, name: Optional[str] = None, force: bool = False) -> str:
         if name is None:
             name = ""
         return self._call_impl(name, force)
 
     def _call_impl(self, name: str, force: bool) -> str:
         index = self._indices[name]
         self._indices[name] += 1
         if force:
-            assert index == 0
-            return name
+            if not self._disallow_duplicates:
+                return name
+            if index != 0:
+                raise RuntimeError(f"Found duplicate name {name}")
         return name + str(index)
```

### Comparing `magma-lang-2.2.9/magma/backend/mlir/sv.py` & `magma-lang-2.3.0/magma/backend/mlir/hw.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,249 +1,286 @@
 import dataclasses
-from typing import List, Optional
+from typing import Any, ClassVar, List, Mapping, Optional, Tuple
 
-from magma.backend.mlir.hw import hw
+from magma.backend.mlir.common import default_field
 from magma.backend.mlir.mlir import (
-    MlirDialect, MlirOp, MlirBlock, MlirValue, MlirSymbol,
-    begin_dialect, end_dialect)
-from magma.backend.mlir.mlir_printer_utils import print_names, print_types
+    begin_dialect,
+    end_dialect,
+    MlirAttribute,
+    MlirDialect,
+    MlirOp,
+    MlirSymbol,
+    MlirType,
+    MlirValue,
+)
+from magma.backend.mlir.mlir_printer_utils import (
+    print_attr_dict,
+    print_names,
+    print_signature,
+    print_types,
+)
+from magma.backend.mlir.print_opts import PrintOpts
 from magma.backend.mlir.printer_base import PrinterBase
 
 
-sv = MlirDialect("sv")
-begin_dialect(sv)
+hw = MlirDialect("hw")
+begin_dialect(hw)
 
 
-@dataclasses.dataclass
-class RegOp(MlirOp):
-    results: List[MlirValue]
-    name: str
+@dataclasses.dataclass(frozen=True)
+class ArrayType(MlirType):
+    dims: Tuple[int]
+    T: MlirType
 
-    def print_op(self, printer: PrinterBase):
-        print_names(self.results, printer)
-        printer.print(f" = sv.reg {{name = \"{self.name}\"}} : ")
-        print_types(self.results, printer)
+    def emit(self) -> str:
+        dim_str = "x".join(map(str, self.dims))
+        return f"!hw.array<{dim_str}x{self.T.emit()}>"
 
 
-@dataclasses.dataclass
-class ReadInOutOp(MlirOp):
-    operands: List[MlirValue]
-    results: List[MlirValue]
+@dataclasses.dataclass(frozen=True)
+class StructType(MlirType):
+    fields: Tuple[Tuple[str, MlirType]]
 
-    def print_op(self, printer: PrinterBase):
-        print_names(self.results, printer)
-        printer.print(f" = sv.read_inout ")
-        print_names(self.operands, printer)
-        printer.print(" : ")
-        print_types(self.operands, printer)
+    def emit(self) -> str:
+        field_str = ", ".join(f"{k}: {t.emit()}" for k, t in self.fields)
+        return f"!hw.struct<{field_str}>"
 
 
-@dataclasses.dataclass
-class AssignBaseOp(MlirOp):
-    operands: List[MlirValue]
+@dataclasses.dataclass(frozen=True)
+class InOutType(MlirType):
+    T: MlirType
 
-    def print_op(self, printer: PrinterBase):
-        printer.print(f"sv.{self.op_name} ")
-        print_names(self.operands, printer)
-        printer.print(" : ")
-        print_types(self.operands[1], printer)
+    def emit(self) -> str:
+        return f"!hw.inout<{self.T.emit()}>"
 
 
-@dataclasses.dataclass
-class AssignOp(AssignBaseOp):
-    operands: List[MlirValue]
-    op_name = "assign"
+@dataclasses.dataclass(frozen=True)
+class InnerRefAttr(MlirAttribute):
+    module: MlirSymbol
+    name: MlirSymbol
 
+    def emit(self) -> str:
+        return f"#hw.innerNameRef<{self.module.name}::{self.name.name}>"
 
-@dataclasses.dataclass
-class PAssignOp(AssignBaseOp):
-    operands: List[MlirValue]
-    op_name = "passign"
 
+@dataclasses.dataclass(frozen=True)
+class ParamDeclAttr(MlirAttribute):
+    name: str
+    type: MlirType
+    value: Optional[MlirAttribute] = None
 
-@dataclasses.dataclass
-class BPAssignOp(AssignBaseOp):
-    operands: List[MlirValue]
-    op_name = "bpassign"
+    def emit(self) -> str:
+        s = f"{self.name}: {self.type.emit()}"
+        if self.value is None:
+            return s
+        return f"{s} = {self.value.emit()}"
 
 
-@dataclasses.dataclass
-class AlwaysFFOp(MlirOp):
-    operands: List[MlirValue]
-    clock_edge: str
-    reset_type: str = None
-    reset_edge: str = None
+@dataclasses.dataclass(frozen=True)
+class OutputFileAttr(MlirAttribute):
+    filename: str
+    exclude_from_file_list: bool = False
+    include_replicated_ops: bool = False
 
-    def __post_init__(self):
-        self._body_block = self.new_region().new_block()
-        if self.reset_type is None:
-            return
-        self._reset_block = self.new_region().new_block()
-
-    @property
-    def body_block(self) -> MlirBlock:
-        return self._body_block
-
-    @property
-    def reset_block(self) -> MlirBlock:
-        return self._reset_block
+    def emit(self) -> str:
+        s = f"#hw.output_file<\"{self.filename}\""
+        if self.exclude_from_file_list:
+            s += f", excludeFromFileList"
+        if self.include_replicated_ops:
+            s += f", includeReplicatedOps"
+        return f"{s}>"
 
-    def print(self, printer: PrinterBase):
-        printer.print(f"sv.alwaysff({self.clock_edge} ")
-        print_names(self.operands[0], printer)
-        printer.print(") {")
-        printer.flush()
-        printer.push()
-        self.body_block.print(printer)
-        printer.pop()
-        printer.print("}")
-        if self.reset_type is None:
-            printer.flush()
-            return
-        printer.print(f" ({self.reset_type} : {self.reset_edge} ")
-        print_names(self.operands[1], printer)
-        printer.print(") {")
-        printer.flush()
-        printer.push()
-        self.reset_block.print(printer)
-        printer.pop()
-        printer.print_line("}")
 
-    def print_op(self, printer: PrinterBase):
-        raise NotImplementedError()
+@dataclasses.dataclass(frozen=True)
+class FileListAttr(MlirAttribute):
+    filename: str
+
+    def emit(self) -> str:
+        return f"#hw.output_filelist<\"{self.filename}\">"
+
+
+@dataclasses.dataclass
+class ModuleOpBase(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
+    name: MlirSymbol
+    parameters: List[ParamDeclAttr] = default_field(list)
+
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        printer.print(f"hw.{self.op_name} {self.name.name}")
+        if self.parameters:
+            printer.print("<")
+            printer.print(", ".join(param.emit() for param in self.parameters))
+            printer.print(">")
+        printer.print("(")
+        print_signature(self.operands, printer, print_opts)
+        printer.print(") -> (")
+        print_signature(self.results, printer, print_opts, raw_names=True)
+        printer.print(")")
+        if self.attr_dict:
+            printer.print(" attributes ")
+            print_attr_dict(self.attr_dict, printer)
 
 
 @dataclasses.dataclass
-class InitialOp(MlirOp):
+class ModuleOp(ModuleOpBase):
+    op_name: ClassVar[str] = "module"
+
     def __post_init__(self):
         self._block = self.new_region().new_block()
 
     def add_operation(self, operation: MlirOp):
         self._block.add_operation(operation)
 
-    def print_op(self, printer: PrinterBase):
-        printer.print("sv.initial")
+
+@dataclasses.dataclass
+class ModuleExternOp(ModuleOpBase):
+    op_name: ClassVar[str] = "module.extern"
+
+
+@dataclasses.dataclass
+class OutputOp(MlirOp):
+    operands: List[MlirValue]
+
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        printer.print(f"hw.output ")
+        print_names(self.operands, printer)
+        printer.print(" : ")
+        print_types(self.operands, printer)
+
+
+@dataclasses.dataclass
+class ConstantOp(MlirOp):
+    results: List[MlirValue]
+    value: int
+
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(f" = hw.constant {self.value} : ")
+        print_types(self.results, printer)
 
 
 @dataclasses.dataclass
-class WireOp(MlirOp):
+class InstanceOp(MlirOp):
+    operands: List[MlirValue]
     results: List[MlirValue]
     name: str
+    module: ModuleOpBase
+    parameters: List[ParamDeclAttr] = default_field(list)
     sym: Optional[MlirSymbol] = None
 
-    def print_op(self, printer: PrinterBase):
-        print_names(self.results, printer)
-        printer.print(" = sv.wire ")
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        if self.results:
+            print_names(self.results, printer)
+            printer.print(" = ")
+        printer.print(f"hw.instance \"{self.name}\" ")
         if self.sym is not None:
             printer.print(f"sym {self.sym.name} ")
-        printer.print(f"{{name=\"{self.name}\"}} : ")
-        print_types(self.results, printer)
+        printer.print(f"{self.module.name.name}")
+        if self.parameters:
+            printer.print("<")
+            printer.print(", ".join(param.emit() for param in self.parameters))
+            printer.print(">")
+        printer.print("(")
+        operands = [
+            f"{m_operand.raw_name}: {operand.name}: {operand.type.emit()}"
+            for operand, m_operand in zip(self.operands, self.module.operands)
+        ]
+        printer.print(", ".join(operands))
+        printer.print(") -> (")
+        results = [
+            f"{m_result.raw_name}: {result.type.emit()}"
+            for result, m_result in zip(self.results, self.module.results)
+        ]
+        printer.print(", ".join(results))
+        printer.print(")")
+        if self.attr_dict:
+            printer.print(" ")
+            print_attr_dict(self.attr_dict, printer)
 
 
 @dataclasses.dataclass
-class VerbatimOp(MlirOp):
-    operands: List[MlirOp]
-    string: str
+class ArrayGetOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
-        # NOTE(rsetaluri): This is a hack to "double-escape" escape characters
-        # like `\n`, `\t`.
-        string = repr(self.string)[1:-1]
-        string = string.replace("\"", "\\\"")
-        string = string.replace("\\\'", "'")
-        printer.print(f"sv.verbatim \"{string}\"")
-        if self.operands:
-            printer.print(" (")
-            print_names(self.operands, printer)
-            printer.print(") : ")
-            print_types(self.operands, printer)
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.array_get ")
+        print_names(self.operands[0], printer)
+        printer.print("[")
+        print_names(self.operands[1], printer)
+        printer.print("] : ")
+        print_types(self.operands, printer)
 
 
 @dataclasses.dataclass
-class BindOp(MlirOp):
-    instance: hw.InnerRefAttr
+class ArraySliceOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
-        printer.print(f"sv.bind {self.instance.emit()}")
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.array_slice ")
+        print_names(self.operands[0], printer)
+        printer.print("[")
+        print_names(self.operands[1], printer)
+        printer.print("] : (")
+        print_types(self.operands[0], printer)
+        printer.print(") -> ")
+        print_types(self.results[0], printer)
 
 
 @dataclasses.dataclass
-class IfDefOp(MlirOp):
-    cond: str
+class ArrayCreateOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
+
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.array_create ")
+        print_names(self.operands, printer)
+        printer.print(" : ")
+        print_types(self.operands[0], printer)
 
-    def __post_init__(self):
-        self._then_block = self.new_region().new_block()
-        self._else_block = None
 
-    @property
-    def then_block(self) -> MlirBlock:
-        return self._then_block
-
-    @property
-    def else_block(self) -> MlirBlock:
-        if self._else_block is None:
-            self._else_block = self.new_region().new_block()
-        return self._else_block
-
-    def print(self, printer: PrinterBase):
-        printer.print(f"sv.ifdef \"{self.cond}\" {{")
-        printer.flush()
-        printer.push()
-        self._then_block.print(printer)
-        printer.pop()
-        printer.print("}")
-        if self._else_block is None:
-            printer.flush()
-            return
-        printer.print(" else {")
-        printer.flush()
-        printer.push()
-        self._else_block.print(printer)
-        printer.pop()
-        printer.print_line("}")
+@dataclasses.dataclass
+class ArrayConcatOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
-        raise NotImplementedError()
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.array_concat ")
+        print_names(self.operands, printer)
+        printer.print(" : ")
+        print_types(self.operands, printer)
 
 
 @dataclasses.dataclass
-class IfOp(MlirOp):
-    operands: List[MlirOp]
+class StructExtractOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
+    field: str
 
-    def __post_init__(self):
-        self._then_block = self.new_region().new_block()
-        self._else_block = None
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.struct_extract ")
+        print_names(self.operands, printer)
+        printer.print(f"[\"{self.field}\"] : ")
+        print_types(self.operands, printer)
 
-    @property
-    def then_block(self) -> MlirBlock:
-        return self._then_block
-
-    @property
-    def else_block(self) -> MlirBlock:
-        if self._else_block is None:
-            self._else_block = self.new_region().new_block()
-        return self._else_block
 
-    def print(self, printer: PrinterBase):
-        printer.print(f"sv.if ")
-        print_names(self.operands[0], printer)
-        printer.print(" {")
-        printer.flush()
-        printer.push()
-        self._then_block.print(printer)
-        printer.pop()
-        printer.print("}")
-        if self._else_block is None:
-            printer.flush()
-            return
-        printer.print(" else {")
-        printer.flush()
-        printer.push()
-        self._else_block.print(printer)
-        printer.pop()
-        printer.print_line("}")
+@dataclasses.dataclass
+class StructCreateOp(MlirOp):
+    operands: List[MlirValue]
+    results: List[MlirValue]
 
-    def print_op(self, printer: PrinterBase):
-        raise NotImplementedError()
+    def print_op(self, printer: PrinterBase, print_opts: PrintOpts):
+        print_names(self.results, printer)
+        printer.print(" = hw.struct_create (")
+        print_names(self.operands, printer)
+        printer.print(") : ")
+        print_types(self.results, printer)
 
 
 end_dialect()
```

### Comparing `magma-lang-2.2.9/magma/backend/verilog.py` & `magma-lang-2.3.0/magma/backend/verilog.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,17 @@
         if not isinstance(v, str): v = str(v)
         return '.%s(%s)' % (k, v)
 
     args = []
     debug_str = ""
     for k, v in self.interface.ports.items():
         if getattr(v, "debug_info", False) and get_codegen_debug_info():
-            filename, lineno, module = v.debug_info
+            filename, lineno, module = (
+                v.debug_info.filename, v.debug_info.lineno, v.debug_info.module
+            )
         #print('arg', k, v,)
         if v.is_input():
             # find the output connected to v
             w = v.trace()
             if w is None:
                 _logger.warning(f'{v.debug_name} not connected')
                 continue
@@ -172,15 +174,20 @@
         if isinstance(port, Array):
             if not issubclass(port.T, Digital):
                 raise Exception(f'Argument {cls.__name__}.{name} of type {type(port)} is not supported, the verilog backend only supports simple 1-d array of bits of the form Array(N, Bit)')
 
 
     args = ', '.join(vmoduleargs(cls.interface))
     s = ''
-    if get_codegen_debug_info() and cls.debug_info.filename and cls.debug_info.lineno:
+    if (
+        get_codegen_debug_info() and
+        cls.debug_info and
+        cls.debug_info.filename and
+        cls.debug_info.lineno
+    ):
         s += f'// Defined at {make_relative(cls.debug_info.filename)}:{cls.debug_info.lineno}\n'
     s += 'module %s (%s);\n' % (cls.verilog_name, args)
     if cls.verilog:
         s += cls.verilog + '\n'
         if cls.verilogLib:
             import re
             for libName in cls.verilogLib:
@@ -228,15 +235,15 @@
                                     iname = vname(input[i])
                                     oname = vname(output[i])
                                     s += 'assign %s = %s;\n' % (iname, oname)
                     else:
                         iname = vname(port)
                         oname = vname(output)
                         if getattr(port, "debug_info", False) and get_codegen_debug_info():
-                            s += f"// Wired at {make_relative(port.debug_info[0])}:{port.debug_info[1]}\n"
+                            s += f"// Wired at {make_relative(port.debug_info.filename)}:{port.debug_info.lineno}\n"
                         s += 'assign %s = %s;\n' % (iname, oname)
                 else:
                     _logger.warning(f"{cls.__name__}.{port.name} is unwired")
 
     s += "endmodule\n"
 
     return s
```

### Comparing `magma-lang-2.2.9/magma/bfloat.py` & `magma-lang-2.3.0/magma/bfloat.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/bind.py` & `magma-lang-2.3.0/magma/bind.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         ports += _gen_bind_port(cls, mon_arg, cls_arg)
     extra_mon_args = list(
         monitor.interface.ports.values()
     )[len(cls.interface):]
     for mon_arg, bind_arg in zip(extra_mon_args, args):
         if isinstance(bind_arg, PortView):
             T = type(bind_arg.port)
-            parent = _get_view_inst_parent(bind_arg).parent
+            parent = _get_view_inst_parent(bind_arg).parent_view
             if isinstance(parent, InstView):
                 defn = parent.circuit
             else:
                 assert isinstance(parent, Circuit)
                 defn = type(parent)
             driver = bind_arg.port
         else:
@@ -91,15 +91,15 @@
                 defn.num_bind_wires = 0
             name = f"_magma_bind_wire_{defn.num_bind_wires}"
             defn.num_bind_wires += 1
             temp = T.qualify(Direction.Undirected)(name=name)
             _wire_temp(driver, temp)
             temp.unused()
         if isinstance(bind_arg, PortView):
-            temp = PortView[type(temp)](temp, bind_arg.parent.parent)
+            temp = PortView[type(temp)](temp, bind_arg.parent_view.parent_view)
         bind_arg = temp
         ports += _gen_bind_port(cls, mon_arg, bind_arg)
     ports_str = ",\n    ".join(ports)
     cls_name = cls.name
     monitor_name = monitor.name
     if user_namespace is not None:
         cls_name = user_namespace + "_" + cls_name
```

### Comparing `magma-lang-2.2.9/magma/bit_primitives.py` & `magma-lang-2.3.0/magma/bit_primitives.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from functools import lru_cache
 import operator
 
 import hwtypes as ht
 
 from magma.bit import Bit
+from magma.debug import magma_helper_function
 from magma.digital import Digital
 from magma.circuit import Circuit, coreir_port_mapping
 from magma.interface import IO
 from magma.language_utils import primitive_to_python
 from magma.t import In, Out
 
 
@@ -91,23 +92,25 @@
     return DefineCorebit
 
 
 DefineUndriven = make_Define("undriven", "O", Out)
 DefineUnused = make_Define("term", "I", In)
 
 
+@magma_helper_function
 def unused(self):
     if self.is_input() or self.is_inout():
         raise TypeError("unused cannot be used with input/inout")
     if not getattr(self, "_magma_unused_", False):
         DefineUnused()().I.wire(self)
         # "Cache" unused calls so only one is produced
         self._magma_unused_ = True
 
 
+@magma_helper_function
 def undriven(self):
     if self.is_output() or self.is_inout():
         raise TypeError("undriven cannot be used with output/inout")
     self.wire(DefineUndriven()().O)
 
 
 # NOTE(leonardt): Monkey patched functions.
```

### Comparing `magma-lang-2.2.9/magma/bits.py` & `magma-lang-2.3.0/magma/bits.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,35 +12,39 @@
 from hwtypes import AbstractBitVector, AbstractBitVectorMeta, AbstractBit, \
     InconsistentSizeError
 from .compatibility import IntegerTypes
 from .bit import Bit
 from .array import ArrayMeta, Array
 from .t import Type, Direction, In, Out
 from magma.circuit import Circuit, coreir_port_mapping
+from magma.debug import magma_helper_function
 from magma.bitutils import seq2int, int2seq
 from magma.family import get_family
 from magma.interface import IO
 from magma.language_utils import primitive_to_python
 from magma.logging import root_logger
 from magma.generator import Generator2
 from magma.debug import debug_wire
 from magma.operator_utils import output_only
 from magma.protocol_type import magma_type, magma_value
 from magma.ref import ConstRef
 
 
 def _error_handler(fn):
+
+    @magma_helper_function
     @functools.wraps(fn)
     def _wrapper(*args, **kwargs):
         try:
             return fn(*args, **kwargs)
         except InconsistentSizeError as e:
             raise e from None
         except TypeError:
             return NotImplemented
+
     return _wrapper
 
 
 _logger = root_logger()
 
 
 def _check_size(val, T):
@@ -55,23 +59,27 @@
         val = val.bits()
     if not isinstance(val, Bits):
         return T(val)
     _check_size(val, T)
     return val
 
 
-def bits_cast(fn: tp.Callable[['Bits', 'Bits'], tp.Any]) -> \
-        tp.Callable[['Bits', tp.Any], tp.Any]:
-    @wraps(fn)
+def bits_cast(
+        fn: tp.Callable[['Bits', 'Bits'], tp.Any]
+) -> tp.Callable[['Bits', tp.Any], tp.Any]:
+
+    @magma_helper_function
+    @functools.wraps(fn)
     def wrapped(self: 'Bits', other: tp.Any) -> tp.Any:
         try:
             other = _coerce(type(self), other)
         except TypeError:
             return NotImplemented
         return fn(self, other)
+
     return wrapped
 
 
 class BitsMeta(AbstractBitVectorMeta, ArrayMeta):
     def __new__(mcs, name, bases, namespace, info=(None, None, None), **kwargs):
         return ArrayMeta.__new__(mcs, name, bases, namespace, info, **kwargs)
 
@@ -362,33 +370,39 @@
                 I1 = cls.hwtypes_T[N](value_store.get_value(self.I1))
                 S = ht.Bit(value_store.get_value(self.S))
                 O = I1 if S else I0
                 value_store.set_value(self.O, O)
 
         return _MagmBitsOp
 
+    @magma_helper_function
     def bvnot(self) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_unary_op("not")()(self)
 
+    @magma_helper_function
     @bits_cast
     def bvand(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("and")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvor(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("or")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvxor(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("xor")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvshl(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("shl")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvlshr(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("lshr")()(self, other)
 
     def bvashr(self, other) -> 'AbstractBitVector':
         raise NotImplementedError()
 
@@ -397,37 +411,42 @@
 
     def bvror(self, other) -> 'AbstractBitVector':
         raise NotImplementedError()
 
     def bvcomp(self, other) -> 'AbstractBitVector[1]':
         return Bits[1](self == other)
 
+    @magma_helper_function
     @bits_cast
     def bveq(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("eq")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvult(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("ult")()(self, other)
 
+    @magma_helper_function
     def bvule(self, other) -> AbstractBit:
         # For wiring
         if self.is_input():
             return Type.__le__(self, other)
         # We coerce after wiring for simplicity
         try:
             other = _coerce(type(self), other)
         except TypeError:
             return NotImplemented
         return type(self).undirected_t._declare_compare_op("ule")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvugt(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("ugt")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvuge(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("uge")()(self, other)
 
     def bvslt(self, other) -> AbstractBit:
         raise NotImplementedError()
 
@@ -436,17 +455,19 @@
 
     def bvsgt(self, other) -> AbstractBit:
         raise NotImplementedError()
 
     def bvsge(self, other) -> AbstractBit:
         raise NotImplementedError()
 
+    @magma_helper_function
     def bvneg(self) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_unary_op("neg")()(self)
 
+    @magma_helper_function
     def adc(self, other: 'Bits', carry: Bit) -> tp.Tuple['Bits', Bit]:
         """
         add with carry
         returns a two element tuple of the form (result, carry)
         """
         T = type(self)
         other = _coerce(T, other)
@@ -455,37 +476,43 @@
         a = self.zext(1)
         b = other.zext(1)
         c = carry.zext(T.size)
 
         res = a + b + c
         return res[0:-1], res[-1]
 
+    @magma_helper_function
     def ite(self, t_branch, f_branch) -> 'AbstractBitVector':
         type_ = type(t_branch)
         if type_ != type(f_branch):
             raise TypeError("ite expects same type for both branches")
         return type(self).undirected_t._declare_ite(type_)()(
             t_branch, f_branch, self != self.make_constant(0))
 
+    @magma_helper_function
     @bits_cast
     def bvadd(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("add")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsub(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("sub")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvmul(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("mul")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvudiv(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("udiv")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvurem(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("urem")()(self, other)
 
     def bvsdiv(self, other) -> 'AbstractBitVector':
         raise NotImplementedError()
 
@@ -514,90 +541,110 @@
         ext = int(other)
         if ext < 0:
             raise ValueError()
 
         T = type(self).unsized_t
         return self.concat(T[ext](0))
 
+    @magma_helper_function
     def __invert__(self):
         return self.bvnot()
 
+    @magma_helper_function
     @_error_handler
     def __and__(self, other):
         return self.bvand(other)
 
+    @magma_helper_function
     @_error_handler
     def __rand__(self, other):
         return self.bvand(other)
 
+    @magma_helper_function
     @_error_handler
     def __or__(self, other):
         return self.bvor(other)
 
+    @magma_helper_function
     @_error_handler
     def __ror__(self, other):
         return self.bvor(other)
 
+    @magma_helper_function
     @_error_handler
     def __xor__(self, other):
         return self.bvxor(other)
 
+    @magma_helper_function
     @_error_handler
     def __rxor__(self, other):
         return self.bvxor(other)
 
+    @magma_helper_function
     @_error_handler
     def __lshift__(self, other):
         return self.bvshl(other)
 
+    @magma_helper_function
     @_error_handler
     def __rlshift__(self, other):
         return type(self)(other) << self
 
+    @magma_helper_function
     @_error_handler
     def __rshift__(self, other):
         return self.bvlshr(other)
 
+    @magma_helper_function
     @_error_handler
     def __rrshift__(self, other):
         return type(self)(other) >> self
 
+    @magma_helper_function
     @output_only("Cannot use == on an input")
     @_error_handler
     def __eq__(self, other):
         return self.bveq(other)
 
+    @magma_helper_function
     @output_only("Cannot use != on an input")
     @_error_handler
     def __ne__(self, other):
         return self.bvne(other)
 
+    @magma_helper_function
     def __neg__(self):
         return self.bvneg()
 
+    @magma_helper_function
     @_error_handler
     def __add__(self, other):
         return self.bvadd(other)
 
+    @magma_helper_function
     @_error_handler
     def __radd__(self, other):
         return self.bvadd(other)
 
+    @magma_helper_function
     @_error_handler
     def __sub__(self, other):
         return self.bvsub(other)
 
+    @magma_helper_function
     @_error_handler
     def __rsub__(self, other):
         return type(self)(other) - self
 
+    @magma_helper_function
     @_error_handler
     def __mul__(self, other):
         return self.bvmul(other)
 
+    @magma_helper_function
     @_error_handler
     def __rmul__(self, other):
         return self.bvmul(other)
 
     @classmethod
     def get_family(cls):
         return get_family()
@@ -633,20 +680,23 @@
             if isinstance(index, int):
                 return Bit(self._const_value[index])
             assert isinstance(index, slice)
             result = self._const_value[index]
             return type(self)[len(result)](result)
         return super().__getitem__(index)
 
+    @magma_helper_function
     def reduce_or(self):
         return reduce(operator.or_, self)
 
+    @magma_helper_function
     def reduce_xor(self):
         return reduce(operator.xor, self)
 
+    @magma_helper_function
     def reduce_and(self):
         return reduce(operator.and_, self)
 
     @property
     def debug_name(self):
         if self.const():
             return repr(self)
@@ -680,129 +730,155 @@
 BitsType = Bits
 
 
 class Int(Bits):
     """
     Defines shared right-hand operators for UInt/SInt
     """
+    @magma_helper_function
     @_error_handler
     def __rfloordiv__(self, other):
         return type(self)(other) // self
 
+    @magma_helper_function
     @_error_handler
     def __rtruediv__(self, other):
         return type(self)(other) / self
 
+    @magma_helper_function
     @_error_handler
     def __rmod__(self, other):
         return type(self)(other) % self
 
 
 class UInt(Int):
     hwtypes_T = ht.UIntVector
 
+    @magma_helper_function
     @_error_handler
     def __floordiv__(self, other):
         return self.bvudiv(other)
 
+    @magma_helper_function
     @_error_handler
     def __truediv__(self, other):
         return self.bvudiv(other)
 
+    @magma_helper_function
     @_error_handler
     def __mod__(self, other):
         return self.bvurem(other)
 
+    @magma_helper_function
     @_error_handler
     def __ge__(self, other):
         return self.bvuge(other)
 
+    @magma_helper_function
     @_error_handler
     def __gt__(self, other):
         return self.bvugt(other)
 
+    @magma_helper_function
     @_error_handler
     def __le__(self, other):
         return self.bvule(other)
 
+    @magma_helper_function
     @_error_handler
     def __lt__(self, other):
         return self.bvult(other)
 
 
 class SInt(Int):
     hwtypes_T = ht.SIntVector
 
     @classmethod
     def _extend(cls, args):
         return args + [args[-1] for _ in range(cls.N - len(args))]
 
+    @magma_helper_function
     @bits_cast
     def bvslt(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("slt")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsle(self, other) -> AbstractBit:
         # For wiring
         if self.is_input():
             return Type.__le__(self, other)
         return type(self).undirected_t._declare_compare_op("sle")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsgt(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("sgt")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsge(self, other) -> AbstractBit:
         return type(self).undirected_t._declare_compare_op("sge")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsdiv(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("sdiv")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvsrem(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("srem")()(self, other)
 
+    @magma_helper_function
     @bits_cast
     def bvashr(self, other) -> 'AbstractBitVector':
         return type(self).undirected_t._declare_binary_op("ashr")()(self, other)
 
+    @magma_helper_function
     @_error_handler
     def __mod__(self, other):
         return self.bvsrem(other)
 
+    @magma_helper_function
     @_error_handler
     def __floordiv__(self, other):
         return self.bvsdiv(other)
 
+    @magma_helper_function
     @_error_handler
     def __truediv__(self, other):
         return self.bvsdiv(other)
 
+    @magma_helper_function
     @_error_handler
     def __ge__(self, other):
         return self.bvsge(other)
 
+    @magma_helper_function
     @_error_handler
     def __gt__(self, other):
         return self.bvsgt(other)
 
+    @magma_helper_function
     @_error_handler
     def __le__(self, other):
         return self.bvsle(other)
 
+    @magma_helper_function
     @_error_handler
     def __lt__(self, other):
         return self.bvslt(other)
 
+    @magma_helper_function
     @_error_handler
     def __rshift__(self, other):
         return self.bvashr(other)
 
+    @magma_helper_function
     def adc(self, other: 'Bits', carry: Bit) -> tp.Tuple['Bits', Bit]:
         """
         add with carry
         returns a two element tuple of the form (result, carry)
         """
         T = type(self)
         other = _coerce(T, other)
@@ -856,13 +932,14 @@
 _OP_MAP = {
     operator.and_: _reduce_factory("andr", operator.and_),
     operator.or_: _reduce_factory("orr", operator.or_),
     operator.xor: _reduce_factory("xorr", operator.xor)
 }
 
 
+@magma_helper_function
 def reduce(operator, bits: Bits):
     if not isinstance(bits, Bits):
         raise TypeError("m.reduce only works with Bits")
     if operator not in _OP_MAP:
         raise ValueError(f"{operator} not supported")
     return _OP_MAP[operator](len(bits))()(bits)
```

### Comparing `magma-lang-2.2.9/magma/bitutils.py` & `magma-lang-2.3.0/magma/bitutils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/braid.py` & `magma-lang-2.3.0/magma/braid.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/circuit.py` & `magma-lang-2.3.0/magma/circuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,89 +2,85 @@
 import enum
 import textwrap
 import inspect
 import itertools
 from functools import wraps
 import functools
 import operator
-from collections import namedtuple
+from collections import namedtuple, Counter, UserDict
 import os
+from typing import Callable, Dict, List, Union
 
-import six
 from . import cache_definition
-from .common import deprecated, setattrs, Stack, OrderedIdentitySet
+from .common import deprecated, setattrs, OrderedIdentitySet
 from .interface import *
 from .wire import *
-from .config import get_debug_mode
-from .debug import get_callee_frame_info, debug_info
+from .config import get_debug_mode, set_debug_mode
+from .debug import get_debug_info, debug_info
 from .is_definition import isdefinition
 from .placer import Placer, StagedPlacer
 from magma.syntax.combinational import combinational
 try:
     import kratos
     from magma.syntax.verilog import combinational_to_verilog, \
         sequential_to_verilog
 except ImportError:
     pass
 
 from magma.clock import is_clock_or_nested_clock, Clock, ClockTypes
-from magma.definition_context import DefinitionContext
-from magma.logging import root_logger
-from magma.ref import TempNamedRef
-from magma.t import In
-from magma.view import PortView
-from magma.wire_container import WiringLog
+from magma.common import (
+    only,
+    IterableException,
+    EmptyIterableException,
+    NonSingletonIterableException,
+)
+from magma.config import get_debug_mode, set_debug_mode, config, RuntimeConfig
+from magma.definition_context import (
+    DefinitionContext,
+    definition_context_manager,
+    push_definition_context,
+    pop_definition_context,
+    get_definition_context,
+)
+from magma.find_unconnected_ports import find_and_log_unconnected_ports
+from magma.logging import root_logger, capture_logs
+from magma.protocol_type import MagmaProtocol
+from magma.ref import TempNamedRef, AnonRef
+from magma.t import In, Type
+from magma.wire_container import WiringLog, AggregateWireable
 
 
 __all__ = ['AnonymousCircuitType']
 __all__ += ['AnonymousCircuit']
 
 __all__ += ['CircuitType']
-__all__ += ['Circuit']
+__all__ += ['Circuit', 'DebugCircuit']
 __all__ += ['DeclareCircuit']
 __all__ += ['DefineCircuit', 'EndDefine', 'EndCircuit']
 __all__ += ['DefineCircuitKind']
 
 __all__ += ['CopyInstance']
 __all__ += ['circuit_type_method']
 __all__ += ['circuit_generator']
 __all__ += ['CircuitBuilder', 'builder_method']
+__all__ += ['register_instance_callback', 'get_instance_callback']
 
 circuit_type_method = namedtuple('circuit_type_method', ['name', 'definition'])
 
 _logger = root_logger()
 
+config.register(use_namer_dict=RuntimeConfig(False))
+
 
 class _SyntaxStyle(enum.Enum):
     NONE = enum.auto()
     OLD = enum.auto()
     NEW = enum.auto()
 
 
-_definition_context_stack = Stack()
-
-
-def peek_definition_context_stack() -> DefinitionContext:
-    return _definition_context_stack.peek()
-
-
-class _DefinitionContextManager:
-    def __init__(self, context: DefinitionContext):
-        self._context = context
-
-    def __enter__(self):
-        _definition_context_stack.push(self._context)
-
-    def __exit__(self, typ, value, traceback):
-        _definition_context_stack.pop()
-
-
-DefinitionContextManager = _DefinitionContextManager
-
-
 def _has_definition(cls, port=None):
     if cls.instances:
         return True
     if port is None:
         interface = getattr(cls, "interface", None)
         if not interface:
             return False
@@ -193,39 +189,102 @@
         # Mixed
         return functools.reduce(operator.or_,
                                 (_get_intermediate_values(v) for v in value),
                                 OrderedIdentitySet())
     driver = value.value()
     if driver is None:
         return OrderedIdentitySet()
-    if getattr(type(driver), "N", False) and driver.name.anon():
-        conn_iter = list(value.connection_iter())
-        if len(conn_iter) > 1:
-            return functools.reduce(
-                operator.or_, (_get_intermediate_values(v) for v, _ in
-                               conn_iter),
-                OrderedIdentitySet())
+    if (
+            isinstance(driver, AggregateWireable) and
+            driver.name.anon() and
+            driver.has_elaborated_children()
+    ):
+        return functools.reduce(
+            operator.or_, (_get_intermediate_values(v) for v, _ in
+                           value.connection_iter()),
+            OrderedIdentitySet())
     values = OrderedIdentitySet()
     while driver is not None:
         values |= _add_intermediate_value(driver)
         if not driver.driven():
             break
         value = driver
         driver = driver.value()
     return values
 
 
+class NamerDict(UserDict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._inferred_names = {}
+
+    def _set_name(self, key, value):
+        if isinstance(value, (Type, MagmaProtocol)):
+            key = TempNamedRef(key, value)
+        value.name = key
+
+    def _check_unique_name(
+        self,
+        key: str,
+        value: Union[Type, 'Circuit'],
+    ):
+        """If key has been seen more than once, "uniquify" the names by append
+           _{i} to them."""
+        values = self._inferred_names.setdefault(key, [])
+        if len(values) == 0:
+            self._set_name(key, value)
+        elif any(value is x for x in values):
+            return  # already uniquified
+        else:
+            if len(values) == 1:
+                # Make the first value consistent by appending _0.
+                self._set_name(f"{key}_0", values[0])
+            self._set_name(f"{key}_{len(values)}", value)
+        values.append(value)
+
+    def _set_value_name(self, key: str, value: Type):
+        if not hasattr(value, "name"):
+            return  # interface object is a Type without a name
+        if isinstance(value.name, AnonRef):
+            self._check_unique_name(key, value)
+        elif isinstance(value.name, TempNamedRef):
+            self._check_unique_name(value.name.name, value)
+
+    def _set_inst_name(self, key: str, value: 'Circuit'):
+        if not value.name:
+            self._check_unique_name(key, value)
+        else:
+            self._check_unique_name(value.name, value)
+
+    def __setitem__(self, key, value):
+        super().__setitem__(key, value)
+        if isinstance(value, (Type, MagmaProtocol)):
+            self._set_value_name(key, value)
+        elif isinstance(type(value), CircuitKind):
+            # NOTE(leonardt): we check type(value) because this code is run in
+            # the Circuit class creation pipeline (so Circuit may not be defined
+            # yet).
+            self._set_inst_name(key, value)
+
+    def __hash__(self):
+        return hash(tuple(sorted(self.items())))
+
+
 class CircuitKind(type):
     def __prepare__(name, bases, **kwargs):
-        context = DefinitionContext(StagedPlacer(name))
-        _definition_context_stack.push(context)
+        ctx = DefinitionContext(StagedPlacer(name))
+        push_definition_context(ctx, use_staged_logger=True)
+        if config.use_namer_dict:
+            return NamerDict()
         return type.__prepare__(name, bases, **kwargs)
 
     """Metaclass for creating circuits."""
     def __new__(metacls, name, bases, dct):
+        if isinstance(dct, NamerDict):
+            dct = dict(dct)  # resolve to dict, no longer need name logic
         # Override class name if supplied (and save class name).
         cls_name = dct.get("_cls_name_", name)
         name = dct.setdefault('name', name)
 
         dct.setdefault("_circuit_base_", False)
         dct.setdefault('renamed_ports', {})
         dct.setdefault('primitive', False)
@@ -249,33 +308,37 @@
         cls = type.__new__(metacls, name, bases, dct)
 
         for method in dct.get('circuit_type_methods', []):
             setattr(cls, method.name, method.definition)
 
         cls._syntax_style_ = _SyntaxStyle.NONE
         cls._renamed_ports_ = dct["renamed_ports"]
+        # NOTE(rsetaluri): We first peek the definition context
+        # (get_definition_context()) so that we can finalize it before popping
+        # it. This is necessary because we want the unstaging of the logger to
+        # happen (inside of pop) after finalization.
         try:
-            context = _definition_context_stack.pop()
+            context = get_definition_context()
         except IndexError:  # no staged placer
             cls._context_ = DefinitionContext(Placer(cls))
         else:
             assert context.placer.name == cls_name
             # Override staged context with '_context_' from namespace if
             # available.
             cls._context_ = dct.get("_context_", context)
             cls._context_.place_instances(cls)
             _setup_interface(cls)
             cls._context_.finalize(cls)
+            pop_definition_context(use_staged_logger=True)
 
         return cls
 
     def __call__(cls, *largs, **kwargs):
-        if get_debug_mode():
-            debug_info = get_callee_frame_info()
-            kwargs["debug_info"] = debug_info
+        if "debug_info" not in kwargs:
+            kwargs["debug_info"] = get_debug_info(3)
         self = super(CircuitKind, cls).__call__(*largs, **kwargs)
         if hasattr(cls, 'IO'):
             interface = cls.IO(inst=self, renamed_ports=cls.renamed_ports)
             self.setinterface(interface)
         return self
 
     def __str__(cls):
@@ -358,20 +421,19 @@
         return defn
 
     @deprecated(msg="cls.inline_verilog is deprecated, use m.inline_verilog"
                 "instead")
     def inline_verilog(cls, inline_str, **kwargs):
         # NOTE(rsetaluri): This is a hack to avoid a circular import.
         from magma.inline_verilog import inline_verilog as m_inline_verilog
-        with _DefinitionContextManager(cls._context_):
+        with definition_context_manager(cls._context_):
             m_inline_verilog(inline_str, **kwargs)
 
 
-@six.add_metaclass(CircuitKind)
-class AnonymousCircuitType(object):
+class AnonymousCircuitType(object, metaclass=CircuitKind):
     """Abstract base class for circuits"""
 
     _circuit_base_ = True
 
     def __init__(self, *largs, **kwargs):
         self.kwargs = dict(**kwargs)
 
@@ -393,20 +455,26 @@
         self.is_instance = True
         self.debug_info = kwargs.get("debug_info", None)
 
     def set_debug_info(self, debug_info):
         self.debug_info = debug_info
 
     def __str__(self):
-        if self.name:
-            return f"{self.name}<{type(self)}>"
-        name = f"AnonymousCircuitInst{id(self)}"
-        interface = ", ".join(f"{name}: {type(value)}"
-                              for name, value in self.interface.ports.items())
-        return f"{name}<{interface}>"
+        name = self.name
+        if not name:
+            name = f"AnonymousCircuitInst{id(self)}"
+        if type(self) is AnonymousCircuitType:
+            interface = ", ".join(
+                f"{name}: {type(value)}"
+                for name, value in self.interface.ports.items()
+            )
+            name += f"<{interface}>"
+        else:
+            name += f"<{type(self)}>"
+        return name
 
     def __repr__(self):
         args = []
         for k, v in self.interface.ports.items():
             args.append(f"\"{k}\"")
             args.append(repr(v))
         args = ", ".join(args)
@@ -461,17 +529,15 @@
     def debug_name(self):
         defn_str = ""
         if hasattr(self, 'defn') and self.defn is not None:
             defn_str = str(self.defn.name)
         return f"{defn_str}.{self.name}"
 
     def __call__(input, *outputs, **kw):
-        debug_info = None
-        if get_debug_mode():
-            debug_info = get_callee_frame_info()
+        debug_info = get_debug_info(3)
 
         no = len(outputs)
         if len(outputs) == 1:
             input.wire(outputs[0], debug_info)
         elif len(outputs) >= 1:  # In case there are only kw
             input.wireoutputs(outputs, debug_info)
 
@@ -526,15 +592,15 @@
         return self.interface.inputargs()
 
     def outputargs(self):
         return self.interface.outputargs()
 
     @classmethod
     def open(cls):
-        return _DefinitionContextManager(cls._context_)
+        return definition_context_manager(cls._context_)
 
 
 def AnonymousCircuit(*decl):
     """
     AnonymousCircuits are like macros - the circuit instances are not placed
     """
     if len(decl) == 1:
@@ -545,15 +611,15 @@
 class CircuitType(AnonymousCircuitType):
     _circuit_base_ = True
 
     """Placed circuit - instances placed in a definition"""
     def __init__(self, *largs, **kwargs):
         super(CircuitType, self).__init__(*largs, **kwargs)
         try:
-            context = _definition_context_stack.peek()
+            context = get_definition_context()
             context.placer.place(self)
         except IndexError:  # instances must happen inside a definition context
             raise Exception("Can not instance a circuit outside a definition")
 
     def __repr__(self):
         args = []
         for k, v in self.kwargs.items():
@@ -577,17 +643,15 @@
         return f"{typ}({args})"
 
 
 @deprecated(
     msg="DeclareCircuit factory method is deprecated, subclass Circuit instead")
 def DeclareCircuit(name, *decl, **args):
     """DeclareCircuit Factory"""
-    debug_info = None
-    if get_debug_mode():
-        debug_info = get_callee_frame_info()
+    debug_info = get_debug_info(4)
     metacls = CircuitKind
     bases = (CircuitType,)
     dct = metacls.__prepare__(name, bases)
     dct.update(dict(IO=decl,
                     debug_info=debug_info,
                     is_definition=False,
                     primitive=args.get('primitive', True),
@@ -652,89 +716,96 @@
                 _logger.warning("'definition' class method syntax is "
                                 "deprecated, use inline definition syntax "
                                 "instead", debug_info=self.debug_info)
                 # NOTE(leonardt): We can call setup here before placing
                 # instances because old style IO syntax doesn't support the
                 # automatic clock lifting anyways
                 _setup_interface(self)
-                with _DefinitionContextManager(self._context_):
+                with definition_context_manager(self._context_):
                     self.definition()
                 self._context_.place_instances(self)
                 self._context_.finalize(self)
                 self._is_definition = True
                 run_unconnected_check = True
             elif self._syntax_style_ is _SyntaxStyle.NEW:
                 _logger.warning("Supplying method 'definition' with new inline "
                                 "definition syntax is not supported, ignoring "
                                 "'definition'")
         run_unconnected_check = run_unconnected_check or (
             has_definition and self._syntax_style_ is _SyntaxStyle.NEW)
         run_unconnected_check = run_unconnected_check and not \
             dct.get("_ignore_undriven_", False)
         if run_unconnected_check:
-            self.check_unconnected()
+            with capture_logs(self._context_):
+                find_and_log_unconnected_ports(self)
 
         return self
 
-    def _check_port_unconnected(self, port, debug_info):
-        if port.is_output():
-            return
-        if port.is_mixed():
-            for elem in port:
-                self._check_port_unconnected(elem, debug_info)
-            return
-        if port.trace() is None:
-            if isinstance(port, ClockTypes):
-                msg = "{} not driven, will attempt to automatically wire"
-                _logger.info(WiringLog(msg, port), debug_info=debug_info)
-            elif is_clock_or_nested_clock(type(port)):
-                # Must be nested, otherwise caught in previous case
-                for elem in port:
-                    self._check_port_unconnected(elem,
-                                                 debug_info)
-            else:
-                msg = "{} not driven"
-                _logger.error(WiringLog(msg, port), debug_info=debug_info)
-
-    def check_unconnected(self):
-        for port in self.interface.ports.values():
-            self._check_port_unconnected(port, self.debug_info)
-
-        for inst in self.instances:
-            for port in inst.interface.ports.values():
-                self._check_port_unconnected(port, inst.debug_info)
+    def __getattr__(self, attr):
+        error = None
+        try:
+            return object.__getattribute__(self, attr)
+        except AttributeError as e:
+            # NOTE(rsetaluri): The scope of `e` is only within this `except`
+            # block. Therefore we have to stash it in a local variable to be
+            # able to raise it later.
+            error = e
+        # NOTE(rsetaluri): We need to use object.__getattribute__ to avoid
+        # potential infinite loops. See
+        # https://github.com/phanrahan/magma/pull/1263.
+        instances = object.__getattribute__(self, "instances")
+        try:
+            return only(filter(lambda i: i.name == attr, instances))
+        except IterableException:
+            pass
+        raise error from None
 
     @property
     def is_definition(self):
         return self._is_definition or self.verilog or self.verilogFile
 
     @property
     def instances(self):
-        return self._context_.placer.instances()
+        # NOTE(rsetaluri): We need to use object.__getattribute__ here because
+        # the instances() property might get called in the __getattr__ pipeline
+        # resulting in an infinite loop. See
+        # https://github.com/phanrahan/magma/pull/1263.
+        context = object.__getattribute__(self, "_context_")
+        return context.placer.instances()
+
+    def get_instance(self, name: str) -> 'AnonymousCircuitType':
+        instances = self.instances
+        try:
+            return only(filter(lambda i: i.name == name, instances))
+        except EmptyIterableException:
+            raise KeyError(name) from None
+        except NonSingletonIterableException:
+            raise KeyError(f"Found multiple instances with name '{name}'")
+
+    @property
+    def logs(self):
+        return self._context_.logs
 
     def place(cls, inst):
         """Place a circuit instance in this definition"""
         cls._context_.placer.place(inst)
 
     def bind(cls, monitor, *args, compile_guard=None):
         cls.bind_modules[monitor] = (args, compile_guard)
 
 
-@six.add_metaclass(DefineCircuitKind)
-class Circuit(CircuitType):
+class Circuit(CircuitType, metaclass=DefineCircuitKind):
     _circuit_base_ = True
 
 
 @deprecated(
     msg="DefineCircuit factory method is deprecated, subclass Circuit instead")
 def DefineCircuit(name, *decl, **args):
     """DefineCircuit Factory"""
-    debug_info = None
-    if get_debug_mode():
-        debug_info = get_callee_frame_info()
+    debug_info = get_debug_info(4)
     metacls = DefineCircuitKind
     bases = (Circuit,)
     dct = metacls.__prepare__(name, bases)
     dct.update(dict(IO=decl,
                     is_definition=True,
                     primitive=args.get('primitive', False),
                     stateful=args.get('stateful', False),
@@ -745,28 +816,32 @@
                     coreir_lib=args.get('coreir_lib', "global"),
                     coreir_genargs=args.get('coreir_genargs', None),
                     coreir_configargs=args.get('coreir_configargs', None),
                     default_kwargs=args.get('default_kwargs', {}),
                     renamed_ports=args.get('renamed_ports', {}),
                     kratos=args.get("kratos", None)))
     defn = metacls(name, bases, dct)
-    _definition_context_stack.push(defn._context_)
+    push_definition_context(defn._context_)
     return defn
 
 
 def EndDefine():
+    # NOTE(rsetaluri): We first peek the definition context
+    # (get_definition_context()) so that we avoid pushing on a log capturer for
+    # the find_and_log_unconnected_ports() call.
     try:
-        context = _definition_context_stack.pop()
+        context = get_definition_context()
     except IndexError:
         raise Exception("EndDefine not matched to DefineCircuit")
     placer = context.placer
-    placer._defn.check_unconnected()
-    debug_info = get_callee_frame_info()
-    placer._defn.end_circuit_filename = debug_info[0]
-    placer._defn.end_circuit_lineno = debug_info[1]
+    find_and_log_unconnected_ports(placer._defn)
+    debug_info = get_debug_info(3)
+    placer._defn.end_circuit_filename = debug_info.filename
+    placer._defn.end_circuit_lineno = debug_info.lineno
+    pop_definition_context()
 
 
 EndCircuit = EndDefine
 
 
 def CopyInstance(instance):
     circuit = type(instance)
@@ -828,15 +903,15 @@
     pass
 
 
 def builder_method(func):
 
     @wraps(func)
     def _wrapped(this, *args, **kwargs):
-        with _DefinitionContextManager(this.context):
+        with definition_context_manager(this.context):
             result = func(this, *args, **kwargs)
         return result
 
     return _wrapped
 
 
 class CircuitBuilder(metaclass=_CircuitBuilderMeta):
@@ -844,26 +919,27 @@
 
     def __init__(self, name):
         # Try to add this builder to a context if one exists currently. A
         # builder can still be constructed outside of a context, but (a) the
         # builder will not be automatically finalized, and (b) instantation
         # might fail.
         try:
-            context = _definition_context_stack.peek()
+            context = get_definition_context()
         except IndexError:
             pass
         else:
             context.add_builder(self)
         self._name = name
         self._io = SingletonInstanceIO()
         self._finalized = False
         self._dct = {}
         self._inst_attrs = {}
         self._context = DefinitionContext(StagedPlacer(self._name))
         self._instance_name = None
+        self.debug_info = get_debug_info(4)
 
     def _port(self, name):
         return self._io.ports[name]
 
     def _add_port(self, name, typ):
         self._io.add(name, typ)
         setattr(self, name, self._io.inst_ports[name])
@@ -881,15 +957,15 @@
             raise Exception(f"Can not set reserved attr '{key}'")
         self._dct[key] = value
 
     def _set_inst_attr(self, key, value):
         self._inst_attrs[key] = value
 
     def _open(self):
-        return _DefinitionContextManager(self._context)
+        return definition_context_manager(self._context)
 
     def _finalize(self):
         pass
 
     def set_instance_name(self, name):
         self._instance_name = name
 
@@ -912,17 +988,67 @@
     def finalize(self, dont_instantiate: bool = False):
         if self._finalized:
             raise Exception("Can only call finalize on a CircuitBuilder once")
         self._finalize()
         bases = (AnonymousCircuitType,)
         dct = {"io": self._io, "_context_": self._context, "name": self._name}
         dct.update(self._dct)
+        dct.setdefault("debug_info", self.debug_info)
         DefineCircuitKind.__prepare__(self._name, bases)
         self._defn = DefineCircuitKind(self._name, bases, dct)
         self._context.finalize(self._defn)
         self._finalized = True
         if dont_instantiate:
             return None
         inst = self._defn(name=self.instance_name)
+        inst.debug_info = self.debug_info
         for k, v in self._inst_attrs.items():
             setattr(inst, k, v)
         return inst
+
+
+class DebugDefineCircuitKind(DefineCircuitKind):
+    def __prepare__(name, bases, **kwargs):
+        prev_debug_mode = get_debug_mode()
+        set_debug_mode(True)
+        # NOTE(leonardt): Using super() here doesn't work:
+        #   cls = super().__prepare__(name, bases, **kwargs)
+        #   TypeError: super(type, obj): obj must be an instance or subtype of
+        #   type
+        cls = DefineCircuitKind.__prepare__(name, bases, **kwargs)
+        ctx = get_definition_context()
+        ctx.set_metadata("prev_debug_mode", prev_debug_mode)
+        return cls
+
+    def __new__(metacls, name, bases, dct):
+        ctx = get_definition_context()
+        set_debug_mode(ctx.get_metadata("prev_debug_mode"))
+        return DefineCircuitKind.__new__(metacls, name, bases, dct)
+
+
+class DebugCircuit(Circuit, metaclass=DebugDefineCircuitKind):
+    pass
+
+
+InstanceCallback = Callable[[List[CircuitType], Dict], None]
+
+
+def register_instance_callback(
+        instance: CircuitType,
+        callback: InstanceCallback,
+):
+    if hasattr(instance, "_callback_"):
+        raise AttributeError(
+            f"Instance {instance} already has callback registered"
+        )
+    instance._callback_ = callback
+
+
+def get_instance_callback(instance: CircuitType) -> InstanceCallback:
+    try:
+        return instance._callback_
+    except AttributeError:
+        msg = (
+            f"Instance {instance} has no callback registered. Did you call "
+            f"m.register_instance_callback()?"
+        )
+        raise AttributeError(msg) from None
```

### Comparing `magma-lang-2.2.9/magma/clock.py` & `magma-lang-2.3.0/magma/clock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 
 from .t import Direction, In
 from .digital import DigitalMeta, Digital
-from .wire import wire
 from magma.bit import Bit
 from magma.array import Array
-from magma.debug import debug_wire
+from magma.debug import get_debug_info
 from magma.tuple import Tuple
 
 
 class _ClockType(Digital):
     @classmethod
     def is_clock(cls):
         return True
@@ -77,15 +76,38 @@
 AsyncResetNIn = AsyncResetN[Direction.In]
 AsyncResetNOut = AsyncResetN[Direction.Out]
 
 
 # Preset
 # Clear
 class Enable(Bit):
-    pass
+    def __init__(self, value=None, name=None):
+        super().__init__(value, name)
+        # We use this flag to track whether an enable as been driven implictly
+        # inside a when context. This allows the user to override the implicit
+        # behavior by wiring a value directly. The when logic will only add
+        # implicit wiring behavior if an enable has not been explicitly wired.
+        self._driven_implicitly_by_when = False
+
+    @property
+    def driven_implicitly_by_when(self):
+        return self._driven_implicitly_by_when
+
+    def wire(self, o, debug_info=None, driven_implicitly_by_when=False):
+        if debug_info is None:
+            debug_info = get_debug_info(3)
+        if self._driven_implicitly_by_when and not driven_implicitly_by_when:
+            # In this case, the enable value was previously implicitly driven by
+            # a when statement, but now the user is explicitly wiring the enable
+            # When this happens, we choose the user's explicit wiring, and
+            # discard the implicit logic (rather than forcing the user to call
+            # rewire explicitly).
+            self.unwire(debug_info=debug_info)
+        super().wire(o, debug_info)
+        self._driven_implicitly_by_when = driven_implicitly_by_when
 
 
 EnableIn = Enable[Direction.In]
 EnableOut = Enable[Direction.Out]
 
 ClockTypes = (Clock, Reset, ResetN, AsyncReset, AsyncResetN, Enable)
```

### Comparing `magma-lang-2.2.9/magma/clock_io.py` & `magma-lang-2.3.0/magma/clock_io.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/compile.py` & `magma-lang-2.3.0/magma/compile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from inspect import getouterframes, currentframe
 from pathlib import PurePath
 
 from magma.backend import verilog, blif, firrtl, dot
 from magma.backend.coreir.coreir_compiler import CoreIRCompiler
 from magma.backend.mlir.mlir_compiler import MlirCompiler
 from magma.bind import BindPass
-from magma.compiler import Compiler
+from magma.bind2 import bind_generators
 from magma.compile_exception import MagmaCompileException
 from magma.config import get_compile_dir
 from magma.inline_verilog import ProcessInlineVerilogPass
 from magma.is_definition import isdefinition
-from magma.passes.clock import WireClockPass
-from magma.passes.drive_undriven import DriveUndrivenPass
-from magma.passes.terminate_unused import TerminateUnusedPass
-from magma.uniquification import (uniquification_pass, UniquificationMode,
-                                  reset_names)
+from magma.passes.drive_undriven import drive_undriven
+from magma.passes.instance_callback_pass import instance_callback_pass
+from magma.passes.terminate_unused import terminate_unused
+from magma.uniquification import (
+    uniquification_pass,
+    reset_names,
+)
 
 
 __all__ = ["compile"]
 
 
 def _make_compiler(output, main, basename, opts):
     if output == "verilog":
@@ -32,53 +34,81 @@
     if output == "coreir":
         return CoreIRCompiler(main, basename, opts)
     if output == "coreir-verilog":
         opts["output_verilog"] = True
         return CoreIRCompiler(main, basename, opts)
     if output == "mlir":
         return MlirCompiler(main, basename, opts)
+    if output == "mlir-verilog":
+        opts["output_verilog"] = True
+        return MlirCompiler(main, basename, opts)
     raise NotImplementedError(f"Backend '{output}' not supported")
 
 
 def _get_basename(basename):
     if get_compile_dir() == "callee_file_dir":
         callee_filename = getouterframes(currentframe())[2][1]
         callee_dir = PurePath(callee_filename).parent
         return str(callee_dir.joinpath(basename))
     return basename
 
 
+def _partial_kw(fn, **specialized_kwargs):
+
+    def func(*args, **kwargs):
+        return fn(*args, **kwargs, **specialized_kwargs)
+
+    return func
+
+
+def _make_bind_compile_fn(output: str):
+    output_is_mlir = (output == "mlir" or output == "mlir-verilog")
+    if not output_is_mlir:
+        return compile
+    return _partial_kw(compile, use_packed_arrays=True)
+
+
 def compile(basename, main, output="coreir-verilog", **kwargs):
     if not isdefinition(main):
         raise MagmaCompileException(
             f"Trying to compile empty definition {main}")
     if hasattr(main, "circuit_definition"):
         main = main.circuit_definition
     basename = _get_basename(basename)
     opts = kwargs.copy()
     compiler = _make_compiler(output, main, basename, opts)
 
+    bind_generators(main)
+
+    compiler.run_pre_uniquification_passes()
     # Default behavior is to perform uniquification, but can be overriden.
     original_names = uniquification_pass(main, opts.get("uniquify", "UNIQUIFY"))
 
     # Steps to process inline verilog generation. Required to be run after
     # uniquification.
     ProcessInlineVerilogPass(main).run()
 
     # Bind after uniquification so the bind logic works on unique modules.
-    BindPass(main, compile, opts.get("user_namespace"),
+    # NOTE(rsetaluri): This is a hack to use packed arrays when the compilation
+    # goes through MLIR.
+    compile_fn = _make_bind_compile_fn(output)
+    BindPass(main, compile_fn, opts.get("user_namespace"),
              opts.get("verilog_prefix")).run()
 
     if opts.get("drive_undriven", False):
-        DriveUndrivenPass(main).run()
+        drive_undriven(main)
     if opts.get("terminate_unused", False):
-        TerminateUnusedPass(main).run()
+        terminate_unused(main)
+
+    instance_callback_pass_data = instance_callback_pass(main)
 
     result = compiler.compile()
     result = {} if result is None else result
 
     if hasattr(main, "fpga"):
         main.fpga.constraints(basename)
 
+    result["instance_callback_pass_data"] = instance_callback_pass_data
+
     reset_names(original_names)
 
     return result
```

### Comparing `magma-lang-2.2.9/magma/compiler.py` & `magma-lang-2.3.0/magma/compiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 
 
 __all__ = ["Compiler", "make_compiler"]
 
 
 class Compiler:
     def __init__(self, main, basename, opts={}):
         self.main = main
         self.basename = basename
         self.opts = opts
 
+    def run_pre_uniquification_passes(self):
+        pass
+
     def compile(self):
         suffix = self.suffix()
         code = self.generate_code()
         with open(f"{self.basename}.{suffix}", "w") as f:
             f.write(code)
 
     @abstractmethod
```

### Comparing `magma-lang-2.2.9/magma/config.py` & `magma-lang-2.3.0/magma/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,23 +55,25 @@
         self.set(value)
 
 
 class ConfigManager:
     __entries = {}
 
     def __init__(self, **kwargs):
-        for key, value in kwargs.items():
-            ConfigManager.__entries[key] = value
+        self._register(**kwargs)
 
     def _register(self, **kwargs):
         for key, value in kwargs.items():
             if key in ConfigManager.__entries:
                 raise RuntimeError(f"Config with key '{key}' already exists")
             ConfigManager.__entries[key] = value
 
+    def register(self, **kwargs):
+        self._register(**kwargs)
+
     def __get(self, key):
         return ConfigManager.__entries[key].get()
 
     def __set(self, key, value):
         ConfigManager.__entries[key].set(value)
 
     def __getattr__(self, key):
@@ -85,15 +87,15 @@
 
     def __setitem__(self, key, value):
         self.__set(key, value)
 
 
 config = ConfigManager(
     compile_dir=RuntimeConfig("normal"),
-    debug_mode=RuntimeConfig(False),
+    debug_mode=RuntimeConfig(False)
 )
 
 
 def get_debug_mode():
     return config.debug_mode
```

### Comparing `magma-lang-2.2.9/magma/conversions.py` & `magma-lang-2.3.0/magma/conversions.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,33 +13,19 @@
 from .digital import Digital
 from .tuple import Tuple, Product
 from .protocol_type import magma_type, magma_value
 from .bitutils import int2seq
 import hwtypes as ht
 from magma.array import Array
 from magma.circuit import coreir_port_mapping
-from magma.common import is_int, Finalizable, lca_of_types
+from magma.common import is_int, Finalizable, lca_of_types, deprecated
 from magma.generator import Generator2
 from magma.interface import IO
 
 
-__all__ = ['bit']
-__all__ += ['clock', 'reset', 'enable', 'asyncreset', 'asyncresetn']
-
-__all__ += ['array']
-__all__ += ['bits', 'uint', 'sint']
-
-__all__ += ['tuple_', 'namedtuple']
-
-__all__ += ['concat', 'repeat']
-__all__ += ['sext', 'zext', 'sext_to', 'sext_by', 'zext_to', 'zext_by']
-__all__ += ['replace']
-__all__ += ['as_bits', 'from_bits']
-
-
 class _Concatter(Finalizable):
     def __init__(self):
         self._ts = []
         self._types = []
 
     def _consume_impl(self, value):
         if isinstance(value, ht.BitVector):
@@ -70,17 +56,19 @@
     return isinstance(magma_value(value), (Digital, Array, Tuple, IntegerTypes))
 
 
 def can_convert_to_bit_type(value):
     return issubclass(magma_type(value), (Digital, Array, Tuple))
 
 
-def convertbit(value, totype):
+def convertbit(value, totype, name=None):
+    # NOTE: We don't do `isinstance` here because we want an upcast to cause a
+    # conversion
     value = magma_value(value)
-    if isinstance(value, totype):
+    if type(value) is totype:
         return value
 
     if not can_convert_to_bit(value):
         raise ValueError(
             "bit can only be used on a Bit, an Array, or an int"
             f"; not {type(value)}")
 
@@ -98,50 +86,55 @@
     assert isinstance(value, (IntegerTypes, Digital))
 
     if isinstance(value, IntegerTypes):
         # Just return VCC or GND here, otherwise we lose VCC/GND singleton
         # invariant
         return totype(1) if value else totype(0)
 
+    if name is None:
+        name = value.name
+
     if value.is_input():
-        b = In(totype)(name=value.name)
+        b = In(totype)(name=name)
     elif value.is_output():
-        b = Out(totype)(name=value.name)
+        b = Out(totype)(name=name)
     else:
-        b = totype()
+        b = totype(name=name)
     b._wire = value._wire
     return b
 
 
-def bit(value):
-    return convertbit(value, Bit)
+def bit(value, name=None):
+    return convertbit(value, Bit, name=name)
 
 
-def clock(value):
-    return convertbit(value, Clock)
+def clock(value, name=None):
+    return convertbit(value, Clock, name=name)
 
 
-def reset(value):
-    return convertbit(value, Reset)
+def reset(value, name=None):
+    return convertbit(value, Reset, name=name)
 
 
-def asyncreset(value):
-    return convertbit(value, AsyncReset)
+def asyncreset(value, name=None):
+    return convertbit(value, AsyncReset, name=name)
 
 
-def asyncresetn(value):
-    return convertbit(value, AsyncResetN)
+def asyncresetn(value, name=None):
+    return convertbit(value, AsyncResetN, name=name)
 
 
-def enable(value):
-    return convertbit(value, Enable)
+def enable(value, name=None):
+    return convertbit(value, Enable, name=name)
 
 
-def convertbits(value, n, totype, checkbit):
-    if isinstance(value, totype):
+def convertbits(value, n, totype, checkbit, name=None):
+    # NOTE: We don't do `isinstance` here because we want an upcast to cause a
+    # conversion
+    if type(value) is totype:
         if n is not None and n != len(value):
             raise ValueError("converting a value should not change the size, use concat, zext, or sext instead.")
         return value
 
     value = magma_value(value)
     convertible_types = (Digital, Tuple, Array, IntegerTypes,
                          Sequence, ht.BitVector)
@@ -206,38 +199,42 @@
         ts = [bit(t) for t in ts]
         T = {
             Direction.In: In,
             Direction.Out: Out,
             Direction.InOut: InOut
         }[T.direction](Bit)
 
-    value = totype[len(Ts), T](ts)
+    value = totype[len(Ts), T](ts, name=name)
     if n is not None and len(value) < n:
+        # TODO(leonardt): The extended value isn't named, but perhaps we'd like to move
+        # to an explicit convert + extend rather than doing them in a single
+        # operation? If so, then we could provide the same name interface for
+        # the extension operators.
         value = value.ext_to(n)
     return value
 
 
-def array(value, n=None):
-    return convertbits(value, n, Array, False)
+def array(value, n=None, name=None):
+    return convertbits(value, n, Array, False, name=name)
 
 
-def bits(value, n=None):
-    return convertbits(value, n, Bits, True)
+def bits(value, n=None, name=None):
+    return convertbits(value, n, Bits, True, name=name)
 
 
-def uint(value, n=None):
-    return convertbits(value, n, UInt, True)
+def uint(value, n=None, name=None):
+    return convertbits(value, n, UInt, True, name=name)
 
 
-def sint(value, n=None):
-    return convertbits(value, n, SInt, True)
+def sint(value, n=None, name=None):
+    return convertbits(value, n, SInt, True, name=name)
 
 
-def bfloat(value, n=None):
-    return convertbits(value, n, BFloat, True)
+def bfloat(value, n=None, name=None):
+    return convertbits(value, n, BFloat, True, name=name)
 
 
 def concat(*args):
     concatter = _Concatter()
     for arg in args:
         concatter.consume(arg)
     return concatter.finalize()
@@ -368,15 +365,15 @@
             decl[d] = Bits[len(decl[d])]
 
     if t == Tuple:
         return t[tuple(decl.values())](*args)
     assert t == Product
     return t.from_fields("anon", decl)(*args)
 
-
+@deprecated(msg="namedtuple() is deprecated, use product() instead")
 def namedtuple(**kwargs):
     return _tuple(kwargs, t=Product)
 
 
 def product(**kwargs):
     return _tuple(kwargs, t=Product)
```

### Comparing `magma-lang-2.2.9/magma/digital.py` & `magma-lang-2.3.0/magma/digital.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from functools import lru_cache
 import weakref
 from abc import ABCMeta
 import hwtypes as ht
-from .t import Kind, Direction, Type, In, Out
-from .debug import debug_wire, get_callee_frame_info
+from .t import Kind, Direction, Type
+from .debug import debug_wire, get_debug_info
 from .compatibility import IntegerTypes
 from .logging import root_logger
 from .protocol_type import magma_type, magma_value
 
-from magma.ref import ArrayRef
-from magma.wire_container import Wire, WiringLog, Wireable
+from magma.wire_container import WiringLog, Wireable
 
 
 _logger = root_logger()
 
 
 class DigitalMeta(ABCMeta, Kind):
     _class_cache = weakref.WeakValueDictionary()
@@ -133,17 +132,18 @@
 
     @lru_cache()
     def is_wireable(cls, rhs):
         if issubclass(rhs, (bool, int, ht.Bit)):
             return True
         rhs = magma_type(rhs)
         # allows undirected types to match (e.g. for temporary values)
-        return (issubclass(rhs.flip(), cls) or issubclass(cls, rhs.flip()) or
-                cls.qualify(Direction.Undirected) is rhs or
-                rhs.qualify(Direction.Undirected) is cls)
+        return (
+            issubclass(rhs.undirected_t, cls.undirected_t)
+            or issubclass(cls.undirected_t, rhs.undirected_t)
+        )
 
     def is_bindable(cls, rhs):
         return issubclass(cls, magma_type(rhs))
 
     __hash__ = type.__hash__
 
 
@@ -160,15 +160,15 @@
         return cls.direction == direction
 
     @classmethod
     def is_clock(cls):
         return False
 
     def __call__(self, output):
-        return self.wire(output, get_callee_frame_info())
+        return self.wire(output, get_debug_info(3))
 
     @debug_wire
     def wire(self, o, debug_info):
         # promote integer types to LOW/HIGH
         if isinstance(o, (IntegerTypes, bool, ht.Bit)):
             o = HIGH if o else LOW
```

### Comparing `magma-lang-2.2.9/magma/display.py` & `magma-lang-2.3.0/magma/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from magma.circuit import peek_definition_context_stack
+from magma.definition_context import get_definition_context
 from magma.t import Type
 
 
 class _Time:
     pass
 
 
@@ -128,26 +128,26 @@
     {cond_str}{display_str}\"{self.display_str}\"{display_args_str});
 end
 """
         return format_str, format_args, {}
 
 
 def display(display_str, *args, file=None):
-    context = peek_definition_context_stack()
+    context = get_definition_context()
     disp = Display(display_str, args, file)
     context.get_child("display").add_display(disp)
     return disp
 
 
 class File:
     def __init__(self, filename, mode):
         self.filename = filename
         self.mode = mode
 
-        context = peek_definition_context_stack()
+        context = get_definition_context()
         context.get_child("display").add_file(self)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
```

### Comparing `magma-lang-2.2.9/magma/enum.py` & `magma-lang-2.3.0/magma/enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             if field == "N":
                 # TODO: Make N unreserved
                 raise ValueError("N is a reserved name in Enum")
         max_value = max(value for value in fields.values())
         num_bits = max(max_value.bit_length(), 1)
         type_ = cls[num_bits]
         type_._is_magma_enum = True
+        type_.fields = fields
         for key, value in fields.items():
             setattr(type_, key, BitVector[num_bits](value))
         return type_
 
 
 class Enum(Bits, metaclass=EnumMeta):
     pass
```

### Comparing `magma-lang-2.2.9/magma/frontend/coreir.py` & `magma-lang-2.3.0/magma/frontend/coreir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/frontend/coreir_.py` & `magma-lang-2.3.0/magma/frontend/coreir_.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/frontend/pyverilog_importer.py` & `magma-lang-2.3.0/magma/frontend/pyverilog_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import pyverilog.dataflow.visit
 import pyverilog.vparser.parser
 from ..array import Array
 from ..bit import Bit
 from ..bits import Bits
 from ..circuit import Circuit
 from ..interface import IO
-from ..math import log2_ceil
 from ..passes.tsort import tsort
 from ..t import In, Out, InOut
 from .verilog_importer import (ImportMode, MultipleModuleDeclarationError,
                                MultiplePortDeclarationError, VerilogImporter,
                                VerilogImportError)
 from .verilog_utils import int_const_str_to_int
+from magma.bitutils import clog2
 
 
 class PyverilogImportError(VerilogImportError):
     pass
 
 
 def _evaluate_node(node, params):
@@ -45,15 +45,15 @@
         return l * r  # floor division
     if isinstance(node, pyverilog.vparser.ast.Identifier):
         return params[node.name]
     if isinstance(node, pyverilog.vparser.ast.SystemCall):
         syscall = node.syscall
         if syscall == "clog2":
             operand = _evaluate_node(node.children()[0], params)
-            return log2_ceil(operand)
+            return clog2(operand)
         raise PyverilogImportError(
             f"Unsupported verilog system call: {syscall}")
     raise PyverilogImportError(f"Unsupported expression: {type(node)}")
 
 
 def _get_width(width, param_map):
     """Evaluates width.msb, width.lsb and returns their difference"""
```

### Comparing `magma-lang-2.2.9/magma/frontend/verilog.py` & `magma-lang-2.3.0/magma/frontend/verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/frontend/verilog_importer.py` & `magma-lang-2.3.0/magma/frontend/verilog_importer.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/frontend/verilog_utils.py` & `magma-lang-2.3.0/magma/frontend/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/interface.py` & `magma-lang-2.3.0/magma/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
-from collections import OrderedDict
 from itertools import chain
 from .common import deprecated
 from .compatibility import IntegerTypes, StringTypes
 from .protocol_type import MagmaProtocolMeta
 from .ref import InstRef, DefnRef, LazyDefnRef, LazyInstRef, NamedRef
 from .t import Type, Kind, Direction
+import weakref
 
 
 __all__  = ['make_interface']
 __all__ += ['InterfaceKind', 'Interface', 'AnonymousInterface']
 __all__ += ['IO', 'SingletonInstanceIO']
 
 
@@ -110,38 +110,37 @@
     """
     if value.is_output():
         return ""
     if value.is_mixed():
         return "".join(_make_wires(v, wired)
                        for v, _ in value.connection_iter())
     driver = value.value()
+    if (driver, value) in wired:
+        return ""
+    while driver is not None and driver.is_driven_anon_temporary():
+        driver = driver.value()
     if driver is None:
         return ""
     if driver.has_children() and driver.name.anon():
         return "".join(_make_wires(v, wired)
                        for v, _ in value.connection_iter())
-    while driver is not None and driver.is_driven_anon_temporary():
-        driver = driver.value()
-    s = ""
-    while driver is not None:
-        if (driver, value) in wired:
-            break
-        s += _make_wire_str(driver, value, wired)
-        if not driver.driven():
-            break
-        value = driver
-        driver = driver.value()
+    s = _make_wire_str(driver, value, wired)
+    if driver.driven():
+        s += _make_wires(driver, wired)
     return s
 
 
+def _dict_from_decl(decl):
+    return dict(zip(decl[::2], decl[1::2]))
+
+
 class InterfaceKind(Kind):
     def __init__(cls, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        args = zip(cls._decl[::2], cls._decl[1::2])
-        cls.ports = OrderedDict(args)
+        cls.ports = _dict_from_decl(cls._decl)
 
     def items(cls):
         return cls.ports.items()
 
     def __iter__(cls):
         return iter(cls.ports)
 
@@ -153,14 +152,16 @@
     def __str__(cls):
         return f"Interface({cls.args_to_str()})"
 
     def __repr__(cls):
         return str(cls)
 
     def __eq__(cls, rhs):
+        if not isinstance(rhs, InterfaceKind):
+            return False
         return cls._decl == rhs._decl
 
     def __ne__(cls, rhs):
         return super().__ne__(rhs)
 
     def __hash__(cls):
         return super().__hash__()
@@ -278,15 +279,15 @@
             # Convert integer to str, e.g. 0 to "0".
             if isinstance(name, IntegerTypes):
                 return str(name)
             return name
 
         names, types = _parse_decl(decl)
         names = map(_map_name, names)
-        self.ports = OrderedDict(zip(names, types))
+        self.ports = dict(zip(names, types))
 
     def __str__(self):
         s = ", ".join(f"{k}: {v}" for k, v in self.ports.items())
         return f"Interface({s})"
 
 
 class AnonymousInterface(Interface):
@@ -325,14 +326,16 @@
         assert not (inst is not None and defn is not None)
         cls = type(self)
         names, types = _parse_decl(cls._decl)
         refs = (_make_ref(name, inst, defn) for name in names)
         args = zip(names, zip(types, refs))
         flip = defn is not None
         self.ports = {n: _make_port(t, r, flip) for n, (t, r) in args}
+        for port in self.ports.values():
+            port.name._value = weakref.ref(port)
         _rename_ports(self.ports, renamed_ports)
 
 
 class _DeclareSingletonInterface(_DeclareInterface):
     """_DeclareSingletonInterface class"""
     def __init__(self, renamed_ports={}, *, inst=None, defn=None):
         assert not (inst is not None and defn is not None)
@@ -340,15 +343,15 @@
         # definition (not instances or further definition instancing).
         cls = type(self)
         if cls._initialized:
             super().__init__(renamed_ports, inst=inst, defn=defn)
             return
         assert defn is not None
         cls._io.bind(defn)  # bind IO to @defn
-        self.ports = OrderedDict(cls._io.ports.items())
+        self.ports = dict(cls._io.ports.items())
         _rename_ports(self.ports, renamed_ports)  # rename ports
         cls._initialized = True
 
 
 class _DeclareSingletonInstanceInterface(_DeclareInterface):
     """_DeclareSingletonInterface class"""
     def __init__(self, renamed_ports={}, *, inst=None, defn=None):
@@ -358,24 +361,24 @@
         cls = type(self)
 
         if defn:
             if cls._initialized:
                 super().__init__(renamed_ports, inst=inst, defn=defn)
                 return
             cls._io.bind(defn)  # bind IO to @defn
-            self.ports = OrderedDict(cls._io.ports.items())
+            self.ports = dict(cls._io.ports.items())
             _rename_ports(self.ports, renamed_ports)  # rename ports
             cls._initialized = True
             return
         if inst:
             if cls._initialized_inst:
                 super().__init__(renamed_ports, inst=inst, defn=defn)
                 return
             cls._io.bind_inst(inst)  # bind IO to @inst
-            self.ports = OrderedDict(cls._io.inst_ports.items())
+            self.ports = dict(cls._io.inst_ports.items())
             _rename_ports(self.ports, renamed_ports)  # rename ports
             cls._initialized_inst = True
             return
         super().__init__(renamed_ports, inst=inst, defn=defn)
 
 
 def make_interface(*decl):
@@ -414,14 +417,17 @@
     def __add__(self, other):
         raise NotImplementedError()
 
     def __iadd__(self, other):
         # __iadd__ is explicitly overriden to enforce that it is non-mutating.
         return self + other
 
+    def flip(self) -> "IOInterface":
+        raise NotImplementedError()
+
 
 class IO(IOInterface):
     """
     Class for creating an interface bundle.
 
     @kwargs: ordered dict of {name: type}, ala decl.
     """
@@ -430,16 +436,15 @@
     # https://www.python.org/dev/peps/pep-0468/.
     def __init__(self, **kwargs):
         self._ports = {}
         self._decl = []
         self._bound = False
         for name, typ in kwargs.items():
             self.add(name, typ)
-            self._decl.append(name)
-            self._decl.append(typ)
+            self._decl.extend((name, typ))
 
     @property
     def ports(self):
         return self._ports.copy()
 
     def bind(self, defn):
         if self._bound:
@@ -472,29 +477,42 @@
             raise TypeError(f"unsupported operand type(s) for +: 'IO' and "
                             f"'{type(other).__name__}'")
         if self._bound or other._bound:
             raise Exception("Adding bound IO not allowed")
         if self._ports.keys() & other._ports.keys():
             raise Exception("Adding IO with duplicate port names not allowed")
         decl = self._decl + other._decl
-        return IO(**dict(zip(decl[::2], decl[1::2])))
+        return IO(**_dict_from_decl(decl))
 
     def add(self, name, typ):
         if self._bound:
             raise RuntimeError("Can not add to a bound IO")
         # Definition port.
         ref = LazyDefnRef(name=name)
         port = _make_port(typ, ref, flip=True)
         self._ports[name] = port
 
-    def __getattr__(self, key):
-        if key in self._ports:
-            return self._ports[key]
+    def _get(self, key: str):
+        return self._ports[key]
+
+    def __getitem__(self, key: str):
+        return self._get(key)
+
+    def __getattr__(self, key: str):
+        try:
+            return self._get(key)
+        except KeyError:
+            pass
         return super().__getattribute__(key)
 
+    def fields(self):
+        return _dict_from_decl(self._decl)
+
+    def flip(self):
+        return IO(**{name: T.flip() for name, T in self.fields().items()})
 
 
 class SingletonInstanceIO(IO):
     """
     Class for creating an interface bundle for a singleton instance.
 
     @kwargs: ordered dict of {name: type}, ala decl.
@@ -532,7 +550,10 @@
         inst_ref = LazyInstRef(name=name)
         inst_port = _make_port(typ, inst_ref, flip=False)
         self._inst_ports[name] = inst_port
 
     def __add__(self, other):
         raise NotImplementedError(f"Addition operator disallowed on "
                                   f"{cls.__name__}")
+
+    def flip(self):
+        raise NotImplementedError()
```

### Comparing `magma-lang-2.2.9/magma/ir.py` & `magma-lang-2.3.0/magma/ir.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/linking.py` & `magma-lang-2.3.0/magma/linking.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/log.py` & `magma-lang-2.3.0/magma/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 
-from magma.circuit import peek_definition_context_stack
+from magma.definition_context import get_definition_context
 from magma.display import Display
 
 
 class Log(Display):
     level = None
 
     def __init__(self, display_str, args, file=None):
@@ -34,15 +34,15 @@
 class Error(Log):
     level = 3
 
 
 def _make_log_func(T):
     @functools.wraps(_make_log_func)
     def log_func(log_str, *args, file=None):
-        context = peek_definition_context_stack()
+        context = get_definition_context()
         log = T(log_str, args, file=file)
         context.get_child("display").add_display(log)
         context.get_child("display").insert_default_log_level()
         return log
     return log_func
```

### Comparing `magma-lang-2.2.9/magma/logging.py` & `magma-lang-2.3.0/magma/logging.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+import abc
 import colorlog
+import contextlib
 import inspect
 import io
 import logging
 import sys
 import traceback
-from .backend.util import make_relative
-from .config import config, EnvConfig
+
+from magma.backend.util import make_relative
+from magma.common import Stack
+from magma.config import config, EnvConfig
 
 
 config._register(
     log_stream=EnvConfig("MAGMA_LOG_STREAM", "stderr"),
     log_level=EnvConfig("MAGMA_LOG_LEVEL", "INFO"),
     include_traceback=EnvConfig("MAGMA_INCLUDE_WIRE_TRACEBACK", False, bool),
     traceback_limit=EnvConfig("MAGMA_ERROR_TRACEBACK_LIMIT", 5, int),
 )
 
 
-_staged_logging = False
-_staged_logs = []
+_staged_logs_stack = Stack()
+_log_capturer_stack = Stack()
 
 
 def _make_bold(string):
     return f"\033[1m{string}\033[0m"
 
 
 def _get_source_line(filename, lineno):
     with open(filename, "r") as f:
         return f.readlines()[lineno - 1]
 
 
 def _attach_debug_info(msg, debug_info):
-    file = debug_info[0]
-    line = debug_info[1]
+    file = debug_info.filename
+    line = debug_info.lineno
     line_info = _make_bold(f"{make_relative(file)}:{line}")
     msg = f"{line_info}: {msg}"
     try:
         source = _get_source_line(file, line).rstrip("\n")
         source = f">> {source}"
     except FileNotFoundError:
         source = f"(Could not file file {file})"
@@ -67,94 +71,189 @@
     try:
         value = kwargs.pop(key)
         return value
     except KeyError:
         return None
 
 
+def get_staged_logs_stack() -> Stack:
+    global _staged_logs_stack
+    return _staged_logs_stack
+
+
 class _MagmaLogger(logging.Logger):
     """
     Derivative of logging.Logger class, with two additional keyword args:
     * 'debug_info': Tuple of (file_name, line_no). If 'debug_info' is included,
        this source-level information is logged along with the message.
     * 'include_traceback': If True, a traceback is printed along with the
        message.
     """
-    @staticmethod
-    def __with_preamble(fn, msg, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._raw = False
+
+    @property
+    def raw(self) -> bool:
+        return self._raw
+
+    @raw.setter
+    def raw(self, raw: bool):
+        self._raw = raw
+
+    @contextlib.contextmanager
+    def as_raw(self):
+        prev_raw = self.raw
+        self.raw = True
+        try:
+            yield self
+        finally:
+            self.raw = prev_raw
+
+    def _log(self, level, msg, args, **kwargs):
+        if not self.raw and self._staged_log(level, msg, args, **kwargs):
+            return
+        self._raw_log(level, msg, args, **kwargs)
+
+    def _staged_log(self, level, msg, args, **kwargs) -> bool:
+        staged_logs_stack = get_staged_logs_stack()
+        try:
+            staged_logs = staged_logs_stack.peek()
+        except IndexError:
+            return False
+        staged_logs.append((self, level, msg, args, kwargs))
+        return True
+
+    def _capture_log(self, level, msg, args, **kwargs):
+        try:
+            log_capturer = get_log_capturer()
+        except IndexError:
+            return
+        log_capturer.add_log((level, msg, args, kwargs))
+
+    def _raw_log(self, level, msg, args, **kwargs):
         debug_info = _get_additional_kwarg(kwargs, "debug_info")
         if debug_info:
             msg = _attach_debug_info(msg, debug_info)
         include_traceback = _get_additional_kwarg(kwargs, "include_traceback")
         if include_traceback or config.include_traceback:
             msg = _attach_traceback(
                 msg, _frame_selector, config.traceback_limit)
-        fn(msg, *args, **kwargs)
-
-    def log(self, level, msg, *args, **kwargs):
-        key = logging.getLevelName(level).lower()
-        fn = getattr(_MagmaLogger, key)
-        fn(self, msg, *args, **kwargs)
-
-    def debug(self, msg, *args, **kwargs):
-        global _staged_logging
-        if _staged_logging:
-            _staged_logs.append((self, logging.DEBUG, msg, args, kwargs))
-            return
-        _MagmaLogger.__with_preamble(super().debug, msg, *args, **kwargs)
-
-    def info(self, msg, *args, **kwargs):
-        global _staged_logging
-        if _staged_logging:
-            _staged_logs.append((self, logging.INFO, msg, args, kwargs))
-            return
-        _MagmaLogger.__with_preamble(super().info, msg, *args, **kwargs)
-
-    def warning(self, msg, *args, **kwargs):
-        global _staged_logging
-        if _staged_logging:
-            _staged_logs.append((self, logging.WARNING, msg, args, kwargs))
-            return
-        _MagmaLogger.__with_preamble(super().warning, msg, *args, **kwargs)
-
-    def error(self, msg, *args, **kwargs):
-        global _staged_logging
-        if _staged_logging:
-            _staged_logs.append((self, logging.ERROR, msg, args, kwargs))
-            return
-        _MagmaLogger.__with_preamble(super().error, msg, *args, **kwargs)
+        self._capture_log(level, msg, args, **kwargs)
+        super()._log(level, msg, args, **kwargs)
 
 
 # Set logging class to _MagmaLogger to override logging behavior. Also, setup
 # root logger parameters.
 logging.setLoggerClass(_MagmaLogger)
 _log_stream = getattr(sys, config.log_stream)
 _root_logger = logging.getLogger("magma")
 _handler = colorlog.StreamHandler(_log_stream)
 _handler.setFormatter(colorlog.ColoredFormatter(
     '%(log_color)s%(levelname)s%(reset)s:%(name)s:%(message)s'))
 _root_logger.addHandler(_handler)
 _root_logger.setLevel(config.log_level)
 
 
-def flush():
-    global _staged_logs
-    curr_logs = _staged_logs.copy()
-    for logger, level, obj, args, kwargs in curr_logs:
-        logger.log(level, obj, *args, **kwargs)
-    _staged_logs = []
-    return curr_logs
-
-
 def root_logger():
     return logging.getLogger("magma")
 
 
+# NOTE(rsetaluri): For some reason the following code which uses
+# contextlib.contextmanager results in the context manager being entered into
+# twice. It may be cached somewhere in the pipeline.
+#
+#    @contextlib.contextmanager
+#    def logging_level(level):
+#        root = root_logger()
+#        prev_level = root.level
+#        root.setLevel(level)
+#        try:
+#            yield
+#        finally:
+#            root.setLevel(prev_level)
+class logging_level:
+    def __init__(self, level):
+        self.level = level
+        self.root = root_logger()
+
+    def __enter__(self):
+        self.prev_level = self.root.level
+        self.root.setLevel(self.level)
+
+    def __exit__(self, *_):
+        self.root.setLevel(self.prev_level)
+
+
 def stage_logger():
-    global _staged_logging
-    _staged_logging = True
+    get_staged_logs_stack().push([])
+
+
+def _flush(staged_logs):
+    for logger, level, obj, args, kwargs in staged_logs:
+        with logger.as_raw():
+            logger.log(level, obj, *args, **kwargs)
+
+
+def flush():
+    staged_logs = get_staged_logs_stack().pop()
+    _flush(staged_logs)
+    return staged_logs
 
 
 def unstage_logger():
-    global _staged_logging
-    _staged_logging = False
     return flush()
+
+
+def flush_all():
+    staged_logs_stack = get_staged_logs_stack()
+    while staged_logs_stack:
+        staged_logs = staged_logs_stack.pop()
+        _flush(staged_logs)
+
+
+@contextlib.contextmanager
+def staged_logs():
+    stage_logger()
+    staged_logs = get_staged_logs_stack().peek()
+    try:
+        yield staged_logs
+    finally:
+        unstage_logger()
+
+
+class StagedLogRecord(abc.ABC):
+    def __init__(self, tpl: str):
+        self._tpl = tpl
+
+    @abc.abstractmethod
+    def args(self):
+        raise NotImplementedError()
+
+    def __str__(self):
+        return self._tpl.format(*self.args())
+
+
+def _get_log_capturer_stack() -> Stack:
+    global _log_capturer_stack
+    return _log_capturer_stack
+
+
+def push_log_capturer(log_capturer):
+    _get_log_capturer_stack().push(log_capturer)
+
+
+def pop_log_capturer():
+    _get_log_capturer_stack().pop()
+
+
+def get_log_capturer():
+    return _get_log_capturer_stack().peek()
+
+
+@contextlib.contextmanager
+def capture_logs(log_capturer):
+    push_log_capturer(log_capturer)
+    try:
+        yield
+    finally:
+        pop_log_capturer()
```

### Comparing `magma-lang-2.2.9/magma/passes/clock.py` & `magma-lang-2.3.0/magma/passes/clock.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from magma.array import Array
 from magma.circuit import Circuit, DefineCircuitKind
 from magma.clock import (
     ClockTypes, Clock, Reset, Enable, ResetN, AsyncReset, AsyncResetN,
     is_clock_or_nested_clock)
 from magma.common import (
     only, IterableException, EmptyIterableException,
-    NonSignletonIterableException)
+    NonSingletonIterableException)
 from magma.logging import root_logger
-from magma.passes.passes import DefinitionPass
+from magma.passes.passes import DefinitionPass, pass_lambda
 from magma.primitives.wire import Wire
 from magma.t import Type, Kind
 from magma.tuple import Tuple
 
 
 _logger = root_logger()
 
@@ -26,26 +26,36 @@
     """
     if not is_clock_or_nested_clock(type(value).T, (clock_type, )):
         return None
     for elem in value:
         yield from get_output_clocks_in_value(elem, clock_type)
 
 
+def _get_output_clocks_in_tuple(
+        value: Tuple, clock_type: Kind
+) -> Iterable[Type]:
+    """
+    Gets all output values of type @clock_type recursively contained in @value.
+    """
+    for key, type_ in type(value).field_dict.items():
+        if is_clock_or_nested_clock(type_, (clock_type, )):
+            yield from get_output_clocks_in_value(value[key], clock_type)
+
+
 def get_output_clocks_in_value(value: Type, clock_type: Kind) -> Iterable[Type]:
     """
     Gets all output values of type @clock_type recursively contained in @value.
     """
     # Since we are looking for default drivers, only need to consider outputs.
     if value.is_input():
         return None
     if isinstance(value, clock_type):
         yield value
     if isinstance(value, Tuple):
-        for elem in value:
-            yield from get_output_clocks_in_value(elem, clock_type)
+        yield from _get_output_clocks_in_tuple(value, clock_type)
     if isinstance(value, Array):
         yield from _get_output_clocks_in_array(value, clock_type)
 
 
 def get_output_clocks_in_defn(
         defn: DefineCircuitKind, clock_type: Kind) -> Iterable[Type]:
     """
@@ -101,14 +111,17 @@
     for elem in value[1:]:
         yield from get_undriven_clocks_in_value(elem, clock_type)
 
 
 def get_undriven_clocks_in_value(
         value: Type, clock_type: Kind) -> Iterable[Type]:
     """Returns all undriven values of type @clock_type contained in @value."""
+    if not is_clock_or_nested_clock(type(value), (clock_type, )):
+        # Avoid descening into tuple/array if possible
+        return
     if isinstance(value, Tuple):
         for elem in value:
             yield from get_undriven_clocks_in_value(elem, clock_type)
         return
     if isinstance(value, Array):
         yield from _get_undriven_clocks_in_array(value, clock_type)
         return
@@ -117,15 +130,15 @@
         while value.driven():
             value = value.value()
         yield value
     return
 
 
 def _drive_value_with_clock(value: Type, clk: Type):
-    _logger.info(f"Auto-wiring {repr(clk)} to {repr(value)}")
+    _logger.debug(f"Auto-wiring {repr(clk)} to {repr(value)}")
     value @= clk
 
 
 def drive_undriven_clocks_in_inst(
         defn: DefineCircuitKind, inst: Circuit, clock_type: Kind):
     """
     Drives all undriven input ports of @inst of type @clock_type with a default
@@ -146,18 +159,19 @@
     try:
         clk = only(clks)
     except EmptyIterableException:
         _logger.warning(
             f"Found no clocks in {defn.name}; skipping auto-wiring "
             f"{clock_type}")
         return
-    except NonSignletonIterableException:
+    except NonSingletonIterableException as e:
         _logger.warning(
             f"Found multiple clocks in {defn.name}; skipping auto-wiring "
-            f"{clock_type}")
+            f"{clock_type} ({', '.join(map(repr, e.args[0]))})"
+        )
         return
     # Restore undrivens after popping off the first element.
     undrivens = itertools.chain([undriven], undrivens)
     for undriven in undrivens:
         _drive_value_with_clock(undriven, clk)
 
 
@@ -193,7 +207,10 @@
 
 class WireClockPass(DefinitionPass):
     def __call__(self, definition):
         with definition.open():
             for instance in definition.instances:
                 drive_undriven_clock_types_in_inst(definition, instance)
                 drive_undriven_other_clock_types_in_inst(definition, instance)
+
+
+wire_clocks = pass_lambda(WireClockPass)
```

### Comparing `magma-lang-2.2.9/magma/passes/debug_name.py` & `magma-lang-2.3.0/magma/passes/debug_name.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/passes/drive_undriven.py` & `magma-lang-2.3.0/magma/passes/drive_undriven.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from .passes import EditDefinitionPass
-from ..is_definition import isdefinition
 from magma.array import Array
 from magma.clock import is_clock_or_nested_clock
+from magma.is_definition import isdefinition
 from magma.passes.clock import (
-    drive_all_undriven_clocks_in_value, get_all_output_clocks_in_defn)
+    drive_all_undriven_clocks_in_value,
+    get_all_output_clocks_in_defn,
+)
+from magma.passes.passes import EditDefinitionPass, pass_lambda
 from magma.tuple import Tuple
 
 
 def _drive_undriven_children(port, clocks):
     # list comp so it doesn't short circuit
     undrivens = [_drive_if_undriven_input(p, clocks) for p in port]
     return any(undrivens)
@@ -43,7 +45,10 @@
         clocks = get_all_output_clocks_in_defn(circuit)
         if _drive_undriven(circuit.interface, clocks):
             circuit._is_definition = True
         if not isdefinition(circuit):
             return
         for inst in circuit.instances:
             _drive_undriven(inst.interface, clocks)
+
+
+drive_undriven = pass_lambda(DriveUndrivenPass)
```

### Comparing `magma-lang-2.2.9/magma/passes/passes.py` & `magma-lang-2.3.0/magma/passes/passes.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/passes/terminate_unused.py` & `magma-lang-2.3.0/magma/passes/terminate_unused.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .passes import EditDefinitionPass
-from ..is_definition import isdefinition
+from magma.is_definition import isdefinition
+from magma.passes.passes import EditDefinitionPass, pass_lambda
 
 
 def _terminate_if_unwired_output(port):
     if port.is_mixed():
         # list comp so it doesn't short circuit
         terminated = [_terminate_if_unwired_output(p) for p in port]
         return any(terminated)
@@ -24,7 +24,10 @@
     def edit(self, circuit):
         if _terminate_unused(circuit.interface):
             circuit._is_definition = True
         if not isdefinition(circuit):
             return
         for inst in circuit.instances:
             _terminate_unused(inst.interface)
+
+
+terminate_unused = pass_lambda(TerminateUnusedPass)
```

### Comparing `magma-lang-2.2.9/magma/passes/tsort.py` & `magma-lang-2.3.0/magma/passes/tsort.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/placer.py` & `magma-lang-2.3.0/magma/placer.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     def place(self, inst):
         raise NotImplementedError()
 
     @abstractmethod
     def instances(self):
         raise NotImplementedError()
 
+    @abstractmethod
+    def is_staged(self) -> bool:
+        raise NotImplementedError()
+
 
 def _setup_view(inst):
     inst_view = InstView(inst)
     # Setup view now because inline strings might use it during defn
     for sub_inst in getattr(type(inst), "instances", []):
         setattr(inst, sub_inst.name, InstView(sub_inst, inst_view))
 
@@ -131,14 +135,17 @@
         self._name(inst)
         self._instances.append(inst)
         inst.defn = self._defn
         if get_debug_mode():
             inst.stack = inspect.stack()
         _setup_view(inst)
 
+    def is_staged(self) -> bool:
+        return False
+
     def finalize(self, defn):
         if self._finalized:
             raise Exception("Can only call finalize on a placer once")
         self._finalized = True
         return self
 
 
@@ -157,14 +164,17 @@
         return self._name
 
     def place(self, inst):
         self._instances.append(inst)
         inst.defn = LazyCircuit
         _setup_view(inst)
 
+    def is_staged(self) -> bool:
+        return True
+
     def finalize(self, defn):
         if self._finalized:
             raise Exception("Can only call finalize on a staged placer once")
         placer = Placer(defn)
         for inst in self._instances:
             placer.place(inst)
         self._finalized = True
```

### Comparing `magma-lang-2.2.9/magma/primitives/lut.py` & `magma-lang-2.3.0/magma/primitives/lut.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/primitives/memory.py` & `magma-lang-2.3.0/magma/primitives/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,29 +101,20 @@
 
 class StagedMemoryPort(MagmaProtocol, metaclass=StagedMemoryPortMeta):
     def __init__(self, memory, addr):
         self.memory = memory
         self.addr = addr
 
     def __imatmul__(self, data):
-        if self.memory.WADDR.driven() or self.memory.WDATA.driven():
-            _logger.warning(
-                "Wiring __getitem__ result from a Memory instance with WADDR"
-                " or WDATA already driven, will overwrite previous values"
-            )
         self.memory.WADDR @= self.addr
         self.memory.WDATA @= data
+        self.memory.WE @= 1
         return self
 
     def _get_magma_value_(self):
-        if self.memory.RADDR.driven():
-            _logger.warning(
-                "Reading __getitem__ result from a Memory instance with RADDR"
-                " already driven, will overwrite previous value"
-            )
         self.memory.RADDR @= self.addr
         return self.memory.RDATA
 
 
 class Memory(Generator2):
     def __init__(self, height, T: Kind,
                  read_latency: int = 0, read_only: bool = False,
```

### Comparing `magma-lang-2.2.9/magma/primitives/mux.py` & `magma-lang-2.3.0/magma/primitives/mux.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from magma.array import Array
 from magma.bit import Bit
 from magma.bits import Bits, UInt, SInt
 from magma.bitutils import clog2, seq2int
 from magma.circuit import coreir_port_mapping
 from magma.common import is_int
+from magma.debug import magma_helper_function
 from magma.generator import Generator2
 from magma.interface import IO
 from magma.protocol_type import MagmaProtocol, magma_type
 from magma.t import Type, In, Out, Direction
 from magma.tuple import Product, Tuple
 from magma.type_utils import type_to_sanitized_string
 from magma.conversions import tuple_, as_bits, from_bits
@@ -42,39 +43,54 @@
 
 class Mux(Generator2):
     def __init__(self, height: int, T: Type):
         if issubclass(T, BitVector):
             T = Bits[len(T)]
         if issubclass(T, (bool, ht.Bit)):
             T = Bit
+
         # TODO(rsetaluri): Type should be hashable so the generator instance can
         # be cached.
         T_str = type_to_sanitized_string(T)
         self.name = f"Mux{height}x{T_str}"
-        N = magma_type(T).flat_length()
 
         ports = {f"I{i}": In(T) for i in range(height)}
         T_S = Bit if height == 2 else Bits[clog2(height)]
         ports["S"] = In(T_S)
         ports["O"] = Out(T)
 
-        self.io = io = IO(**ports)
+        self.io = IO(**ports)
 
-        mux = CoreIRCommonLibMuxN(height, N)()
-        data = [as_bits(getattr(io, f"I{i}")) for i in range(height)]
-        mux.I.data @= Array[height, Bits[N]](data)
-        if height == 2:
-            mux.I.sel[0] @= io.S
-        else:
-            mux.I.sel @= io.S
-        if issubclass(T, MagmaProtocol):
-            out = Out(T)._from_magma_value_(from_bits(T._to_magma_(), mux.O))
+        self.height = height
+        self.T = T
+
+        self.primitive = True
+        self.stateful = False
+
+        def _simulate(_, __, ___):
+            raise NotImplementedError()
+
+        self.simulate = _simulate
+
+    def elaborate(self):
+        N = magma_type(self.T).flat_length()
+        mux = CoreIRCommonLibMuxN(self.height, N)()
+        data = [as_bits(self.io[f"I{i}"]) for i in range(self.height)]
+        mux.I.data @= Array[self.height, Bits[N]](data)
+        sel = mux.I.sel
+        if self.height == 2:
+            sel = sel[0]
+        sel @= self.io.S
+        if issubclass(self.T, MagmaProtocol):
+            out = Out(self.T)._from_magma_value_(
+                from_bits(self.T._to_magma_(), mux.O)
+            )
         else:
-            out = from_bits(T, mux.O)
-        io.O @= out
+            out = from_bits(self.T, mux.O)
+        self.io.O @= out
 
 
 def _infer_mux_type(args):
     """
     Try to infer type by traversing arguments in order:
     * If we encounter a magma Type/Protocol, use that
     * BitVector/Bit/bool are converted to their magma equivalent Bits/Bit
@@ -123,14 +139,15 @@
         args = [tuple_(a) for a in args]
     return T, args
 
 
 infer_mux_type = _infer_mux_type
 
 
+@magma_helper_function
 def mux(I: Union[Sequence, Array], S, **kwargs):
     """
     How type inference works on I:
         This operator will traverse the list of inputs I and use the first
         magma value to determine the type.  This allows I to contain coerceable
         objects like ints (e.g. `mux([1, x], s)` where `x: UInt[2]`).  Coercion
         is peformed when wiring the arguments to the input of an instance of
@@ -161,34 +178,37 @@
 # Monkey patch for ite impl without circular dependency
 Bit._mux = staticmethod(mux)
 
 
 # NOTE(rsetaluri): We monkeypatch this function on to Array due to the circular
 # dependency between Mux and Array. See the discussion on
 # https://github.com/phanrahan/magma/pull/658.
+@magma_helper_function
 def _dynamic_mux_select(this, key):
     return mux(this.ts, key)
 
 
 Array.dynamic_mux_select = _dynamic_mux_select
 
 
+@magma_helper_function
 def dict_lookup(dict_, select, default=0):
     """
     Use `select` as an index into `dict` (similar to a case statement)
 
     `default` is used when `select` does not match any of the keys and has a
     default value of 0
     """
     output = default
     for key, value in dict_.items():
         output = mux([output, value], key == select)
     return output
 
 
+@magma_helper_function
 def list_lookup(list_, select, default=0):
     """
     Use `select` as an index into `list` (similar to a case statement)
 
     `default` is used when `select` does not match any of the indices (e.g.
     when the select width is longer than the list) and has a default value of
     0.
```

### Comparing `magma-lang-2.2.9/magma/primitives/register.py` & `magma-lang-2.3.0/magma/primitives/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import hwtypes as ht
 
 from magma.array import Array
 from magma.bit import Bit
 from magma.clock import Enable
 from magma.common import ParamDict
 from magma.bits import Bits, UInt, SInt
-from magma.circuit import coreir_port_mapping
+from magma.circuit import coreir_port_mapping, Circuit
 from magma.conversions import as_bits, from_bits, bit
+from magma.debug import magma_helper_function
 from magma.interface import IO
 from magma.generator import Generator2
 from magma.t import Type, Kind, In, Out, Direction
 from magma.tuple import Tuple
-from magma.clock import (AbstractReset,
-                         AsyncReset, AsyncResetN, Clock, get_reset_args)
+from magma.clock import (
+    AbstractReset, AsyncReset, AsyncResetN, Clock, get_reset_args
+)
 from magma.clock_io import ClockIO
 from magma.primitives.mux import Mux
 from magma.wire import wire
 
 
 class _CoreIRRegister(Generator2):
     """
@@ -127,15 +129,24 @@
         # Allow int for bit
         if len(init_T) > 1:
             return False
         return True
     return init_T.is_wireable(T)
 
 
-class Register(Generator2):
+class AbstractRegister(Generator2):
+    """Abstract base class for all Register circuits. User-defined register
+    types should implement this interface.
+    """
+
+    def get_enable(self, inst: Circuit) -> Enable:
+        raise NotImplementedError()
+
+
+class Register(AbstractRegister):
     def __init__(self, T: Kind = None,
                  init: Union[Type, int, ht.BitVector] = None,
                  reset_type: AbstractReset = None, has_enable: bool = False,
                  reset_priority: bool = True, name_map=ParamDict(I="I",
                                                                  O="O",
                                                                  CE="CE")):
         """
@@ -173,15 +184,15 @@
 
         (
             has_async_reset, has_async_resetn, has_reset, has_resetn
         ) = get_reset_args(reset_type)
 
         I_name = name_map.get("I", "I")
         O_name = name_map.get("O", "O")
-        CE_name = name_map.get("CE", "CE")
+        self.CE_name = CE_name = name_map.get("CE", "CE")
         self.io = IO(**{I_name: In(T), O_name: Out(T)})
         if has_enable:
             self.io += IO(**{CE_name: In(Enable)})
         self.io += ClockIO(has_async_reset=has_async_reset,
                            has_async_resetn=has_async_resetn,
                            has_reset=has_reset,
                            has_resetn=has_resetn)
@@ -221,15 +232,19 @@
                 I = Mux(2, T)(name="enable_mux")(O, I, enable)
         elif has_enable:
             I = Mux(2, T)(name="enable_mux")(O, I, enable)
         elif (has_reset or has_resetn):
             I = Mux(2, T)()(I, init, reset_select)
         reg.I @= as_bits(I)
 
+    def get_enable(self, inst):
+        return getattr(inst, self.CE_name, None)
+
 
+@magma_helper_function
 def register(value, **kwargs):
     T = type(value).qualify(Direction.Undirected)
     inst_kwargs = {}
     try:
         name = kwargs.pop("name")
         inst_kwargs["name"] = name
     except KeyError:
```

### Comparing `magma-lang-2.2.9/magma/primitives/set_index.py` & `magma-lang-2.3.0/magma/primitives/set_index.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/primitives/slice.py` & `magma-lang-2.3.0/magma/primitives/slice.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/primitives/wire.py` & `magma-lang-2.3.0/magma/primitives/wire.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 from magma.bits import Bits
 from magma.circuit import coreir_port_mapping
 from magma.clock import AsyncReset, AsyncResetN, Clock, _ClockType
 from magma.conversions import bit, convertbit
 from magma.digital import Digital
 from magma.generator import Generator2
 from magma.interface import IO
-from magma.t import In, Out
+from magma.t import Kind, In, Out
+from magma.type_utils import type_to_sanitized_string
 
 
-def _simulate_wire(self, value_store, state_store):
-    value_store.set_value(self.O, value_store.get_value(self.I))
+def _simulate_wire(this, value_store, state_store):
+    value_store.set_value(this.O, value_store.get_value(this.I))
 
 
 class Wire(Generator2):
-    def __init__(self, T):
+    def __init__(self, T: Kind, flatten: bool = True):
+        self.T = T
+        self.flattened = flatten
+        if not flatten:
+            self._init_unflattened(T)
+            return
         if issubclass(T, (AsyncReset, AsyncResetN, Clock)):
-            self._gen_named_type_wrapper(T)
-            # Standalone return to avoid return-in-init lint warning
+            self._init_named_type_wrapper(T)
             return
         if issubclass(T, Digital):
             coreir_lib = "corebit"
             coreir_genargs = None
         else:
             width = T.flat_length()
             T = Bits[width]
@@ -32,16 +37,21 @@
         self.simulate = _simulate_wire
         self.coreir_name = "wire"
         self.coreir_lib = coreir_lib
         self.coreir_genargs = coreir_genargs
         self.renamed_ports = coreir_port_mapping
         self.primitive = True
 
-    def _gen_named_type_wrapper(self, T):
-        """
-        Generates a container around Wire(Bit) so named types are wrapped
-        properly
+    def _init_unflattened(self, T: Kind):
+        self.name = f"Wire{type_to_sanitized_string(T)}"
+        self.io = IO(I=In(T), O=Out(T))
+        self.simulate = _simulate_wire
+        self.primitive = True
+
+    def _init_named_type_wrapper(self, T: Kind):
+        """Generates a container around Wire(Bit) so named types are wrapped
+        properly.
         """
         assert issubclass(T, Digital)
         self.io = IO(I=In(T), O=Out(T))
         self.name = f"Wire{T}"
         self.io.O @= convertbit(Wire(Bit)()(bit(self.io.I)), T)
```

### Comparing `magma-lang-2.2.9/magma/protocol_type.py` & `magma-lang-2.3.0/magma/protocol_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 
-from magma.debug import debug_wire
+from magma.debug import debug_wire, debug_unwire
 
 
 class MagmaProtocolMeta(type):
     @abc.abstractmethod
     def _to_magma_(cls):
         # To retrieve underlying magma type.
         raise NotImplementedError()
@@ -25,14 +25,17 @@
         return cls._qualify_magma_(direction)
 
     @abc.abstractmethod
     def _from_magma_value_(cls, val: 'Type'):
         # To create an instance from a value.
         raise NotImplementedError()
 
+    def _from_magma_ref_(cls, ref: 'Ref'):
+        return cls._from_magma_value_(cls._to_magma_()(name=ref))
+
     def _is_oriented_magma_(cls, direction):
         return cls._to_magma_().is_oriented(direction)
 
     def is_oriented(cls, direction):
         return cls._is_oriented_magma_(direction)
 
     def flip(cls):
@@ -47,21 +50,39 @@
     def is_bindable(cls, rhs):
         return cls._to_magma_().is_bindable(rhs)
 
     @property
     def direction(cls) -> int:
         return cls._to_magma_().direction
 
+    def flat_length(cls):
+        return cls._to_magma_().flat_length()
+
+    def unflatten(cls, ts):
+        return cls._from_magma_value_(cls._to_magma_().unflatten(ts))
+
+    @property
+    def undirected_t(cls):
+        return cls._to_magma_().undirected_t
+
 
 class MagmaProtocol(metaclass=MagmaProtocolMeta):
     @abc.abstractmethod
     def _get_magma_value_(self):
         # To access underlying magma value.
         raise NotImplementedError()
 
+    @property
+    def parent(self):
+        return self._get_magma_value_().parent
+
+    @parent.setter
+    def parent(self, value):
+        self._get_magma_value_().parent = value
+
     @classmethod
     def is_clock(cls):
         return cls._to_magma_().is_clock()
 
     @classmethod
     def is_inout(cls):
         return cls._to_magma_().is_inout()
@@ -80,16 +101,16 @@
 
     def iswhole(self):
         return self._get_magma_value_().iswhole()
 
     def value(self):
         return self._get_magma_value_().value()
 
-    def trace(self):
-        return self._get_magma_value_().trace()
+    def trace(self, skip_self=True):
+        return self._get_magma_value_().trace(skip_self)
 
     def driven(self):
         return self._get_magma_value_().driven()
 
     def flatten(self):
         return self._get_magma_value_().flatten()
 
@@ -102,26 +123,43 @@
 
     @debug_wire
     def wire(self, other, debug_info):
         if isinstance(other, MagmaProtocol):
             other = other._get_magma_value_()
         self._get_magma_value_().wire(other, debug_info)
 
-    def unwire(self, other):
+    @debug_unwire
+    def unwire(self, other, debug_info=None, keep_wired_when_contexts=False):
         if isinstance(other, MagmaProtocol):
             other = other._get_magma_value_()
-        self._get_magma_value_().unwire(other)
+        self._get_magma_value_().unwire(
+            other, debug_info, keep_wired_when_contexts
+        )
 
     def __imatmul__(self, other):
         self.wire(other)
         return self
 
     def connection_iter(self):
         return self._get_magma_value_().connection_iter()
 
+    def const(self):
+        return self._get_magma_value_().const()
+
+    def set_enclosing_when_context(self, ctx):
+        self._get_magma_value_().set_enclosing_when_context(ctx)
+
+    @property
+    def name(self):
+        return self._get_magma_value_().name
+
+    @name.setter
+    def name(self, value):
+        self._get_magma_value_().name = value
+
 
 def magma_type(T):
     if issubclass(T, MagmaProtocol):
         return T._to_magma_()
     return T
```

### Comparing `magma-lang-2.2.9/magma/ref.py` & `magma-lang-2.3.0/magma/ref.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,51 +16,80 @@
     def qualifiedname(self, sep="."):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def anon(self):
         raise NotImplementedError()
 
+    @abc.abstractmethod
+    def named(self) -> bool:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def bound(self) -> bool:
+        raise NotImplementedError()
+
     def parent(self):
         return self
 
     def root(self) -> typing.Optional['Ref']:
         parent = self.parent()
         if parent is self:
             return self
         return parent.root()
 
+    def root_iter(self, stop_if=None) -> typing.Optional['Ref']:
+        if stop_if is not None and stop_if(self):
+            return
+        yield self
+        parent = self.parent()
+        if parent is self:
+            return
+        yield from parent.root_iter(stop_if=stop_if)
+
 
 class AnonRef(Ref):
     def __init__(self):
         self.name = None
 
     def __str__(self):
         return f"AnonymousValue_{id(self)}"
 
     def qualifiedname(self, sep='.'):
         return f"AnonymousValue_{id(self)}"
 
     def anon(self):
         return True
 
+    def named(self) -> bool:
+        return False
+
+    def bound(self) -> bool:
+        return False
+
 
 class ConstRef(Ref):
     def __init__(self, name):
         self.name = name
 
     def __str__(self):
         return self.name
 
     def qualifiedname(self, sep="."):
         return self.name
 
     def anon(self):
         return False
 
+    def named(self) -> bool:
+        return False
+
+    def bound(self) -> bool:
+        return False
+
 
 class NamedRef(Ref):
     def __init__(self, name, value=None):
         if not isinstance(name, (str, int)):
             raise TypeError("Expected string or int")
         self.name = name
         self._value = value if value is None else weakref.ref(value)
@@ -73,17 +102,21 @@
 
     def anon(self):
         return False
 
     def value(self):
         return self._value if self._value is None else self._value()
 
+    def named(self) -> bool:
+        return True
+
 
 class TempNamedRef(NamedRef):
-    pass
+    def bound(self) -> bool:
+        return False
 
 
 class InstRef(NamedRef):
     def __init__(self, inst, name):
         super().__init__(name)
         if not inst:
             raise ValueError(f"Bad inst: {inst}")
@@ -98,25 +131,28 @@
             # index instead of name and we use the array indexing syntax to
             # represent them
             # See mantle's generic verilog target for example use case
             if sep == ".":
                 return f"{self.inst.name}[{self.name}]"
         return self.inst.name + sep + str(name)
 
+    def bound(self) -> bool:
+        return True
+
 
 class LazyInstRef(InstRef):
     def __init__(self, name):
         self.name = name
         self._inst = None
 
     @property
     def inst(self):
         if self._inst is not None:
             return self._inst
-        return LazyCircuit
+        return LazyCircuit()
 
     def qualifiedname(self, sep="."):
         return super().qualifiedname(sep)
 
     def set_inst(self, inst):
         if self._inst is not None:
             raise Exception("Can only set definition of LazyInstRef once")
@@ -131,17 +167,25 @@
         self.defn = defn
 
     def qualifiedname(self, sep="."):
         if sep == ".":
             return self.defn.__name__ + sep + self.name
         return self.name
 
+    def bound(self) -> bool:
+        return True
+
 
 class LazyCircuit:
     name = ""
+    debug_name = ""
+
+    @property
+    def defn(self):
+        return LazyCircuit
 
 
 class LazyDefnRef(DefnRef):
     def __init__(self, name):
         self.name = name
         self._defn = None
 
@@ -156,55 +200,66 @@
 
     def set_defn(self, defn):
         if self._defn is not None:
             raise Exception("Can only set definition of LazyDefnRef once")
         self._defn = defn
 
 
-class ArrayRef(Ref):
-    def __init__(self, array, index):
-        self.array = array
-        self.index = index
+class DerivedRef(Ref):
+    def __init__(self, parent, index):
+        self._parent = parent
+        self._index = index
 
     def __str__(self):
         return self.qualifiedname()
 
-    def qualifiedname(self, sep="."):
-        return f"{self.array.name.qualifiedname(sep=sep)}[{self.index}]"
+    def anon(self) -> bool:
+        return self.parent().anon()
 
-    def anon(self):
-        return self.array.name.anon()
+    def named(self) -> bool:
+        return self.parent().named()
+
+    def bound(self) -> bool:
+        return self.parent().bound()
 
     def parent(self):
-        return self.array.name
+        return self._parent.name
+
+    @property
+    def parent_value(self):
+        return self._parent
+
+    @property
+    def index(self):
+        return self._index
 
 
-class TupleRef(Ref):
+class ArrayRef(DerivedRef):
+    def __init__(self, array, index):
+        super().__init__(array, index)
+        self.array = array
+
+    def qualifiedname(self, sep="."):
+        return f"{self.parent().qualifiedname(sep=sep)}[{self.index}]"
+
+
+class TupleRef(DerivedRef):
     def __init__(self, tuple, index):
+        super().__init__(tuple, index)
         self.tuple = tuple
-        self.index = index
-
-    def __str__(self):
-        return self.qualifiedname()
 
     def qualifiedname(self, sep="."):
         try:
             int(self.index)
-            return (self.tuple.name.qualifiedname(sep=sep) +
+            return (self.parent().qualifiedname(sep=sep) +
                     "[" + str(self.index) + "]")
         except ValueError:
-            return (self.tuple.name.qualifiedname(sep=sep) +
+            return (self.parent().qualifiedname(sep=sep) +
                     sep + str(self.index))
 
-    def anon(self):
-        return self.tuple.name.anon()
-
-    def parent(self):
-        return self.tuple.name
-
 
 class PortViewRef(Ref):
     """
     Used for values that are connection references to a hierarchical value
     (using the view logic)
     """
```

### Comparing `magma-lang-2.2.9/magma/scope.py` & `magma-lang-2.3.0/magma/scope.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/simulator/coreir_simulator.py` & `magma-lang-2.3.0/magma/simulator/coreir_simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/simulator/mdb.py` & `magma-lang-2.3.0/magma/simulator/mdb.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/simulator/python_simulator.py` & `magma-lang-2.3.0/magma/simulator/python_simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/simulator/simulator.py` & `magma-lang-2.3.0/magma/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/smart/smart_bits.py` & `magma-lang-2.3.0/magma/smart/smart_bits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,600 +1,503 @@
 import abc
-import copy
+import dataclasses
 import inspect
 import operator
+from typing import Any, Callable, Optional, Union
 
-from magma.bits import Bits, BitsMeta, SInt, reduce
+from magma.bit import Bit
+from magma.bits import Bits, BitsMeta, SInt, reduce as bits_reduce
 from magma.conversions import uint, bits, sint
 from magma.conversions import concat as bits_concat
 from magma.debug import debug_wire
 from magma.protocol_type import MagmaProtocolMeta, MagmaProtocol
-from magma.t import Direction
-from magma.type_utils import TypeTransformer, issint
-from magma.value_utils import ValueVisitor, make_selector
+from magma.ref import AnonRef
 
 
-def _is_int(value):
-    try:
-        int(value)
-    except (ValueError, TypeError):
-        return False
-    return True
-
-
-class Context:
-    def __init__(self, assignee, root):
-        self.assignee = assignee
-        self.root = root
-
-    def max_width(self):
-
-        def _visit(node):
-            if hasattr(node, "_width_"):
-                return node._width_
-            if isinstance(node, _SmartBitsExpr):
-                return len(node.bits)
-            return max(_visit(arg) for arg in node.args)
-
-        max_width = _visit(self.root)
-        if self.assignee is not None:
-            max_width = max(max_width, len(self.assignee.bits))
-        return max_width
+class SmartExprMeta(MagmaProtocolMeta):
+    pass
 
-    def __str__(self):
-        return f"Context(lhs={repr(self.assignee)}, rhs={repr(self.root)})"
 
+class SmartExpr(MagmaProtocol, metaclass=SmartExprMeta):
+    __hash__ = object.__hash__
 
-class _SmartExprMeta(MagmaProtocolMeta):
-    pass
-
+    def __init__(self):
+        self._name = AnonRef()
+        self._value = None
 
-class _SmartExpr(MagmaProtocol, metaclass=_SmartExprMeta):
-    @abc.abstractmethod
-    def resolve(self, context):
-        raise NotImplementedError()
+    @property
+    def name(self):
+        if self._value is None:
+            return self._name
+        return self._value.name
+
+    @name.setter
+    def name(self, value):
+        if self._value is None:
+            self._name = value
+        else:
+            self._value.name = value
 
+    @property
     @abc.abstractmethod
-    def eval(self):
+    def args(self):
         raise NotImplementedError()
 
     # Binary arithmetic operators.
-    def __add__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __add__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.add, self, other)
+        return SmartBinaryOp(operator.add, self, other)
 
-    def __sub__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __sub__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.sub, self, other)
+        return SmartBinaryOp(operator.sub, self, other)
 
-    def __mul__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __mul__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.mul, self, other)
+        return SmartBinaryOp(operator.mul, self, other)
 
-    def __floordiv__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __floordiv__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.floordiv, self, other)
+        return SmartBinaryOp(operator.floordiv, self, other)
 
-    def __truediv__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __truediv__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.truediv, self, other)
+        return SmartBinaryOp(operator.truediv, self, other)
 
-    def __mod__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __mod__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.mod, self, other)
+        return SmartBinaryOp(operator.mod, self, other)
 
     # Binary logic operators.
-    def __and__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __and__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.and_, self, other)
+        return SmartBinaryOp(operator.and_, self, other)
 
-    def __or__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __or__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.or_, self, other)
+        return SmartBinaryOp(operator.or_, self, other)
 
-    def __xor__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __xor__(self, other: 'SmartExpr') -> 'SmartBinaryOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartBinaryOpExpr(operator.xor_, self, other)
+        return SmartBinaryOp(operator.xor, self, other)
 
     # Comparison operators.
-    def __eq__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __eq__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.eq, self, other)
+        return SmartComparisonOp(operator.eq, self, other)
 
-    def __ne__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __ne__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.ne, self, other)
+        return SmartComparisonOp(operator.ne, self, other)
 
-    def __ge__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __ge__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.ge, self, other)
+        return SmartComparisonOp(operator.ge, self, other)
 
-    def __gt__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __gt__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.gt, self, other)
+        return SmartComparisonOp(operator.gt, self, other)
 
-    def __le__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __le__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.le, self, other)
+        return SmartComparisonOp(operator.le, self, other)
 
-    def __lt__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __lt__(self, other: 'SmartExpr') -> 'SmartComparisonOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartComparisonOpExpr(operator.lt, self, other)
+        return SmartComparisonOp(operator.lt, self, other)
 
     # Shift operators.
-    def __lshift__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __lshift__(self, other: 'SmartExpr') -> 'SmartShiftOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartShiftOpExpr(operator.lshift, self, other)
+        return SmartShiftOp(operator.lshift, self, other)
 
-    def __rshift__(self, other: '_SmartExpr'):
-        if not isinstance(other, _SmartExpr):
+    def __rshift__(self, other: 'SmartExpr') -> 'SmartShiftOp':
+        if not isinstance(other, SmartExpr):
             return NotImplemented
-        return _SmartShiftOpExpr(operator.rshift, self, other)
+        return SmartShiftOp(operator.rshift, self, other)
 
     # Unary operators.
-    def __invert__(self):
-        return _SmartUnaryOpExpr(operator.invert, self)
+    def __invert__(self) -> 'SmartUnaryOp':
+        return SmartUnaryOp(operator.invert, self)
 
-    def __neg__(self):
-        return _SmartUnaryOpExpr(operator.neg, self)
+    def __neg__(self) -> 'SmartUnaryOp':
+        return SmartUnaryOp(operator.neg, self)
 
     # Reduction operators.
-    def reduce(self, op):
-        return _SmartReductionOpExpr(op, self)
+    def reduce(self, op) -> 'SmartReductionOp':
+        return SmartReductionOp(op, self)
+
+    def reduce_and(self) -> 'SmartReductionOp':
+        return self.reduce(operator.and_)
+
+    def reduce_or(self) -> 'SmartReductionOp':
+        return self.reduce(operator.or_)
+
+    def reduce_xor(self) -> 'SmartReductionOp':
+        return self.reduce(operator.xor)
 
     # Extension operators.
-    def zext(self, width):
-        return _SmartExtendOpExpr(width, False, self, resolved=False)
+    def zext(self, width) -> 'SmartExtendOp':
+        return SmartExtendOp(width, False, self)
+
+    def sext(self, width) -> 'SmartExtendOp':
+        return SmartExtendOp(width, True, self)
 
-    def sext(self, width):
-        return _SmartExtendOpExpr(width, True, self, resolved=False)
+    def const(self) -> bool:
+        return False
 
 
-class _SmartOpExpr(_SmartExpr, metaclass=_SmartExprMeta):
+class SmartOp(SmartExpr, metaclass=SmartExprMeta):
     def __init__(self, op, *args):
+        super().__init__()
         self._op = op
         self._args = args
 
     @property
-    def args(self):
-        return self._args
-
-    @property
     def op(self):
         return self._op
 
-    def _update(self, *args):
-        self._args = args
-
-    def _resolve_args(self, context):
-        for arg in self._args:
-            arg.resolve(context)
-
-    def _eval_args(self):
-        return [arg.eval() for arg in self._args]
+    @property
+    def args(self):
+        return self._args
 
     def __str__(self):
-        if inspect.isbuiltin(self._op):
-            op_str = self._op.__name__
-        else:
-            op_str = str(self._op)
-        args = ", ".join(str(arg) for arg in self._args)
-        return f"{op_str}({args})"
-
-
-class _SmartExtendOpExpr(_SmartOpExpr):
-
-    class _ExtendOp:
-        def __init__(self, width, signed):
-            self._width = width
-            self._signed = signed
-
-        def __call__(self, operand):
-            if self._signed:
-                return sint(operand).sext(self._width)
-            return uint(operand).zext(self._width)
+        op = self.op.__name__ if inspect.isbuiltin(self.op) else str(self.op)
+        args = ", ".join(str(arg) for arg in self.args)
+        return f"{op}({args})"
+
+
+class SmartExtendOp(SmartOp):
+
+    @dataclasses.dataclass(frozen=True)
+    class Op:
+        width: int
+        signed: bool
+
+        def __call__(self, operand: Bits) -> Bits:
+            if self.signed:
+                return sint(operand).sext(self.width)
+            return uint(operand).zext(self.width)
 
         def __str__(self):
-            return f"Extend[width={self._width}, signed={self._signed}]"
+            func = "Sext" if self.signed else "Zext"
+            return f"{func}[{self.width}]"
 
-    def __init__(self, width, signed, operand, resolved=True):
-        extend = _SmartExtendOpExpr._ExtendOp(width, signed)
-        super().__init__(extend, operand)
-        self._resolved = resolved
+    def __init__(self, width, signed, operand):
+        super().__init__(SmartExtendOp.Op(width, signed), operand)
 
-    def resolve(self, context):
-        if self._resolved:
-            return
-        context = Context(None, self)
-        self._resolve_args(context)
-        self._width_ = self._args[0]._width_ + self.op._width
-        self._signed_ = self.op._signed
-
-    def eval(self):
-        args = self._eval_args()
-        return self.op(*args)
-
-
-def _extend_if_needed(expr, to_width, signed):
-    diff = expr._width_ - to_width
-    assert diff <= 0
-    if diff == 0:
-        return expr
-    expr = _SmartExtendOpExpr(-diff, signed, expr)
-    expr._width_ = to_width
-    expr._signed_ = signed
-    return expr
-
-
-class _SmartReductionOpExpr(_SmartOpExpr):
-
-    class _ReductionOp:
-        _OP_TO_NAME = {
-            operator.and_: "And",
-            operator.or_: "Or",
-            operator.xor: "Xor",
-        }
-
-        def __init__(self, op):
-            cls = _SmartReductionOpExpr._ReductionOp
-            if op not in cls._OP_TO_NAME:
+
+class SmartReductionOp(SmartOp):
+    OP_TO_NAME = {
+        operator.and_: "And",
+        operator.or_: "Or",
+        operator.xor: "Xor",
+    }
+
+    @dataclasses.dataclass(frozen=True)
+    class Op:
+        op: Callable
+
+        def __post_init__(self):
+            if self.op not in SmartReductionOp.OP_TO_NAME:
                 raise ValueError(f"Reduction operator {op} not supported")
-            self._op = op
 
-        def __call__(self, operand):
-            return reduce(self._op, operand)
+        def __call__(self, operand: Bits) -> Bits:
+            return bits(bits_reduce(self.op, operand))
 
         def __str__(self):
-            cls = _SmartReductionOpExpr._ReductionOp
-            op_name = cls._OP_TO_NAME[self._op]
-            return f"{op_name}Reduce"
+            func = SmartReductionOp.OP_TO_NAME[self.op]
+            return f"{func}Reduce"
 
     def __init__(self, op, operand):
-        reduction = _SmartReductionOpExpr._ReductionOp(op)
-        super().__init__(reduction, operand)
-
-    def resolve(self, context):
-        context = Context(None, self)
-        self._resolve_args(context)
-        self._width_ = 1
-        self._signed_ = all(arg._signed_ for arg in self._args)
-
-    def eval(self):
-        args = self._eval_args()
-        fn = sint if self._signed_ else uint
-        return fn(self.op(*args))
+        super().__init__(SmartReductionOp.Op(op), operand)
 
 
-class _SmartNAryContextualOpExr(_SmartOpExpr):
-    def __init__(self, op, *args):
-        super().__init__(op, *args)
-
-    def resolve(self, context):
-        self._resolve_args(context)
-        self._signed_ = all(arg._signed_ for arg in self._args)
-        to_width = context.max_width()
-        args = (_extend_if_needed(arg, to_width, self._signed_)
-                for arg in self._args)
-        self._update(*args)
-        self._width_ = to_width
-
-    def eval(self):
-        args = self._eval_args()
-        if self._signed_:
-            args = (sint(arg) for arg in args)
-        else:
-            args = (uint(arg) for arg in args)
-        return self.op(*args)
+class SmartNAryContextualOp(SmartOp):
+    pass
 
 
-class _SmartBinaryOpExpr(_SmartNAryContextualOpExr):
+class SmartBinaryOp(SmartNAryContextualOp):
     def __init__(self, op, loperand, roperand):
         super().__init__(op, loperand, roperand)
 
 
-class _SmartUnaryOpExpr(_SmartNAryContextualOpExr):
+class SmartUnaryOp(SmartNAryContextualOp):
     def __init__(self, op, operand):
         super().__init__(op, operand)
 
 
-class _SmartComparisonOpExpr(_SmartOpExpr):
-    def __init__(self, op, loperand, roperand):
-        super().__init__(op, loperand, roperand)
+class SmartComparisonOp(SmartOp):
+
+    @dataclasses.dataclass(frozen=True)
+    class Op:
+        op: Callable
 
-    def resolve(self, context):
-        context = Context(None, self)
-        self._resolve_args(context)
-        signed_args = all(arg._signed_ for arg in self._args)
-        to_width = max(arg._width_ for arg in self._args)
-        args = (_extend_if_needed(arg, to_width, signed_args)
-                for arg in self._args)
-        self._update(*args)
-        self._width_ = 1
-        self._signed_ = False
-
-    def eval(self):
-        args = self._eval_args()
-        signed_args = all(arg._signed_ for arg in self._args)
-        fn = sint if signed_args else uint
-        args = (fn(arg) for arg in args)
-        return uint(self.op(*args))
+        def __call__(self, *args) -> Bits:
+            return bits(self.op(*args))
 
+        def __str__(self) -> str:
+            return self.op.__name__
 
-class _SmartShiftOpExpr(_SmartOpExpr):
     def __init__(self, op, loperand, roperand):
-        super().__init__(op, loperand, roperand)
+        super().__init__(SmartComparisonOp.Op(op), loperand, roperand)
 
-    def resolve(self, context):
-        loperand, roperand = self._args
-        loperand.resolve(context)
-        self_context = Context(None, self)
-        roperand.resolve(self_context)
-        to_width = max(arg._width_ for arg in self._args)
-        self._signed_ = all(arg._signed_ for arg in self._args)
-        args = (_extend_if_needed(arg, to_width, self._signed_)
-                for arg in self._args)
-        self._update(*args)
-        self._width_ = to_width
-
-    def eval(self):
-        args = self._eval_args()
-        if self._signed_:
-            args = (sint(arg) for arg in args)
-        else:
-            args = (uint(arg) for arg in args)
-        return self.op(*args)
+
+class SmartShiftOp(SmartOp):
+    def __init__(self, op, loperand, roperand):
+        super().__init__(op, loperand, roperand)
 
 
-class _SmartConcatOpExpr(_SmartOpExpr):
+class SmartConcatOp(SmartOp):
 
-    class _ConcatOp:
-        def __call__(self, *args):
+    class Op:
+        def __call__(self, *args) -> Bits:
             return bits_concat(*args)
 
-        def __str__(self):
+        def __str__(self) -> str:
             return "Concat"
 
     def __init__(self, *args):
-        concat = _SmartConcatOpExpr._ConcatOp()
-        super().__init__(concat, *args)
+        super().__init__(SmartConcatOp.Op(), *args)
+
+
+class SmartMuxOp(SmartOp):
+
+    class Op:
+        def __call__(self, *args) -> Bits:
+            import magma as m
+            values, select = args[:-1], args[-1]
+            return m.mux(values, select)
+
+        def __str__(self) -> str:
+            return "Mux"
 
-    def resolve(self, context):
-        for arg in self._args:
-            context = Context(None, arg)
-            arg.resolve(context)
-        self._width_ = sum(arg._width_ for arg in self._args)
-        self._signed_ = False
-
-    def eval(self):
-        args = self._eval_args()
-        args = [uint(arg) for arg in args]
-        return uint(self.op(*args))
+    def __init__(self, *args):
+        super().__init__(SmartMuxOp.Op(), *args)
 
 
-def concat(*args):
-    if not all(isinstance(arg, _SmartExpr) for arg in args):
+def concat(*args) -> SmartExpr:
+    if not all(isinstance(arg, SmartExpr) for arg in args):
         types = ", ".join(str(type(arg)) for arg in args)
-        raise NotImplementedError(f"Concat not supported for {types}")
-    return _SmartConcatOpExpr(*args)
+        raise NotImplementedError(f"Concat not supported for [{types}]")
+    return SmartConcatOp(*args)
+
+
+def repeat(value, num) -> SmartExpr:
+    """Repeats @value @num number of times flat. Note that for single bit values
+    (e.g. x[0]) this is the same as m.repeat, but for bits this function retruns
+    a flattened type, whereas m.repeat constructs a higher-dimensional
+    array. This function is equivalent to m.smart.concat(*(value for _ in
+    range(num))).
+    """
+    return concat(*(value for _ in range(num)))
+
+
+def mux(values, select) -> SmartExpr:
+    if not all(isinstance(value, SmartExpr) for value in values):
+        types = ", ".join(str(type(value)) for value in values)
+        raise NotImplementedError(f"Mux not supported for [{types}]")
+    return SmartMuxOp(*values, select)
 
 
-class _SmartSignedOpExpr(_SmartOpExpr):
+class SmartSignedOp(SmartOp):
 
-    class _SignedOp:
-        def __init__(self, signed):
-            self._signed = signed
+    @dataclasses.dataclass
+    class Op:
+        signed: bool
 
-        @property
-        def signed(self):
-            return self._signed
+        def __call__(self, operand: Bits) -> Bits:
+            cons = sint if self.signed else uint
+            return cons(operand)
 
         def __str__(self):
-            return "Signed" if self._signed else "Unsigned"
+            return "Signed" if self.signed else "Unsigned"
 
     def __init__(self, signed, operand):
-        signed = _SmartSignedOpExpr._SignedOp(signed)
-        super().__init__(signed, operand)
-
-    def resolve(self, context):
-        self._resolve_args(context)
-        self._width_ = self._args[0]._width_
-        self._signed_ = self._op.signed
-
-    def eval(self):
-        args = self._eval_args()
-        fn = sint if self._signed_ else uint
-        return fn(args[0])
+        super().__init__(SmartSignedOp.Op(signed), operand)
 
 
 def signed(expr):
-    return _SmartSignedOpExpr(True, expr)
+    return SmartSignedOp(True, expr)
 
 
 def unsigned(expr):
-    return _SmartSignedOpExpr(False, expr)
+    return SmartSignedOp(False, expr)
 
 
-class _SmartBitsExpr(_SmartExpr, metaclass=_SmartExprMeta):
-    def __init__(self, bits):
-        self._bits = bits
+@dataclasses.dataclass(frozen=True)
+class SmartBitsExpr(SmartExpr, metaclass=SmartExprMeta):
+    bits: 'SmartBits'
 
     @property
-    def bits(self):
-        return self._bits
+    def args(self):
+        return []
 
     def __str__(self):
-        return str(self._bits)
-
-    def resolve(self, context):
-        self._width_ = len(self._bits)
-        self._signed_ = type(self._bits)._signed
+        return str(self.bits)
 
-    def eval(self):
-        return self._bits.typed_value()
 
-
-class _SmartBitsMeta(_SmartExprMeta):
-    def __getitem__(cls, key):
-        if issubclass(cls, SmartBits) and (hasattr(cls, "_T") or
-                                           hasattr(cls, "_signed")):
-            raise TypeError("Can not doubly qualify SmartBits, i.e. "
-                            "SmartBits[n][m] not allowed")
+class SmartBitsMeta(SmartExprMeta):
+    def _parse_key(cls, key):
+        qualified = (
+            issubclass(cls, SmartBits) and
+            (
+                hasattr(cls, "_T_") or
+                hasattr(cls, "_signed_")
+            )
+        )
+        if qualified:
+            raise TypeError("Can not doubly qualify SmartBits")
+        width_or_type = key
         signed = False
         if isinstance(key, tuple):
             if len(key) == 1:
-                pass
+                width_or_type = key[0]
             elif len(key) == 2:
-                key, signed = key
+                width_or_type, signed = key
             else:
                 raise ValueError(f"{key} unsupported")
-        if _is_int(key):
-            T = Bits[key]
+        try:
+            int(width_or_type)
+        except (ValueError, TypeError):
+            assert isinstance(width_or_type, BitsMeta)
+            T = width_or_type
         else:
-            assert isinstance(key, BitsMeta)
-            T = key
+            T = Bits[width_or_type]
+        return T, signed
+
+    def __eq__(cls, other):
+        return (
+            isinstance(other, SmartExprMeta) and
+            cls._to_magma_() == other._to_magma_()
+        )
+
+    __hash__ = type.__hash__
+
+    def __getitem__(cls, key):
+        T, signed = SmartBitsMeta._parse_key(cls, key)
         name = f"SmartBits[{len(T)}, {signed}]"
-        dct = {"_T": T, "_signed": signed}
+        dct = {"_T_": T, "_signed_": signed}
         return type(cls)(name, (cls,), dct)
 
     def _to_magma_(cls):
-        return cls._T
+        return cls._T_
 
     def _qualify_magma_(cls, d):
-        return SmartBits[cls._T.qualify(d), cls._signed]
+        return SmartBits[cls._T_.qualify(d), cls._signed_]
 
     def _flip_magma_(cls):
-        return SmartBits[cls._T.flip(), cls._signed]
+        return SmartBits[cls._T_.flip(), cls._signed_]
 
     def _from_magma_value_(cls, value):
         return cls(value)
 
     def __repr__(cls):
-        has_T = hasattr(cls, "_T")
-        has_signed = hasattr(cls, "_signed")
+        has_T = hasattr(cls, "_T_")
+        has_signed = hasattr(cls, "_signed_")
         if not (has_T or has_signed):
             return "SmartBits"
         assert has_T and has_signed
-        return f"SmartBits[{len(cls._T)}, {cls._signed}]"
+        return f"SmartBits[{len(cls._T_)}, {cls._signed_}]"
+
 
+def _make_initializer(
+        value: Optional[Any],
+        T: SmartBitsMeta,
+        name: Optional[str]
+) -> Bits:
+    if value is None:
+        return T._to_magma_()(name=name)
+    size = len(T._T_)
+    if isinstance(value, Bits[size]):
+        return value
+    return Bits[size](value)
 
-class SmartBits(_SmartBitsExpr, metaclass=_SmartBitsMeta):
-    def __init__(self, value=None):
+
+class SmartBits(SmartBitsExpr, metaclass=SmartBitsMeta):
+    def __init__(self, value=None, name=None):
         super().__init__(self)
-        if value is None:
-            value = type(self)._to_magma_()()
-        self._value = bits(value)
+        self._value = _make_initializer(value, type(self), name)
+
+    def __len__(self):
+        return len(type(self)._T_)
 
     def typed_value(self):
-        if type(self)._signed:
+        if type(self)._signed_:
             return sint(self._value)
         return uint(self._value)
 
     def untyped_value(self):
         return self._value
 
     def __hash__(self):
         return hash(self._value)
 
     def _get_magma_value_(self):
         return self.untyped_value()
 
-    def __deepcopy__(self, memo):
-        return type(self)(self._value)
+    # Slice operators.
+    def __getitem__(self, key_or_slice) -> 'SmartBits':
+        return SmartBits.from_bits(self._value[key_or_slice])
 
     @debug_wire
     def wire(self, other, debug_info):
         if isinstance(other, Bits):
-            super().wire(other, debug_info)
+            MagmaProtocol.wire(self, other, debug_info)
             return
-        if not isinstance(other, _SmartExpr):
+        if not isinstance(other, SmartExpr):
             raise ValueError(f"Can not wire {type(self)} to {type(other)}")
-        evaluated, resolved = _eval(self, other)
-        evaluated = evaluated.force_width(len(self))
-        MagmaProtocol.wire(self, evaluated)
-        self._smart_expr_ = resolved  # attach debug info
-
-    def __len__(self):
-        return len(type(self)._T)
-
-    def force_width(self, width):
-        diff = len(self) - width
-        if diff == 0:
-            return copy.deepcopy(self)
-        value = self.typed_value()
-        value = value.ext(-diff) if diff < 0 else value[:-diff]
-        return SmartBits.from_bits(value)
+        # NOTE(rsetaluri): We delay the import of the evaluation method to avoid
+        # a circular import, since the evaluation depends on the implementation
+        # of SmartBits.
+        from magma.smart.eval import evaluate_assignment
+        other = evaluate_assignment(self, other)
+        MagmaProtocol.wire(self, other, debug_info)
 
     @staticmethod
     def from_bits(value):
-        assert isinstance(value, Bits), type(value)
+        if isinstance(value, Bit):
+            value = bits(value)
+        if not isinstance(value, Bits):
+            raise TypeError(value)
         signed = isinstance(value, SInt)
         return SmartBits[len(value), signed](value)
 
     def __str__(self):
-        signed = type(self)._signed
+        signed = type(self)._signed_
         return f"SmartBits[{len(self)}, {signed}]({str(self._value)})"
 
     def connection_iter(self):
         yield from zip(self, self.trace())
 
 
 SmartBit = SmartBits[1]
 
 
-def _eval(lhs: SmartBits, rhs: _SmartExpr) -> (SmartBits, _SmartExpr):
-    rhs = copy.deepcopy(rhs)
-    rhs.resolve(Context(lhs, rhs))
-    res = rhs.eval()
-    return SmartBits.from_bits(res), rhs
+def issigned(value_or_type: Union[SmartBits, SmartBitsMeta]) -> bool:
+    if isinstance(value_or_type, SmartBits):
+        return type(value_or_type)._signed_
+    if isinstance(value_or_type, SmartBitsMeta):
+        return value_or_type._signed_
+    raise TypeError(value_or_type)
 
 
-def eval(expr: _SmartExpr, width: int, signed: bool = False):
+def eval(expr: SmartExpr, width: int, signed: bool = False):
     lhs = SmartBits[width, signed]()
     lhs @= expr
     return lhs
-
-
-class _SmartifyTypeTransformer(TypeTransformer):
-    def visit_Bits(self, T):
-        signed = issint(T)
-        return SmartBits[len(T), signed]
-
-
-class _LeafCollector(ValueVisitor):
-    def __init__(self):
-        self.leaves = []
-
-    def visit_Digital(self, value):
-        self.leaves.append(value)
-
-    def visit_Bits(self, value):
-        self.leaves.append(value)
-
-
-def make_smart(value):
-    T = type(value)
-    Tsmart = _SmartifyTypeTransformer().visit(T)
-    Tsmart = Tsmart.qualify(Direction.Undirected)
-    smart_value = Tsmart()
-    leaf_collector = _LeafCollector()
-    leaf_collector.visit(value)
-    for leaf in leaf_collector.leaves:
-        selector = make_selector(leaf)
-        smart_leaf = selector.select(smart_value)
-        smart_leaf @= leaf
-    return smart_value
```

### Comparing `magma-lang-2.2.9/magma/ssa/ssa.py` & `magma-lang-2.3.0/magma/ssa/ssa.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/symbol_table.py` & `magma-lang-2.3.0/magma/symbol_table.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/symbol_table_utils.py` & `magma-lang-2.3.0/magma/symbol_table_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/combinational.py` & `magma-lang-2.3.0/magma/syntax/combinational.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/combinational2.py` & `magma-lang-2.3.0/magma/syntax/combinational2.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/coroutine.py` & `magma-lang-2.3.0/magma/syntax/coroutine.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/inline_combinational.py` & `magma-lang-2.3.0/magma/syntax/inline_combinational.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/sequential2.py` & `magma-lang-2.3.0/magma/syntax/sequential2.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,49 +218,14 @@
         return len(self._get_magma_value_())
 
     @property
     def debug_name(self):
         return self._get_magma_value_().debug_name
 
 
-def sequential_getattribute(self, key):
-    """
-    Wrap lists so we can use the setattr interface with lists of registers
-    """
-    result = object.__getattribute__(self, key)
-    if isinstance(result, list):
-        return _SequentialListWrapper(result)
-    if isinstance(type(result), Register):
-        return _SequentialRegisterWrapper[type(result())](result)
-    return result
-
-
-def sequential_setattr(self, key, value):
-    # TODO: for now we assume this is a register, ideally we'd type check this,
-    # but we need to have a notion of a register primitive (e.g. right now the
-    # mantle reg wraps the coreir reg primitive, so technically the register is
-    # an arbitrary user-defined circuit)
-
-    target = object.__getattribute__(self, key)
-    # We can at least match the value is a circuit with outputs that match the
-    # input of the attribute circuit
-    if not isinstance(target, Circuit):
-        raise TypeError("Excepted setattr key to be a Circuit")
-
-    if isinstance(value, MagmaProtocol):
-        value = value._get_magma_value_()
-    if not isinstance(value, (Circuit, int, Type)):
-        raise TypeError("Excepted setattr value to be a Circuit, Type, or int",
-                        f"not {type(value)}")
-
-    # Simply use function call syntax for now (should automatically retrieve
-    # the output of value)
-    target(value)
-
-
 def _process_phi_arg(arg):
     if isinstance(arg, Circuit):
         # Call with no args to retrieve output(s)
         arg = arg()
         if isinstance(arg, list):
             # TODO: We could support tuples/products
             raise TypeError("Cannot use circuit with multiple outputs as "
@@ -444,14 +409,50 @@
             _annotations = annotations
 
         if "self" in _annotations:
             raise Exception("Assumed self did not have annotation")
 
         io_args = build_io_args(_annotations, output_port_names)
 
+        cls_setattr = cls.__setattr__
+        cls_getattribute = cls.__getattribute__
+
+        def sequential_getattribute(self, key):
+            """
+            Wrap lists so we can use the setattr interface with lists of
+            registers
+            """
+            result = cls_getattribute(self, key)
+            if isinstance(result, list):
+                return _SequentialListWrapper(result)
+            if isinstance(type(result), Register):
+                return _SequentialRegisterWrapper[type(result())](result)
+            return result
+
+        def sequential_setattr(self, key, value):
+            # TODO: for now we assume this is a register, ideally we'd type
+            # check this,but we need to have a notion of a register primitive
+            # (e.g. right now the mantle reg wraps the coreir reg primitive,
+            # so technically the register is an arbitrary user-defined circuit)
+            target = cls_getattribute(self, key)
+            if isinstance(target, Circuit):
+                if isinstance(value, MagmaProtocol):
+                    value = value._get_magma_value_()
+
+                if not isinstance(value, (Circuit, int, Type)):
+                    raise TypeError("Excepted setattr value to be a Circuit, "
+                                    f"Type, or int not {type(value)}")
+
+                # Simply use function call syntax for now (should
+                # automatically retrieve the output of value)
+                target(value)
+            else:
+                # fall back to the cls's original setattr
+                cls_setattr(self, key, value)
+
         class SequentialCircuit(Circuit):
             name = cls.__name__
             io = IO(**io_args) + clock_io
             call_args = [cls()]
 
             # Monkey patch setattribute for register assign syntax, we could
             # also add this in a Sequential base class, but if we do that we
```

### Comparing `magma-lang-2.2.9/magma/syntax/transforms/inline_yield_from.py` & `magma-lang-2.3.0/magma/syntax/transforms/inline_yield_from.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/transforms/replace_symbols.py` & `magma-lang-2.3.0/magma/syntax/transforms/replace_symbols.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/util.py` & `magma-lang-2.3.0/magma/syntax/util.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/verilog.py` & `magma-lang-2.3.0/magma/syntax/verilog.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/syntax/verilog_utils.py` & `magma-lang-2.3.0/magma/syntax/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/t.py` & `magma-lang-2.3.0/magma/t.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import abc
 import enum
 from functools import lru_cache
 from magma.common import deprecated
 from magma.compatibility import IntegerTypes, StringTypes
-from magma.ref import AnonRef, NamedRef, TempNamedRef, DefnRef, InstRef
+from magma.debug import get_debug_info
+from magma.ref import (
+    AnonRef, NamedRef, TempNamedRef, DefnRef, InstRef, PortViewRef
+)
 from magma.protocol_type import magma_value
 from magma.wire import wire
 
 
 class Direction(enum.Enum):
     In = 0
     Out = 1
@@ -94,29 +97,31 @@
         defn_str = ""
         inst_str = ""
         if isinstance(self.name, DefnRef):
             defn_str = str(self.name.defn.name) + "."
         elif isinstance(self.name, InstRef):
             inst_str = str(self.name.inst.name) + "."
             defn_str = str(self.name.inst.defn.name) + "."
+        elif isinstance(self.name, PortViewRef):
+            return ".".join(self.name.view.path())
         return f"{defn_str}{inst_str}{str(self)}"
 
     def __le__(self, other):
         if self.is_output():
             raise TypeError(f"Cannot use <= to assign to output: "
                             f"{self.debug_name} (trying to assign "
                             f"{other.debug_name})")
         wire(other, self)
 
     def __imatmul__(self, other):
         other = magma_value(other)
         if self.is_output():
             raise TypeError(f"Cannot use @= to assign to output: {self} "
                             f"(trying to assign {other})")
-        wire(other, self)
+        wire(other, self, get_debug_info(3))
         return self
 
     @abc.abstractmethod
     def unused(self):
         # Mark value is unused by calling unused on the underlying magma
         # elements. For example, m.Bit is wired up to a coreir term primitive A
         # general m.Array and m.Tuple will recursively call `unused` on its
```

### Comparing `magma-lang-2.2.9/magma/testing/utils.py` & `magma-lang-2.3.0/magma/testing/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Infrastructure for writing magma tests
 """
 import difflib
 import filecmp
 import os
+import pytest
+import re
+import shutil
 import sys
+
 from typing import Optional
 
-from magma.config import get_debug_mode, set_debug_mode
+from magma.config import get_debug_mode, set_debug_mode, config
 from magma.conversions import bits
 from magma.protocol_type import MagmaProtocolMeta, MagmaProtocol
 from magma.t import Type, Direction
 
 
 def check_files_equal(callee_file, file1_name, file2_name):
     """
@@ -48,27 +52,37 @@
         set_debug_mode(self.__restore)
 
 
 def magma_debug_section():
     return _MagmaDebugSection()
 
 
+def _unformat(msg):
+    # Remove escaped formatting, e.g. bold or color in stdout log.
+    ansi_escape = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]')
+    return ansi_escape.sub('', str(msg))
+
+
 def has_log(caplog, level=None, msg=None):
     if level is None and msg is None:
         return len(caplog.records) > 0
     if level and not msg:
         gen = (log.levelname == level for log in caplog.records)
     elif msg and not level:
-        gen = (str(log.msg) == str(msg) for log in caplog.records)
+        gen = (_unformat(log.msg) == _unformat(msg) for log in caplog.records)
     else:
-        gen = (log.levelname == level and str(log.msg) == str(msg)
+        gen = (log.levelname == level and _unformat(log.msg) == _unformat(msg)
                for log in caplog.records)
     return any(gen)
 
 
+def has_debug(caplog, msg=None):
+    return has_log(caplog, "DEBUG", msg)
+
+
 def has_info(caplog, msg=None):
     return has_log(caplog, "INFO", msg)
 
 
 def has_error(caplog, msg=None):
     return has_log(caplog, "ERROR", msg)
 
@@ -117,7 +131,33 @@
     def _get_magma_value_(self):
         return self._val
 
     def non_standard_operation(self):
         v0 = self._val << 2
         v1 = bits(self._val[0], len(self.T)) << 1
         return SimpleMagmaProtocol(v0 | v1 | bits(self._val[0], len(self.T)))
+
+
+def with_config(key, value):
+
+    def fixture():
+        prev_value = getattr(config, key)
+        setattr(config, key, value)
+        yield
+        setattr(config, key, prev_value)
+
+    return pytest.fixture(fixture)
+
+
+def check_gold(callee_file, filename):
+    try:
+        return check_files_equal(callee_file,
+                                 f"build/{filename}",
+                                 f"gold/{filename}")
+    except FileNotFoundError:
+        return False
+
+
+def update_gold(callee_file, filename):
+    file_path = os.path.dirname(callee_file)
+    return shutil.copy(f"{file_path}/build/{filename}",
+                       f"{file_path}/gold/{filename}")
```

### Comparing `magma-lang-2.2.9/magma/transforms.py` & `magma-lang-2.3.0/magma/transforms.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/tuple.py` & `magma-lang-2.3.0/magma/tuple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import itertools
 from functools import lru_cache
+import functools
+import operator
 from collections import OrderedDict
 from hwtypes.adt import (
     TupleMeta,
     Tuple as Tuple_,
-    AnonymousProduct,
     AnonymousProductMeta,
-    Product,
     ProductMeta,
 )
 from hwtypes import BitVector, Bit
-from hwtypes.adt_meta import BoundMeta, RESERVED_SUNDERS
+from hwtypes.adt_meta import BoundMeta, RESERVED_SUNDERS, ReservedNameError
 from hwtypes.util import TypedProperty, OrderedFrozenDict
 from .common import deprecated
-from .ref import AnonRef, TupleRef
+from .ref import TupleRef
 from .t import Type, Kind, Direction
 from .compatibility import IntegerTypes
-from .debug import debug_wire, get_callee_frame_info
+from .debug import debug_wire, get_debug_info, debug_unwire
 from .logging import root_logger
 from .protocol_type import magma_type, magma_value
 
-from magma.wire_container import WiringLog
+from magma.wire_container import (WiringLog, AggregateWireable,
+                                  aggregate_wireable_method)
 from magma.wire import wire
 from magma.protocol_type import MagmaProtocol
 from magma.operator_utils import output_only
 
 
 _logger = root_logger()
 
@@ -38,15 +38,16 @@
 #  - creates a new tuple value where each field equals vi
 #
 
 class TupleKind(TupleMeta, Kind):
     def __new__(mcs, name, bases, namespace, fields=None, **kwargs):
         for rname in RESERVED_SUNDERS:
             if rname in namespace:
-                raise ReservedNameError(f'class attribute {rname} is reserved by the type machinery')
+                raise ReservedNameError(f'class attribute {rname} is reserved '
+                                        'by the type machinery')
 
         bound_types = fields
         has_bound_base = False
         unbound_bases = []
         for base in bases:
             if isinstance(base, BoundMeta):
                 if base.is_bound:
@@ -63,15 +64,16 @@
                                     pass
                                 try:
                                     if y.is_bindable(x):
                                         continue
                                 except AttributeError:
                                     pass
                                 raise TypeError(
-                                    "Can't inherit from multiple different bound_types"
+                                    "Can't inherit from multiple different "
+                                    "bound_types"
                                 )
                 else:
                     unbound_bases.append(base)
 
         t = type.__new__(mcs, name, bases, namespace, **kwargs)
         t._fields_ = bound_types
         t._unbound_base_ = None
@@ -104,15 +106,15 @@
         if any(x is not y for x, y in zip(undirected_idx, idx)):
             bases = [cls[undirected_idx]]
         else:
             bases = [cls]
         bases = tuple(bases)
         class_name = cls._name_cb(idx)
 
-        t = mcs(class_name, bases, {'__module__' : cls.__module__}, fields=idx)
+        t = mcs(class_name, bases, {'__module__': cls.__module__}, fields=idx)
         if t._unbound_base_ is None:
             t._unbound_base_ = cls
         mcs._class_cache[cls, idx] = t
         t._cached_ = True
         return t
 
     def qualify(cls, direction):
@@ -141,14 +143,17 @@
         obj.__init__(*args, **kwargs)
         return obj
 
     @property
     def N(cls):
         return len(cls.fields)
 
+    def __len__(cls):
+        return cls.N
+
     def __str__(cls):
         if not cls.is_bound:
             return cls.__name__
         s = "Tuple("
         s += ",".join(str(T) for T in cls.fields)
         s += ")"
         return s
@@ -179,38 +184,42 @@
             return not rhs.is_bound
 
         return cls.fields == rhs.fields
 
     __hash__ = TupleMeta.__hash__
 
 
-class Tuple(Type, Tuple_, metaclass=TupleKind):
+class Tuple(Type, Tuple_, AggregateWireable, metaclass=TupleKind):
     def __init__(self, *largs, **kwargs):
 
-        Type.__init__(self, **kwargs) # name=
+        Type.__init__(self, **kwargs)
+        AggregateWireable.__init__(self)
 
-        self.ts = []
-        if len(largs) > 0:
+        self._ts = {}
+        if largs:
             assert len(largs) == len(self)
-            for k, t, T in zip(self.keys(), largs, self.types()):
+            for i, (k, t, T) in enumerate(zip(self.keys(),
+                                              largs,
+                                              self.types())):
                 if isinstance(t, (IntegerTypes, BitVector, Bit)):
                     t = T(t)
-                self.ts.append(t)
-                if not isinstance(self, AnonProduct):
-                    setattr(self, k, t)
-        else:
-            for k, T in zip(self.keys(), self.types()):
-                ref = TupleRef(self, k)
-                if issubclass(T, MagmaProtocol):
-                    t = T._from_magma_value_(T._to_magma_()(name=ref))
-                else:
-                    t = T(name=ref)
-                self.ts.append(t)
+                self._ts[i] = t
                 if not isinstance(self, AnonProduct):
                     setattr(self, k, t)
+            self._resolved = True
+
+        self._keys_list = list(self.keys())
+
+    def __getattr__(self, key):
+        if not isinstance(self, AnonProduct) and key in self.keys():
+            # On demand setattr for lazy children
+            t = self[key]
+            setattr(self, key, t)
+            return t
+        return object.__getattribute__(self, key)
 
     __hash__ = Type.__hash__
 
     @classmethod
     def is_oriented(cls, direction):
         return all(v.is_oriented(direction) for v in cls.fields)
 
@@ -228,31 +237,62 @@
         return [str(i) for i in range(len(cls.fields))]
 
     @output_only("Cannot use == on an input")
     def __eq__(self, rhs):
         if not isinstance(rhs, type(self)):
             return NotImplemented
         else:
-            return self.ts == rhs.ts
+            # NOTE: Use functools.reduce so import * doesn't clobber m.reduce
+            # from bits
+            return functools.reduce(operator.and_,
+                                    (x == y for x, y in zip(self, rhs)))
 
     @output_only("Cannot use != on an input")
     def __ne__(self, rhs):
         return ~(self == rhs)
 
     def __repr__(self):
         if not self.name.anon():
             return super().__repr__()
-        ts = [repr(t) for t in self.ts]
+        ts = [repr(t) for t in self]
         kts = ['{}={}'.format(k, v) for k, v in zip(self.keys(), ts)]
         return 'tuple(dict({})'.format(', '.join(kts))
 
+    def _make_t(self, idx):
+        T = self.types()[idx]
+        ref = TupleRef(self, self._keys_list[idx])
+        if issubclass(T, MagmaProtocol):
+            value = T._from_magma_ref_(ref)
+        else:
+            value = T(name=ref)
+        value.set_enclosing_when_context(self._enclosing_when_context)
+        return value
+
+    def has_elaborated_children(self):
+        return bool(self._ts)
+
+    def _enumerate_children(self):
+        return self.items()
+
     def __getitem__(self, key):
-        if key in self.keys():
-            key = list(self.keys()).index(key)
-        return self.ts[key]
+        if isinstance(key, str):
+            try:
+                key = list(self.keys()).index(key)
+            except ValueError:
+                raise KeyError(key) from None
+        if not isinstance(key, int):
+            raise KeyError(key)
+        if key not in self._ts:
+            self._ts[key] = self._make_t(key)
+            self._ts[key].parent = self
+        return self._ts[key]
+
+    @property
+    def ts(self):
+        return [self[k] for k in self.keys()]
 
     def __setitem__(self, key, val):
         old = self[key]
         if old is not val:
             _logger.error(
                 WiringLog(f"May not mutate tuple, trying to replace "
                           f"{{}}[{key}] ({{}}) with {{}}", self, old, val)
@@ -262,125 +302,130 @@
         return len(type(self).fields)
 
     @classmethod
     def flat_length(cls):
         return sum(magma_type(T).flat_length() for T in cls.types())
 
     def __call__(self, o):
-        return self.wire(o, get_callee_frame_info())
-
+        return self.wire(o, get_debug_info(3))
 
     @debug_wire
-    def wire(i, o, debug_info):
+    def wire(self, o, debug_info):
         o = magma_value(o)
         if not isinstance(o, Tuple):
             _logger.error(
                 WiringLog(f"Cannot wire {{}} (type={type(o)}) to {{}} "
-                          f"(type={type(i)}) because {{}} is not a Tuple",
-                          o, i, o),
+                          f"(type={type(self)}) because {{}} is not a Tuple",
+                          o, self, o),
                 debug_info=debug_info
             )
             return
 
-        if i.keys() != o.keys():
+        if self.keys() != o.keys():
             _logger.error(
                 WiringLog(f"Cannot wire {{}} (type={type(o)}, "
-                          f"keys={list(i.keys())}) to {{}} (type={type(i)}, "
+                          f"keys={list(self.keys())}) to "
+                          f" {{}} (type={type(self)}, "
                           f"keys={list(o.keys())}) because the tuples do not "
-                          f"have the same keys", o, i),
+                          f"have the same keys", o, self),
                 debug_info=debug_info
             )
             return
+        if self._should_wire_children(o):
+            for self_elem, o_elem in zip(self, o):
+                self_elem = magma_value(self_elem)
+                o_elem = magma_value(o_elem)
+                wire(o_elem, self_elem, debug_info)
+        else:
+            AggregateWireable.wire(self, o, debug_info)
 
-        for i_elem, o_elem in zip(i, o):
-            i_elem = magma_value(i_elem)
-            o_elem = magma_value(o_elem)
-            wire(o_elem, i_elem, debug_info)
-
-    def unwire(i, o):
-        for i_elem, o_elem in zip(i, o):
-            if o_elem.is_input():
-                o_elem.unwire(i_elem)
+    @debug_unwire
+    @aggregate_wireable_method
+    def unwire(self, o=None, debug_info=None, keep_wired_when_contexts=False):
+        for k, t in self.items():
+            if o is None:
+                t.unwire(debug_info=debug_info,
+                         keep_wired_when_contexts=keep_wired_when_contexts)
+            elif o[k].is_input():
+                o[k].unwire(t, debug_info=debug_info,
+                            keep_wired_when_contexts=keep_wired_when_contexts)
             else:
-                i_elem.unwire(o_elem)
+                t.unwire(o[k], debug_info=debug_info,
+                         keep_wired_when_contexts=keep_wired_when_contexts)
 
+    @aggregate_wireable_method
     def driven(self):
-        for t in self.ts:
-            if not t.driven():
-                return False
-        return True
+        return all(t.driven() for t in self)
 
+    @aggregate_wireable_method
     def wired(self):
-        for t in self.ts:
-            if not t.wired():
-                return False
-        return True
+        return all(t.wired() for t in self)
 
-    # test whether the values refer a whole tuple
     @staticmethod
     def _iswhole(ts, keys):
 
         for i in range(len(ts)):
             if ts[i].anon():
-                #print('not an inst or defn')
                 return False
 
         for i in range(len(ts)):
             # elements must be an tuple reference
             if not isinstance(ts[i].name, TupleRef):
-                #print('not an tuple ref')
                 return False
 
-        for i in range(1,len(ts)):
+        for i in range(1, len(ts)):
             # elements must refer to the same tuple
-            if ts[i].name.tuple is not ts[i-1].name.tuple:
+            if ts[i].name.tuple is not ts[i - 1].name.tuple:
                 return False
 
         for i in range(len(ts)):
             # elements should be numbered consecutively
             if ts[i].name.index != list(keys)[i]:
                 return False
 
         if len(ts) != len(ts[0].name.tuple):
             # elements should refer to a whole tuple
             return False
 
         return True
 
     def iswhole(self):
-        return Tuple._iswhole(self.ts, self.keys())
+        return Tuple._iswhole(list(self), self.keys())
 
+    @aggregate_wireable_method
     def trace(self, skip_self=True):
         ts = []
-        for t in self.ts:
+        for t in self:
             result = t.trace(skip_self)
             if result is not None:
                 ts.append(result)
             elif not skip_self and (t.is_output() or t.is_inout()):
                 ts.append(t)
             else:
                 return None
 
         if len(ts) == len(self) and Tuple._iswhole(ts, self.keys()):
             return ts[0].name.tuple
 
         return type(self).flip()(*ts)
 
+    @aggregate_wireable_method
     def value(self):
-        ts = [t.value() for t in self.ts]
+        ts = [t.value() for t in self]
 
         for t in ts:
             if t is None:
                 return None
 
         if len(ts) == len(self) and Tuple._iswhole(ts, self.keys()):
             return ts[0].name.tuple
 
         return type(self).flip()(*ts)
 
+    @aggregate_wireable_method
     def driving(self):
         return {k: t.driving() for k, t in self.items()}
 
     @classmethod
     def unflatten(cls, value):
         values = []
         offset = 0
@@ -388,32 +433,28 @@
             size = field.flat_length()
             ts = value[offset:offset + size]
             values.append(field.unflatten(ts))
             offset += size
         return cls(*values)
 
     def flatten(self):
-        return sum([t.flatten() for t in self.ts], [])
+        return sum([t.flatten() for t in self], [])
 
     def const(self):
-        for t in self.ts:
-            if not t.const():
-                return False
-
-        return True
+        return all(t.const() for t in self)
 
     @classmethod
     def types(cls):
         return cls.fields
 
     def values(self):
-        return self.ts
+        return list(self)
 
     def items(self):
-        return zip(self.keys(), self.ts)
+        return zip(self.keys(), self)
 
     def undriven(self):
         for elem in self:
             elem.undriven()
 
     def unused(self):
         for elem in self:
@@ -432,14 +473,19 @@
     def connection_iter(self, only_slice_bits=False):
         for elem in self:
             yield elem, elem.trace()
 
     def has_children(self):
         return True
 
+    def set_enclosing_when_context(self, ctx):
+        self._enclosing_when_context = ctx
+        for value in self._ts.values():
+            value.set_enclosing_when_context(ctx)
+
 
 def _add_properties(ns, fields):
     def _make_prop(field_type, idx):
         @TypedProperty(field_type)
         def prop(self):
             return self[idx]
 
@@ -477,15 +523,15 @@
         if undirected_idx != idx:
             bases = [cls[undirected_idx]]
         else:
             bases = [cls]
         bases = tuple(bases)
         class_name = cls._name_from_idx(idx)
 
-        ns = {'__module__' : cls.__module__}
+        ns = {'__module__': cls.__module__}
         # add properties to namespace
         # build properties
         _add_properties(ns, idx)
 
         t = mcs(class_name, bases, ns, fields=tuple(idx.values()))
         t._field_table_ = idx
         if t._unbound_base_ is None:
@@ -533,27 +579,33 @@
         if not cls.is_bound:
             return not rhs.is_bound
 
         return cls.field_dict == rhs.field_dict
 
     def is_wireable(cls, rhs):
         rhs = magma_type(rhs)
-        if not isinstance(rhs, AnonProductKind) or len(cls.fields) != len(rhs.fields):
+        if (
+            not isinstance(rhs, AnonProductKind) or
+            len(cls.fields) != len(rhs.fields)
+        ):
             return False
         for k, v in cls.field_dict.items():
-            if not k in rhs.field_dict or not v.is_wireable(rhs.field_dict[k]):
+            if k not in rhs.field_dict or not v.is_wireable(rhs.field_dict[k]):
                 return False
         return True
 
     def is_bindable(cls, rhs):
         rhs = magma_type(rhs)
-        if not isinstance(rhs, AnonProductKind) or len(cls.fields) != len(rhs.fields):
+        if (
+            not isinstance(rhs, AnonProductKind) or
+            len(cls.fields) != len(rhs.fields)
+        ):
             return False
         for k, v in cls.field_dict.items():
-            if not k in rhs.field_dict or not v.is_bindable(rhs.field_dict[k]):
+            if k not in rhs.field_dict or not v.is_bindable(rhs.field_dict[k]):
                 return False
         return True
 
     def __len__(cls):
         return len(cls.fields)
 
     def __str__(cls):
@@ -566,54 +618,38 @@
 
 
 class AnonProduct(Tuple, metaclass=AnonProductKind):
     @classmethod
     def keys(cls):
         return cls.field_dict.keys()
 
-    @classmethod
-    def types(cls):
-        return cls.fields
-
-    def value(self):
-        ts = [t.value() for t in self.ts]
-
-        for t in ts:
-            if t is None:
-                return None
-
-        if len(ts) == len(self) and Tuple._iswhole(ts, self.keys()):
-            return ts[0].name.tuple
-
-        return type(self).flip()(*ts)
-
 
 class ProductKind(ProductMeta, AnonProductKind, Kind):
     __hash__ = type.__hash__
 
     def __new__(mcs, name, bases, namespace, cache=True, **kwargs):
         return super().__new__(mcs, name, bases, namespace, cache, **kwargs)
 
-    def from_fields(cls, name, fields , cache=True):
+    def from_fields(cls, name, fields, cache=True):
         return super().from_fields(name, fields, cache)
 
     @classmethod
     def _from_fields(mcs, fields, name, bases, ns, **kwargs):
 
         cls = bases[0]
 
         # add properties to namespace
         # build properties
         _add_properties(ns, fields)
 
         # this is all really gross but I don't know how to do this cleanly
         # need to build t so I can call super() in new and init
         # need to exec to get proper signatures
-        t = TupleKind.__new__(mcs, name, bases, ns, fields=tuple(fields.values()),
-                              **kwargs)
+        t = TupleKind.__new__(mcs, name, bases, ns,
+                              fields=tuple(fields.values()), **kwargs)
         if t._unbound_base_ is None:
             t._unbound_base_ = cls
 
         # not strictly necessary could iterative over class dict finding
         # TypedProperty to reconstruct _field_table_ but that seems bad
         t._field_table_ = OrderedFrozenDict(fields)
         return t
```

### Comparing `magma-lang-2.2.9/magma/type_utils.py` & `magma-lang-2.3.0/magma/type_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 
 import hwtypes as ht
 
 from magma.array import Array
 from magma.bit import Bit
 from magma.bits import Bits, UInt, SInt
+from magma.common import replace_all
 from magma.digital import Digital
 from magma.protocol_type import MagmaProtocol
 from magma.t import Kind
 from magma.tuple import Tuple, Product
 
 
 def isprotocol(T):
@@ -145,21 +146,35 @@
         return ht.Product.from_fields(T.__name__, _fields)
     if issubclass(T, Tuple):
         _fields = tuple(to_hwtypes(v) for v in T.fields)
         return ht.Tuple[_fields]
     raise NotImplementedError(T)
 
 
+_TYPE_STR_SANITIZATION_MAP = {
+    "(": "",
+    ")": "",
+    ",": "_",
+    "=": "_",
+    "[": "",
+    "]": "",
+    " ": "",
+    "<": "",
+    ">": "",
+    ".": "",
+    "'": "",
+    ":": "",
+    "{": "",
+    "}": "",
+}
+
+
 def type_to_sanitized_string(T: Kind) -> str:
-    return str(T).\
-        replace("(", "").\
-        replace(")", "").\
-        replace(",", "_").\
-        replace("=", "_").\
-        replace("[", "").\
-        replace("]", "").\
-        replace(" ", "").\
-        replace("<", "").\
-        replace(">", "").\
-        replace(".", "").\
-        replace("'", "").\
-        replace(":", "")
+    return replace_all(str(T), _TYPE_STR_SANITIZATION_MAP)
+
+
+def contains_tuple(T):
+    if issubclass(T, Tuple):
+        return True
+    if issubclass(T, Array):
+        return contains_tuple(T.T)
+    return False
```

### Comparing `magma-lang-2.2.9/magma/types/bit_pattern.py` & `magma-lang-2.3.0/magma/types/bit_pattern.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/uniquification.py` & `magma-lang-2.3.0/magma/uniquification.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/value_utils.py` & `magma-lang-2.3.0/magma/value_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 
 
 class ValueVisitor(WrappedVisitor):
     def wrap(self, value):
         return _wrap_value(value)
 
 
+class ValueTransformer(ValueVisitor):
+    def generic_visit(self, value):
+        wrapped = _wrap_value(value)
+        args = (self.visit(child) for child in wrapped.children)
+        return type(value)(*args)
+
+
 @dataclasses.dataclass(frozen=True)
 class Selector:
     child: 'Selector'
 
     def select(self, value):
         value = self._select(value)
         if self.child is None:
@@ -76,23 +83,43 @@
     def _select(self, value):
         return value[self.index]
 
     def __str__(self):
         return f"[{self.index}]{self._child_str()}"
 
 
-def _make_selector_impl(value, child):
+def _make_selector_impl(value, child, stop_at):
     value = _unwrap_protocol_value(value)
-    ref = value.name
-    if isinstance(ref, ArrayRef):
-        child = ArraySelector(child, ref.index)
-        return _make_selector_impl(ref.array, child)
-    if isinstance(ref, TupleRef):
-        child = TupleSelector(child, ref.index)
-        return _make_selector_impl(ref.tuple, child)
+    if value is not stop_at:
+        ref = value.name
+        if isinstance(ref, ArrayRef):
+            child = ArraySelector(child, ref.index)
+            return _make_selector_impl(ref.array, child, stop_at)
+        if isinstance(ref, TupleRef):
+            child = TupleSelector(child, ref.index)
+            return _make_selector_impl(ref.tuple, child, stop_at)
     if child is not None:
         return child
     return Selector(None)
 
 
-def make_selector(value):
-    return _make_selector_impl(value, None)
+def make_selector(value, stop_at=None):
+    """stop_at (optional): indicate parent value to 'stop at', useful if you
+    want a partial selector of a child"""
+    return _make_selector_impl(value, None, stop_at)
+
+
+class _FillVisitor(ValueVisitor):
+    def __init__(self, fill_value: bool):
+        self._fill_value = fill_value
+
+    def visit_Digital(self, value):
+        value @= self._fill_value
+
+    def visit_Bits(self, value):
+        size = len(value)
+        fill_value = 0 if not self._fill_value else (1 << size) - 1
+        value @= fill_value
+
+
+def fill(value, fill_value: bool):
+    _FillVisitor(fill_value).visit(value)
```

### Comparing `magma-lang-2.2.9/magma/verilog_utils.py` & `magma-lang-2.3.0/magma/verilog_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,31 @@
         elems = ", ".join(value_to_verilog_name(t, disable_ndarray)
                           for t in reversed(value))
         return f"'{{{elems}}}"
     elif isinstance(value, Tuple):
         raise NotImplementedError("Inlining unflattened tuple")
     elif isinstance(value, InstView):
         prefix = ""
-        if value.parent is not None:
-            prefix = value_to_verilog_name(value.parent, disable_ndarray) + "."
+        if value.parent_view is not None:
+            prefix = value_to_verilog_name(
+                value.parent_view, disable_ndarray
+            ) + "."
         return prefix + value.inst.name
     return verilog_name(value.name, disable_ndarray=disable_ndarray)
 
 
 def verilog_name(name, inst_sep="_", disable_ndarray=False):
     if isinstance(name, PortViewRef):
-        curr = name.view.parent
+        curr = name.view.parent_view
         hierarchical_path = curr.inst.name + "."
-        while isinstance(curr.parent, InstView):
-            hierarchical_path = curr.parent.inst.name + "." + hierarchical_path
-            curr = curr.parent
+        while isinstance(curr.parent_view, InstView):
+            hierarchical_path = (
+                curr.parent_view.inst.name + "." + hierarchical_path
+            )
+            curr = curr.parent_view
         return hierarchical_path + verilog_name(
             name.view.port.name, disable_ndarray=disable_ndarray)
     if isinstance(name, DefnRef):
         return str(name)
     if isinstance(name, InstRef):
         return f"{name.inst.name}{inst_sep}{str(name)}"
     if isinstance(name, NamedRef):
```

### Comparing `magma-lang-2.2.9/magma/view.py` & `magma-lang-2.3.0/magma/view.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Tuple
+
 from magma.protocol_type import MagmaProtocol, MagmaProtocolMeta
 from magma.ref import PortViewRef
 from magma.t import Out
 
 
 class PortViewMeta(MagmaProtocolMeta):
     def _to_magma_(cls):
@@ -17,48 +19,53 @@
         return type(cls)(f"PortView{T}", (cls, ), {"T": T})
 
 
 class PortView(MagmaProtocol, metaclass=PortViewMeta):
     def _get_magma_value_(self):
         return self._magma_value
 
-    def __init__(self, port, parent):
+    def __init__(self, port, parent_view):
         self.port = port
-        self.parent = parent
+        self.parent_view = parent_view
         self._magma_value = Out(type(port))(name=PortViewRef(self))
 
     def __getitem__(self, key):
         port = self.port
         try:
             item = port[key]
         except KeyError:
             raise Exception(f"Can only use getitem with arrays and "
                             f"tuples not {type(self.port)}")
-        return PortView[type(item)](item, self.parent)
+        return PortView[type(item)](item, self.parent_view)
 
     def __getattr__(self, key):
         port = self.port
         try:
             attr = getattr(port, key)
         except AttributeError:
             return object.__getattribute__(self, key)
-        return PortView[type(attr)](attr, self.parent)
+        return PortView[type(attr)](attr, self.parent_view)
+
+    def path(self) -> Tuple[str]:
+        path = (self.port.name.name,)
+        curr = self.parent_view
+        while isinstance(curr, InstView):
+            path = (curr.inst.name,) + path
+            curr = curr.parent_view
+        return path
 
     def get_hierarchical_coreir_select(self):
-        curr = self.parent
-        hierarchical_path = curr.inst.name + ";"
-        while isinstance(curr.parent, InstView):
-            hierarchical_path = curr.parent.inst.name + ";" + hierarchical_path
-            curr = curr.parent
-        return hierarchical_path
+        if self.parent_view is None:
+            return ";"
+        return ";".join(self.parent_view.path()) + ";"
 
     def root(self):
-        curr = self.parent
-        while isinstance(curr.parent, InstView):
-            curr = curr.parent
+        curr = self.parent_view
+        while isinstance(curr.parent_view, InstView):
+            curr = curr.parent_view
         return curr
 
     def __str__(self):
         return (self.get_hierarchical_coreir_select() +
                 self.port.name.qualifiedname())
 
     def __iter__(self):
@@ -66,29 +73,35 @@
         return self
 
     def __len__(self):
         return len(self.port)
 
     def __next__(self):
         n = next(self.__iter)
-        return PortView[type(n)](n, self.parent)
+        return PortView[type(n)](n, self.parent_view)
 
 
 class InstView:
-    def __init__(self, inst, parent=None):
+    def __init__(self, inst, parent_view=None):
         self.inst = inst
         self.circuit = type(inst)
         self.instance_map = None
         if hasattr(self.circuit, "instances"):
             self.instance_map = {instance.name: instance for instance in
                                  self.circuit.instances}
-        self.parent = parent
+        self.parent_view = parent_view
 
     def __getattr__(self, attr):
         try:
             if attr in self.circuit.interface.ports.keys():
                 port = self.inst.interface.ports[attr]
                 return PortView[type(port)](port, self)
             elif attr in self.instance_map:
                 return InstView(self.instance_map[attr], self)
         except AttributeError:
             return object.__getattribute__(self, attr)
+
+    def path(self) -> Tuple[str]:
+        path = (self.inst.name,)
+        if self.parent_view is None:
+            return path
+        return self.parent_view.path() + path
```

### Comparing `magma-lang-2.2.9/magma/waveform.py` & `magma-lang-2.3.0/magma/waveform.py`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/magma/wire.py` & `magma-lang-2.3.0/magma/wire.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,7 +59,12 @@
                       o, i),
             debug_info=debug_info
         )
         return
 
     # Wire(o, Type).
     i.wire(o, debug_info)
+
+
+@debug_wire
+def unwire(input, output=None, debug_info=None):
+    input.unwire(output, debug_info)
```

### Comparing `magma-lang-2.2.9/magma_lang.egg-info/PKG-INFO` & `magma-lang-2.3.0/magma_lang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: magma-lang
-Version: 2.2.9
+Version: 2.3.0
 Summary: An embedded DSL for constructing hardware circuits
 Home-page: https://github.com/phanrahan/magma
 Maintainer: Lenny Truong
 Maintainer-email: lenny@cs.stanford.edu
 License: MIT
 Description: # Magma
         [![Documentation Status](https://readthedocs.org/projects/magma/badge/?version=latest)](https://magma.readthedocs.io/en/latest/?badge=latest)
         [![Linux Test](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml/badge.svg)](https://github.com/phanrahan/magma/actions/workflows/linux-test.yml)
         [![codecov](https://codecov.io/gh/phanrahan/magma/branch/master/graph/badge.svg)](https://codecov.io/gh/phanrahan/magma)
         [![Join the chat at https://gitter.im/Magma-HDL/community](https://badges.gitter.im/Magma-HDL/community.svg)](https://gitter.im/Magma-HDL/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         
-        [CHANGELOG](https://github.com/phanrahan/magma/blob/master/CHANGELOG.md)
-        
         [CHEAT SHEET](https://github.com/phanrahan/magma/blob/master/docs/cheat_sheet.md)
         
         Magma is a hardware design language embedded in python.
         
         The central abstraction in Magma is a circuit.
         A circuit is a set of functional units that are wired together.
         Magma circuits are analagous to verilog modules.
@@ -56,15 +54,15 @@
         [magmathon](https://github.com/phanrahan/magmathon) repository contains
         a set of [Jupyter
         Notebooks](https://github.com/phanrahan/magmathon/tree/master/notebooks/tutorial)
         that introduce the system. There's also
         [magma_examples](https://github.com/leonardt/magma_examples) and
         [magma_tutorial](https://github.com/leonardt/magma_tutorial) which contain a
         set of basic circuits and tests, providing an example templates for a magma
-        projects.  Finally there is [magma_riscv_mini](https://github.com/leonardt/magma_riscv_mini)
+        projects.  Finally there is [magma_riscv_mini](./examples/riscv_mini)
         which provides an example of a simple RISCV processor. Please also refer to the
         [documentation](http://magma.readthedocs.io/).
         
         The design of Magma was heavily influenced by 
         [Chisel](https://chisel.eecs.berkeley.edu/),
         so Magma should be easy to learn if you know Chisel.
         Some examples from the Chisel tutorial have been ported to
```

### Comparing `magma-lang-2.2.9/magma_lang.egg-info/SOURCES.txt` & `magma-lang-2.3.0/magma_lang.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 setup.py
 bin/magma
 magma/__init__.py
 magma/array.py
 magma/ast_utils.py
 magma/bfloat.py
 magma/bind.py
+magma/bind2.py
 magma/bit.py
 magma/bit_primitives.py
 magma/bits.py
 magma/bitutils.py
 magma/braid.py
 magma/circuit.py
-magma/circuit_utils.py
 magma/clock.py
 magma/clock_io.py
 magma/common.py
 magma/compatibility.py
 magma/compile.py
 magma/compile_exception.py
 magma/compile_guard.py
@@ -27,17 +27,20 @@
 magma/conversions.py
 magma/debug.py
 magma/definition_context.py
 magma/digital.py
 magma/display.py
 magma/enum.py
 magma/family.py
+magma/find_unconnected_ports.py
 magma/generator.py
 magma/if_def.py
 magma/inline_verilog.py
+magma/inline_verilog2.py
+magma/inline_verilog_expression.py
 magma/interface.py
 magma/ir.py
 magma/is_definition.py
 magma/is_primitive.py
 magma/language_utils.py
 magma/linking.py
 magma/log.py
@@ -46,28 +49,31 @@
 magma/monitor.py
 magma/operator_utils.py
 magma/placer.py
 magma/protocol_type.py
 magma/ref.py
 magma/scope.py
 magma/set_name.py
+magma/stubify.py
 magma/symbol_table.py
 magma/symbol_table_utils.py
 magma/t.py
 magma/transforms.py
 magma/tuple.py
 magma/type_utils.py
 magma/uniquification.py
 magma/util.py
 magma/value_utils.py
 magma/verilog_utils.py
 magma/view.py
 magma/waveform.py
+magma/when.py
 magma/wire.py
 magma/wire_container.py
+magma/wire_utils.py
 magma/backend/__init__.py
 magma/backend/blif.py
 magma/backend/check_wiring_context.py
 magma/backend/dot.py
 magma/backend/firrtl.py
 magma/backend/util.py
 magma/backend/verilog.py
@@ -80,59 +86,74 @@
 magma/backend/coreir/insert_coreir_wires.py
 magma/backend/coreir/insert_wrap_casts.py
 magma/backend/mlir/build_magma_graph.py
 magma/backend/mlir/builtin.py
 magma/backend/mlir/comb.py
 magma/backend/mlir/common.py
 magma/backend/mlir/compile_to_mlir.py
+magma/backend/mlir/compile_to_mlir_opts.py
+magma/backend/mlir/errors.py
 magma/backend/mlir/graph_lib.py
 magma/backend/mlir/hardware_module.py
 magma/backend/mlir/hw.py
 magma/backend/mlir/magma_common.py
 magma/backend/mlir/magma_ops.py
+magma/backend/mlir/mem_utils.py
 magma/backend/mlir/mlir.py
 magma/backend/mlir/mlir_compiler.py
 magma/backend/mlir/mlir_printer_utils.py
 magma/backend/mlir/mlir_to_verilog.py
-magma/backend/mlir/mlir_to_verilog_main.py
+magma/backend/mlir/print_opts.py
 magma/backend/mlir/printer_base.py
 magma/backend/mlir/scoped_name_generator.py
 magma/backend/mlir/sv.py
 magma/backend/mlir/translation_unit.py
+magma/backend/mlir/when_utils.py
+magma/backend/mlir/xmr_utils.py
 magma/frontend/__init__.py
 magma/frontend/coreir.py
 magma/frontend/coreir_.py
 magma/frontend/dummy_verilog_importer.py
 magma/frontend/pyverilog_importer.py
 magma/frontend/verilog.py
 magma/frontend/verilog_importer.py
 magma/frontend/verilog_utils.py
 magma/passes/__init__.py
 magma/passes/clock.py
 magma/passes/debug_name.py
 magma/passes/drive_undriven.py
-magma/passes/find_errors.py
+magma/passes/elaborate_circuit.py
+magma/passes/elaborate_tuples.py
+magma/passes/finalize_whens.py
+magma/passes/group.py
+magma/passes/instance_callback_pass.py
 magma/passes/ir.py
 magma/passes/passes.py
+magma/passes/raise_logs_as_exceptions.py
 magma/passes/terminate_unused.py
 magma/passes/tsort.py
 magma/primitives/__init__.py
 magma/primitives/lut.py
 magma/primitives/memory.py
+magma/primitives/multiport_memory.py
 magma/primitives/mux.py
 magma/primitives/register.py
 magma/primitives/set_index.py
 magma/primitives/slice.py
+magma/primitives/when.py
 magma/primitives/wire.py
+magma/primitives/xmr.py
 magma/simulator/__init__.py
 magma/simulator/coreir_simulator.py
 magma/simulator/mdb.py
 magma/simulator/python_simulator.py
 magma/simulator/simulator.py
 magma/smart/__init__.py
+magma/smart/eval.py
+magma/smart/make_smart.py
 magma/smart/smart_bits.py
 magma/ssa/__init__.py
 magma/ssa/ssa.py
 magma/syntax/__init__.py
 magma/syntax/combinational.py
 magma/syntax/combinational2.py
 magma/syntax/coroutine.py
@@ -144,14 +165,14 @@
 magma/syntax/transforms/__init__.py
 magma/syntax/transforms/inline_yield_from.py
 magma/syntax/transforms/replace_symbols.py
 magma/testing/__init__.py
 magma/testing/utils.py
 magma/types/__init__.py
 magma/types/bit_pattern.py
-magma/types/ready_valid.py
+magma/types/handshake.py
 magma/types/valid.py
 magma_lang.egg-info/PKG-INFO
 magma_lang.egg-info/SOURCES.txt
 magma_lang.egg-info/dependency_links.txt
 magma_lang.egg-info/requires.txt
 magma_lang.egg-info/top_level.txt
```

### Comparing `magma-lang-2.2.9/setup.cfg` & `magma-lang-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `magma-lang-2.2.9/setup.py` & `magma-lang-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='magma-lang',
-    version='2.2.9',
+    version='2.3.0',
     url='https://github.com/phanrahan/magma',
     license='MIT',
     maintainer='Lenny Truong',
     maintainer_email='lenny@cs.stanford.edu',
     description='An embedded DSL for constructing hardware circuits',
     scripts=['bin/magma'],
     packages=[
@@ -33,17 +34,19 @@
         "astor",
         "six",
         "dataclasses",
         "mako",
         "pyverilog",
         "numpy",
         "graphviz",
-        "coreir>=2.0.144",
+        "coreir>=2.0.151",
         "hwtypes>=1.4.4",
         "ast_tools>=0.0.16",
         "staticfg",
         "networkx",
+        "uinspect",
+        "circt==1.48.1.dev34",
     ],
     python_requires='>=3.6',
     long_description=long_description,
     long_description_content_type="text/markdown"
 )
```

