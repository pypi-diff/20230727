# Comparing `tmp/starrailcard-0.0.5.tar.gz` & `tmp/starrailcard-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-0.0.5.tar", max compression
+gzip compressed data, was "starrailcard-0.0.6.tar", max compression
```

## Comparing `starrailcard-0.0.5.tar` & `starrailcard-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,86 @@
--rw-r--r--   0        0        0      506 2023-06-22 14:02:35.726822 starrailcard-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1304 2023-06-22 11:25:16.479693 starrailcard-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-17 13:06:01.306235 starrailcard-0.0.5/starrailcard/__init__.py
--rw-r--r--   0        0        0     4348 2023-06-22 13:26:21.104875 starrailcard-0.0.5/starrailcard/honkaicard.py
--rw-r--r--   0        0        0        0 2023-06-17 13:05:17.443970 starrailcard-0.0.5/starrailcard/src/__init__.py
--rw-r--r--   0        0        0     5623 2023-06-14 18:06:59.215231 starrailcard-0.0.5/starrailcard/src/assets/ARTIFACT.png
--rw-r--r--   0        0        0    83412 2023-06-14 17:57:00.250514 starrailcard-0.0.5/starrailcard/src/assets/bg/bg.png
--rw-r--r--   0        0        0   158031 2023-06-17 14:05:49.423459 starrailcard-0.0.5/starrailcard/src/assets/bg/bg_charters.png
--rw-r--r--   0        0        0     6705 2023-06-14 17:57:52.444545 starrailcard-0.0.5/starrailcard/src/assets/bg/frame_charters.png
--rw-r--r--   0        0        0     5628 2023-06-17 15:44:07.301010 starrailcard-0.0.5/starrailcard/src/assets/bg/maska.png
--rw-r--r--   0        0        0     7216 2023-05-24 10:00:18.675835 starrailcard-0.0.5/starrailcard/src/assets/const/Closed.png
--rw-r--r--   0        0        0     8219 2023-05-24 10:00:45.643719 starrailcard-0.0.5/starrailcard/src/assets/const/Lock.png
--rw-r--r--   0        0        0    23211 2023-05-23 20:21:03.593475 starrailcard-0.0.5/starrailcard/src/assets/const/open.png
--rw-r--r--   0        0        0  4909668 2022-09-27 23:11:24.000000 starrailcard-0.0.5/starrailcard/src/assets/font/NotoSansKR-Bold.otf
--rw-r--r--   0        0        0     8848 2023-06-14 18:09:06.500975 starrailcard-0.0.5/starrailcard/src/assets/lc/bg.png
--rw-r--r--   0        0        0     6756 2023-06-14 18:09:18.448917 starrailcard-0.0.5/starrailcard/src/assets/lc/bg_lc.png
--rw-r--r--   0        0        0     5014 2023-06-17 15:41:55.506646 starrailcard-0.0.5/starrailcard/src/assets/lc/maska.png
--rw-r--r--   0        0        0    10376 2023-06-14 18:04:44.670067 starrailcard-0.0.5/starrailcard/src/assets/LOGO.png
--rw-r--r--   0        0        0     5250 2023-06-14 18:07:34.766685 starrailcard-0.0.5/starrailcard/src/assets/Sets/bg.png
--rw-r--r--   0        0        0     4795 2023-06-14 18:07:50.587159 starrailcard-0.0.5/starrailcard/src/assets/Sets/count.png
--rw-r--r--   0        0        0     4939 2023-05-23 20:18:52.221269 starrailcard-0.0.5/starrailcard/src/assets/stars/strs_1.png
--rw-r--r--   0        0        0     5285 2023-05-23 20:18:40.906875 starrailcard-0.0.5/starrailcard/src/assets/stars/strs_2.png
--rw-r--r--   0        0        0     5270 2023-05-23 20:18:31.351225 starrailcard-0.0.5/starrailcard/src/assets/stars/strs_3.png
--rw-r--r--   0        0        0     5276 2023-05-23 20:18:20.816749 starrailcard-0.0.5/starrailcard/src/assets/stars/strs_4.png
--rw-r--r--   0        0        0     5247 2023-05-23 20:18:00.663473 starrailcard-0.0.5/starrailcard/src/assets/stars/strs_5.png
--rw-r--r--   0        0        0     5977 2023-06-14 18:06:19.159817 starrailcard-0.0.5/starrailcard/src/assets/STATS.png
--rw-r--r--   0        0        0     5536 2023-06-14 18:00:51.102004 starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg.png
--rw-r--r--   0        0        0     5767 2023-06-14 18:04:23.681149 starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg_dop.png
--rw-r--r--   0        0        0     5621 2023-06-14 18:02:14.042865 starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg_main.png
--rw-r--r--   0        0        0     3741 2023-06-14 18:01:09.230188 starrailcard-0.0.5/starrailcard/src/assets/Tallants/count.png
--rw-r--r--   0        0        0     4256 2023-06-14 18:04:05.609136 starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_0.png
--rw-r--r--   0        0        0     4834 2023-06-14 18:03:52.230355 starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_1.png
--rw-r--r--   0        0        0     4907 2023-06-14 18:03:41.048412 starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_2.png
--rw-r--r--   0        0        0     4876 2023-06-14 18:03:27.694098 starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_3.png
--rw-r--r--   0        0        0     6131 2023-06-14 18:05:43.805818 starrailcard-0.0.5/starrailcard/src/assets/UID.png
--rw-r--r--   0        0        0    16523 2023-06-22 14:02:24.624889 starrailcard-0.0.5/starrailcard/src/generators/one.py
--rw-r--r--   0        0        0        0 2023-06-17 13:05:44.515063 starrailcard-0.0.5/starrailcard/src/tools/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-22 10:12:37.123912 starrailcard-0.0.5/starrailcard/src/tools/modal.py
--rw-r--r--   0        0        0     2224 2023-06-22 10:12:18.164061 starrailcard-0.0.5/starrailcard/src/tools/openFile.py
--rw-r--r--   0        0        0     5184 2023-06-22 10:12:31.195560 starrailcard-0.0.5/starrailcard/src/tools/pill.py
--rw-r--r--   0        0        0     2191 2023-06-22 10:15:06.259650 starrailcard-0.0.5/starrailcard/src/tools/translation.py
--rw-r--r--   0        0        0     1910 2023-06-22 10:12:25.055325 starrailcard-0.0.5/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 starrailcard-0.0.5/setup.py
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 starrailcard-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-07-27 11:32:38.807804 starrailcard-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1578 2023-07-27 11:49:01.094311 starrailcard-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 13:06:01.306235 starrailcard-0.0.6/starrailcard/__init__.py
+-rw-r--r--   0        0        0     4907 2023-07-27 11:18:06.040285 starrailcard-0.0.6/starrailcard/honkaicard.py
+-rw-r--r--   0        0        0        0 2023-06-17 13:05:17.443970 starrailcard-0.0.6/starrailcard/src/__init__.py
+-rw-r--r--   0        0        0     5623 2023-06-14 18:06:59.215231 starrailcard-0.0.6/starrailcard/src/assets/ARTIFACT.png
+-rw-r--r--   0        0        0    83412 2023-06-14 17:57:00.250514 starrailcard-0.0.6/starrailcard/src/assets/bg/bg.png
+-rw-r--r--   0        0        0   158031 2023-06-17 14:05:49.423459 starrailcard-0.0.6/starrailcard/src/assets/bg/bg_charters.png
+-rw-r--r--   0        0        0     6705 2023-06-14 17:57:52.444545 starrailcard-0.0.6/starrailcard/src/assets/bg/frame_charters.png
+-rw-r--r--   0        0        0     5628 2023-06-17 15:44:07.301010 starrailcard-0.0.6/starrailcard/src/assets/bg/maska.png
+-rw-r--r--   0        0        0     7216 2023-05-24 10:00:18.675835 starrailcard-0.0.6/starrailcard/src/assets/const/Closed.png
+-rw-r--r--   0        0        0     8219 2023-05-24 10:00:45.643719 starrailcard-0.0.6/starrailcard/src/assets/const/Lock.png
+-rw-r--r--   0        0        0    23211 2023-05-23 20:21:03.593475 starrailcard-0.0.6/starrailcard/src/assets/const/open.png
+-rw-r--r--   0        0        0  4909668 2022-09-27 23:11:24.000000 starrailcard-0.0.6/starrailcard/src/assets/font/NotoSansKR-Bold.otf
+-rw-r--r--   0        0        0     8848 2023-06-14 18:09:06.500975 starrailcard-0.0.6/starrailcard/src/assets/lc/bg.png
+-rw-r--r--   0        0        0     6756 2023-06-14 18:09:18.448917 starrailcard-0.0.6/starrailcard/src/assets/lc/bg_lc.png
+-rw-r--r--   0        0        0     5014 2023-06-17 15:41:55.506646 starrailcard-0.0.6/starrailcard/src/assets/lc/maska.png
+-rw-r--r--   0        0        0    10376 2023-06-14 18:04:44.670067 starrailcard-0.0.6/starrailcard/src/assets/LOGO.png
+-rw-r--r--   0        0        0     5250 2023-06-14 18:07:34.766685 starrailcard-0.0.6/starrailcard/src/assets/Sets/bg.png
+-rw-r--r--   0        0        0     4795 2023-06-14 18:07:50.587159 starrailcard-0.0.6/starrailcard/src/assets/Sets/count.png
+-rw-r--r--   0        0        0     4939 2023-05-23 20:18:52.221269 starrailcard-0.0.6/starrailcard/src/assets/stars/strs_1.png
+-rw-r--r--   0        0        0     5285 2023-05-23 20:18:40.906875 starrailcard-0.0.6/starrailcard/src/assets/stars/strs_2.png
+-rw-r--r--   0        0        0     5270 2023-05-23 20:18:31.351225 starrailcard-0.0.6/starrailcard/src/assets/stars/strs_3.png
+-rw-r--r--   0        0        0     5276 2023-05-23 20:18:20.816749 starrailcard-0.0.6/starrailcard/src/assets/stars/strs_4.png
+-rw-r--r--   0        0        0     5247 2023-05-23 20:18:00.663473 starrailcard-0.0.6/starrailcard/src/assets/stars/strs_5.png
+-rw-r--r--   0        0        0     5977 2023-06-14 18:06:19.159817 starrailcard-0.0.6/starrailcard/src/assets/STATS.png
+-rw-r--r--   0        0        0     5536 2023-06-14 18:00:51.102004 starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg.png
+-rw-r--r--   0        0        0     5767 2023-06-14 18:04:23.681149 starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg_dop.png
+-rw-r--r--   0        0        0     5621 2023-06-14 18:02:14.042865 starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg_main.png
+-rw-r--r--   0        0        0     3741 2023-06-14 18:01:09.230188 starrailcard-0.0.6/starrailcard/src/assets/Tallants/count.png
+-rw-r--r--   0        0        0     4256 2023-06-14 18:04:05.609136 starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_0.png
+-rw-r--r--   0        0        0     4834 2023-06-14 18:03:52.230355 starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_1.png
+-rw-r--r--   0        0        0     4907 2023-06-14 18:03:41.048412 starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_2.png
+-rw-r--r--   0        0        0     4876 2023-06-14 18:03:27.694098 starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_3.png
+-rw-r--r--   0        0        0     5684 2023-07-04 08:56:16.747056 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/ANEMO.png
+-rw-r--r--   0        0        0     5729 2023-07-04 08:57:43.987247 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/ELECTRO.png
+-rw-r--r--   0        0        0     5605 2023-07-04 08:59:37.122714 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/FIRE.png
+-rw-r--r--   0        0        0     3864 2023-07-04 09:00:58.352717 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/frame.png
+-rw-r--r--   0        0        0     5729 2023-07-04 08:55:27.817666 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/ICE.png
+-rw-r--r--   0        0        0     5736 2023-07-04 08:56:52.855750 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/IMAGINARY.png
+-rw-r--r--   0        0        0    10301 2023-07-19 13:17:45.700898 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/maska.png
+-rw-r--r--   0        0        0     5690 2023-07-04 09:00:04.462472 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/PSYHICAL.png
+-rw-r--r--   0        0        0     5702 2023-07-04 08:57:21.088980 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/QUANTOM.png
+-rw-r--r--   0        0        0     4712 2023-07-19 22:32:52.546801 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/rank.png
+-rw-r--r--   0        0        0     7458 2023-07-27 11:47:42.545004 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/rank_total.png
+-rw-r--r--   0        0        0     4238 2023-07-04 08:54:49.553788 starrailcard-0.0.6/starrailcard/src/assets/teample_two/artifact/sets.png
+-rw-r--r--   0        0        0   256955 2023-07-04 08:25:00.264059 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/ANEMO.png
+-rw-r--r--   0        0        0   338749 2023-07-04 08:25:53.486925 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/ELECTRO.png
+-rw-r--r--   0        0        0   315282 2023-07-04 08:27:23.748335 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/FIRE.png
+-rw-r--r--   0        0        0   252526 2023-07-04 08:23:23.375150 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/ICE.png
+-rw-r--r--   0        0        0   254927 2023-07-04 08:26:47.116739 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/IMAGINARY.png
+-rw-r--r--   0        0        0    11053 2023-07-04 08:35:58.686949 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/MASKA.png
+-rw-r--r--   0        0        0   106584 2023-07-14 19:08:51.655635 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/MASKA_ART.png
+-rw-r--r--   0        0        0   107864 2023-07-14 19:20:20.781092 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/MASKA_ART_CUSTUM.png
+-rw-r--r--   0        0        0    11698 2023-07-14 19:26:43.535333 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/MASKA_ARTS.png
+-rw-r--r--   0        0        0   134813 2023-07-04 08:28:50.373768 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/PSYHICAL.png
+-rw-r--r--   0        0        0   327191 2023-07-04 08:27:55.614946 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/QUANTOM.png
+-rw-r--r--   0        0        0    84834 2023-07-04 08:33:46.540145 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/SHADOW.png
+-rw-r--r--   0        0        0   400535 2023-07-04 08:34:20.377488 starrailcard-0.0.6/starrailcard/src/assets/teample_two/bg/stars.png
+-rw-r--r--   0        0        0     4943 2023-07-17 19:38:45.343050 starrailcard-0.0.6/starrailcard/src/assets/teample_two/LC/icons.png
+-rw-r--r--   0        0        0     4424 2023-07-17 18:59:50.049522 starrailcard-0.0.6/starrailcard/src/assets/teample_two/LC/Maska.png
+-rw-r--r--   0        0        0     4377 2023-07-04 09:01:57.294054 starrailcard-0.0.6/starrailcard/src/assets/teample_two/LC/shadow.png
+-rw-r--r--   0        0        0     4497 2023-07-26 17:56:12.041491 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/closed.png
+-rw-r--r--   0        0        0     4502 2023-07-26 17:52:53.169977 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/closed_2.png
+-rw-r--r--   0        0        0     6079 2023-07-20 11:07:02.161811 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/closed_dop.png
+-rw-r--r--   0        0        0     3992 2023-07-20 16:33:57.645333 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/count.png
+-rw-r--r--   0        0        0    78915 2023-07-20 11:11:51.824719 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Knight.png
+-rw-r--r--   0        0        0    71599 2023-07-20 11:12:39.568190 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Mage.png
+-rw-r--r--   0        0        0    85995 2023-07-20 11:13:08.912172 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Priest.png
+-rw-r--r--   0        0        0    83225 2023-07-20 11:13:29.627537 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Rogue.png
+-rw-r--r--   0        0        0    76991 2023-07-20 11:14:03.465023 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Shaman.png
+-rw-r--r--   0        0        0    80295 2023-07-20 11:14:25.952319 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Warlock.png
+-rw-r--r--   0        0        0    77497 2023-07-20 11:14:51.280086 starrailcard-0.0.6/starrailcard/src/assets/teample_two/path/Warrior.png
+-rw-r--r--   0        0        0     4346 2023-07-04 08:39:17.356006 starrailcard-0.0.6/starrailcard/src/assets/teample_two/stats/bg.png
+-rw-r--r--   0        0        0     6131 2023-06-14 18:05:43.805818 starrailcard-0.0.6/starrailcard/src/assets/UID.png
+-rw-r--r--   0        0        0    16523 2023-06-22 14:02:24.624889 starrailcard-0.0.6/starrailcard/src/generators/one.py
+-rw-r--r--   0        0        0    25003 2023-07-27 11:47:31.201593 starrailcard-0.0.6/starrailcard/src/generators/two.py
+-rw-r--r--   0        0        0        0 2023-06-17 13:05:44.515063 starrailcard-0.0.6/starrailcard/src/tools/__init__.py
+-rw-r--r--   0        0        0     2624 2023-07-26 18:19:49.012142 starrailcard-0.0.6/starrailcard/src/tools/calculator.py
+-rw-r--r--   0        0        0     1241 2023-07-27 10:15:05.143184 starrailcard-0.0.6/starrailcard/src/tools/modal.py
+-rw-r--r--   0        0        0     4618 2023-07-26 18:19:49.012142 starrailcard-0.0.6/starrailcard/src/tools/openFile.py
+-rw-r--r--   0        0        0    13665 2023-07-20 16:43:13.078768 starrailcard-0.0.6/starrailcard/src/tools/pill.py
+-rw-r--r--   0        0        0     2191 2023-06-22 10:15:06.259650 starrailcard-0.0.6/starrailcard/src/tools/translation.py
+-rw-r--r--   0        0        0     7143 2023-07-26 17:52:56.321063 starrailcard-0.0.6/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 starrailcard-0.0.6/setup.py
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 starrailcard-0.0.6/PKG-INFO
```

### Comparing `starrailcard-0.0.5/starrailcard/honkaicard.py` & `starrailcard-0.0.6/starrailcard/honkaicard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2023 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
 
 from .src.tools import translation, pill, modal
