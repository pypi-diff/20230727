# Comparing `tmp/lightcon-1.4.2.post2.tar.gz` & `tmp/lightcon-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.4.2.post2.tar", last modified: Tue Jun 27 12:50:23 2023, max compression
+gzip compressed data, was "lightcon-1.4.3.tar", last modified: Thu Jul 27 09:25:08 2023, max compression
```

## Comparing `lightcon-1.4.2.post2.tar` & `lightcon-1.4.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/
--rw-rw-rw-   0        0        0     1082 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/LICENCE
--rw-rw-rw-   0        0        0      317 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/MANIFEST.in
--rw-rw-rw-   0        0        0     6258 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/
--rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/__config__.py
--rw-rw-rw-   0        0        0      717 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/beam_alignment/
--rw-rw-rw-   0        0        0       93 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/beam_alignment/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/beam_alignment/_beam_alignment.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/calculate/
--rw-rw-rw-   0        0        0      190 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_gauss.py
--rw-rw-rw-   0        0        0     3393 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_iso.py
--rw-rw-rw-   0        0        0     1407 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_calculate_motor_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/camera_app_client/
--rw-rw-rw-   0        0        0       76 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/camera_app_client/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/camera_app_client/_camera_app_client.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/common/
--rw-rw-rw-   0        0        0      614 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/__init__.py
--rw-rw-rw-   0        0        0      931 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_converters.py
--rw-rw-rw-   0        0        0     3155 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_http_methods.py
--rw-rw-rw-   0        0        0     5607 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_leprecan_provider.py
--rw-rw-rw-   0        0        0      336 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_load_motor_and_stage_parameters.py
--rw-rw-rw-   0        0        0     1042 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_serial_tools.py
--rw-rw-rw-   0        0        0     5151 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_udp_locator.py
--rw-rw-rw-   0        0        0      506 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/stage_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/datasets/
--rw-rw-rw-   0        0        0      159 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/__init__.py
--rw-rw-rw-   0        0        0     3055 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/datasets/data/
--rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/data/__init__.py
--rw-rw-rw-   0        0        0    11968 2023-06-27 12:49:31.000000 lightcon-1.4.2.post2/lightcon/datasets/data/motor_parameters.json
--rw-rw-rw-   0        0        0     4990 2023-06-27 12:49:31.000000 lightcon-1.4.2.post2/lightcon/datasets/data/stage_parameters.json
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/eth_motor_board/
--rw-rw-rw-   0        0        0      204 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/__init__.py
--rw-rw-rw-   0        0        0    15177 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board.py
--rw-rw-rw-   0        0        0     1920 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/fast_daq/
--rw-rw-rw-   0        0        0    70144 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0    25088 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    23552 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
--rw-rw-rw-   0        0        0    29600 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/System.Threading.dll
--rw-rw-rw-   0        0        0      130 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/__init__.py
--rw-rw-rw-   0        0        0     5442 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/_fast_daq.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/harpia/
--rw-rw-rw-   0        0        0      237 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/__init__.py
--rw-rw-rw-   0        0        0    24803 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia.py
--rw-rw-rw-   0        0        0     2222 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia_leprecan_provider.py
--rw-rw-rw-   0        0        0     8813 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia_model_decoder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/harpia_daq/
--rw-rw-rw-   0        0        0    70144 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0   108908 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.xml
--rw-rw-rw-   0        0        0    17920 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    26624 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
--rw-rw-rw-   0        0        0    18130 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml
--rw-rw-rw-   0        0        0    29600 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/System.Threading.dll
--rw-rw-rw-   0        0        0       84 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/__init__.py
--rw-rw-rw-   0        0        0     5744 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/_harpia_daq.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/laser_clients/
--rw-rw-rw-   0        0        0       91 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/laser_clients/__init__.py
--rw-rw-rw-   0        0        0     8634 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/laser_clients/_laser_clients.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/style/
--rw-rw-rw-   0        0        0      229 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/_plotstyle_1d.py
--rw-rw-rw-   0        0        0     7839 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/plotstyle_1d.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/timing_controller/
--rw-rw-rw-   0        0        0      172 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/__init__.py
--rw-rw-rw-   0        0        0     6326 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller.py
--rw-rw-rw-   0        0        0     7234 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller_v2.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/utils/
--rw-rw-rw-   0        0        0       50 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/utils/__init__.py
--rw-rw-rw-   0        0        0      591 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/utils/_fixes.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/lightcon/wintopas/
--rw-rw-rw-   0        0        0       65 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/wintopas/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/wintopas/_wintopas.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6258 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2354 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/setup.cfg
--rw-rw-rw-   0        0        0     1745 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/
+-rw-rw-rw-   0        0        0     1082 2023-07-27 09:23:25.000000 lightcon-1.4.3/LICENCE
+-rw-rw-rw-   0        0        0      317 2023-07-27 09:23:25.000000 lightcon-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6252 2023-07-27 09:25:08.948416 lightcon-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-07-27 09:23:25.000000 lightcon-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.917166 lightcon-1.4.3/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/__config__.py
+-rw-rw-rw-   0        0        0      715 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.917166 lightcon-1.4.3/lightcon/beam_alignment/
+-rw-rw-rw-   0        0        0       93 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/beam_alignment/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/beam_alignment/_beam_alignment.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.917166 lightcon-1.4.3/lightcon/calculate/
+-rw-rw-rw-   0        0        0      190 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/calculate/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/calculate/_beam_profiling_gauss.py
+-rw-rw-rw-   0        0        0     3393 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/calculate/_beam_profiling_iso.py
+-rw-rw-rw-   0        0        0     1407 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/calculate/_calculate_motor_parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.917166 lightcon-1.4.3/lightcon/camera_app_client/
+-rw-rw-rw-   0        0        0       76 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/camera_app_client/__init__.py
+-rw-rw-rw-   0        0        0     2965 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/camera_app_client/_camera_app_client.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/common/
+-rw-rw-rw-   0        0        0      614 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_converters.py
+-rw-rw-rw-   0        0        0     3724 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_http_methods.py
+-rw-rw-rw-   0        0        0     5607 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_leprecan_provider.py
+-rw-rw-rw-   0        0        0      336 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_load_motor_and_stage_parameters.py
+-rw-rw-rw-   0        0        0     1042 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_serial_tools.py
+-rw-rw-rw-   0        0        0     5151 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/_udp_locator.py
+-rw-rw-rw-   0        0        0      506 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/common/stage_parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/datasets/
+-rw-rw-rw-   0        0        0      159 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3055 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/datasets/_base.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/datasets/data/
+-rw-rw-rw-   0        0        0        0 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0    11968 2023-07-27 09:24:25.000000 lightcon-1.4.3/lightcon/datasets/data/motor_parameters.json
+-rw-rw-rw-   0        0        0     6678 2023-07-27 09:24:25.000000 lightcon-1.4.3/lightcon/datasets/data/stage_parameters.json
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/eth_motor_board/
+-rw-rw-rw-   0        0        0      204 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/eth_motor_board/__init__.py
+-rw-rw-rw-   0        0        0    15177 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/eth_motor_board/_eth_motor_board.py
+-rw-rw-rw-   0        0        0     1920 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/fast_daq/
+-rw-rw-rw-   0        0        0    70144 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0    25088 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    23552 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
+-rw-rw-rw-   0        0        0    29600 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0      130 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/__init__.py
+-rw-rw-rw-   0        0        0     5442 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/fast_daq/_fast_daq.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.932791 lightcon-1.4.3/lightcon/harpia/
+-rw-rw-rw-   0        0        0      237 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia/__init__.py
+-rw-rw-rw-   0        0        0    24803 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia/_harpia.py
+-rw-rw-rw-   0        0        0     2222 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia/_harpia_leprecan_provider.py
+-rw-rw-rw-   0        0        0     8813 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia/_harpia_model_decoder.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/harpia_daq/
+-rw-rw-rw-   0        0        0    70144 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0   108908 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/FTD2XX_NET.xml
+-rw-rw-rw-   0        0        0    17920 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    26624 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
+-rw-rw-rw-   0        0        0    18130 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml
+-rw-rw-rw-   0        0        0    29600 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0       84 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/__init__.py
+-rw-rw-rw-   0        0        0     5744 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/harpia_daq/_harpia_daq.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/laser_clients/
+-rw-rw-rw-   0        0        0       91 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/laser_clients/__init__.py
+-rw-rw-rw-   0        0        0     8634 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/laser_clients/_laser_clients.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/style/
+-rw-rw-rw-   0        0        0      229 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/style/__init__.py
+-rw-rw-rw-   0        0        0     7848 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/style/_plotstyle_1d.py
+-rw-rw-rw-   0        0        0     7839 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/style/plotstyle_1d.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/timing_controller/
+-rw-rw-rw-   0        0        0      172 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/timing_controller/__init__.py
+-rw-rw-rw-   0        0        0     6326 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/timing_controller/_timing_controller.py
+-rw-rw-rw-   0        0        0     7234 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/timing_controller/_timing_controller_v2.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/utils/__init__.py
+-rw-rw-rw-   0        0        0      591 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/utils/_fixes.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.948416 lightcon-1.4.3/lightcon/wintopas/
+-rw-rw-rw-   0        0        0       65 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/wintopas/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-07-27 09:23:25.000000 lightcon-1.4.3/lightcon/wintopas/_wintopas.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:25:08.917166 lightcon-1.4.3/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-07-27 09:25:08.000000 lightcon-1.4.3/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2354 2023-07-27 09:25:08.000000 lightcon-1.4.3/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:25:08.000000 lightcon-1.4.3/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-07-27 09:25:08.000000 lightcon-1.4.3/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 09:25:08.000000 lightcon-1.4.3/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:25:08.964041 lightcon-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-07-27 09:23:25.000000 lightcon-1.4.3/setup.py
```

### Comparing `lightcon-1.4.2.post2/LICENCE` & `lightcon-1.4.3/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/PKG-INFO` & `lightcon-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2.post2
+Version: 1.4.3
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2.post2/README.md` & `lightcon-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/__init__.py` & `lightcon-1.4.3/lightcon/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.2-2"
+__version__ = "1.4.3"
 
 from . import wintopas
 from . import timing_controller
 from . import style
 from . import laser_clients
 from . import harpia
 from . import harpia_daq
