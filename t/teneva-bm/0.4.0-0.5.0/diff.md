# Comparing `tmp/teneva_bm-0.4.0.tar.gz` & `tmp/teneva_bm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.4.0.tar", last modified: Tue Jul 25 22:45:22 2023, max compression
+gzip compressed data, was "teneva_bm-0.5.0.tar", last modified: Thu Jul 27 18:27:58 2023, max compression
```

## Comparing `teneva_bm-0.4.0.tar` & `teneva_bm-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.533345 teneva_bm-0.4.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.4.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.4.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    18288 2023-07-25 22:45:22.533554 teneva_bm-0.4.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    17027 2023-07-25 22:44:31.000000 teneva_bm-0.4.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      779 2023-07-24 16:41:37.000000 teneva_bm-0.4.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-25 22:45:22.534178 teneva_bm-0.4.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.4.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.504854 teneva_bm-0.4.0/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      233 2023-07-25 22:44:38.000000 teneva_bm-0.4.0/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.509336 teneva_bm-0.4.0/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)       45 2023-07-25 20:49:49.000000 teneva_bm-0.4.0/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4457 2023-07-25 22:27:59.000000 teneva_bm-0.4.0/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     1185 2023-07-25 22:09:12.000000 teneva_bm-0.4.0/teneva_bm/agent/bm_agent_swimmer.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.511345 teneva_bm-0.4.0/teneva_bm/agent_toe/
--rw-r--r--   0 andrei     (501) staff       (20)       52 2023-07-25 20:50:12.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2959 2023-07-25 22:32:56.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/agent_toe.py
--rw-r--r--   0 andrei     (501) staff       (20)     1277 2023-07-25 22:25:31.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/bm_agent_toe_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)    29490 2023-07-25 21:41:50.000000 teneva_bm-0.4.0/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.518279 teneva_bm-0.4.0/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.4.0/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3523 2023-07-25 15:25:46.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2398 2023-07-24 16:50:33.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2457 2023-07-24 16:49:31.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2392 2023-07-24 16:50:42.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2840 2023-07-24 16:50:21.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3388 2023-07-24 16:49:54.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2402 2023-07-24 16:50:01.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2580 2023-07-24 16:50:11.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3152 2023-07-24 16:50:59.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3244 2023-07-24 16:51:02.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2096 2023-07-24 16:51:10.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3204 2023-07-24 16:51:17.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.520121 teneva_bm-0.4.0/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.4.0/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1624 2023-07-22 16:16:15.000000 teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2120 2023-07-22 17:59:30.000000 teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.524315 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.528595 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.530101 teneva_bm-0.4.0/teneva_bm/oc/
--rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.4.0/teneva_bm/oc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4185 2023-07-24 12:59:27.000000 teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-22 17:35:02.000000 teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.531725 teneva_bm-0.4.0/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.4.0/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7130 2023-07-22 16:59:19.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1864 2023-07-25 16:21:14.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2929 2023-07-25 15:27:50.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2935 2023-07-25 15:26:50.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3386 2023-07-24 16:41:38.000000 teneva_bm-0.4.0/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.533047 teneva_bm-0.4.0/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.4.0/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7815 2023-07-24 13:03:33.000000 teneva_bm-0.4.0/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12451 2023-07-24 13:04:15.000000 teneva_bm-0.4.0/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1877 2023-07-24 12:57:04.000000 teneva_bm-0.4.0/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.507712 teneva_bm-0.4.0/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    18288 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2143 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.821829 teneva_bm-0.5.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.5.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.5.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    18567 2023-07-27 18:27:58.822271 teneva_bm-0.5.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    17306 2023-07-27 18:27:03.000000 teneva_bm-0.5.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-27 07:20:23.000000 teneva_bm-0.5.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-06-19 10:36:15.000000 teneva_bm-0.5.0/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-27 18:27:58.823494 teneva_bm-0.5.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.5.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.784493 teneva_bm-0.5.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      208 2023-07-27 18:26:56.000000 teneva_bm-0.5.0/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.792385 teneva_bm-0.5.0/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      168 2023-07-27 13:43:14.000000 teneva_bm-0.5.0/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5812 2023-07-27 15:14:05.000000 teneva_bm-0.5.0/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1818 2023-07-27 18:00:55.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1868 2023-07-27 18:01:50.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_humanoid.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6836 2023-07-27 15:13:48.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1831 2023-07-27 15:13:53.000000 teneva_bm-0.5.0/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2113 2023-07-27 13:10:46.000000 teneva_bm-0.5.0/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    31229 2023-07-27 15:44:59.000000 teneva_bm-0.5.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.798770 teneva_bm-0.5.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.5.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3606 2023-07-27 10:01:49.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2487 2023-07-27 10:01:53.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2526 2023-07-27 10:01:57.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2481 2023-07-27 10:02:00.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2928 2023-07-27 10:02:04.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3519 2023-07-27 10:02:08.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2493 2023-07-27 10:02:11.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2669 2023-07-27 10:02:15.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3277 2023-07-27 10:02:21.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3334 2023-07-27 10:02:24.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2187 2023-07-27 10:02:28.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3335 2023-07-27 10:02:33.000000 teneva_bm-0.5.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.800286 teneva_bm-0.5.0/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.5.0/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1622 2023-07-27 10:24:15.000000 teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2147 2023-07-27 10:24:20.000000 teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.806077 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.812441 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.815366 teneva_bm-0.5.0/teneva_bm/oc/
+-rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.5.0/teneva_bm/oc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4166 2023-07-27 10:24:35.000000 teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2265 2023-07-27 10:24:30.000000 teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.818583 teneva_bm-0.5.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.5.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7023 2023-07-27 10:23:51.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1861 2023-07-27 10:23:56.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2979 2023-07-27 10:24:01.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2985 2023-07-27 10:24:04.000000 teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3386 2023-07-24 16:41:38.000000 teneva_bm-0.5.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.821270 teneva_bm-0.5.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.5.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7794 2023-07-27 11:58:55.000000 teneva_bm-0.5.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12653 2023-07-27 13:50:14.000000 teneva_bm-0.5.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-27 10:23:32.000000 teneva_bm-0.5.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 18:27:58.787775 teneva_bm-0.5.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    18567 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2179 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-27 18:27:58.000000 teneva_bm-0.5.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.4.0/LICENSE.txt` & `teneva_bm-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/PKG-INFO` & `teneva_bm-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,61 +30,61 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.4.0".
+> Current version "0.5.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
 - Сollections `oc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
-> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
-bm = BmQuboMaxcut().prep()
+bm = BmQuboMaxcut()
+bm.prep()
 print(bm.info())
 ```
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
-> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
 
-- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
-
-- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
+- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
@@ -101,46 +101,50 @@
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
-bm = BmFuncAckley().prep()
+bm = BmFuncAckley()
+bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
+
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
+
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
+
 - `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
+
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
--
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
+
 - `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
-- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
-
-- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
 
-- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
@@ -192,14 +196,18 @@
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
 The following function may be used to print the corresponding values: `print(bm.info_history())`.
 
+##### Notes
+
+- For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
+
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_bm-0.4.0/README.md` & `teneva_bm-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,61 +4,61 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.4.0".
+> Current version "0.5.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
 - Сollections `oc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
-> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
-bm = BmQuboMaxcut().prep()
+bm = BmQuboMaxcut()
+bm.prep()
 print(bm.info())
 ```
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
-> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
 
-- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
-
-- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
+- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
@@ -75,46 +75,50 @@
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
-bm = BmFuncAckley().prep()
+bm = BmFuncAckley()
+bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
+
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
+
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
+
 - `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
+
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
--
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
+
 - `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
-- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
-
-- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
 
-- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
@@ -166,14 +170,18 @@
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
 The following function may be used to print the corresponding values: `print(bm.info_history())`.
 
+##### Notes
+
+- For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
+
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_bm-0.4.0/demo.py` & `teneva_bm-0.5.0/demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 Call it as "python demo.py" to run demo for all existing benchmarks or as
 "python demo.py bm_<name_of_collection>_<name_of_benchmark>" to run an example
 for a specific benchmark "<name_of_benchmark>" from the collection (folder)
 "<name_of_collection" (e.g., "python demo.py bm_qubo_knap_amba"). Note that the
 code for the demo run is at the end of the corresponding benchmark file in the
 section "if __name__ == '__main__':".
 
+You can also run this script as ""python demo.py info" to present only info
+about existing collections and benchmarks.
+
 """
 import sys
 
 
 from teneva_bm import teneva_bm_demo
```

### Comparing `teneva_bm-0.4.0/setup.py` & `teneva_bm-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.5.0/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 from teneva_bm.agent.agent import Agent
 
 
 
 DESC = """
     Agent from myjoco environment "Swimmer". For details, see
     https://mgoulao.github.io/gym-docs/environments/mujoco/swimmer
