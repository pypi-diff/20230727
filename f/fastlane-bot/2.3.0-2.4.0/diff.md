# Comparing `tmp/fastlane_bot-2.3.0.tar.gz` & `tmp/fastlane_bot-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-2.3.0.tar", last modified: Wed Jul 26 14:30:05 2023, max compression
+gzip compressed data, was "fastlane_bot-2.4.0.tar", last modified: Thu Jul 27 12:57:58 2023, max compression
```

## Comparing `fastlane_bot-2.3.0.tar` & `fastlane_bot-2.4.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.846561 fastlane_bot-2.3.0/fastlane_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 14:29:31.000000 fastlane_bot-2.3.0/fastlane_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/config/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/cloaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/pools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/poolandtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/receipthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/routehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/submithandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/tradeinstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/txhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/univ3calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/modes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/modes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/tests/test_pairwise_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single_bancor3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.862561 fastlane_bot-2.3.0/fastlane_bot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_000_Template.py
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20948 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_003_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    29819 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_004_GraphCode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_005_Uniswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_007_NoneResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_033_Pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_034_Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_035_Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_036_Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_037_Exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_039_TestMultiMode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_040_TestSingleMode.py
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_047_Randomizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25275 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/arbgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86957 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/noneresult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18750 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/convexoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/cpcarboptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/dcbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/margpoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/simpleoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/simplepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/tokenscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/univ3calc_DELETE.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.846561 fastlane_bot-2.3.0/fastlane_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.739841 fastlane_bot-2.4.0/fastlane_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 12:57:28.000000 fastlane_bot-2.4.0/fastlane_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.743841 fastlane_bot-2.4.0/fastlane_bot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/cloaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/config/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.743841 fastlane_bot-2.4.0/fastlane_bot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/data/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/data/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.743841 fastlane_bot-2.4.0/fastlane_bot/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.743841 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/exchanges/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.747841 fastlane_bot-2.4.0/fastlane_bot/events/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/managers/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.747841 fastlane_bot-2.4.0/fastlane_bot/events/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/pools/uniswap_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.747841 fastlane_bot-2.4.0/fastlane_bot/events/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/test_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.747841 fastlane_bot-2.4.0/fastlane_bot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/poolandtokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/receipthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/routehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/submithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/tradeinstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/txhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/helpers/univ3calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.751841 fastlane_bot-2.4.0/fastlane_bot/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/base_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/base_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/pairwise_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/pairwise_single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.751841 fastlane_bot-2.4.0/fastlane_bot/modes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/tests/test_pairwise_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/triangle_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/triangle_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/modes/triangle_single_bancor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.751841 fastlane_bot-2.4.0/fastlane_bot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_000_Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20948 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_003_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29819 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_004_GraphCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_005_Uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_007_NoneResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_033_Pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_034_Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_035_Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_036_Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_037_Exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_039_TestMultiMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_040_TestSingleMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_047_Randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25275 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/fastlane_bot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/arbgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86957 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/noneresult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18750 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/convexoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/cpcarboptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/dcbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/margpoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/simpleoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/simplepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/tokenscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/tools/univ3calc_DELETE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/fastlane_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:58.739841 fastlane_bot-2.4.0/fastlane_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-27 12:57:58.000000 fastlane_bot-2.4.0/fastlane_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-27 12:57:58.000000 fastlane_bot-2.4.0/fastlane_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:57:58.000000 fastlane_bot-2.4.0/fastlane_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 12:57:58.000000 fastlane_bot-2.4.0/fastlane_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 12:57:58.000000 fastlane_bot-2.4.0/fastlane_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:57:58.755841 fastlane_bot-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-27 12:56:20.000000 fastlane_bot-2.4.0/setup.py
```

### Comparing `fastlane_bot-2.3.0/LICENSE` & `fastlane_bot-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/PKG-INFO` & `fastlane_bot-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane_bot
-Version: 2.3.0
+Version: 2.4.0
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-2.3.0/README.md` & `fastlane_bot-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/bot.py` & `fastlane_bot-2.4.0/fastlane_bot/bot.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/base.py` & `fastlane_bot-2.4.0/fastlane_bot/config/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/cloaker.py` & `fastlane_bot-2.4.0/fastlane_bot/config/cloaker.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/config.py` & `fastlane_bot-2.4.0/fastlane_bot/config/config.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/connect.py` & `fastlane_bot-2.4.0/fastlane_bot/config/connect.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/db.py` & `fastlane_bot-2.4.0/fastlane_bot/config/db.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/logger.py` & `fastlane_bot-2.4.0/fastlane_bot/config/logger.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/network.py` & `fastlane_bot-2.4.0/fastlane_bot/config/network.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/provider.py` & `fastlane_bot-2.4.0/fastlane_bot/config/provider.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/config/selectors.py` & `fastlane_bot-2.4.0/fastlane_bot/config/selectors.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/data/abi.py` & `fastlane_bot-2.4.0/fastlane_bot/data/abi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/data/pools.py` & `fastlane_bot-2.4.0/fastlane_bot/data/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/__init__.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/bancor_v3.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/base.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/carbon_v1.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/factory.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/sushiswap_v2.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v2.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v3.py` & `fastlane_bot-2.4.0/fastlane_bot/events/exchanges/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/interface.py` & `fastlane_bot-2.4.0/fastlane_bot/events/interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/managers/base.py` & `fastlane_bot-2.4.0/fastlane_bot/events/managers/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/managers/contracts.py` & `fastlane_bot-2.4.0/fastlane_bot/events/managers/contracts.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/managers/events.py` & `fastlane_bot-2.4.0/fastlane_bot/events/managers/events.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/managers/manager.py` & `fastlane_bot-2.4.0/fastlane_bot/events/managers/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,16 @@
             If no event or pool info is provided.
             If the pool info is invalid.
         """
         while True:
             if limiter:
                 rate_limiter = 0.1 + 0.9 * random.random()
                 time.sleep(rate_limiter)
+            else:
+                rate_limiter = 0
             try:
                 if event:
                     self.update_from_event(event=event, block_number=block_number)
                 elif address:
                     self.update_from_contract(
                         address, contract, block_number=block_number
                     )
```

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/managers/pools.py` & `fastlane_bot-2.4.0/fastlane_bot/events/managers/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/__init__.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/bancor_v3.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/base.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/carbon_v1.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/factory.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/sushiswap_v2.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v2.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v3.py` & `fastlane_bot-2.4.0/fastlane_bot/events/pools/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_exchanges.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_interface.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_manager.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_pools.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_utils.py` & `fastlane_bot-2.4.0/fastlane_bot/events/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/events/utils.py` & `fastlane_bot-2.4.0/fastlane_bot/events/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/poolandtokens.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/poolandtokens.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/routehandler.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/routehandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/submithandler.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/submithandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/tradeinstruction.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/tradeinstruction.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/txhelpers.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/txhelpers.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/helpers/univ3calc.py` & `fastlane_bot-2.4.0/fastlane_bot/helpers/univ3calc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/base.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/base_pairwise.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/base_pairwise.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/base_triangle.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/base_triangle.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_multi.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/pairwise_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_single.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/tests/test_pairwise_single.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/tests/test_pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_multi.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/triangle_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/triangle_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single_bancor3.py` & `fastlane_bot-2.4.0/fastlane_bot/modes/triangle_single_bancor3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/testing.py` & `fastlane_bot-2.4.0/fastlane_bot/testing.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_000_Template.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_000_Template.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_003_Serialization.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_003_Serialization.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_004_GraphCode.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_004_GraphCode.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_005_Uniswap.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_005_Uniswap.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_007_NoneResult.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_007_NoneResult.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_033_Pools.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_033_Pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_034_Interface.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_034_Interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_035_Utils.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_035_Utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_036_Manager.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_036_Manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_037_Exchanges.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_037_Exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_039_TestMultiMode.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_039_TestMultiMode.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_040_TestSingleMode.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_040_TestSingleMode.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_047_Randomizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_047_Randomizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py` & `fastlane_bot-2.4.0/fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/analyzer.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/arbgraphs.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/arbgraphs.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/cpc.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/cpc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/cryptocompare.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/noneresult.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/noneresult.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/__init__.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/base.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/convexoptimizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/convexoptimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/cpcarboptimizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/cpcarboptimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/dcbase.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/dcbase.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/margpoptimizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/margpoptimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/simpleoptimizer.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/optimizer/simpleoptimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/params.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/params.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/simplepair.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/simplepair.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/tokenscale.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/tokenscale.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/tools/univ3calc_DELETE.py` & `fastlane_bot-2.4.0/fastlane_bot/tools/univ3calc_DELETE.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot/utils.py` & `fastlane_bot-2.4.0/fastlane_bot/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/fastlane_bot.egg-info/PKG-INFO` & `fastlane_bot-2.4.0/fastlane_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane-bot
-Version: 2.3.0
+Version: 2.4.0
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-2.3.0/fastlane_bot.egg-info/SOURCES.txt` & `fastlane_bot-2.4.0/fastlane_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.3.0/setup.py` & `fastlane_bot-2.4.0/setup.py`

 * *Files identical despite different names*