```

### Comparing `lightcon-1.4.2.post2/lightcon/beam_alignment/_beam_alignment.py` & `lightcon-1.4.3/lightcon/beam_alignment/_beam_alignment.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_gauss.py` & `lightcon-1.4.3/lightcon/calculate/_beam_profiling_gauss.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_iso.py` & `lightcon-1.4.3/lightcon/calculate/_beam_profiling_iso.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/calculate/_calculate_motor_parameters.py` & `lightcon-1.4.3/lightcon/calculate/_calculate_motor_parameters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/camera_app_client/_camera_app_client.py` & `lightcon-1.4.3/lightcon/camera_app_client/_camera_app_client.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/common/__init__.py` & `lightcon-1.4.3/lightcon/common/__init__.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/common/_converters.py` & `lightcon-1.4.3/lightcon/common/_converters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/common/_http_methods.py` & `lightcon-1.4.3/lightcon/common/_http_methods.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,109 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#==========================================================================
-#
-#--------------------------------------------------------------------------
-# Copyright (c) 2022 Light Conversion, UAB
-# All rights reserved.
-# www.lightcon.com
-#==========================================================================
+"""lightcon - a Python library for controlling Light Conversion devices.
+
+HTTP methods class, which implements REST communication.
+
+Copyright 2020-2023 Light Conversion
+Contact: support@lightcon.com
+"""
 import json
 import urllib
 import urllib.error
 import urllib.request
 import urllib.parse
 import time
 import http
 