+
+    By default ("policy_name" is 'none"), no policy is used. The Toeplitz
+    discrete policy may be also used (if "policy_name" is 'toeplitz"), see
+    https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py
 """
 
 
 class BmAgentSwimmer(Agent):
     def __init__(self, d=None, n=32, name='AgentSwimmer', desc=DESC,
-                 steps=1000):
-        env = Agent.env_build('Swimmer', 'Swimmer-v4')
-        super().__init__(d, n, name, desc, steps, env)
+                 steps=1000, policy_name='none'):
+        super().__init__(d, n, name, desc, steps, policy_name)
 
-        if d is not None:
-            self.set_err('Dimension number (d) should not be set manually')
+    def prep_bm(self, policy=None):
+        env = Agent.env_build('Swimmer-v4')
+        return super().prep_bm(env, policy)
 
-    def set_state(self, state, x=0., y=0.):
+    def _set_state(self, state, x=0., y=0.):
         qpos = np.array([x, y] + list(state[:3]))
         qvel = state[3:]
-        self.env.set_state(qpos, qvel)
+        self._env.set_state(qpos, qvel)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmAgentSwimmer().prep()
     print(bm.info())
@@ -38,10 +42,21 @@
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
     text = 'Generate video for a random multi-index  :  '
-    bm.render()
-    text += 'see "_result" folder with mp4 file'
+    bm = BmAgentSwimmer(steps=200).prep()
+    i = [np.random.choice(k) for k in bm.n]
+    y = bm[i]
+    bm.render('result/BmAgentSwimmer_demo_none')
+    text += 'see "result/...demo_none.mp4'
+    print(text)
+
+    text = 'Generate video for a random multi-index  :  '
+    bm = BmAgentSwimmer(steps=200, policy_name='toeplitz').prep()
+    i = [np.random.choice(k) for k in bm.n]
+    y = bm[i]
+    bm.render('result/BmAgentSwimmer_demo_toeplitz')
+    text += 'see "result/...demo_toeplitz.mp4'
     print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/agent_toe/bm_agent_toe_swimmer.py` & `teneva_bm-0.5.0/teneva_bm/agent/bm_agent_humanoid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 import numpy as np
 
 
 from teneva_bm.agent.agent import Agent
-from teneva_bm.agent_toe.agent_toe import AgentToe
 
 
 
 DESC = """
-    Agent from myjoco environment "Swimmer". For details, see
-    https://mgoulao.github.io/gym-docs/environments/mujoco/swimmer
-    The Toeplitz discrete policy is used, see for details
+    Agent from myjoco environment "Humanoid". For details, see
+    https://mgoulao.github.io/gym-docs/environments/mujoco/humanoid/
+
+    By default ("policy_name" is 'none"), no policy is used. The Toeplitz
+    discrete policy may be also used (if "policy_name" is 'toeplitz"), see
     https://github.com/jparkerholder/ASEBO/blob/master/asebo/policies.py
 """
 
 
-class BmAgentToeSwimmer(AgentToe):
-    def __init__(self, d=None, n=3, name='AgentToeSwimmer', desc=DESC,
-                 steps=1000):
-        env = Agent.env_build('Swimmer', 'Swimmer-v4')
-        super().__init__(d, n, name, desc, steps, env)
+class BmAgentHumanoid(Agent):
+    def __init__(self, d=None, n=32, name='AgentHumanoid', desc=DESC,
+                 steps=1000, policy_name='none'):
+        super().__init__(d, n, name, desc, steps, policy_name)
+
+    def prep_bm(self, policy=None):
+        env = Agent.env_build('Humanoid-v4')
+        return super().prep_bm(env, policy)
 
-    def set_state(self, state, x=0., y=0.):
+    def _set_state(self, state, x=0., y=0.):
+        return # TODO !!!
         qpos = np.array([x, y] + list(state[:3]))
         qvel = state[3:]
-        self.env.set_state(qpos, qvel)
+        self._env.set_state(qpos, qvel)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmAgentToeSwimmer().prep()
+    bm = BmAgentHumanoid().prep()
     print(bm.info())
 
-    #I_trn, y_trn = bm.build_trn(1.E+1)
-    #print(bm.info_history())
+    I_trn, y_trn = bm.build_trn(1.E+1)
+    print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
     text = 'Generate video for a random multi-index  :  '
-    bm.render()
-    text += 'see "_result" folder with mp4 file'
+    bm = BmAgentHumanoid(steps=200).prep()
+    i = [np.random.choice(k) for k in bm.n]
+    y = bm[i]
+    bm.render('result/BmAgentHumanoid_demo_none')
+    text += 'see "result/...demo_none.mp4'
+    print(text)
+
+    text = 'Generate video for a random multi-index  :  '
+    bm = BmAgentHumanoid(steps=200, policy_name='toeplitz').prep()
+    i = [np.random.choice(k) for k in bm.n]
+    y = bm[i]
+    bm.render('result/BmAgentHumanoid_demo_toeplitz')
+    text += 'see "result/...demo_toeplitz.mp4'
     print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/bm.py` & `teneva_bm-0.5.0/teneva_bm/bm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
+import os
 import teneva
 from time import perf_counter as tpc
 
 
 from teneva_bm import __version__
 
 
 class Bm:
     def __init__(self, d=None, n=None, name='', desc=''):
-        self._init()
+        self.init()
 
         self.set_seed()
 
         self.set_size(d, n)
-        self.set_quantization()
         self.set_constr()
 
         self.set_grid()
         self.set_grid_kind()
 
         self.set_name(name)
         self.set_desc(desc)
@@ -37,27 +37,32 @@
 
     def __getitem__(self, I):
         """Return a value or batch of values for provided multi-index."""
         return self.get(I)
 
     @property
     def a0(self):
-        """Return the lower grid size value if it is constant."""
+        """Return the lower grid size float value if it is constant."""
         if not self.is_a_equal:
             raise ValueError('Lower grid size is not constant, can`t get a0')
         return self.a[0]
 
     @property
     def b0(self):
-        """Return the upper grid size value if it is constant."""
+        """Return the upper grid size float value if it is constant."""
         if not self.is_b_equal:
             raise ValueError('Upper grid size is not constant, can`t get b0')
         return self.b[0]
 
     @property
+    def identity(self):
+        """Returns a list of parameter names that define the benchmark."""
+        return ['d', 'n']
+
+    @property
     def is_a_equal(self):
         """Check if all the lower grid sizes are the same."""
         v = self.list_convert(self.a, 'float')
         return v is None or isinstance(v, (float,))
 
     @property
     def is_b_equal(self):
@@ -88,74 +93,79 @@
 
     @property
     def is_n_odd(self):
         """Check if all the mode sizes are odd (1, 3, ...)."""
         return not self.is_n_even
 
     @property
+    def is_opti_max(self):
+        """If the benchmark relates to maximization task."""
+        return False
+
+    @property
     def is_tens(self):
         """Check if BM relates to tensor (i.e., discrete function)."""
         return not self.is_func
 
     @property
     def n0(self):
-        """Return the mode size value if it is constant."""
+        """Return the mode size int value if it is constant."""
         if not self.is_n_equal:
             raise ValueError('Mode size is not constant, can`t get n0')
         return self.n[0]
 
     @property
+    def time_full(self):
+        """Full time of benchmark existence in seconds."""
+        return tpc() - self.time_stamp_start
+
+    @property
     def with_constr(self):
         """Return True if benchmark has a constraint."""
         return False
 
     @property
     def with_cores(self):
         """Return True if exact TT-cores can be constructed for benchmark."""
         return False
 
     def build_cores(self):
         """Return exact TT-cores for the TT-representation of the tensor."""
         if self.is_tens:
-            # TODO: check why
             msg = 'Construction of the TT-cores does not work for tensors'
             raise ValueError(msg)
 
+        if not self.with_cores:
+            msg = 'Construction of the TT-cores does not supported for this BM'
+            raise ValueError(msg)
+
         I = np.array([teneva.grid_flat(k) for k in self.n], dtype=int).T
         X = teneva.ind_to_poi(I, self.a, self.b, self.n, self.grid_kind)
 
-        return self._cores(X)
+        return self.cores(X)
 
     def build_trn(self, m=0, skip_process=False):
         """Generate random (from LHS) train dataset of (index, value)."""
-        m = int(m)
-        n = [2]*self.quantization*self.d if self.with_quantization else self.n
-
         if m < 1:
             return None, None
 
-        # TODO: add fixed random seed support
-        I_trn = teneva.sample_lhs(n, m)
+        I_trn = self.sample_lhs(m)
         y_trn = self.get(I_trn, skip_process)
 
         if y_trn is None:
             raise ValueError('The specified budget is exceeded')
 
         return I_trn, y_trn
 
     def build_tst(self, m=0, skip_process=True):
         """Generate random (from "choice") test dataset of (index, value)."""
-        m = int(m)
-        n = [2]*self.quantization*self.d if self.with_quantization else self.n
-
         if m < 1:
             return None, None
 
-        # TODO: add fixed random seed support
-        I_tst = np.vstack([np.random.choice(k, m) for k in n]).T
+        I_tst = self.sample_random(m)
         y_tst = self.get(I_tst, skip_process)
 
         if y_tst is None:
             raise ValueError('The specified budget is exceeded')
 
         return I_tst, y_tst
 
@@ -173,21 +183,75 @@
             msg = f'BM "{self.name}" is not ready'
             for e in self.err:
                 msg += f'\n    Error > {e}'
             raise ValueError(msg)
 
         return True
 
+    def compute(self, X, skip_process=False):
+        m = self.m
+        m_cur = X.shape[0]
+        m_max = self.budget_m
+
+        if not skip_process and m_max:
+            if (m >= m_max) or (m + m_cur > m_max and self.budget_is_strict):
+                return None
+
+        if not self.with_constr:
+            return self.target_batch(X)
+
+        y = np.ones(m_cur, dtype=float) * self.constr_penalty
+
+        c = self.constr_batch(X)
+        ind_good = c < self.constr_eps
+        y[ind_good] = self.target_batch(X[ind_good])
+        if self.constr_with_amplitude:
+            y[~ind_good] *= c[~ind_good]
+
+        return y
+
+    def constr(self, x):
+        """Function that check constraint for a given point/index."""
+        return self.constr_batch(x.reshape(1, -1))[0]
+
+    def constr_batch(self, X):
+        """Function that check constraint for a given batch of poi./indices."""
+        return np.array([self.constr(x) for x in X])
+
+    def cores(self, X):
+        """Return the exact TT-cores for the provided points."""
+        raise NotImplementedError()
+
+    def cores_add(self, X, a0=0):
+        """Helper function for the construction of the TT-cores."""
+        Y = []
+
+        for x in X:
+            G = np.ones([2, len(x), 2])
+            G[1, :, 0] = 0.
+            G[0, :, 1] = x
+            Y.append(G)
+
+        Y[0] = Y[0][0:1, ...].copy()
+        Y[-1] = Y[-1][..., 1:2].copy()
+        Y[-1][0, :, 0] += a0
+
+        return Y
+
+    def cores_mul(self, X):
+        """Helper function for the construction of the TT-cores."""
+        return [x[None, :, None] for x in X]
+
     def get(self, I, skip_process=False):
         """Return a value or batch of values for provided multi-index."""
         t = tpc()
 
         self.check()
 
-        I, X, is_batch = self._parse_input(I=I)
+        I, X, is_batch = self.parse_input(I=I)
 
         if self.with_cache:
             m = I.shape[0]
             ind = [k for k in range(m) if tuple(I[k]) not in self.cache]
 
             m_new = len(ind)
             dm_cache = m - m_new
@@ -198,45 +262,44 @@
                         return None
                 else:
                     if self.m_cache > self.budget_m_cache:
                         return None
 
             if m_new > 0:
                 Z = X[ind] if self.is_func else I[ind]
-                y_new = self._compute(Z, skip_process)
+                y_new = self.compute(Z, skip_process)
                 if y_new is None:
                     return None
 
                 for k in range(m_new):
                     self.cache[tuple(I[ind[k]])] = y_new[k]
 
             y = np.array([self.cache[tuple(i)] for i in I])
 
         else:
             dm_cache = 0
 
             Z = X if self.is_func else I
-            y = self._compute(Z, skip_process)
+            y = self.compute(Z, skip_process)
             if y is None:
                 return None
 
-        return self._process(I, X, y, dm_cache, t, is_batch, skip_process)
+        return self.process(I, X, y, dm_cache, t, is_batch, skip_process)
 
     def get_config(self):
         """Return a dict with configuration of the benchmark."""
         conf = {
             'd': self.d,
             'n': self.list_convert(self.n, 'int'),
             'seed': self.seed,
             'name': self.name,
             'benchmark': self.__class__.__name__,
             'version': __version__,
             'is_tens': self.is_tens,
             'is_func': self.is_func,
-            'with_quantization': self.with_quantization,
             'with_cache': self.with_cache,
             'with_constr': self.with_constr,
             'with_cores': self.with_cores,
         }
 
         if self.is_func:
             conf['a'] = self.list_convert(self.a, 'float')
@@ -280,33 +343,48 @@
             'x_max': self.x_max,
             'y_max': self.y_max,
             'i_min': self.i_min,
             'x_min': self.x_min,
             'y_min': self.y_min,
             'y_list': self.y_list,
             'time': self.time,
-            'time_full': tpc() - self.log_t,
+            'time_full': self.time_full,
             'err': '; '.join(self.err) if len(self.err) else '',
         }
 
         return hist
 
+    def get_solution(self, i=None, best=True):
+        """Return the solution for given i or current solution or the best."""
+        if i is None:
+            if best:
+                i = self.i_max if self.is_opti_max else self.i_min
+            else:
+                i = self.i
+
+        if i is None:
+            raise ValueError('Input is not set')
+
+        y = self.get(i, skip_process=True)
+
+        return i, y
+
     def get_poi(self, X, skip_process=False):
         """Return a value or batch of values for provided x-point."""
         t = tpc()
 
         self.check()
 
-        I, X, is_batch = self._parse_input(X=X)
+        I, X, is_batch = self.parse_input(X=X)
 
-        y = self._compute(X, skip_process)
+        y = self.compute(X, skip_process)
         if y is None:
             return None
 
-        return self._process(I, X, y, 0, t, is_batch, skip_process)
+        return self.process(I, X, y, 0, t, is_batch, skip_process)
 
     def info(self, footer=''):
         """Returns a detailed description of the benchmark as text."""
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
         text += f'DIMS = {self.d:-4d} | '
         n = np.mean(self.n)
@@ -366,18 +444,14 @@
             v = self.grid_kind
             text += f'{v}\n'
 
         text += 'Function kind                            : '
         v = 'discrete' if self.is_tens else 'continuous'
         text += f'{v}\n'
 
-        text += 'With quantization                        : '
-        v = 'YES' if self.with_quantization else 'no'
-        text += f'{v}\n'
-
         text += 'With cache                               : '
         v = 'YES' if self.with_cache else 'no'
         text += f'{v}\n'
 
         text += 'With constraint                          : '
         v = 'YES' if self.with_constr else 'no'
         text += f'{v}\n'
@@ -457,15 +531,15 @@
             text += '>               Options'
             text += '\n'
             text += footer
 
         text += '=' * 78 + '\n'
         return text
 
-    def info_history(self):
+    def info_history(self, footer=''):
         """Returns an information about the request history (text)."""
         text = ''
 
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
         text += f'DIMS = {self.d:-4d} | '
         n = np.mean(self.n)
@@ -489,15 +563,15 @@
         text += 'Average time of one request (sec)        : '
         text += f'{self.time/self.m:-10.3e}\n'
 
         text += 'Total requests time (sec)                : '
         text += f'{self.time:-10.3e}\n'
 
         text += 'Total work time (sec)                    : '
-        text += f'{tpc() - self.log_t:-10.3e}\n'
+        text += f'{self.time_full:-10.3e}\n'
 
         if self.y_min is not None and self.y_min_real is not None:
             text += 'Minimum (found / real)                   : '
             text += f'{self.y_min:-10.3e}   / {self.y_min_real:-10.3e}\n'
         elif self.y_min is not None:
             text += 'Minimum (found)                          : '
             text += f'{self.y_min:-10.3e}\n'
@@ -509,75 +583,270 @@
         if self.y_max is not None and self.y_max_real is not None:
             text += 'Maximum (found / real)                   : '
             text += f'{self.y_max:-10.3e}   / {self.y_max_real:-10.3e}\n'
         elif self.y_max is not None:
             text += 'Maximum (found)                          : '
             text += f'{self.y_max:-10.3e}\n'
 
+        if footer:
+            text += '-' * 41 + '|             '
+            text += '>               Options'
+            text += '\n'
+            text += footer
+
         text += '=' * 78 + '\n'
         return text
 
+    def init(self):
+        self.err = []
+
+        # Last solution:
+        self.i = None
+        self.x = None
+        self.y = None
+
+        self.is_y_max_new = False
+        self.i_max = None
+        self.x_max = None
+        self.y_max = None
+
+        self.is_y_min_new = False
+        self.i_min = None
+        self.x_min = None
+        self.y_min = None
+
+        self.y_list = []
+
+        self.m = 0
+        self.m_cache = 0
+        self.time = 0.
+
+        self.log_m_last = 0
+
+        self.is_prep = False
+
+        self.time_stamp_start = tpc()
+
     def list_convert(self, x, kind='float', eps=1.E-16):
         """Convert list of equal values to one number and back."""
         if x is None:
             return None
+
         if kind == 'int':
             if isinstance(x, (int, float)):
                 return np.array([x]*self.d, dtype=int)
             return int(x[0]) if len(set(x))==1 else np.asanyarray(x, dtype=int)
+
         elif kind == 'float':
             if isinstance(x, (int, float)):
                 return np.array([x]*self.d, dtype=float)
             for v in x:
                 if np.abs(v - x[0]) > eps:
                     return np.asanyarray(x, dtype=float)
             return float(x[0])
+
         else:
             raise ValueError('Unsupported kind for list conversion')
 
     def log(self, postfix='', out=False):
-        self.log_m_last = self.m
-        t = tpc() - self.log_t
-
         text = ''
 
         if self.log_prefix:
             text += self.log_prefix + ' > '
 
         text += f'm {self.m:-7.1e}'
         if self.with_cache:
             text += f' [+ {self.m_cache:-7.1e}]'
         text += ' | '
 
-        text += f't {t:-7.1e} | '
+        text += f't {self.time_full:-7.1e} | '
 
         if self.log_with_min and self.y_min is not None:
             text += f'min {self.y_min:-10.3e} | '
 
         if self.log_with_max and self.y_max is not None:
             text += f'max {self.y_max:-10.3e} | '
 
         if postfix:
             text = text + postfix
 
         if out:
             print(text)
 
+        self.log_m_last = self.m
+
         return text
 
+    def log_check(self):
+        if not self.with_log:
+            return False
+
+        if self.log_cond == 'min':
+            return self.is_y_min_new
+
+        if self.log_cond == 'max':
+            return self.is_y_max_new
+
+        if self.log_cond == 'min-max':
+            return self.is_y_min_new or self.is_y_max_new
+
+        if self.log_cond == 'step':
+            return self.log_step and self.m - self.log_m_last >= self.log_step
+
+    def parse_input(self, I=None, X=None):
+        if I is None and X is None or I is not None and X is not None:
+            raise ValueError('Can`t parse input. Invalid case')
+
+        if X is not None and self.is_tens:
+            msg = f'BM "{self.name}" is a tensor. '
+            msg += 'Can`t compute it in the point'
+            raise ValueError(msg)
+
+        if I is not None:
+            I = np.asanyarray(I, dtype=int)
+
+            is_batch = len(I.shape) == 2
+            if not is_batch:
+                I = I.reshape(1, -1)
+
+            if self.is_func:
+                X = teneva.ind_to_poi(I, self.a, self.b, self.n, self.grid_kind)
+
+        elif X is not None:
+            X = np.asanyarray(X, dtype=float)
+
+            is_batch = len(X.shape) == 2
+            if not is_batch:
+                X = X.reshape(1, -1)
+
+            if self.is_func:
+                I = teneva.poi_to_ind(X, self.a, self.b, self.n, self.grid_kind)
+
+        return I, X, is_batch
+
+    def path_build(self, fpath=None, ext=None):
+        if not fpath:
+            return
+
+        fold = os.path.dirname(fpath)
+        if fold:
+            os.makedirs(fold, exist_ok=True)
+
+        if ext and not fpath.endswith('.' + ext):
+            fpath += '.' + ext
+
+        return fpath
+
     def prep(self):
         """A function with a specific benchmark preparation code."""
-        # Note that when inherited, the function in the child class
-        # must starts with the following line:
         self.check_err()
-
-        # and it should ends with the following two lines:
+        self.prep_bm()
         self.is_prep = True
         return self
 
+    def prep_bm(self):
+        """A function with a specific benchmark preparation code (inner)."""
+        return
+
+    def process(self, I, X, y, dm_cache, t, is_batch, skip=False):
+        if skip:
+            return y if is_batch else y[0]
+
+        self.y_list.extend(list(y))
+
+        self.m += y.shape[0] - dm_cache
+        self.m_cache += dm_cache
+
+        self.time += tpc() - t
+
+        self.i = I[-1, :].copy() if I is not None else None
+        self.x = X[-1, :].copy() if X is not None else None
+        self.y = y[-1]
+
+        ind = np.argmax(y)
+        if self.y_max is None or self.y_max < y[ind]:
+            self.is_y_max_new = True
+            self.i_max = I[ind, :] if I is not None else None
+            self.x_max = X[ind, :] if X is not None else None
+            self.y_max = y[ind]
+        else:
+            self.is_y_max_new = False
+
+
+        ind = np.argmin(y)
+        if self.y_min is None or self.y_min > y[ind]:
+            self.is_y_min_new = True
+            self.i_min = I[ind, :] if I is not None else None
+            self.x_min = X[ind, :] if X is not None else None
+            self.y_min = y[ind]
+        else:
+            self.is_y_min_new = False
+
+        if self.log_check():
+            print(self.log())
+
+        if self.cache_m_max and len(self.cache.keys()) > self.cache_m_max:
+            self.cache = {}
+            self.wrn('The maximum cache size has been exceeded. Cache cleared')
+
+        return y if is_batch else y[0]
+
+    def recover(self, i=None, best=True):
+        """Restores some benchmark-specific values."""
+        raise NotImplementedError
+        i, y = self.get_solution(i, best)
+
+    def render(self, fpath=None, i=None, best=True):
+        """Render the solution for benchmark."""
+        raise NotImplementedError
+        i, y = self.get_solution(i, best)
+        fpath = self.path_build(fpath)
+
+    def sample_lhs(self, m):
+        """Generate LHS smaples (multi-indices).
+
+        Args:
+            m (int, float): number of samples.
+
+        Returns:
+            np.ndarray: generated multi-indices for the tensor in the form of
+            array of the shape [m, d], where d is the dimension of the tensor.
+
+        """
+        d = self.d
+        n = self.n
+        m = int(m)
+
+        I = np.empty((m, d), dtype=int)
+        for i, k in enumerate(n):
+            I1 = np.repeat(np.arange(k), m // k)
+            I2 = self.rand.choice(np.arange(k), m-len(I1), replace=False)
+            I[:, i] = np.concatenate([I1, I2])
+            self.rand.shuffle(I[:, i])
+
+        return I
+
+    def sample_random(self, m):
+        """Generate random smaples (multi-indices).
+
+        Args:
+            m (int, float): number of samples.
+
+        Returns:
+            np.ndarray: generated multi-indices for the tensor in the form of
+            array of the shape [m, d], where d is the dimension of the tensor.
+
+        """
+        n = self.n
+        m = int(m)
+
+        I = np.vstack([self.rand.choice(np.arange(k), m) for k in n]).T
+
+        return I
+
     def set_budget(self, m=None, m_cache=None, is_strict=True):
         """Set computation buget."""
         self.budget_m = int(m) if m else None
         self.budget_m_cache = int(m_cache) if m_cache else None
         self.budget_is_strict = is_strict
 
     def set_cache(self, with_cache=False, cache=None, m_max=1.E+8):
@@ -598,14 +867,17 @@
 
     def set_err(self, err=''):
         """Set the error text (can not import external module, etc.)."""
         self.err.append(err)
 
     def set_grid(self, a=None, b=None):
         """Set grid lower (a) and upper (b) limits for the function-like BM."""
+        if (a is not None or b is not None) and not self.d:
+            raise ValueError('Please, set dimension "d" before')
+
         self.a = teneva.grid_prep_opt(a, self.d)
         self.b = teneva.grid_prep_opt(b, self.d)
 
     def set_grid_kind(self, kind='cheb'):
         """Set the kind of the grid ('cheb' or 'uni').
 
         Note:
@@ -627,16 +899,14 @@
         self.with_log = with_log
         self.log_cond = cond
         self.log_step = int(step) if step else None
         self.log_prefix = prefix
         self.log_with_min = with_min
         self.log_with_max = with_max
 
-        self.log_t = tpc()
-
         if not self.log_cond in ['min', 'max', 'min-max', 'step']:
             raise ValueError(f'Invalid "log_cond" argument "{self.log_cond}"')
 
     def set_max(self, i=None, x=None, y=None):
         """Set exact (real) global maximum (index, point and related value)."""
         self.i_max_real = i
         self.x_max_real = x
@@ -666,244 +936,43 @@
         """Set display name for the problem."""
         self.name = name
 
     def set_opts(self):
         """Set options specific to the benchmark."""
         return
 
-    def set_quantization(self, with_quantization=False):
-        """Set quantization usage."""
-        self.with_quantization = with_quantization
-
-        if not self.with_quantization:
-            self.quantization = None
-            return
-
-        if not self.is_n_equal:
-            msg = 'Quantization now works only if all mode sizes are equal'
-            raise NotImplementedError(msg)
-
-        n = self.n0
-        self.quantization = int(np.log2(n))
-        if 2**self.quantization != n:
-            msg = 'Invalid mode size for quantization '
-            msg += '(it should be a power of two)'
-            raise ValueError(msg)
-
     def set_seed(self, seed=42):
         self.seed = seed
         self.rand = np.random.default_rng(self.seed)
 
     def set_size(self, d=None, n=None):
         """Set dimension (d) and sizes for all d-modes (n: int or list)."""
         self.d = None if d is None else int(d)
+
+        if n is not None and not self.d:
+            raise ValueError('Please, set dimension "d" before')
+
         self.n = teneva.grid_prep_opt(n, self.d, int)
 
     def shift_grid(self, scale=25):
         """Apply random shift for the grid limits."""
         shift = self.rand.normal(size=self.d) / scale
         self.a = self.a - (self.b-self.a) * shift
         self.b = self.b + (self.b-self.a) * shift
 
-    def _c(self, x):
-        """Function that check constraint for a given point/index."""
-        return self._c_batch(x.reshape(1, -1))[0]
-
-    def _c_batch(self, X):
-        """Function that check constraint for a given batch of poi./indices."""
-        return np.array([self._c(x) for x in X])
-
-    def _compute(self, X, skip_process=False):
-        m = self.m
-        m_cur = X.shape[0]
-        m_max = self.budget_m
+    def show(self, fpath=None, i=None, best=True):
+        """Present the state of the benchmark (image, graph, etc.)."""
+        raise NotImplementedError
+        i, y = self.get_solution(i, best)
+        fpath = self.path_build(fpath)
 
-        if not skip_process and m_max:
-            if (m >= m_max) or (m + m_cur > m_max and self.budget_is_strict):
-                return None
-
-        if not self.with_constr:
-            return self._f_batch(X)
-
-        y = np.ones(X.shape[0]) * self.constr_penalty
-
-        c = self._c_batch(X)
-        ind_good = c < self.constr_eps
-
-        y[ind_good] = self._f_batch(X[ind_good])
-        if self.constr_with_amplitude:
-            y[~ind_good] *= c[~ind_good]
-
-        return y
-
-    def _cores(self, X):
-        """Return the exact TT-cores for the provided points."""
-        raise NotImplementedError()
-
-    def _cores_add(self, X, a0=0):
-        """Helper function for the construction of the TT-cores."""
-        Y = []
-
-        for x in X:
-            G = np.ones([2, len(x), 2])
-            G[1, :, 0] = 0.
-            G[0, :, 1] = x
-            Y.append(G)
-
-        Y[0] = Y[0][0:1, ...].copy()
-        Y[-1] = Y[-1][..., 1:2].copy()
-        Y[-1][0, :, 0] += a0
-
-        return Y
-
-    def _cores_mul(self, X):
-        """Helper function for the construction of the TT-cores."""
-        return [x[None, :, None] for x in X]
-
-    def _f(self, x):
+    def target(self, x):
         """Function that computes value for a given point/index."""
-        return self._f_batch(x.reshape(1, -1))[0]
+        return self.target_batch(x.reshape(1, -1))[0]
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         """Function that computes values for a given batch of points/indices."""
-        return np.array([self._f(x) for x in X])
-
-    def _init(self):
-        self.err = []
-
-        self.is_y_max_new = False
-        self.i_max = None
-        self.x_max = None
-        self.y_max = None
-
-        self.is_y_min_new = False
-        self.i_min = None
-        self.x_min = None
-        self.y_min = None
-
-        self.y_list = []
-
-        self.m = 0
-        self.m_cache = 0
-        self.time = 0.
-
-        self.log_m_last = 0
-
-        self.is_prep = False
-
-    def _log_check(self):
-        if not self.with_log:
-            return False
-
-        if self.log_cond == 'min':
-            return self.is_y_min_new
-
-        if self.log_cond == 'max':
-            return self.is_y_max_new
-
-        if self.log_cond == 'min-max':
-            return self.is_y_min_new or self.is_y_max_new
-
-        if self.log_cond == 'step':
-            return self.log_step and self.m - self.log_m_last >= self.log_step
-
-    def _parse_input(self, I=None, X=None):
-        if I is not None and X is not None:
-            raise ValueError('Can`t parse input. Invalid case')
-
-        if I is None and X is None:
-            raise ValueError('Can`t parse input. Invalid case')
-
-        if X is not None and self.is_tens:
-            msg = f'BM "{self.name}" is a tensor. '
-            msg += 'Can`t compute it in the point'
-            raise ValueError(msg)
-
-        if I is not None:
-            I = np.asanyarray(I, dtype=int)
-
-            is_batch = len(I.shape) == 2
-            if not is_batch:
-                I = I.reshape(1, -1)
-
-            if self.with_quantization:
-                I = self._unquantize(I)
-
-            if self.is_func:
-                X = teneva.ind_to_poi(I, self.a, self.b, self.n, self.grid_kind)
-
-        elif X is not None:
-            X = np.asanyarray(X, dtype=float)
-
-            is_batch = len(X.shape) == 2
-            if not is_batch:
-                X = X.reshape(1, -1)
-
-            if self.with_quantization:
-                X = self._unquantize(X)
-
-            if self.is_func:
-                I = teneva.poi_to_ind(X, self.a, self.b, self.n, self.grid_kind)
-
-        return I, X, is_batch
-
-    def _process(self, I, X, y, dm_cache, t, is_batch, skip=False):
-        if skip:
-            return y if is_batch else y[0]
-
-        self.y_list.extend(list(y))
-
-        self.m += y.shape[0] - dm_cache
-        self.m_cache += dm_cache
-
-        self.time += tpc() - t
-
-        ind = np.argmax(y)
-        if self.y_max is None or self.y_max < y[ind]:
-            self.is_y_max_new = True
-            self.i_max = I[ind, :] if I is not None else None
-            self.x_max = X[ind, :] if X is not None else None
-            self.y_max = y[ind]
-        else:
-            self.is_y_max_new = False
-
-
-        ind = np.argmin(y)
-        if self.y_min is None or self.y_min > y[ind]:
-            self.is_y_min_new = True
-            self.i_min = I[ind, :] if I is not None else None
-            self.x_min = X[ind, :] if X is not None else None
-            self.y_min = y[ind]
-        else:
-            self.is_y_min_new = False
-
-        if self._log_check():
-            print(self.log())
-
-        if self.cache_m_max and len(self.cache.keys()) > self.cache_m_max:
-            self._wrn('The maximum cache size has been exceeded. Cache cleared')
-            self.cache = {}
-
-        return y if is_batch else y[0]
-
-    def _unquantize(self, I_qtt):
-        if len(I_qtt.shape) == 1:
-            is_many = False
-            I_qtt = I_qtt.reshape(1, -1)
-        else:
-            is_many = True
-
-        d = self.d
-        q = self.quantization
-        n = [2] * q
-        m = I_qtt.shape[0]
-
-        I = np.zeros((m, d), dtype=I_qtt.dtype)
-        for k in range(d):
-            I_qtt_curr = I_qtt[:, q*k:q*(k+1)].T
-            I[:, k] = np.ravel_multi_index(I_qtt_curr, n, order='F')
-
-        return I if is_many else I[0, :]
+        return np.array([self.target(x) for x in X])
 
-    def _wrn(self, text):
+    def wrn(self, text):
         text = '!!! BM-WARNING | ' + text
         print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/__init__.py` & `teneva_bm-0.5.0/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_ackley.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Ackley function (continuous).
@@ -25,71 +24,77 @@
 
         self.set_grid(-32.768, +32.768)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_a'] = self.opt_a
-        conf['opt_b'] = self.opt_b
-        conf['opt_c'] = self.opt_c
+        conf['_a'] = self._a
+        conf['_b'] = self._b
+        conf['_c'] = self._c
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param a for Ackley function              : '
-        v = self.opt_a
+        v = self._a
         text += f'{v:.6f}\n'
 
         text += 'Param b for Ackley function              : '
-        v = self.opt_b
+        v = self._b
         text += f'{v:.6f}\n'
 
         text += 'Param c for Ackley function              : '
-        v = self.opt_c
+        v = self._c
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, a=20., b=0.2, c=2.*np.pi):
-        """Setting options specific to this benchmark.
+        """Set options specific to this benchmark.
+
+        There are no plans to manually change the default values.
 
         Args:
             a (float): parameter of the function.
             b (float): parameter of the function.
             c (float): parameter of the function.
 
         """
-        self.opt_a = a
-        self.opt_b = b
-        self.opt_c = c
+        self._a = a
+        self._b = b
+        self._c = c
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         y1 = np.sqrt(np.sum(X**2, axis=1) / self.d)
-        y1 = -self.opt_a * np.exp(-self.opt_b * y1)
+        y1 = -self._a * np.exp(-self._b * y1)
 
-        y2 = np.sum(np.cos(self.opt_c * X), axis=1)
+        y2 = np.sum(np.cos(self._c * X), axis=1)
         y2 = -np.exp(y2 / self.d)
 
-        y3 = self.opt_a + np.exp(1.)
+        y3 = self._a + np.exp(1.)
 
         return y1 + y2 + y3
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_a = torch.tensor(self.opt_a)
-        par_b = torch.tensor(self.opt_b)
-        par_c = torch.tensor(self.opt_c)
+        par_a = torch.tensor(self._a)
+        par_b = torch.tensor(self._b)
+        par_c = torch.tensor(self._c)
 
         y1 = torch.sqrt(torch.sum(x**2) / d)
         y1 = - par_a * torch.exp(-par_b * y1)
 
         y2 = torch.sum(torch.cos(par_c * x))
         y2 = - torch.exp(y2 / d)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_alpine.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,32 @@
 
         self.set_grid(-10., +10.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
-    def _cores(self, X):
-        return self._cores_add([np.abs(x * (np.sin(x) + 0.1)) for x in X.T])
+    def cores(self, X):
+        return self.cores_add([np.abs(x * (np.sin(x) + 0.1)) for x in X.T])
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         return torch.sum(torch.abs(x * torch.sin(x) + 0.1 * x))
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_dixon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Analytical Dixon function (continuous).
@@ -22,33 +21,37 @@
 
 class BmFuncDixon(Bm):
     def __init__(self, d=50, n=15, name='FuncDixon', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-10., +10.)
         self.shift_grid()
-        
+
         x_min = [1.]
         for _ in range(d-1): # TODO: check this formula one more time:
             x_min.append(np.sqrt(x_min[-1]/2.))
         self.set_min(x=np.array(x_min), y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         y1 = (X[:, 0] - 1)**2
 
         y2 = np.arange(2, self.d+1) * (2. * X[:, 1:]**2 - X[:, :-1])**2
         y2 = np.sum(y2, axis=1)
 
         return y1 + y2
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
 
         y1 = (x[0] - 1)**2
         y2 = torch.arange(2, d+1) * (2. * x[1:]**2 - x[:-1])**2
         y2 = torch.sum(y2)
         return y1 + y2
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_exp.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,30 +26,34 @@
 
         self.set_grid(-1., +1.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=-1.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
-    def _cores(self, X):
-        Y = self._cores_mul([np.exp(-0.5 * x**2) for x in X.T])
+    def cores(self, X):
+        Y = self.cores_mul([np.exp(-0.5 * x**2) for x in X.T])
         Y[-1] *= -1.
         return Y
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         return -np.exp(-0.5 * np.sum(X**2, axis=1))
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         return -torch.exp(-0.5 * torch.sum(x**2))
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_griewank.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,37 +27,41 @@
 
         self.set_grid(-100., +100.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
-    def _cores(self, X):
-        Y = self._cores_mul([np.cos(x/np.sqrt(i)) for i,x in enumerate(X.T,1)])
+    def cores(self, X):
+        Y = self.cores_mul([np.cos(x/np.sqrt(i)) for i,x in enumerate(X.T,1)])
         Y[-1] *= -1
-        return teneva.add(Y, self._cores_add([x**2 / 4000. for x in X.T], a0=1))
+        return teneva.add(Y, self.cores_add([x**2 / 4000. for x in X.T], a0=1))
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         y1 = np.sum(X**2, axis=1) / 4000
 
         y2 = np.cos(X / np.sqrt(np.arange(self.d) + 1))
         y2 = - np.prod(y2, axis=1)
 
         y3 = 1.
 
         return y1 + y2 + y3
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
 
         y1 = torch.sum(x**2) / 4000
 
         y2 = torch.cos(x / torch.sqrt(torch.arange(d) + 1.))
         y2 = - torch.prod(y2)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,60 +32,66 @@
             self.set_min(x=[2.20, 1.57], y=-1.8013)
         if self.d == 5:
             self.set_min(y=-4.687658)
         if self.d == 10:
             self.set_min(y=-9.66015)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_m'] = self.opt_m
+        conf['_m'] = self._m
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param m for Michalewicz function         : '
-        v = self.opt_m
+        v = self._m
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, m=10.):
-        """Setting options specific to this benchmark.
+        """Set options specific to this benchmark.
+
+        There are no plans to manually change the default values.
 
         Args:
             m (float): parameter of the function.
 
         """
-        self.opt_m = m
+        self._m = m
 
-    def _cores(self, X):
-        Y = self._cores_add(
-            [np.sin(x) * np.sin(i*x**2/np.pi)**(2*self.opt_m)
+    def cores(self, X):
+        Y = self.cores_add(
+            [np.sin(x) * np.sin(i*x**2/np.pi)**(2*self._m)
                 for i, x in enumerate(X.T, 1)])
         Y[-1] *= -1.
         return Y
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         y1 = np.sin(((np.arange(self.d) + 1) * X**2 / np.pi))
-        y = -np.sum(np.sin(X) * y1**(2 * self.opt_m), axis=1)
+        y = -np.sum(np.sin(X) * y1**(2 * self._m), axis=1)
         return y
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_m = torch.tensor(self.opt_m)
+        par_m = torch.tensor(self._m)
         pi = torch.tensor(np.pi)
         y1 = torch.sin(((torch.arange(d) + 1) * x**2 / pi))
         y = -torch.sum(torch.sin(x) * y1**(2 * par_m))
         return y
 
 
 if __name__ == '__main__':
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_piston.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,22 @@
 
         self.set_grid(
             [30., 0.005, 0.002, 1000,  90000, 290, 340],
             [60., 0.020, 0.010, 5000, 110000, 296, 360])
         self.shift_grid()
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         _M  = X[:, 0]
         _S  = X[:, 1]
         _V0 = X[:, 2]
         _k  = X[:, 3]
         _P0 = X[:, 4]
         _Ta = X[:, 5]
         _T0 = X[:, 6]
@@ -43,15 +47,15 @@
         _A = _P0 * _S + 19.62 * _M - _k * _V0 / _S
         _Q = _P0 * _V0 / _T0
         _V = _S / 2 / _k * (np.sqrt(_A**2 + 4 * _k * _Q * _Ta) - _A)
         _C = 2 * np.pi * np.sqrt(_M / (_k + _S**2 * _Q * _Ta / _V**2))
 
         return _C
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         pi = torch.tensor(np.pi)
 
         _M  = x[0]
         _S  = x[1]
         _V0 = x[2]
         _k  = x[3]
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_qing.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,32 @@
 
         self.set_grid(0., +500.)
         self.shift_grid()
 
         self.set_min(x=np.sqrt(np.arange(1, self.d+1)), y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
-    def _cores(self, X):
-        return self._cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
+    def cores(self, X):
+        return self.cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
 
         return torch.sum((x**2 - torch.arange(1, d+1))**2)
 
 
 if __name__ == '__main__':
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,58 +25,64 @@
 
         self.set_grid(-5.12, +5.12)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_A'] = self.opt_A
+        conf['_A'] = self._A
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param A for Rastrigin function           : '
-        v = self.opt_A
+        v = self._A
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, A=10.):
-        """Setting options specific to this benchmark.
+        """Set options specific to this benchmark.
+
+        There are no plans to manually change the default values.
 
         Args:
             A (float): parameter of the function.
 
         """
-        self.opt_A = A
+        self._A = A
 
-    def _cores(self, X):
-        return self._cores_add(
-            [x**2 - self.opt_A * np.cos(2 * np.pi * x) for x in X.T],
-            a0=self.opt_A*self.d)
-
-    def _f_batch(self, X):
-        y1 = self.opt_A * self.d
-        y2 = np.sum(X**2 - self.opt_A * np.cos(2. * np.pi * X), axis=1)
+    def cores(self, X):
+        return self.cores_add(
+            [x**2 - self._A * np.cos(2 * np.pi * x) for x in X.T],
+            a0=self._A*self.d)
+
+    def target_batch(self, X):
+        y1 = self._A * self.d
+        y2 = np.sum(X**2 - self._A * np.cos(2. * np.pi * X), axis=1)
         return y1 + y2
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_A = torch.tensor(self.opt_A)
+        par_A = torch.tensor(self._A)
         pi = torch.tensor(np.pi)
 
         y1 = par_A * d
         y2 = torch.sum(x**2 - par_A * torch.cos(2. * pi * x))
 
         return y1 + y2
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,22 +27,26 @@
 
         self.set_grid(-2.048, +2.048)
         self.shift_grid()
 
         self.set_min(x=[1.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
-    def _cores(self, X):
+    def cores(self, X):
         Y = []
         for i, x in enumerate(X.T):
             x2 = x*x
             if i == 0:
                 G = np.zeros([1, len(x), 3])
                 G[0, :, 0] = 1
                 G[0, :, 1] = x2
@@ -58,20 +62,20 @@
                 G[2, :, 2] = 1.
                 G[0, :, 1] = x2
                 G[0, :, 2] = 100*x2 + 100*(x2**2) + (1-x)**2
                 G[1, :, 2] = -200*x
             Y.append(G)
         return Y
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         y1 = 100. * (X[:, 1:] - X[:, :-1]**2)**2
         y2 = (X[:, :-1] - 1.)**2
         return np.sum(y1 + y2, axis=1)
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         y1 = 100. * (x[1:] - x[:-1]**2)**2
         y2 = (x[:-1] - 1.)**2
         return torch.sum(y1 + y2)
 
 
 if __name__ == '__main__':
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 
         self.set_grid(-100., +100.)
         self.shift_grid()
 
         self.set_min(x=[0.]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         Z = X[:, :-1]**2 + X[:, 1:]**2
         Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
         return np.sum(Y, axis=1)
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         z = x[:-1]**2 + x[1:]**2
         y = 0.5 + (torch.sin(torch.sqrt(z))**2 - 0.5) / (1. + 0.001 * z)**2
         return torch.sum(y)
 
 
 if __name__ == '__main__':
```

### Comparing `teneva_bm-0.4.0/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.5.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,57 +27,63 @@
 
         self.set_grid(-500., +500.)
         self.shift_grid()
 
         self.set_min(x=[420.9687]*self.d, y=0.)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_func(self):
         return True
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_a'] = self.opt_a
+        conf['_a'] = self._a
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param a for Schwefel function            : '
-        v = self.opt_a
+        v = self._a
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, a=418.9829):
-        """Setting options specific to this benchmark.
+        """Set options specific to this benchmark.
+
+        There are no plans to manually change the default values.
 
         Args:
             a (float): parameter of the function.
 
         """
-        self.opt_a = a
+        self._a = a
 
-    def _cores(self, X):
-        return self._cores_add(
+    def cores(self, X):
+        return self.cores_add(
             [-x * np.sin(np.sqrt(np.abs(x))) for x in X.T],
-            a0=self.opt_a*self.d)
+            a0=self._a*self.d)
 
-    def _f_batch(self, X):
-        y0 = self.opt_a * self.d
+    def target_batch(self, X):
+        y0 = self._a * self.d
         return y0 - np.sum(X * np.sin(np.sqrt(np.abs(X))), axis=1)
 
-    def _f_pt(self, x):
+    def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_a = torch.tensor(self.opt_a)
+        par_a = torch.tensor(self._a)
         y0 = par_a * d
         return y0 - torch.sum(x * torch.sin(torch.sqrt(torch.abs(x))))
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,64 +2,76 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    The function 001 from the Hock & Schittkowski collection.
-    The dimension should be 2, and the mode size may be any (default is 21),
-    the default limits for function inputs are [-10, 10].
-    The exact global minimum is known: x = [1, 1], y = 0.
+    Continuous optimal control (OC) problem:
+    .-------------.
+    | F(i) -> min |
+    .-------------.
+    i - integer control
+        i[0] = 1.125 | >= 1 | <= 10
+        i[1] = 0.125 | >= 0 | <= 10
+    F - objective function
+        (i[0] + 1)^3/3 + i[1]
+    The best value is 8/3 and the corresponding solution is [1, 0].
+    The dimension d is 2, and the mode size is 21.
 """
 
 
-class BmHsFunc001(Bm):
-    def __init__(self, d=2, n=21, name='HsFunc001', desc=DESC):
+class BmHS004(Bm):
+    def __init__(self, d=3, n=21, name='hs4', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        if self.d != 2:
-            self.set_err('Dimension should be 2')
-
-        self.set_grid(-10., +10.)
+        self.set_grid([1, 0, -10], 10)
 
         self.set_min(
-            x=[1.]*self.d,
-            y=0.)
+            i=None,
+            x=np.array([1.0, 0.0, 0.0]),
+            y=8/3
+        )
 
     @property
     def is_func(self):
         return True
 
     def _f_batch(self, X):
-        return 100. * (X[:, 1] - X[:, 0]**2)**2 + (1. - X[:, 0])**2
+        y1 = (X[:, 0] + 1) ** 3
+        y = y1 / 3 + X[:, 1]
+        return y
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmHsFunc001().prep()
+    bm = BmHS004().prep()
     print(bm.info())
 
-    I_trn, y_trn = bm.build_trn(1.E+4)
-    print(bm.info_history())
+    text = 'Range of y for 10 random samples : '
+    bm.build_trn(1.E+1)
+    text += f'[{np.min(bm.y_trn):-10.3e},'
+    text += f' {np.max(bm.y_trn):-10.3e}] '
+    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
+    print(text)
 
-    text = 'Value at a random multi-index            :  '
+    text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices          :  '
+    text = 'Value at 3 random multi-indices   :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at the minimum (real vs calc)      :  '
+    text = 'Value at minimum (real vs calc)   :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
-    print(text)
+    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func006.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     The function 006 from the Hock & Schittkowski collection
@@ -16,32 +15,32 @@
 """
 
 
 class BmHsFunc006(Bm):
     def __init__(self, d=2, n=21, name='HsFunc006', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-10., +10.)
+        self.set_grid(-10., +10.) # TODO: do we need random shift?
 
         self.set_min(x=[1.]*self.d, y=0.)
 
         self.set_constr(penalty=1.E+3, eps=1.E-2, with_amplitude=True)
 
     @property
     def is_func(self):
         return True
 
     @property
     def with_constr(self):
         return True
 
-    def _c_batch(self, X):
+    def constr_batch(self, X):
         return np.abs(10. * (X[:, 1] - X[:, 0]**2))
 
-    def _f_batch(self, X):
+    def target_batch(self, X):
         return (1. - X[:, 0])**2
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmHsFunc006().prep()
```

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,49 +7,57 @@
 
 DESC = """
     Continuous optimal control (OC) problem:
     .-------------.
     | F(i) -> min |
     .-------------.
     i - integer control
-        i[0] = 1.125 | >= 1 | <= 10
-        i[1] = 0.125 | >= 0 | <= 10
+        i[0] = -3 | >= -10 | <= 10
+        i[1] = -1 | >= -10 | <= 10
+        i[2] = -3 | >= -10 | <= 10
+        i[3] = -1 | >= -10 | <= 10
     F - objective function
-        (i[0] + 1)^3/3 + i[1]
-    The best value is 8/3 and the corresponding solution is [1, 0].
-    The dimension d is 2, and the mode size is 21.
+        100 * (i[1] - i[0]^2)^2 + (1 - i[0])^2 +  
+        90 * (i[3] - i[2]^2)^2 + (1 - i[2])^2 + 
+        10.1 * ((i[1] - 1)^2 + (i[3] - 1)^2) + 
+        19.8 * (i[1] - 1) * (i[3] - 1)
+    The best value is 0 and the corresponding solution is [1, 1, 1, 1]
+    The dimension d is 4, and the mode size is 21.
 """
 
 
-class BmHS004(Bm):
-    def __init__(self, d=3, n=21, name='hs4', desc=DESC):
+class BmHS038(Bm):
+    def __init__(self, d=4, n=21, name='hs38', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid([1, 0, -10], 10)
+        self.set_grid(-10, 10)
 
         self.set_min(
             i=None,
-            x=np.array([1.0, 0.0, 0.0]),
-            y=8/3
+            x=np.array([0]*self.d),
+            y=0
         )
 
     @property
     def is_func(self):
         return True
 
     def _f_batch(self, X):
-        y1 = (X[:, 0] + 1) ** 3
-        y = y1 / 3 + X[:, 1]
+        y1 = 100 * (X[:, 1] - X[:, 0] ** 2) ** 2 + (1 - X[:, 0]) ** 2
+        y2 = 90 * (X[:, 3] - X[:, 2] ** 2) ** 2 + (1 - X[:, 2]) ** 2
+        y3 = 10.1 * ((X[:, 1] - 1) ** 2 + (X[:, 3] - 1) ** 2) 
+        y4 = 19.8 * (X[:, 1] - 1) * (X[:, 3] - 1)
+        y = y1 + y2 + y3 + y4
         return y
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmHS004().prep()
+    bm = BmHS038().prep()
     print(bm.info())
 
     text = 'Range of y for 10 random samples : '
     bm.build_trn(1.E+1)
     text += f'[{np.min(bm.y_trn):-10.3e},'
     text += f' {np.max(bm.y_trn):-10.3e}] '
     text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
@@ -70,8 +78,8 @@
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
     text = 'Value at minimum (real vs calc)   :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
     text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
-    print(text)
+    print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.5.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,57 +7,51 @@
 
 DESC = """
     Continuous optimal control (OC) problem:
     .-------------.
     | F(i) -> min |
     .-------------.
     i - integer control
-        i[0] = -3 | >= -10 | <= 10
-        i[1] = -1 | >= -10 | <= 10
-        i[2] = -3 | >= -10 | <= 10
-        i[3] = -1 | >= -10 | <= 10
+        i[0] = 0 | >= 0 | <= 1
+        i[1] = 0 | >= 0 | <= 2
+        i[2] = 0 | >= 0 | <= 3
+        i[3] = 0 | >= 0 | <= 4
+        i[4] = 0 | >= 0 | <= 5
     F - objective function
-        100 * (i[1] - i[0]^2)^2 + (1 - i[0])^2 +  
-        90 * (i[3] - i[2]^2)^2 + (1 - i[2])^2 + 
-        10.1 * ((i[1] - 1)^2 + (i[3] - 1)^2) + 
-        19.8 * (i[1] - 1) * (i[3] - 1)
-    The best value is 0 and the corresponding solution is [1, 1, 1, 1]
-    The dimension d is 4, and the mode size is 21.
+        2 - i[0] * i[1] * i[2] * i[3] * i[4] / 120
+    The best value is 1 and the corresponding solution is [1, 2, 3, 4, 5]
+    The dimension d is 5, and the mode size is 21.
 """
 
 
-class BmHS038(Bm):
-    def __init__(self, d=4, n=21, name='hs38', desc=DESC):
+class BmHS045(Bm):
+    def __init__(self, d=5, n=21, name='hs45', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-10, 10)
+        self.set_grid(0, [1, 2, 3, 4, 5])
 
         self.set_min(
             i=None,
-            x=np.array([0]*self.d),
-            y=0
+            x=np.array([1, 2, 3, 4, 5]),
+            y=1
         )
 
     @property
     def is_func(self):
         return True
 
     def _f_batch(self, X):
-        y1 = 100 * (X[:, 1] - X[:, 0] ** 2) ** 2 + (1 - X[:, 0]) ** 2
-        y2 = 90 * (X[:, 3] - X[:, 2] ** 2) ** 2 + (1 - X[:, 2]) ** 2
-        y3 = 10.1 * ((X[:, 1] - 1) ** 2 + (X[:, 3] - 1) ** 2) 
-        y4 = 19.8 * (X[:, 1] - 1) * (X[:, 3] - 1)
-        y = y1 + y2 + y3 + y4
+        y = 2 - X.prod(axis=-1) / 120
         return y
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmHS038().prep()
+    bm = BmHS045().prep()
     print(bm.info())
 
     text = 'Range of y for 10 random samples : '
     bm.build_trn(1.E+1)
     text += f'[{np.min(bm.y_trn):-10.3e},'
     text += f' {np.max(bm.y_trn):-10.3e}] '
     text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
```

### Comparing `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.5.0/teneva_bm/hs/bm_hs_func001.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,62 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Continuous optimal control (OC) problem:
-    .-------------.
-    | F(i) -> min |
-    .-------------.
-    i - integer control
-        i[0] = 0 | >= 0 | <= 1
-        i[1] = 0 | >= 0 | <= 2
-        i[2] = 0 | >= 0 | <= 3
-        i[3] = 0 | >= 0 | <= 4
-        i[4] = 0 | >= 0 | <= 5
-    F - objective function
-        2 - i[0] * i[1] * i[2] * i[3] * i[4] / 120
-    The best value is 1 and the corresponding solution is [1, 2, 3, 4, 5]
-    The dimension d is 5, and the mode size is 21.
+    The function 001 from the Hock & Schittkowski collection.
+    The dimension should be 2, and the mode size may be any (default is 21),
+    the default limits for function inputs are [-10, 10].
+    The exact global minimum is known: x = [1, 1], y = 0.
 """
 
 
-class BmHS045(Bm):
-    def __init__(self, d=5, n=21, name='hs45', desc=DESC):
+class BmHsFunc001(Bm):
+    def __init__(self, d=2, n=21, name='HsFunc001', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(0, [1, 2, 3, 4, 5])
+        if self.d != 2:
+            self.set_err('Dimension should be 2')
 
-        self.set_min(
-            i=None,
-            x=np.array([1, 2, 3, 4, 5]),
-            y=1
-        )
+        self.set_grid(-10., +10.) # TODO: do we need random shift?
+
+        self.set_min(x=[1.]*self.d, y=0.)
 
     @property
     def is_func(self):
         return True
 
-    def _f_batch(self, X):
-        y = 2 - X.prod(axis=-1) / 120
-        return y
+    def target_batch(self, X):
+        return 100. * (X[:, 1] - X[:, 0]**2)**2 + (1. - X[:, 0])**2
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmHS045().prep()
+    bm = BmHsFunc001().prep()
     print(bm.info())
 
-    text = 'Range of y for 10 random samples : '
-    bm.build_trn(1.E+1)
-    text += f'[{np.min(bm.y_trn):-10.3e},'
-    text += f' {np.max(bm.y_trn):-10.3e}] '
-    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
-    print(text)
+    I_trn, y_trn = bm.build_trn(1.E+4)
+    print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at minimum (real vs calc)   :  '
+    text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
     y_calc = bm(bm.x_min_real)
-    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
+    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple.py` & `teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 try:
     from gekko import GEKKO
     with_gekko = True
 except Exception as e:
     with_gekko = False
@@ -28,97 +27,100 @@
 
 class BmOcSimple(Bm):
     def __init__(self, d=50, n=2, name='OcSimple', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n[0] != 2:
             self.set_err('Mode size (n) should be "2"')
+
         if not with_gekko:
             msg = 'Need "gekko" module. For installation please run '
             msg += '"pip install gekko==1.0.6"'
             self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
-    def bm_ode(self, x, i):
-        """Target ordinary differential equation (ODE)."""
-        return x**3 - i
-
-    def bm_obj(self, x, i):
-        """Objective function for ODE solution."""
-        return 0.5 * (x - self.opt_x_ref)**2
-
     def get_config(self):
         conf = super().get_config()
-        conf['opt_x_ini'] = self.opt_x_ini
-        conf['opt_x_ref'] = self.opt_x_ref
-        conf['opt_t_max'] = self.opt_t_max
-        conf['opt_y_err'] = self.opt_y_err
+        conf['_x_ini'] = self._x_ini
+        conf['_x_ref'] = self._x_ref
+        conf['_t_max'] = self._t_max
+        conf['_y_err'] = self._y_err
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param x_ini (initial condition)          : '
-        v = self.opt_x_ini
+        v = self._x_ini
         text += f'{v:.6f}\n'
 
         text += 'Param x_ref (target value)               : '
-        v = self.opt_x_ref
+        v = self._x_ref
         text += f'{v:.6f}\n'
 
         text += 'Param t_max (upper limit for time)       : '
-        v = self.opt_t_max
+        v = self._t_max
         text += f'{v:.6f}\n'
 
         text += 'Param y_err (returned value if error)    : '
-        v = self.opt_y_err
+        v = self._y_err
         text += f'{v:-7.1e}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, x_ini=0.8, x_ref=0.7, t_max=1., y_err=1.E+50):
-        """Setting options specific to the benchmark.
+        """Set options specific to the benchmark.
+
+        There are no plans to manually change the default values.
 
         Args:
             x_ini (float): initial condition for the ODE.
             x_ref (float): target (reference) value for solution of the ODE.
             t_max (float): upper limit for time variable in the ODE.
             y_err (float): returned value if GEKKO solver ends with error.
 
         """
-        self.opt_x_ini = x_ini
-        self.opt_x_ref = x_ref
-        self.opt_t_max = t_max
-        self.opt_y_err = y_err
+        self._x_ini = x_ini
+        self._x_ref = x_ref
+        self._t_max = t_max
+        self._y_err = y_err
 
-        self._opt_times = np.linspace(0, t_max, self.d)
+        self._times = np.linspace(0, t_max, self.d)
 
-    def _f(self, i):
+    def target(self, i):
         solver = GEKKO(remote=False)
         solver.options.IMODE = 4
-        solver.time = self._opt_times
+        solver.time = self._times
 
-        x = solver.Var(value=self.opt_x_ini, name='x')
+        x = solver.Var(value=self._x_ini, name='x')
         c = solver.Param(list(i), name='i')
         y = solver.Var(value=0.)
 
-        solver.Equation(x.dt() == self.bm_ode(x, c))
-        solver.Equation(y == self.bm_obj(x, c))
+        solver.Equation(x.dt() == self._ode(x, c))
+        solver.Equation(y == self._obj(x, c))
 
         try:
             solver.solve(disp=False)
             y = sum(y.VALUE)
         except Exception as e:
-            y = self.opt_y_err
+            y = self._y_err
 
         return y
 
+    def _ode(self, x, i):
+        """Target ordinary differential equation (ODE)."""
+        return x**3 - i
+
+    def _obj(self, x, i):
+        """Objective function for ODE solution."""
+        return 0.5 * (x - self._x_ref)**2
+
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmOcSimple().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple_constr.py` & `teneva_bm-0.5.0/teneva_bm/oc/bm_oc_simple_constr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm.oc import BmOcSimple
 
 
 DESC = """
     Discrete optimal control (OC) problem with constraint of the special
@@ -22,15 +21,15 @@
 
         self.set_constr(penalty=1.E+42, with_amplitude=True)
 
     @property
     def with_constr(self):
         return True
 
-    def _c(self, i):
+    def constr(self, i):
         s = ''.join([str(k) for k in i])
 
         condition_false = False
         condition_false = condition_false or s.startswith('10')
         condition_false = condition_false or s.startswith('110')
         condition_false = condition_false or s.startswith('01')
         condition_false = condition_false or s.startswith('011')
```

### Comparing `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Binary knapsack problem -1 * sum p_i x_i -> min s.t. sum w_i x_i < C with
@@ -24,146 +23,146 @@
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if self.d == 10:
             i = [0, 1, 1, 1, 0, 0, 0, 1, 1, 1]
             self.set_min(i=i, y=-295)
+
         elif self.d == 20:
             i = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1, 1]
             self.set_min(i=i, y=-1024)
+
         elif self.d == 50:
             i = [1, 1, 0, 1, 0, 1, 0, 1, 1, 1, 1, 0, 1, 1, 0, 1, 1, 0, 1, 1, 0,
                  1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 1, 0,
                  0, 0, 0, 0, 1, 0, 0, 0]
             self.set_min(i=i, y=-3103.)
+
         elif self.d == 80:
             i = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
                  1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 0, 0, 1, 0, 0, 0,
                  1, 0, 1, 1, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0,
                  0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
             self.set_min(i=i, y=-5183)
+
         elif self.d == 100:
             i = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
                  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
                  1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
                  1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1,
                  1, 0, 1, 0, 0, 0, 1, 1, 0, 0, 0, 1, 1, 0, 1, 0]
             self.set_min(i=i, y=-15170)
+
         else:
             self.set_err('Dimension should be in 10, 20, 50, 80, 100')
 
         self.set_constr(penalty=0.)
 
     @property
     def is_tens(self):
         return True
 
     @property
     def with_constr(self):
         return True
 
-    def prep(self):
-        self.check_err()
+    def constr(self, i):
+        return np.dot(self._w, i) - self._C
 
+    def prep_bm(self):
         if self.d == 10:
-            self.prep_10()
+            self._prep_10()
         elif self.d == 20:
-            self.prep_20()
+            self._prep_20()
         elif self.d == 50:
-            self.prep_50()
+            self._prep_50()
         elif self.d == 80:
-            self.prep_80()
+            self._prep_80()
         elif self.d == 100:
-            self.prep_100()
+            self._prep_100()
 
-        self.bm_w = np.array(self.bm_w)
-        self.bm_p = np.array(self.bm_p)
+        self._w = np.array(self._w)
+        self._p = np.array(self._p)
 
-        self.is_prep = True
-        return self
+    def target(self, i):
+        return -np.dot(self._p, i)
 
-    def prep_10(self):
-        self.bm_w = [
+    def _prep_10(self):
+        self._w = [
             95, 4, 60, 32, 23, 72, 80, 62, 65, 46]
 
-        self.bm_p = [
+        self._p = [
             55, 10, 47, 5, 4, 50, 8, 61, 85, 87]
 
-        self.bm_C = 269
+        self._C = 269
 
-    def prep_20(self):
-        self.bm_w = [
+    def _prep_20(self):
+        self._w = [
             92, 4, 43, 83, 84, 68, 92, 82, 6, 44, 32, 18, 56, 83, 25, 96, 70,
             48, 14, 58]
 
-        self.bm_p = [
+        self._p = [
             44, 46, 90, 72, 91, 40, 75, 35, 8, 54, 78, 40, 77, 15, 61, 17, 75,
             29, 75, 63]
 
-        self.bm_C = 878
+        self._C = 878
 
-    def prep_50(self):
-        self.bm_w = [
+    def _prep_50(self):
+        self._w = [
             80, 82, 85, 70, 72, 70, 66, 50, 55, 25, 50, 55, 40, 48, 59, 32, 22,
             60, 30, 32, 40, 38, 35, 32, 25, 28, 30, 22, 50, 30, 45, 30, 60, 50,
             20, 65, 20, 25, 30, 10, 20, 25, 15, 10, 10, 10, 4, 4, 2, 1]
 
-        self.bm_p = [
+        self._p = [
             220, 208, 198, 192, 180, 180, 165, 162, 160, 158, 155, 130, 125,
             122, 120, 118, 115, 110, 105, 101, 100, 100, 98, 96, 95, 90, 88, 82,
             80, 77, 75, 73, 72, 70, 69, 66, 65, 63, 60, 58, 56, 50, 30, 20, 15,
             10, 8, 5, 3, 1]
 
-        self.bm_C = 1000
+        self._C = 1000
 
-    def prep_80(self):
-        self.bm_w = [
+    def _prep_80(self):
+        self._w = [
             40, 27, 5, 21, 51, 16, 42, 18, 52, 28, 57, 34, 44, 43, 52, 55,
             53, 42, 47, 56, 57, 44, 16, 2, 12, 9, 40, 23, 56, 3, 39, 16,
             54, 36, 52, 5, 53, 48, 23, 47, 41, 49, 22, 42, 10, 16, 53, 58,
             40, 1, 43, 56, 40, 32, 44, 35, 37, 45, 52, 56, 40, 2, 23,49, 50,
             26, 11, 35, 32, 34, 58, 6, 52, 26, 31, 23, 4, 52, 53, 19]
 
-        self.bm_p = [
+        self._p = [
             199, 194, 193, 191, 189, 178, 174, 169, 164, 164, 161, 158, 157,
             154, 152, 152, 149, 142, 131, 125, 124, 124, 124, 122, 119, 116,
             114, 113, 111, 110, 109, 100, 97, 94, 91, 82, 82, 81, 80, 80, 80,
             79, 77, 76, 74, 72, 71, 70, 69,68, 65, 65, 61, 56, 55, 54, 53, 47,
             47, 46, 41, 36, 34, 32, 32,30, 29, 29, 26, 25, 23, 22, 20, 11, 10,
             9, 5, 4, 3, 1]
 
-        self.bm_C = 1173
+        self._C = 1173
 
-    def prep_100(self):
-        self.bm_w = [
+    def _prep_100(self):
+        self._w = [
             54, 95, 36, 18, 4, 71, 83, 16, 27, 84, 88, 45, 94, 64, 14, 80,
             4, 23, 75, 36, 90, 20, 77, 32, 58, 6, 14, 86, 84, 59, 71, 21, 30,
             22, 96, 49, 81, 48, 37, 28, 6, 84, 19, 55, 88, 38, 51, 52, 79, 55,
             70, 53, 64, 99, 61, 86, 1, 64, 32, 60, 42, 45, 34, 22, 49, 37, 33,
             1, 78, 43, 85, 24, 96, 32, 99, 57, 23, 8, 10, 74, 59, 89, 95, 40,
             46, 65, 6, 89, 84, 83, 6, 19, 45, 59, 26, 13, 8, 26, 5, 9]
 
-        self.bm_p = [
+        self._p = [
             297, 295, 293, 292, 291, 289, 284, 284, 283, 283, 281, 280, 279,
             277, 276, 275, 273,264, 260, 257, 250, 236, 236, 235, 235, 233,
             232, 232, 228, 218, 217, 214, 211, 208, 205, 204, 203, 201, 196,
             194, 193, 193, 192, 191, 190, 187, 187, 184, 184, 184, 181, 179,
             176, 173, 172, 171, 160, 128, 123, 114, 113, 107, 105, 101, 100,
             100, 99, 98, 97, 94, 94, 93, 91, 80, 74, 73, 72, 63, 63, 62, 61,
             60, 56, 53, 52, 50, 48, 46, 40, 40, 35, 28, 22, 22, 18, 15, 12,
             11, 6, 5]
 
-        self.bm_C = 3818
-
-    def _c(self, i):
-        return np.dot(self.bm_w, i) - self.bm_C
-
-    def _f(self, i):
-        return -np.dot(self.bm_p, i)
+        self._C = 3818
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboKnapDet().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 try:
     import qubogen
     with_qubogen = True
 except Exception as e:
     with_qubogen = False
@@ -22,36 +21,36 @@
 
 class BmQuboKnapQuad(Bm):
     def __init__(self, d=50, n=2, name='QuboKnapQuad', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
+
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_tens(self):
         return True
 
-    def prep(self):
-        self.check_err()
-
+    def prep_bm(self):
         v = np.diag(self.rand.random(self.d)) / 3.
         a = self.rand.random(self.d)
         b = np.mean(a)
-        self.bm_Q = qubogen.qubo_qkp(v, a, b)
-
-        self.is_prep = True
-        return self
+        self._Q = qubogen.qubo_qkp(v, a, b)
 
-    def _f_batch(self, I):
-        return ((I @ self.bm_Q) * I).sum(axis=1)
+    def target_batch(self, I):
+        return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboKnapQuad().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 try:
     import networkx as nx
     with_networkx = True
 except Exception as e:
     with_networkx = False
@@ -29,67 +28,70 @@
 
 class BmQuboMaxcut(Bm):
     def __init__(self, d=50, n=2, name='QuboMaxcut', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
+
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
             msg += '"pip install networkx==3.0"'
             self.set_err(msg)
+
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_prob_con'] = self.opt_prob_con
+        conf['_prob_con'] = self._prob_con
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param prob_con (connection probability)  : '
-        v = self.opt_prob_con
+        v = self._prob_con
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def prep(self):
-        self.check_err()
-
+    def prep_bm(self):
         d = self.d
-        p = self.opt_prob_con
+        p = self._prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self.bm_Q = qubogen.qubo_max_cut(g)
-
-        self.is_prep = True
-        return self
+        self._Q = qubogen.qubo_max_cut(g)
 
     def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
+        There are no plans to manually change the default values.
+
         Args:
             prob_con (float): probability of the connection in the graph.
 
         """
-        self.opt_prob_con = prob_con
+        self._prob_con = prob_con
 
-    def _f_batch(self, I):
-        return ((I @ self.bm_Q) * I).sum(axis=1)
+    def target_batch(self, I):
+        return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboMaxcut().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.5.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 try:
     import networkx as nx
     with_networkx = True
 except Exception as e:
     with_networkx = False
@@ -29,67 +28,70 @@
 
 class BmQuboMvc(Bm):
     def __init__(self, d=50, n=2, name='QuboMVC', desc=DESC):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
+
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
             msg += '"pip install networkx==3.0"'
             self.set_err(msg)
+
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
+    def identity(self):
+        return super().identity + ['seed']
+
+    @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_prob_con'] = self.opt_prob_con
+        conf['_prob_con'] = self._prob_con
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param prob_con (connection probability)  : '
-        v = self.opt_prob_con
+        v = self._prob_con
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def prep(self):
-        self.check_err()
-
+    def prep_bm(self):
         d = self.d
-        p = self.opt_prob_con
+        p = self._prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
-        self.bm_Q = qubogen.qubo_mvc(g)
-
-        self.is_prep = True
-        return self
+        self._Q = qubogen.qubo_mvc(g)
 
     def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
+        There are no plans to manually change the default values.
+
         Args:
             prob_con (float): probability of the connection in the graph.
 
         """
-        self.opt_prob_con = prob_con
+        self._prob_con = prob_con
 
-    def _f_batch(self, I):
-        return ((I @ self.bm_Q) * I).sum(axis=1)
+    def target_batch(self, I):
+        return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmQuboMvc().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.4.0/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.5.0/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.4.0/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.5.0/teneva_bm/various/bm_matmul.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Problem for fast "size x size" matrix multiplication (like Strassen
@@ -64,70 +63,69 @@
 
                 2, 1, 1, 2, 0, 1, 2,
                 1, 1, 2, 1, 2, 1, 1,
                 1, 2, 1, 2, 1, 1, 1,
                 2, 0, 2, 1, 1, 2, 1]
             self.set_min(i=i, y=0.)
 
-        self.bm_T = T_real
-        self.bm_E = E
+        self._T = T_real
+        self._E = E
 
-        self.opt_size = size
-        self.opt_rank = rank
-        self.opt_only2 = only2
+        self._size = size
+        self._rank = rank
+        self._only2 = only2
+
+    @property
+    def identity(self):
+        return ['_size', '_rank', '_only2']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_size'] = self.opt_size
-        conf['opt_rank'] = self.opt_rank
-        conf['opt_only2'] = self.opt_only2
+        conf['_size'] = self._size
+        conf['_rank'] = self._rank
+        conf['_only2'] = self._only2
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param size (sizes of the matrices)       : '
-        v = self.opt_size
+        v = self._size
         text += f'{v:.0f}\n'
 
         text += 'Param rank (search rank for CP-decomp.)  : '
-        v = self.opt_rank
+        v = self._rank
         text += f'{v:.0f}\n'
 
         text += 'Param only2 (if True, use 2 CP-factors)  : '
-        v = 'YES' if self.opt_only2 else 'no'
+        v = 'YES' if self._only2 else 'no'
         text += f'{v}\n'
 
         return super().info(text+footer)
 
-    def prep(self):
-        self.check_err()
-
-        self.loss = _loss_build(self.bm_T, self.bm_E, self.opt_rank,
-            self.opt_only2)
-
-        self.is_prep = True
-        return self
-
-    def recover(self, i):
-        x = _ind_to_poi(i, self.bm_E)
+    def prep_bm(self):
+        self.loss = _loss_build(self._T, self._E, self._rank, self._only2)
 
-        if self.opt_only2:
-            U, V = _factor_from_poi(x, self.opt_rank, True)
-            W = _factor_recover(U, V, self.bm_T)
+    def recover(self, i=None, best=True):
+        i, y = self.get_solution(i, best)
+        x = _ind_to_poi(i, self._E)
+
+        if self._only2:
+            U, V = _factor_from_poi(x, self._rank, True)
+            W = _factor_recover(U, V, self._T)
         else:
-            U, V, W = _factor_from_poi(x, self.opt_rank, False)
+            U, V, W = _factor_from_poi(x, self._rank, False)
 
         return U, V, W
 
-    def _f(self, i):
+    def target(self, i):
         return self.loss(i)
 
 
 def _factor_from_poi(x, rank, only2=False, order_spec=False):
     """Build canonical rank-"rank" factors from flatten "x"."""
     k = 2 if only2 else 3
     n = x.size // (k * rank)
@@ -229,15 +227,15 @@
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    if bm.opt_size == 2 and bm.n0 == 3:
+    if bm._size == 2 and bm.n0 == 3:
         text = 'Value at the minimum (real vs calc)      :  '
         y_real = bm.y_min_real
         y_calc = bm[bm.i_min_real]
         text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
         print(text)
 
     text = 'Check "only2" case                       :  '
@@ -247,10 +245,10 @@
     text += f'{y:-10.3e}'
     print(text)
 
     text = 'Check "recover" error                    :  '
     bm = BmMatmul(size=2, rank=7).prep()
     U, V, W = bm.recover(bm.i_min_real)
     T_appr = np.einsum('nr,mr,sr->nms', U, V, W)
-    e = np.linalg.norm(T_appr.reshape(-1) - bm.bm_T.reshape(-1))
+    e = np.linalg.norm(T_appr.reshape(-1) - bm._T.reshape(-1))
     text += f'{e:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.5.0/teneva_bm/various/bm_topopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.sparse import coo_matrix
 from scipy.sparse.linalg import spsolve
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Discrete Topology optimization task. This is a draft!!!
@@ -16,211 +15,112 @@
 
 class BmTopopt(Bm):
     def __init__(self, d=None, n=2, name='BmTopopt', desc=DESC, nx=128, ny=32):
         super().__init__(nx*ny, n, name, desc)
 
         if d is not None:
             self.set_err('Dimension number (d) should not be set manually')
+
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
-        self.opt_nx = nx
-        self.opt_ny = ny
+        self._nx = nx
+        self._ny = ny
+
+    @property
+    def identity(self):
+        return ['_nx', '_ny']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['opt_nx'] = self.opt_nx
-        conf['opt_ny'] = self.opt_ny
-        conf['opt_k_frac'] = self.opt_k_frac
-        conf['opt_penal'] = self.opt_penal
-        conf['opt_rmin'] = self.opt_rmin
+        conf['_nx'] = self._nx
+        conf['_ny'] = self._ny
+        conf['_k_frac'] = self._k_frac
+        conf['_penal'] = self._penal
+        conf['_rmin'] = self._rmin
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param nx (grid x-size)                   : '
-        v = self.opt_nx
+        v = self._nx
         text += f'{v:.0f}\n'
 
         text += 'Param ny (grid y-size)                   : '
-        v = self.opt_ny
+        v = self._ny
         text += f'{v:.0f}\n'
 
         text += 'Param k_frac for Topopt                  : '
-        v = self.opt_k_frac
+        v = self._k_frac
         text += f'{v:.6f}\n'
 
         text += 'Param penal for Topopt                   : '
-        v = self.opt_penal
+        v = self._penal
         text += f'{v:.6f}\n'
 
         text += 'Param rmin for Topopt                    : '
-        v = self.opt_rmin
+        v = self._rmin
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def optimize_baseline(self):
-        solver = TopOptLite(self.opt_nx, self.opt_ny, self.opt_penal,
-            self.opt_rmin)
-        solver.init(Emin=1.E-9, Emax=1.0)
-        solver.prep()
-        x_ini = self.opt_k_frac * np.ones(self.opt_nx * self.opt_ny,
-            dtype=float)
-        x_opt = solver.solve(x_ini)
-        return x_opt
-
-    def plot(self, x, name='solver', fpath=None):
-        fig, ax = plt.subplots(1, 1, figsize=(21, 7))
-        x = x.reshape(self.opt_nx, self.opt_ny).T
-        ax.imshow(x, cmap='gray', interpolation='none')
-
-        k_frac_real = np.sum(x) / np.size(x)
-
-        title = 'Result for ' + name + '. '
-        title += f'Shape: {x.shape[0]} x {x.shape[1]}. '
-        title += f'Frac: {k_frac_real:.2f} ({self.opt_k_frac:.2f}). '
-        fig.suptitle(title, fontsize=18)
-
-        if fpath:
-            plt.savefig(fpath, bbox_inches='tight')
-        else:
-            plt.show()
-
-    def prep(self):
-        self.check_err()
-
-        self.bm_f = topopt_lite(self.opt_nx, self.opt_ny,
-            self.opt_k_frac, self.opt_penal, self.opt_rmin)
-
-        self.is_prep = True
-        return self
+    def prep_bm(self):
+        self._solver = _topopt_lite(self._nx, self._ny,
+            self._k_frac, self._penal, self._rmin)
 
     def set_opts(self, k_frac=0.4, penal=3., rmin=5.4):
         """Setting options specific to this benchmark.
 
+        There are no plans to manually change the default values.
+
         Args:
             k_frac (float): ?.
             penal (float): ?.
             rmin (float): ?.
 
         """
-        self.opt_k_frac = k_frac
-        self.opt_penal = penal
-        self.opt_rmin = rmin
-
-    def _f(self, i):
-        return self.bm_f(i)
-
-
-def topopt_lite(nelx, nely, volfrac, penal, rmin, ft=1):
-    Emin = 1.E-9
-    Emax = 1.0
-    ndof = 2 * (nelx+1) * (nely+1)
-
-    # FE: Build the index vectors for the for coo matrix format.
-    KE = lk()
-    edofMat = np.zeros((nelx*nely, 8), dtype=int)
-    for elx in range(nelx):
-        for ely in range(nely):
-            el = ely + elx*nely
-            n1 = (nely+1)*elx + ely
-            n2 = (nely+1)*(elx+1) + ely
-            edofMat[el, :]= np.array(
-                [2*n1+2, 2*n1+3, 2*n2+2, 2*n2+3,2*n2, 2*n2+1, 2*n1, 2*n1+1])
-
-    # Construct the index pointers for the coo format:
-    iK = np.kron(edofMat,np.ones((8,1))).flatten()
-    jK = np.kron(edofMat,np.ones((1,8))).flatten()
-
-    # Filter: Build and assemble the index+data vectors for the coo matrix:
-    nfilter = int(nelx*nely*((2*(np.ceil(rmin)-1)+1)**2))
-    iH = np.zeros(nfilter)
-    jH = np.zeros(nfilter)
-    sH = np.zeros(nfilter)
-    cc = 0
-    for i in range(nelx):
-        for j in range(nely):
-            row = i*nely + j
-            kk1 = int(np.maximum(i - (np.ceil(rmin)-1), 0))
-            kk2 = int(np.minimum(i + np.ceil(rmin), nelx))
-            ll1 = int(np.maximum(j - (np.ceil(rmin)-1), 0))
-            ll2 = int(np.minimum(j + np.ceil(rmin), nely))
-            for k in range(kk1, kk2):
-                for l in range(ll1, ll2):
-                    col = k*nely + l
-                    fac = rmin - np.sqrt(((i-k)*(i-k)+(j-l)*(j-l)))
-                    iH[cc] = row
-                    jH[cc] = col
-                    sH[cc] = np.maximum(0., fac)
-                    cc = cc + 1
-
-    # Finalize assembly and convert to csc format:
-    H = coo_matrix((sH, (iH, jH)), shape=(nelx*nely, nelx*nely)).tocsc()
-    Hs = H.sum(1)
-
-    # BC's and support:
-    dofs = np.arange(2*(nelx+1)*(nely+1))
-    fixed = np.union1d(dofs[0:2*(nely+1):2], np.array([2*(nelx+1)*(nely+1)-1]))
-    free = np.setdiff1d(dofs, fixed)
-
-    # Solution and RHS vectors:
-    f = np.zeros((ndof, 1))
-    u = np.zeros((ndof, 1))
-
-    # Set load:
-    f[1, 0] = -1
-
-    def f_loss(x):
-
-        # Filter design variables:
-        xPhys = np.asarray(H * x[np.newaxis].T / Hs)[:, 0] if ft == 1 else x
+        self._k_frac = k_frac
+        self._penal = penal
+        self._rmin = rmin
 
-        # Setup and solve FE problem:
-        sK = ((KE.flatten()[np.newaxis]).T*(Emin+(xPhys)**penal*(Emax-Emin)))
-        sK = sK.flatten(order='F')
-        K = coo_matrix((sK, (iK, jK)), shape=(ndof, ndof)).tocsc()
+    def show(self, fpath=None, i=None, best=True):
+        i, y = self.get_solution(i, best)
 
-        # Remove constrained dofs from matrix:
-        K = K[free, :][:, free]
+        x = i.reshape(self._nx, self._ny).T
 
-        # Solve system:
-        u[free, 0] = spsolve(K, f[free, 0])
+        fig, ax = plt.subplots(1, 1, figsize=(21, 7))
+        ax.imshow(x, cmap='gray', interpolation='none')
 
-        # Objective and sensitivity:
-        ce = np.dot(u[edofMat].reshape(nelx*nely, 8), KE)
-        ce *= u[edofMat].reshape(nelx*nely, 8)
-        ce = ce.sum(1)
-        obj = Emin + (Emax - Emin) * xPhys**penal
-        obj = (obj * ce).sum()
-        return obj
+        k_frac_real = np.sum(x) / np.size(x)
 
-    return f_loss
+        title = ''
+        title += f'Shape: {x.shape[0]} x {x.shape[1]}. '
+        title += f'Frac: {k_frac_real:.2f} ({self._k_frac:.2f}). '
+        title += f'Value: {y:.2f}.'
+        fig.suptitle(title, fontsize=18)
 
+        fpath = self.path_build(fpath, 'png')
+        plt.savefig(fpath, bbox_inches='tight') if fpath else plt.show()
 
-def lk(E=1, nu=0.3):
-    """Element stiffness matrix."""
-    k = np.array([
-        1/2-nu/6, 1/8+nu/8, -1/4-nu/12, -1/8+3*nu/8,
-        -1/4+nu/12, -1/8-nu/8, nu/6, 1/8-3*nu/8])
+    def target(self, i):
+        return self._solver(i)
 
-    return E / (1-nu**2) * np.array([
-        [k[0], k[1], k[2], k[3], k[4], k[5], k[6], k[7]],
-        [k[1], k[0], k[7], k[6], k[5], k[4], k[3], k[2]],
-        [k[2], k[7], k[0], k[5], k[6], k[3], k[4], k[1]],
-        [k[3], k[6], k[5], k[0], k[7], k[2], k[1], k[4]],
-        [k[4], k[5], k[6], k[7], k[0], k[1], k[2], k[3]],
-        [k[5], k[4], k[3], k[2], k[1], k[0], k[7], k[6]],
-        [k[6], k[3], k[4], k[1], k[2], k[7], k[0], k[5]],
-        [k[7], k[2], k[1], k[4], k[3], k[6], k[5], k[0]]])
+    def _optimize_baseline(self):
+        """Draft!"""
+        solver = TopOptLite(self._nx, self._ny, self._penal, self._rmin)
+        solver.init(Emin=1.E-9, Emax=1.0)
+        solver.prep()
+        x_ini = self._k_frac * np.ones(self._nx * self._ny, dtype=float)
+        x_opt = solver.solve(x_ini)
+        return x_opt
 
 
 class TopOptLite:
     def __init__(self, nx, ny, penal, rmin):
         self.nx = nx
         self.ny = ny
         self.penal = penal
@@ -236,16 +136,16 @@
         # Load (RHS vector):
         self.f = np.zeros((self.ndof, 1))
         self.f[1, 0] = -1
 
         return self
 
     def prep(self):
-        self.edofMat = edof_matrix(self.nx, self.ny)
-        self.KE = stiffness_matrix()
+        self.edofMat = _edof_matrix(self.nx, self.ny)
+        self.KE = _stiffness_matrix()
         self.iK = np.kron(self.edofMat, np.ones((8,1))).flatten()
         self.jK = np.kron(self.edofMat, np.ones((1,8))).flatten()
 
         # Filter: Build and assemble the index+data vectors for the coo matrix:
         nfilter = int(self.n*((2*(np.ceil(self.rmin)-1)+1)**2))
         iH = np.zeros(nfilter)
         jH = np.zeros(nfilter)
@@ -337,27 +237,44 @@
                 l1 = lmid
             else:
                 l2 = lmid
 
         return xnew
 
 
-def edof_matrix(nx, ny):
+def _edof_matrix(nx, ny):
     edofMat = np.zeros((nx * ny, 8), dtype=int)
     for elx in range(nx):
         for ely in range(ny):
             el = ely + elx*ny
             n1 = (ny+1)*elx + ely
             n2 = (ny+1)*(elx+1) + ely
             edofMat[el, :]= np.array(
                 [2*n1+2, 2*n1+3, 2*n2+2, 2*n2+3,2*n2, 2*n2+1, 2*n1, 2*n1+1])
     return edofMat
 
 
-def stiffness_matrix(E=1, nu=0.3):
+def _lk(E=1, nu=0.3):
+    """Element stiffness matrix."""
+    k = np.array([
+        1/2-nu/6, 1/8+nu/8, -1/4-nu/12, -1/8+3*nu/8,
+        -1/4+nu/12, -1/8-nu/8, nu/6, 1/8-3*nu/8])
+
+    return E / (1-nu**2) * np.array([
+        [k[0], k[1], k[2], k[3], k[4], k[5], k[6], k[7]],
+        [k[1], k[0], k[7], k[6], k[5], k[4], k[3], k[2]],
+        [k[2], k[7], k[0], k[5], k[6], k[3], k[4], k[1]],
+        [k[3], k[6], k[5], k[0], k[7], k[2], k[1], k[4]],
+        [k[4], k[5], k[6], k[7], k[0], k[1], k[2], k[3]],
+        [k[5], k[4], k[3], k[2], k[1], k[0], k[7], k[6]],
+        [k[6], k[3], k[4], k[1], k[2], k[7], k[0], k[5]],
+        [k[7], k[2], k[1], k[4], k[3], k[6], k[5], k[0]]])
+
+
+def _stiffness_matrix(E=1, nu=0.3):
     """Element stiffness matrix."""
     k = np.array([
         1/2-nu/6, 1/8+nu/8, -1/4-nu/12, -1/8+3*nu/8,
         -1/4+nu/12, -1/8-nu/8, nu/6, 1/8-3*nu/8])
 
     return E / (1-nu**2) * np.array([
         [k[0], k[1], k[2], k[3], k[4], k[5], k[6], k[7]],
@@ -366,14 +283,99 @@
         [k[3], k[6], k[5], k[0], k[7], k[2], k[1], k[4]],
         [k[4], k[5], k[6], k[7], k[0], k[1], k[2], k[3]],
         [k[5], k[4], k[3], k[2], k[1], k[0], k[7], k[6]],
         [k[6], k[3], k[4], k[1], k[2], k[7], k[0], k[5]],
         [k[7], k[2], k[1], k[4], k[3], k[6], k[5], k[0]]])
 
 
+def _topopt_lite(nelx, nely, volfrac, penal, rmin, ft=1):
+    Emin = 1.E-9
+    Emax = 1.0
+    ndof = 2 * (nelx+1) * (nely+1)
+
+    # FE: Build the index vectors for the for coo matrix format.
+    KE = _lk()
+    edofMat = np.zeros((nelx*nely, 8), dtype=int)
+    for elx in range(nelx):
+        for ely in range(nely):
+            el = ely + elx*nely
+            n1 = (nely+1)*elx + ely
+            n2 = (nely+1)*(elx+1) + ely
+            edofMat[el, :]= np.array(
+                [2*n1+2, 2*n1+3, 2*n2+2, 2*n2+3,2*n2, 2*n2+1, 2*n1, 2*n1+1])
+
+    # Construct the index pointers for the coo format:
+    iK = np.kron(edofMat,np.ones((8,1))).flatten()
+    jK = np.kron(edofMat,np.ones((1,8))).flatten()
+
+    # Filter: Build and assemble the index+data vectors for the coo matrix:
+    nfilter = int(nelx*nely*((2*(np.ceil(rmin)-1)+1)**2))
+    iH = np.zeros(nfilter)
+    jH = np.zeros(nfilter)
+    sH = np.zeros(nfilter)
+    cc = 0
+    for i in range(nelx):
+        for j in range(nely):
+            row = i*nely + j
+            kk1 = int(np.maximum(i - (np.ceil(rmin)-1), 0))
+            kk2 = int(np.minimum(i + np.ceil(rmin), nelx))
+            ll1 = int(np.maximum(j - (np.ceil(rmin)-1), 0))
+            ll2 = int(np.minimum(j + np.ceil(rmin), nely))
+            for k in range(kk1, kk2):
+                for l in range(ll1, ll2):
+                    col = k*nely + l
+                    fac = rmin - np.sqrt(((i-k)*(i-k)+(j-l)*(j-l)))
+                    iH[cc] = row
+                    jH[cc] = col
+                    sH[cc] = np.maximum(0., fac)
+                    cc = cc + 1
+
+    # Finalize assembly and convert to csc format:
+    H = coo_matrix((sH, (iH, jH)), shape=(nelx*nely, nelx*nely)).tocsc()
+    Hs = H.sum(1)
+
+    # BC's and support:
+    dofs = np.arange(2*(nelx+1)*(nely+1))
+    fixed = np.union1d(dofs[0:2*(nely+1):2], np.array([2*(nelx+1)*(nely+1)-1]))
+    free = np.setdiff1d(dofs, fixed)
+
+    # Solution and RHS vectors:
+    f = np.zeros((ndof, 1))
+    u = np.zeros((ndof, 1))
+
+    # Set load:
+    f[1, 0] = -1
+
+    def f_loss(x):
+
+        # Filter design variables:
+        xPhys = np.asarray(H * x[np.newaxis].T / Hs)[:, 0] if ft == 1 else x
+
+        # Setup and solve FE problem:
+        sK = ((KE.flatten()[np.newaxis]).T*(Emin+(xPhys)**penal*(Emax-Emin)))
+        sK = sK.flatten(order='F')
+        K = coo_matrix((sK, (iK, jK)), shape=(ndof, ndof)).tocsc()
+
+        # Remove constrained dofs from matrix:
+        K = K[free, :][:, free]
+
+        # Solve system:
+        u[free, 0] = spsolve(K, f[free, 0])
+
+        # Objective and sensitivity:
+        ce = np.dot(u[edofMat].reshape(nelx*nely, 8), KE)
+        ce *= u[edofMat].reshape(nelx*nely, 8)
+        ce = ce.sum(1)
+        obj = Emin + (Emax - Emin) * xPhys**penal
+        obj = (obj * ce).sum()
+        return obj
+
+    return f_loss
+
+
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmTopopt().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+2)
@@ -389,7 +391,12 @@
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
+
+    text = 'Generate image for a random multi-index  :  '
+    bm.show('result/BmTopopt_demo', np.array(i))
+    text += 'see "result" folder with png file'
+    print(text)
```

### Comparing `teneva_bm-0.4.0/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.5.0/teneva_bm/various/bm_wall_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
     Simple example of the special discrete function ("wall"), which is
@@ -22,15 +21,15 @@
 
         self.set_min(i=[0]*self.d, y=0.)
 
     @property
     def is_tens(self):
         return True
 
-    def _f(self, i):
+    def target(self, i):
         if len(np.where(i == self.i_min_real)[0]) == self.d:
             return 0.
         elif len(np.where(i == self.i_min_real)[0]) > 0:
             return self.d * 10
         else:
             return i[0]
```

### Comparing `teneva_bm-0.4.0/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.5.0/teneva_bm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,61 +30,61 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.4.0".
+> Current version "0.5.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
 - Collections `func`, `hs` and `various` do not require installation of additional libraries.
 
 - Сollections `oc` and `qubo` require installation of the following libraries:
     ```bash
     pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
     ```
 
-- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `gym` and `mujoco` frameworks and related packages, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
 
-> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+> To run benchmark optimization examples (see `demo_opti` folder), you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
-bm = BmQuboMaxcut().prep()
+bm = BmQuboMaxcut()
+bm.prep()
 print(bm.info())
 ```
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
 > We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
-> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
+> We also present some examples in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
-- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. The collection includes the following benchmarks: `BmAgentSwimmer`.
+    > Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) may be performed (i.e., `none` policy) or discrete Toeplitz policy may be used.
 
-- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
-
-- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
+- `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston` (only `d=7` is supported), `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
@@ -101,46 +101,50 @@
 
 First, we create an instance of the desired benchmark class and manually call the `prep` method (optionally, we can also print detailed information about the benchmark):
 ```python
 import numpy as np
 from teneva_bm import *
 np.random.seed(42)
 
-bm = BmFuncAckley().prep()
+bm = BmFuncAckley()
+bm.prep()
 print(bm.info())
 ```
 
 The class constructor of all benchmarks has the following optional arguments:
+
 - `d` - dimension of the benchmark's input (non-negative integer). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., the dimension for benchmark `various.bm_matmul` is determined automatically by the values of auxiliary arguments `size`, `rank` and `only2`). By default, some correct value is used (specified in the benchmark description).
+
 - `n` - number of possible discrete values for benchmark input variables, i.e., the mode size of the related tensor / multidimensional array (non-negative integer if all mode sizes are equal or a list of non-negative integers of the length `d`). For some benchmarks, this number is hardcoded (or depends on other specified auxiliary arguments), if another value is explicitly passed, an error message will be generated (e.g., in `qubo` collection all benchmarks should have `n = 2`). By default, some correct value is used (specified in the benchmark description).
+
 - `name` - the display name of the benchmark (string). By default, the name corresponding to the file/class name is used.
+
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
+
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
--
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`) and for a fixed value of the seed, the behavior of the benchmark will always be the same, however, not all benchmarks depend on a seed.
+
 - `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
 - `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
-- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm.constr`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned). For the case of maximization task you should set negative `penalty` value.
 
-- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks, which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
-
-- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_log(with_log=False, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step (for condition `step`) and a string `prefix` for the log. You can also disable the display of current minimum values (`with_min`) or maximum values (`with_max`) in the log string.
 
-- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_cache(with_cache=False, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used, that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can set `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
@@ -192,14 +196,18 @@
 
 - `bm.i_max`, `bm.x_max`, `bm.y_max` - a discrete multi-index, a continuous multi-dimensional point, and benchmark values corresponding to the maximum of all requested values. Note that for the case of a discrete function, the value of `x_max` will be `None`, and for the case of a continuous function, the values of `i_max` and `x_max` will correlate, while if requests were made for continuous points, then `x_max` will correspond to the exact position of the point, and `i_max` will be the nearest multi-index of the used discrete grid.
 
 - `bm.i_min`, `bm.x_min`, `bm.y_min` - same as in the previous point, but for the minimum value.
 
 The following function may be used to print the corresponding values: `print(bm.info_history())`.
 
+##### Notes
+
+- For some benchmarks (e.g., for all benchmarks from `agent` collection) the method `show` (present the current state, the state for provided input or the final state for the best found input) and `render` (present the animation for the current solution, the solution from the provided input or for the solution from the best found input) are available.
+
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_bm-0.4.0/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.5.0/teneva_bm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 demo.py
+requirements.txt
 setup.cfg
 setup.py
 teneva_bm/__init__.py
 teneva_bm/bm.py
 teneva_bm/teneva_bm_demo.py
 teneva_bm.egg-info/PKG-INFO
 teneva_bm.egg-info/SOURCES.txt
 teneva_bm.egg-info/dependency_links.txt
 teneva_bm.egg-info/requires.txt
 teneva_bm.egg-info/top_level.txt
 teneva_bm/agent/__init__.py
 teneva_bm/agent/agent.py
+teneva_bm/agent/bm_agent_ant.py
+teneva_bm/agent/bm_agent_humanoid.py
+teneva_bm/agent/bm_agent_lake.py
 teneva_bm/agent/bm_agent_swimmer.py
-teneva_bm/agent_toe/__init__.py
-teneva_bm/agent_toe/agent_toe.py
-teneva_bm/agent_toe/bm_agent_toe_swimmer.py
+teneva_bm/agent/policy.py
 teneva_bm/func/__init__.py
 teneva_bm/func/bm_func_ackley.py
 teneva_bm/func/bm_func_alpine.py
 teneva_bm/func/bm_func_dixon.py
 teneva_bm/func/bm_func_exp.py
 teneva_bm/func/bm_func_griewank.py
 teneva_bm/func/bm_func_michalewicz.py
```

