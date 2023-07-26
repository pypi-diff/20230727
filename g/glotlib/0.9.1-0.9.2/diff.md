# Comparing `tmp/glotlib-0.9.1.tar.gz` & `tmp/glotlib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glotlib-0.9.1.tar", last modified: Thu Jul 20 00:13:23 2023, max compression
+gzip compressed data, was "glotlib-0.9.2.tar", last modified: Wed Jul 26 22:36:09 2023, max compression
```

## Comparing `glotlib-0.9.1.tar` & `glotlib-0.9.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.187551 glotlib-0.9.1/
--rw-r--r--   0 greent7    (502) staff       (20)    26526 2023-07-11 00:37:56.000000 glotlib-0.9.1/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)      547 2023-07-20 00:13:23.187612 glotlib-0.9.1/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)       66 2023-07-11 00:59:47.000000 glotlib-0.9.1/README.txt
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.182828 glotlib-0.9.1/glotlib/
--rw-r--r--   0 greent7    (502) staff       (20)      609 2023-07-20 00:12:44.000000 glotlib-0.9.1/glotlib/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1274 2023-07-20 00:12:44.000000 glotlib-0.9.1/glotlib/colors.py
--rw-r--r--   0 greent7    (502) staff       (20)      162 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/constants.py
--rw-r--r--   0 greent7    (502) staff       (20)     6603 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.183519 glotlib-0.9.1/glotlib/font_files/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.185570 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/
--rw-r--r--   0 greent7    (502) staff       (20)     5954 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/COPYRIGHT.TXT
--rw-r--r--   0 greent7    (502) staff       (20)      320 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/README.TXT
--rw-r--r--   0 greent7    (502) staff       (20)     8112 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/RELEASENOTES.TXT
--rw-r--r--   0 greent7    (502) staff       (20)    65932 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/Vera.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    63208 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBI.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    58716 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    63684 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraIt.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    55032 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBI.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    49052 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    54508 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoIt.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    49224 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMono.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    60280 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSe.ttf
--rw-r--r--   0 greent7    (502) staff       (20)    58736 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSeBd.ttf
--rw-r--r--   0 greent7    (502) staff       (20)     1012 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/local.conf
--rw-r--r--   0 greent7    (502) staff       (20)      148 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/fonts.py
--rw-r--r--   0 greent7    (502) staff       (20)     1773 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/hline.py
--rw-r--r--   0 greent7    (502) staff       (20)     4337 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/label.py
--rw-r--r--   0 greent7    (502) staff       (20)     2876 2023-07-20 00:12:44.000000 glotlib-0.9.1/glotlib/main.py
--rw-r--r--   0 greent7    (502) staff       (20)     1882 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/matrix.py
--rw-r--r--   0 greent7    (502) staff       (20)     2740 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/miter_lines.py
--rw-r--r--   0 greent7    (502) staff       (20)    16838 2023-07-20 00:13:14.000000 glotlib-0.9.1/glotlib/plot.py
--rw-r--r--   0 greent7    (502) staff       (20)     2001 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/program.py
--rw-r--r--   0 greent7    (502) staff       (20)     2534 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/programs.py
--rw-r--r--   0 greent7    (502) staff       (20)     4422 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/series.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.186490 glotlib-0.9.1/glotlib/shaders/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)       99 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/frag.frag
--rw-r--r--   0 greent7    (502) staff       (20)     1311 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/miter_line.vert
--rw-r--r--   0 greent7    (502) staff       (20)      161 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/mvp_z.vert
--rw-r--r--   0 greent7    (502) staff       (20)      195 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/points.frag
--rw-r--r--   0 greent7    (502) staff       (20)     1548 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/square_instanced_line.vert
--rw-r--r--   0 greent7    (502) staff       (20)      260 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/text.frag
--rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/shaders/text.vert
--rw-r--r--   0 greent7    (502) staff       (20)     1249 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/step_series.py
--rw-r--r--   0 greent7    (502) staff       (20)     2055 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/ticker.py
--rw-r--r--   0 greent7    (502) staff       (20)     3626 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/vbo.py
--rw-r--r--   0 greent7    (502) staff       (20)     1849 2023-07-11 00:37:56.000000 glotlib-0.9.1/glotlib/vline.py
--rw-r--r--   0 greent7    (502) staff       (20)    12371 2023-07-20 00:13:14.000000 glotlib-0.9.1/glotlib/window.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.183410 glotlib-0.9.1/glotlib.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)      547 2023-07-20 00:13:23.000000 glotlib-0.9.1/glotlib.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     1698 2023-07-20 00:13:23.000000 glotlib-0.9.1/glotlib.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2023-07-20 00:13:23.000000 glotlib-0.9.1/glotlib.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)       46 2023-07-20 00:13:23.000000 glotlib-0.9.1/glotlib.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        8 2023-07-20 00:13:23.000000 glotlib-0.9.1/glotlib.egg-info/top_level.txt
--rw-r--r--   0 greent7    (502) staff       (20)      838 2023-07-20 00:13:23.187876 glotlib-0.9.1/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-11 00:37:56.000000 glotlib-0.9.1/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-20 00:13:23.187445 glotlib-0.9.1/tests/
--rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test1.py
--rw-r--r--   0 greent7    (502) staff       (20)     1046 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test2.py
--rw-r--r--   0 greent7    (502) staff       (20)     1064 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test3.py
--rw-r--r--   0 greent7    (502) staff       (20)     1020 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test4.py
--rw-r--r--   0 greent7    (502) staff       (20)      727 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test5.py
--rw-r--r--   0 greent7    (502) staff       (20)      179 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test6.py
--rw-r--r--   0 greent7    (502) staff       (20)     2250 2023-07-20 00:12:44.000000 glotlib-0.9.1/tests/test7.py
--rw-r--r--   0 greent7    (502) staff       (20)      483 2023-07-11 00:37:56.000000 glotlib-0.9.1/tests/test8.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.314299 glotlib-0.9.2/
+-rw-r--r--   0 greent7    (502) staff       (20)    26526 2023-07-11 00:37:56.000000 glotlib-0.9.2/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)      547 2023-07-26 22:36:09.314348 glotlib-0.9.2/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)       66 2023-07-11 00:59:47.000000 glotlib-0.9.2/README.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.310133 glotlib-0.9.2/glotlib/
+-rw-r--r--   0 greent7    (502) staff       (20)      609 2023-07-20 00:12:44.000000 glotlib-0.9.2/glotlib/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1274 2023-07-20 00:12:44.000000 glotlib-0.9.2/glotlib/colors.py
+-rw-r--r--   0 greent7    (502) staff       (20)      162 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/constants.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6603 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.310752 glotlib-0.9.2/glotlib/font_files/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.312664 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/
+-rw-r--r--   0 greent7    (502) staff       (20)     5954 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/COPYRIGHT.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)      320 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/README.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)     8112 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/RELEASENOTES.TXT
+-rw-r--r--   0 greent7    (502) staff       (20)    65932 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/Vera.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    63208 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBI.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    58716 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    63684 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraIt.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    55032 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBI.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    49052 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    54508 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoIt.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    49224 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMono.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    60280 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSe.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)    58736 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSeBd.ttf
+-rw-r--r--   0 greent7    (502) staff       (20)     1012 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/local.conf
+-rw-r--r--   0 greent7    (502) staff       (20)      148 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/fonts.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1773 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/hline.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4337 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/label.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2876 2023-07-20 00:12:44.000000 glotlib-0.9.2/glotlib/main.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1882 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/matrix.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2740 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/miter_lines.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16700 2023-07-25 22:50:21.000000 glotlib-0.9.2/glotlib/plot.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2001 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/program.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2534 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/programs.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4422 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/series.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.313442 glotlib-0.9.2/glotlib/shaders/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)       99 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/frag.frag
+-rw-r--r--   0 greent7    (502) staff       (20)     1311 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/miter_line.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      161 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/mvp_z.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      195 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/points.frag
+-rw-r--r--   0 greent7    (502) staff       (20)     1548 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/square_instanced_line.vert
+-rw-r--r--   0 greent7    (502) staff       (20)      260 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/text.frag
+-rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/shaders/text.vert
+-rw-r--r--   0 greent7    (502) staff       (20)     1249 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/step_series.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2055 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/ticker.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3626 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/vbo.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1849 2023-07-11 00:37:56.000000 glotlib-0.9.2/glotlib/vline.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12371 2023-07-20 00:13:14.000000 glotlib-0.9.2/glotlib/window.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.310655 glotlib-0.9.2/glotlib.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)      547 2023-07-26 22:36:09.000000 glotlib-0.9.2/glotlib.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     1698 2023-07-26 22:36:09.000000 glotlib-0.9.2/glotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2023-07-26 22:36:09.000000 glotlib-0.9.2/glotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       46 2023-07-26 22:36:09.000000 glotlib-0.9.2/glotlib.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        8 2023-07-26 22:36:09.000000 glotlib-0.9.2/glotlib.egg-info/top_level.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      838 2023-07-26 22:36:09.314593 glotlib-0.9.2/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-11 00:37:56.000000 glotlib-0.9.2/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-07-26 22:36:09.314219 glotlib-0.9.2/tests/
+-rw-r--r--   0 greent7    (502) staff       (20)      251 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test1.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1046 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test2.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1064 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test3.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1020 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test4.py
+-rw-r--r--   0 greent7    (502) staff       (20)      727 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test5.py
+-rw-r--r--   0 greent7    (502) staff       (20)      179 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test6.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2250 2023-07-20 00:12:44.000000 glotlib-0.9.2/tests/test7.py
+-rw-r--r--   0 greent7    (502) staff       (20)      483 2023-07-11 00:37:56.000000 glotlib-0.9.2/tests/test8.py
```

### Comparing `glotlib-0.9.1/LICENSE` & `glotlib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/PKG-INFO` & `glotlib-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotlib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library for creating plots using OpenGL.
 Home-page: https://github.com/tgree/glotlib
 Author: Terry Greeniaus
 Author-email: terry.greeniaus@gmail.com
 License: LGPLv2
 Keywords: glotlib
 Classifier: Operating System :: OS Independent