-from .src.generators import one
+from .src.generators import one, two
 from honkairail import starrailapi
 import asyncio,re,os,datetime
 
 def process_input(characterImgs, characterName):
     if characterImgs:
         if isinstance(characterImgs, dict):
             characterImgs = {key.lower(): value for key, value in characterImgs.items()}
@@ -31,26 +31,30 @@
     data = datetime.datetime.now().strftime("%d_%m_%Y %H_%M")
     path = os.path.join(os.getcwd(), "RailCard", str(uid))
     os.makedirs(path, exist_ok=True)
     file_path = os.path.join(path, f"{name}_{data}.png")
     res.save(file_path)
 
 class MiHoMoCard():
-    def __init__(self,lang = "ru", characterImgs = None, characterName = None, hide = False, save = False, background = True):
+    def __init__(self,lang = "ru", characterImgs = None, characterName = None, hide = False, save = False, background = True, template = 1):
 
         """
         :param lang: str, What language to receive information supported:  en, ru, vi, th, pt, kr, jp, zh, id, fr, es, de, chs, cht.
         :param characterImgs: dict, Dictionary: {"Name_charter_1": "image link","Name_charter_2": "image link",...}.
         :param characterName: str, If we want to get certain characters: "Name_charter_1,Name_charter_1,Name_charter_1" Character names must be in the same language as in the lang parameter.
         :param hide: bool, Display UID.
         :param save: bool, Save images or not.
         :param background: bool, Generate image with or without background.
 
-        """
+        """        
+        
+        self.template = template
 
+        if not int(template) in [1,2]:
+            self.template = 1
 
         if not lang in translation.supportLang:
             self.lang = "en"
         else:
             self.lang = lang
         
         self.translateLang = translation.Translator(lang)
@@ -69,49 +73,56 @@
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         pass
     
-    async def characterImg(self,name):
+    async def characterImg(self,name,ids):
         if name in self.characterImgs:
             self.img = await pill.get_user_image(self.characterImgs[name])
         else:
             self.img = None
+        
+        if ids in self.characterImgs:
+            self.img = await pill.get_user_image(self.characterImgs[ids])
 
     async def creat(self, uid):
         task = []
         data = await self.API.get_full_data(uid)
         user = {
             "settings": {
                 "uid": int(uid),
                 "lang": self.lang,
                 "hide": self.hide,
                 "save": self.save,
                 "background": self.background
             },
             "player": data.player,
             "card": [],
-            "name": ""
+            "name": "",
+            "id": "",
         }
 
         
         for key in data.characters:
             
             user["name"] += f"{key.name}, "
-
+            user["id"] += f"{key.id}, "
+            
             if self.characterName:
-                if not key.name.lower()  in self.characterName:
+                if not key.name.lower() in self.characterName and not str(key.id) in self.characterName:
                     continue       
 
             if self.characterImgs:
-                await self.characterImg(key.name.lower())
-
-            task.append(one.Creat(key, self.translateLang,self.img,self.hide,int(uid),remove_html_tags(data.player.nickname),self.background).start())
+                await self.characterImg(key.name.lower(), str(key.id))
+            if self.template == 1:
+                task.append(one.Creat(key, self.translateLang,self.img,self.hide,int(uid),remove_html_tags(data.player.nickname),self.background).start())
+            else:
+                task.append(two.Creat(key, self.translateLang,self.img,self.hide,int(uid)).start())
 
         user["card"] = await asyncio.gather(*task)
 
         if self.save:
             for keys in user["card"]:
                 await saveBanner(uid,keys["card"], keys["name"])
```

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/ARTIFACT.png` & `starrailcard-0.0.6/starrailcard/src/assets/ARTIFACT.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/bg/bg.png` & `starrailcard-0.0.6/starrailcard/src/assets/bg/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/bg/bg_charters.png` & `starrailcard-0.0.6/starrailcard/src/assets/bg/bg_charters.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/bg/frame_charters.png` & `starrailcard-0.0.6/starrailcard/src/assets/bg/frame_charters.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/bg/maska.png` & `starrailcard-0.0.6/starrailcard/src/assets/bg/maska.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/const/Closed.png` & `starrailcard-0.0.6/starrailcard/src/assets/const/Closed.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/const/Lock.png` & `starrailcard-0.0.6/starrailcard/src/assets/const/Lock.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/const/open.png` & `starrailcard-0.0.6/starrailcard/src/assets/const/open.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/font/NotoSansKR-Bold.otf` & `starrailcard-0.0.6/starrailcard/src/assets/font/NotoSansKR-Bold.otf`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/lc/bg.png` & `starrailcard-0.0.6/starrailcard/src/assets/lc/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/lc/bg_lc.png` & `starrailcard-0.0.6/starrailcard/src/assets/lc/bg_lc.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/lc/maska.png` & `starrailcard-0.0.6/starrailcard/src/assets/lc/maska.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/LOGO.png` & `starrailcard-0.0.6/starrailcard/src/assets/LOGO.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Sets/bg.png` & `starrailcard-0.0.6/starrailcard/src/assets/Sets/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Sets/count.png` & `starrailcard-0.0.6/starrailcard/src/assets/Sets/count.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/stars/strs_1.png` & `starrailcard-0.0.6/starrailcard/src/assets/stars/strs_1.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/stars/strs_2.png` & `starrailcard-0.0.6/starrailcard/src/assets/stars/strs_2.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/stars/strs_3.png` & `starrailcard-0.0.6/starrailcard/src/assets/stars/strs_3.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/stars/strs_4.png` & `starrailcard-0.0.6/starrailcard/src/assets/stars/strs_4.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/stars/strs_5.png` & `starrailcard-0.0.6/starrailcard/src/assets/stars/strs_5.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/STATS.png` & `starrailcard-0.0.6/starrailcard/src/assets/STATS.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg_dop.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg_dop.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/bg_main.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/bg_main.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/count.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/count.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_0.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_0.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_1.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_1.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_2.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_2.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/Tallants/dop_3.png` & `starrailcard-0.0.6/starrailcard/src/assets/Tallants/dop_3.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/assets/UID.png` & `starrailcard-0.0.6/starrailcard/src/assets/UID.png`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/generators/one.py` & `starrailcard-0.0.6/starrailcard/src/generators/one.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/starrailcard/src/tools/modal.py` & `starrailcard-0.0.6/starrailcard/src/tools/modal.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,7 +45,8 @@
     background: Optional[bool]
 
 class HSRCard(BaseModel):
     settings: Settings
     player: PlayerV2
     card: List[Card]
     name: Optional[str]
+    id: Optional[str]
```

### Comparing `starrailcard-0.0.5/starrailcard/src/tools/translation.py` & `starrailcard-0.0.6/starrailcard/src/tools/translation.py`

 * *Files identical despite different names*

### Comparing `starrailcard-0.0.5/PKG-INFO` & `starrailcard-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 0.0.5
+Version: 0.0.6
 Summary: Module for generating Honkai Star Rail character cards
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: None
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,15 @@
  <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/StarRailCardM.png" alt="Баннер"/>
 </p>
 
 ____
 
 ## StarRailCard
 Module for generating Honkai Star Rail character cards
+
 :white_medium_square: Ability to generate with or without background.<br>
 :white_medium_square: Ability to set a custom image.<br>
 :white_medium_square: Flexible map settings.
 
 ## Installation:
 ```
 pip install starrailcard
@@ -33,24 +34,44 @@
 
 ## Launch:
 ``` python
 from starrailcard import honkaicard 
 import asyncio
 
 async def mains():
-    while True:
-        async with honkaicard.MiHoMoCard() as hmhm:
-            r = await hmhm.creat(700649319)
-            print(r)
+    async with honkaicard.MiHoMoCard(template=1) as hmhm:
+        r = await hmhm.creat(700649319)
+        print(r)
 
 asyncio.run(mains())
 ```
 
 ## Languages Supported
 | Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |
 |-------------|---------|-------------|---------|-------------|---------|
 |  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |
 |  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cht  |
 |  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |
 |  日本語      |     jp  | 中文        |     zh  | español    |     es  |
 |  中文        |     zh  | Indonesian |     id  | français   |     fr  |
-|  Khaenri'ah  |     kh  | Khaenri'ah |
+
+
+
+<details>
+<summary>Sample 1 template</summary>
+ 
+[![Adaptation][3]][3]
+ 
+[3]: https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/a-18.png
+  
+</details>
+
+
+<details>
+<summary>Sample 2 template</summary>
+ 
+[![Adaptation][4]][4]
+ 
+[4]: https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/a-19.png
+ 
+</details>
+
```