+
+def print_timer(cmd, time_from):
+    """Print elapsed time for command in ms."""
+    print(cmd + " : {:.3f} ms".format((time.perf_counter() - time_from)*1E3))
+
+
 class HTTP_methods:
+    """REST client."""
     retry_on_incomplete_read = True
     print_full_http_response_on_failure = True
 
     def _open(self, page_url):
         return urllib.request.urlopen(self.url+page_url).read().decode('utf-8')
 
-    def _get (self, command):
+    def _get(self, command):
         time_init = time.perf_counter()
         cont = True
 
         while cont:
             try:
-                data = json.loads(urllib.request.urlopen(self.url+command).read().decode('utf-8'))
+                data = json.loads(urllib.request.urlopen(
+                    self.url+command).read().decode('utf-8'))
                 cont = False
             except urllib.error.HTTPError as e:
                 error_string = e.read().decode('utf-8', 'ignore')
-                print (error_string)
+                print(error_string)
                 return error_string
             except http.client.IncompleteRead:
                 cont = True and self.retry_on_incomplete_read
                 if not self.silent:
-                    print ('Incomplete read')
+                    print('Incomplete read')
 
         if not self.silent:
-            print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
+            print_timer(command, time_init)
         return data
 
-    def _put (self, command, data):
+    def _put(self, command, data):
         time_init = time.perf_counter()
         try:
-            post_url = urllib.request.Request(url=self.url+command, data=data.encode('utf-8'), method='PUT')
+            post_url = urllib.request.Request(
+                url=self.url+command, data=data.encode('utf-8'), method='PUT')
 
             post_url.add_header('Content-Type', 'application/json')
 
             with urllib.request.urlopen(post_url) as f:
                 pass
             if not self.silent:
-                print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
+                print_timer(command, time_init)
             return f.status
         except urllib.error.HTTPError as e:
             print("Exception while PUT to {:} with data {:}".format(post_url.full_url, data))
             error_string = e.read().decode('utf-8', 'ignore')
             if self.print_full_http_response_on_failure:
                 print(error_string)
             return error_string
 
-        if not self.silent:
-            print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
-        return 200
-
-
-    def _post (self, command, details={}):
+    def _post(self, command, details={}):
         time_init = time.perf_counter()
         try:
             post_details = urllib.parse.urlencode(details).encode('UTF-8')
 
             post_url = urllib.request.Request(self.url+command, post_details)
 
             res = urllib.request.urlopen(post_url).read().decode('utf-8', 'ignore')
         except urllib.error.HTTPError as e:
             error_string = e.read().decode('utf-8', 'ignore')
-            print (error_string)
+            print(error_string)
+            return error_string
+
+        if not self.silent:
+            print(command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
+        return res
+
+    def _report(self, command, data={}):
+        time_init = time.perf_counter()
+        try:
+            req = urllib.request.Request(
+                url=self.url+command, data=data.encode('utf-8'),
+                method='REPORT')
+
+            req.add_header('Content-Type', 'application/json')
+
+            res = json.loads(
+                urllib.request.urlopen(req).read().decode('utf-8', 'ignore'))
+        except urllib.error.HTTPError as e:
+            error_string = e.read().decode('utf-8', 'ignore')
+            print(error_string)
             return error_string
 
         if not self.silent:
-            print (command + " : {:.3f} ms".format((time.perf_counter()-time_init)*1000))
-        return res
+            print_timer(command, time_init)
+        return res
```

### Comparing `lightcon-1.4.2.post2/lightcon/common/_leprecan_provider.py` & `lightcon-1.4.3/lightcon/common/_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/common/_serial_tools.py` & `lightcon-1.4.3/lightcon/common/_serial_tools.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/common/_udp_locator.py` & `lightcon-1.4.3/lightcon/common/_udp_locator.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/datasets/_base.py` & `lightcon-1.4.3/lightcon/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/datasets/data/motor_parameters.json` & `lightcon-1.4.3/lightcon/datasets/data/motor_parameters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'Info'": "{'Date': '2023-07-03T09:26:41.5585502+00:00'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "Info": {
-        "Date": "2023-06-26T11:42:22.3986928+00:00",
+        "Date": "2023-07-03T09:26:41.5585502+00:00",
         "MD5": "AA95745FAC085A5DD18092740CAF4427"
     },
     "Values": {
         "8HS11-0204S": {
             "Acc": 170,
             "AlarmEn": 255,
             "Config": 11909,
```

### Comparing `lightcon-1.4.2.post2/lightcon/datasets/data/stage_parameters.json` & `lightcon-1.4.3/lightcon/datasets/data/stage_parameters.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {"'Info'": "{'Date': '2023-07-03T09:26:41.9404376+00:00', 'MD5': "*

 * *           "'2CA11F2E62666AFE1089138B2AC17073'}",*

 * * "'Values'": "{'Light Conversion TA-HA-TA-CR-SWAP': OrderedDict([('AlarmEn', 255), ('Config', "*

 * *             "11909), ('FnSlpAcc', 26), ('FnSlpDec', 26), ('FsSpeed', 1023), ('IntSpeed', 16383), "*

 * *             "('KTherm', 0), ('KvalAcc', 20), ('KvalDec', 20), ('KvalHold', 5), ('KvalRun', 20), "*

 * *             "('MinSpeed', 4305), ('OcdTh', 8), ('StSlp', 17), ('StallTh', 25), ('Acc', 137), "*

 * *     […]*

```diff
@@ -1,11 +1,11 @@
 {
     "Info": {
-        "Date": "2023-06-26T11:42:22.6223486+00:00",
-        "MD5": "78B9F3DD1D86D3A8C954E7488784CDB9"
+        "Date": "2023-07-03T09:26:41.9404376+00:00",
+        "MD5": "2CA11F2E62666AFE1089138B2AC17073"
     },
     "Values": {
         "Light Conversion 987-70A": {
             "Acc": 171,
             "AlarmEn": 255,
             "Config": 11909,
             "Dec": 171,
@@ -87,14 +87,72 @@
             "ReductionCoefficient": 1.0,
             "StSlp": 2,
             "StageName": "Light Conversion TA-HA-STIRRER",
             "StallTh": 19,
             "StepMode": 6,
             "TravelLength": 0
         },
+        "Light Conversion TA-HA-TA-CR-SWAP": {
+            "Acc": 137,
+            "AlarmEn": 255,
+            "Config": 11909,
+            "Dec": 103,
+            "Description": "Crystal swapper/switcher HARPIA-TA",
+            "FnSlpAcc": 26,
+            "FnSlpDec": 26,
+            "FsSpeed": 1023,
+            "IntSpeed": 16383,
+            "KTherm": 0,
+            "KvalAcc": 20,
+            "KvalDec": 20,
+            "KvalHold": 5,
+            "KvalRun": 20,
+            "LsEnable": 2,
+            "LsInvert": 0,
+            "LsSwap": 0,
+            "MaxSpeed": 500,
+            "MinSpeed": 4305,
+            "MotorName": "Sanyo Denki SH2281-5671",
+            "OcdTh": 8,
+            "ReductionCoefficient": 1.0,
+            "StSlp": 17,
+            "StageName": "Light Conversion TA-HA-TA-CR-SWAP",
+            "StallTh": 25,
+            "StepMode": 6,
+            "TravelLength": 0
+        },
+        "Light Conversion TA-HA-TA-VNDF": {
+            "Acc": 68,
+            "AlarmEn": 255,
+            "Config": 11909,
+            "Dec": 68,
+            "Description": "VNDF motor for HARPIA-TA/-TB/-TF/-TG",
+            "FnSlpAcc": 26,
+            "FnSlpDec": 26,
+            "FsSpeed": 1023,
+            "IntSpeed": 16383,
+            "KTherm": 0,
+            "KvalAcc": 20,
+            "KvalDec": 20,
+            "KvalHold": 5,
+            "KvalRun": 20,
+            "LsEnable": 0,
+            "LsInvert": 0,
+            "LsSwap": 0,
+            "MaxSpeed": 163,
+            "MinSpeed": 4305,
+            "MotorName": "Sanyo Denki SH2281-5671",
+            "OcdTh": 8,
+            "ReductionCoefficient": 1.0,
+            "StSlp": 17,
+            "StageName": "Light Conversion TA-HA-TA-VNDF",
+            "StallTh": 25,
+            "StepMode": 6,
+            "TravelLength": 0
+        },
         "Light Conversion TA-RS-0370": {
             "Acc": 343,
             "AlarmEn": 255,
             "Config": 11909,
             "Dec": 343,
             "Description": "Glan-Taylor rotator for HARPIA-TF-KERR",
             "FnSlpAcc": 29,
```

### Comparing `lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board.py` & `lightcon-1.4.3/lightcon/eth_motor_board/_eth_motor_board.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py` & `lightcon-1.4.3/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/fast_daq/FTD2XX_NET.dll` & `lightcon-1.4.3/lightcon/fast_daq/FTD2XX_NET.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Abstractions.dll` & `lightcon-1.4.3/lightcon/fast_daq/LightConversion.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll` & `lightcon-1.4.3/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/fast_daq/System.Threading.dll` & `lightcon-1.4.3/lightcon/fast_daq/System.Threading.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/fast_daq/_fast_daq.py` & `lightcon-1.4.3/lightcon/fast_daq/_fast_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia/_harpia.py` & `lightcon-1.4.3/lightcon/harpia/_harpia.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia/_harpia_leprecan_provider.py` & `lightcon-1.4.3/lightcon/harpia/_harpia_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia/_harpia_model_decoder.py` & `lightcon-1.4.3/lightcon/harpia/_harpia_model_decoder.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.dll` & `lightcon-1.4.3/lightcon/harpia_daq/FTD2XX_NET.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.xml` & `lightcon-1.4.3/lightcon/harpia_daq/FTD2XX_NET.xml`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Abstractions.dll` & `lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll` & `lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml` & `lightcon-1.4.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/System.Threading.dll` & `lightcon-1.4.3/lightcon/harpia_daq/System.Threading.dll`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/harpia_daq/_harpia_daq.py` & `lightcon-1.4.3/lightcon/harpia_daq/_harpia_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/laser_clients/_laser_clients.py` & `lightcon-1.4.3/lightcon/laser_clients/_laser_clients.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/style/_plotstyle_1d.py` & `lightcon-1.4.3/lightcon/style/_plotstyle_1d.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/style/plotstyle_1d.py` & `lightcon-1.4.3/lightcon/style/plotstyle_1d.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller.py` & `lightcon-1.4.3/lightcon/timing_controller/_timing_controller.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller_v2.py` & `lightcon-1.4.3/lightcon/timing_controller/_timing_controller_v2.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/utils/_fixes.py` & `lightcon-1.4.3/lightcon/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon/wintopas/_wintopas.py` & `lightcon-1.4.3/lightcon/wintopas/_wintopas.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/lightcon.egg-info/PKG-INFO` & `lightcon-1.4.3/lightcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2.post2
+Version: 1.4.3
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2.post2/lightcon.egg-info/SOURCES.txt` & `lightcon-1.4.3/lightcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post2/setup.py` & `lightcon-1.4.3/setup.py`

 * *Files identical despite different names*