```

### Comparing `glotlib-0.9.1/glotlib/__init__.py` & `glotlib-0.9.2/glotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/colors.py` & `glotlib-0.9.2/glotlib/colors.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font.py` & `glotlib-0.9.2/glotlib/font.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/COPYRIGHT.TXT` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/COPYRIGHT.TXT`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/RELEASENOTES.TXT` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/RELEASENOTES.TXT`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/Vera.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/Vera.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBI.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBI.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBd.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraIt.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraIt.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBI.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBI.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBd.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoIt.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMoIt.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMono.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraMono.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSe.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSe.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSeBd.ttf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/VeraSeBd.ttf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/font_files/ttf-bitstream-vera-1.10/local.conf` & `glotlib-0.9.2/glotlib/font_files/ttf-bitstream-vera-1.10/local.conf`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/hline.py` & `glotlib-0.9.2/glotlib/hline.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/label.py` & `glotlib-0.9.2/glotlib/label.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/main.py` & `glotlib-0.9.2/glotlib/main.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/matrix.py` & `glotlib-0.9.2/glotlib/matrix.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/miter_lines.py` & `glotlib-0.9.2/glotlib/miter_lines.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/plot.py` & `glotlib-0.9.2/glotlib/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,18 +261,14 @@
         window_h = self.h
         mvp_w    = 2 * self.mvpi[0][0]
         mvp_h    = 2 * self.mvpi[1][1]
         max_x    = max(abs(ml), abs(mr))
         max_y    = max(abs(mb), abs(mt))
         renorm_x = (max_x > mvp_w * K / window_w)
         renorm_y = (max_y > mvp_h * K / window_h)
-        if renorm_x:
-            print('Horizontal renorm required.')
-        if renorm_y:
-            print('Vertical renorm required.')
         if renorm_x or renorm_y:
             self._renormalize(l, r, b, t)
 
     def _gen_mvp_from_dimensions_and_point(self, w, h, d_point, p_point):
         '''
         Generates mvp and mvpi such that we will be viewing a rectangle of
         data dimensions w x h with the (x, y) data point d_point locked to the
```

### Comparing `glotlib-0.9.1/glotlib/program.py` & `glotlib-0.9.2/glotlib/program.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/programs.py` & `glotlib-0.9.2/glotlib/programs.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/series.py` & `glotlib-0.9.2/glotlib/series.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/shaders/miter_line.vert` & `glotlib-0.9.2/glotlib/shaders/miter_line.vert`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/shaders/square_instanced_line.vert` & `glotlib-0.9.2/glotlib/shaders/square_instanced_line.vert`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/step_series.py` & `glotlib-0.9.2/glotlib/step_series.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/ticker.py` & `glotlib-0.9.2/glotlib/ticker.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/vbo.py` & `glotlib-0.9.2/glotlib/vbo.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/vline.py` & `glotlib-0.9.2/glotlib/vline.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib/window.py` & `glotlib-0.9.2/glotlib/window.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/glotlib.egg-info/PKG-INFO` & `glotlib-0.9.2/glotlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotlib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library for creating plots using OpenGL.
 Home-page: https://github.com/tgree/glotlib
 Author: Terry Greeniaus
 Author-email: terry.greeniaus@gmail.com
 License: LGPLv2
 Keywords: glotlib
 Classifier: Operating System :: OS Independent
```

### Comparing `glotlib-0.9.1/glotlib.egg-info/SOURCES.txt` & `glotlib-0.9.2/glotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/setup.cfg` & `glotlib-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = glotlib
-version = 0.9.1
+version = 0.9.2
 author = Terry Greeniaus
 author_email = terry.greeniaus@gmail.com
 description = Library for creating plots using OpenGL.
 long_description = Library for creating plots using OpenGL.
 long_description_content_type = text/x-rst
 keywords = glotlib
 url = https://github.com/tgree/glotlib
```

### Comparing `glotlib-0.9.1/tests/test2.py` & `glotlib-0.9.2/tests/test2.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/tests/test3.py` & `glotlib-0.9.2/tests/test3.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/tests/test4.py` & `glotlib-0.9.2/tests/test4.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/tests/test5.py` & `glotlib-0.9.2/tests/test5.py`

 * *Files identical despite different names*

### Comparing `glotlib-0.9.1/tests/test7.py` & `glotlib-0.9.2/tests/test7.py`

 * *Files identical despite different names*

