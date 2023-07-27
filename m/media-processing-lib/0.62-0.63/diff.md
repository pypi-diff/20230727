# Comparing `tmp/media-processing-lib-0.62.tar.gz` & `tmp/media-processing-lib-0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-processing-lib-0.62.tar", last modified: Thu Jul 13 11:33:19 2023, max compression
+gzip compressed data, was "media-processing-lib-0.63.tar", last modified: Thu Jul 27 09:48:45 2023, max compression
```

## Comparing `media-processing-lib-0.62.tar` & `media-processing-lib-0.63.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2023-03-26 06:25:47.000000 media-processing-lib-0.62/LICENSE.TXT
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2023-03-26 06:25:47.000000 media-processing-lib-0.62/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-13 11:33:19.511968 media-processing-lib-0.62/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2023-03-26 06:25:47.000000 media-processing-lib-0.62/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.503968 media-processing-lib-0.62/media_processing_lib/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_resample.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/audio_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/librosa/reader.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/libs/soundfile/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/melspectrogram.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/mpl_audio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/audio/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/collage_maker/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/collage_maker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3951 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/collage_maker/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      167 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      704 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/image_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/image_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/pil/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1359 2023-05-01 06:22:34.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/pil/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/libs/skimage/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/resize/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3677 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize_black_bars.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/resize/resize_stretch.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib/image/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/text.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1473 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/image/utils/title.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1030 2023-05-28 19:19:53.000000 media-processing-lib-0.62/media_processing_lib/image/utils/to_image.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2916 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/image/utils/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-28 17:34:43.000000 media-processing-lib-0.62/media_processing_lib/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2023-03-26 06:25:47.000000 media-processing-lib-0.62/media_processing_lib/video/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/backends/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/decord.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4140 2023-05-28 19:58:05.000000 media-processing-lib-0.62/media_processing_lib/video/backends/disk_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/imageio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/backends/memory_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/backends/mpl_video_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/backends/opencv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-05-31 16:16:07.000000 media-processing-lib-0.62/media_processing_lib/video/backends/pims.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/mpl_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-05-29 09:32:03.000000 media-processing-lib-0.62/media_processing_lib/video/utils.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-05 14:47:46.000000 media-processing-lib-0.62/media_processing_lib/video/video_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/video_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/imageio/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-04-21 08:08:14.000000 media-processing-lib-0.62/media_processing_lib/video/writer/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.507968 media-processing-lib-0.62/media_processing_lib.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3173 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2023-07-13 11:33:19.000000 media-processing-lib-0.62/media_processing_lib.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-05-31 15:49:33.000000 media-processing-lib-0.62/requirements.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-13 11:33:19.511968 media-processing-lib-0.62/resources/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2023-03-26 06:25:47.000000 media-processing-lib-0.62/resources/OpenSans-Bold.ttf
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-07-13 11:33:19.511968 media-processing-lib-0.62/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1831 2023-07-13 11:33:17.000000 media-processing-lib-0.62/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.588658 media-processing-lib-0.63/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2023-03-26 06:25:47.000000 media-processing-lib-0.63/LICENSE.TXT
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2023-03-26 06:25:47.000000 media-processing-lib-0.63/MANIFEST.in
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-27 09:48:45.588658 media-processing-lib-0.63/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2023-03-26 06:25:47.000000 media-processing-lib-0.63/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/audio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/audio_reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/audio_resample.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/audio_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/audio/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/audio/libs/librosa/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/libs/librosa/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/libs/librosa/reader.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/audio/libs/soundfile/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/libs/soundfile/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/libs/soundfile/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib/audio/melspectrogram/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/melspectrogram/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/melspectrogram/melspectrogram.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/mpl_audio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/audio/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/collage_maker/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/collage_maker/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/collage_maker/collage_maker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4297 2023-07-27 09:48:30.000000 media-processing-lib-0.63/media_processing_lib/collage_maker/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      167 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      704 2023-05-28 17:34:43.000000 media-processing-lib-0.63/media_processing_lib/image/image_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/image_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/libs/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-28 17:34:43.000000 media-processing-lib-0.63/media_processing_lib/image/libs/opencv/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/opencv/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/libs/pil/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/pil/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-28 17:34:43.000000 media-processing-lib-0.63/media_processing_lib/image/libs/pil/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1359 2023-05-01 06:22:34.000000 media-processing-lib-0.63/media_processing_lib/image/libs/pil/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/pil/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/libs/skimage/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/skimage/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/skimage/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/skimage/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/libs/skimage/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.580658 media-processing-lib-0.63/media_processing_lib/image/resize/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/resize/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3677 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/resize/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/resize/resize_black_bars.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/resize/resize_stretch.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.584658 media-processing-lib-0.63/media_processing_lib/image/utils/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/utils/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/utils/text.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1473 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/image/utils/title.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1030 2023-05-28 19:19:53.000000 media-processing-lib-0.63/media_processing_lib/image/utils/to_image.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2916 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/image/utils/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-28 17:34:43.000000 media-processing-lib-0.63/media_processing_lib/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.584658 media-processing-lib-0.63/media_processing_lib/video/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2023-03-26 06:25:47.000000 media-processing-lib-0.63/media_processing_lib/video/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.584658 media-processing-lib-0.63/media_processing_lib/video/backends/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/backends/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/backends/decord.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4140 2023-05-28 19:58:05.000000 media-processing-lib-0.63/media_processing_lib/video/backends/disk_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/backends/imageio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-05 14:47:46.000000 media-processing-lib-0.63/media_processing_lib/video/backends/memory_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-05 14:47:46.000000 media-processing-lib-0.63/media_processing_lib/video/backends/mpl_video_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/backends/opencv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-05-31 16:16:07.000000 media-processing-lib-0.63/media_processing_lib/video/backends/pims.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-05 14:47:46.000000 media-processing-lib-0.63/media_processing_lib/video/mpl_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-05-29 09:32:03.000000 media-processing-lib-0.63/media_processing_lib/video/utils.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-05 14:47:46.000000 media-processing-lib-0.63/media_processing_lib/video/video_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/video_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.584658 media-processing-lib-0.63/media_processing_lib/video/writer/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/writer/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.584658 media-processing-lib-0.63/media_processing_lib/video/writer/imageio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/writer/imageio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/writer/imageio/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.588658 media-processing-lib-0.63/media_processing_lib/video/writer/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/writer/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-04-21 08:08:14.000000 media-processing-lib-0.63/media_processing_lib/video/writer/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.576658 media-processing-lib-0.63/media_processing_lib.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2023-07-27 09:48:45.000000 media-processing-lib-0.63/media_processing_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3173 2023-07-27 09:48:45.000000 media-processing-lib-0.63/media_processing_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-07-27 09:48:45.000000 media-processing-lib-0.63/media_processing_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-07-27 09:48:45.000000 media-processing-lib-0.63/media_processing_lib.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2023-07-27 09:48:45.000000 media-processing-lib-0.63/media_processing_lib.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2023-05-31 15:49:33.000000 media-processing-lib-0.63/requirements.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-07-27 09:48:45.588658 media-processing-lib-0.63/resources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2023-03-26 06:25:47.000000 media-processing-lib-0.63/resources/OpenSans-Bold.ttf
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-07-27 09:48:45.588658 media-processing-lib-0.63/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1831 2023-07-27 09:48:40.000000 media-processing-lib-0.63/setup.py
```

### Comparing `media-processing-lib-0.62/media_processing_lib/audio/audio_reader.py` & `media-processing-lib-0.63/media_processing_lib/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/audio/audio_writer.py` & `media-processing-lib-0.63/media_processing_lib/audio/audio_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/audio/melspectrogram/melspectrogram.py` & `media-processing-lib-0.63/media_processing_lib/audio/melspectrogram/melspectrogram.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/audio/mpl_audio.py` & `media-processing-lib-0.63/media_processing_lib/audio/mpl_audio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/audio/utils.py` & `media-processing-lib-0.63/media_processing_lib/audio/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/collage_maker/collage_maker.py` & `media-processing-lib-0.63/media_processing_lib/collage_maker/collage_maker.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/collage_maker/utils.py` & `media-processing-lib-0.63/media_processing_lib/collage_maker/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return np.load
     if suffix == "npz":
 
         def f(x):
             X = np.load(x, allow_pickle=True)["arr_0"]
             try:
                 _ = X.shape
-            except Exception as _:
+            except Exception:
                 X = X.item()
             return X
 
         return f
     assert False, f"Suffix unknown: '{suffix}'. Path: '{file_path}'"
 
 def get_closest_square(N: int) -> Tuple[int, int]:
@@ -58,39 +58,46 @@
     - kwargs are used for image_add_title method
 
     Return: A numpy array of stacked images according to (rows, cols) inputs.
     """
     assert len(images) > 1, "Must give at least two images to the collage"
     if rows_cols is None:
         rows_cols = get_closest_square(len(images))
-        logger.debug(f"row_cols was not set. Setting automatically to {rows_cols} based on number of images")
+        logger.debug2(f"row_cols was not set. Setting automatically to {rows_cols} based on number of images")
     assert len(rows_cols) == 2, f"rows_cols must be a tuple with 2 numbers, got: {rows_cols}"
     if np.prod(rows_cols) > len(images):
         logger.warning(f"rows_cols: {rows_cols} greater than n images: {len(images)}. Padding with black images!")
+    assert not all(x is None for x in images), "All images are None"
+
+    shapes = [x.shape for x in [img for img in images if img is not None]]
 
-    shapes = [x.shape for x in images]
     # np.pad uses [(0, 0), (0, 0), (0, 0)] to pad (a, b) on each channge of H,W,C. Our images may be H,W or H,W,C
     # If they are H, W, C then we care about [(0, pad_bottom), (0, pad_right), (0, 0)]
     pad = np.zeros((len(shapes[0]), 2), dtype=int)
     pad[0, 1] = pad_bottom
     pad[1, 1] = pad_right
 
+    if any(x is None for x in images):
+        logger.debug("Some images are None. Padding with black images!")
+        images = [np.zeros(shapes[0], dtype=np.uint8) if x is None else x for x in images]
+        shapes = [x.shape for x in images]
+
     if pad.sum() != 0:
         images = [np.pad(image, pad) for image in images]
         shapes = [x.shape for x in images]
 
     if titles is not None:
         images = [image_add_title(image, title, **kwargs) for (image, title) in zip(images, titles)]
         shapes = [x.shape for x in images]
     assert np.std(shapes, axis=0).sum() == 0, f"Shapes not equal: {shapes}"
 
     # Put all the results in a new array
     result = np.zeros((rows_cols[0] * rows_cols[1], *shapes[0]), dtype=np.uint8)
-    result[0 : len(images)] = np.array(images)
+    result[0: len(images)] = np.array(images)
     result = result.reshape((rows_cols[0], rows_cols[1], *shapes[0]))
     result = np.concatenate(np.concatenate(result, axis=1), axis=1)
     # remove pad right from last image
     if pad_right != 0:
-        result = result[:, 0 : result.shape[1] - pad_right]
+        result = result[:, 0: result.shape[1] - pad_right]
     if pad_bottom != 0:
-        result = result[0 : result.shape[0] - pad_bottom]
+        result = result[0: result.shape[0] - pad_bottom]
     return result
```

### Comparing `media-processing-lib-0.62/media_processing_lib/image/image_reader.py` & `media-processing-lib-0.63/media_processing_lib/image/image_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/image_writer.py` & `media-processing-lib-0.63/media_processing_lib/image/image_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/libs/opencv/resize.py` & `media-processing-lib-0.63/media_processing_lib/image/libs/opencv/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/libs/pil/resize.py` & `media-processing-lib-0.63/media_processing_lib/image/libs/pil/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/libs/skimage/resize.py` & `media-processing-lib-0.63/media_processing_lib/image/libs/skimage/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/resize/resize.py` & `media-processing-lib-0.63/media_processing_lib/image/resize/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/resize/resize_black_bars.py` & `media-processing-lib-0.63/media_processing_lib/image/resize/resize_black_bars.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/resize/resize_stretch.py` & `media-processing-lib-0.63/media_processing_lib/image/resize/resize_stretch.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/utils/text.py` & `media-processing-lib-0.63/media_processing_lib/image/utils/text.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/utils/title.py` & `media-processing-lib-0.63/media_processing_lib/image/utils/title.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/utils/to_image.py` & `media-processing-lib-0.63/media_processing_lib/image/utils/to_image.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/image/utils/utils.py` & `media-processing-lib-0.63/media_processing_lib/image/utils/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/logger.py` & `media-processing-lib-0.63/media_processing_lib/logger.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/decord.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/decord.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/disk_backend.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/disk_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/imageio.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/imageio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/memory_backend.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/memory_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/mpl_video_backend.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/mpl_video_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/opencv.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/opencv.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/backends/pims.py` & `media-processing-lib-0.63/media_processing_lib/video/backends/pims.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/mpl_video.py` & `media-processing-lib-0.63/media_processing_lib/video/mpl_video.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/utils.py` & `media-processing-lib-0.63/media_processing_lib/video/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/video_reader.py` & `media-processing-lib-0.63/media_processing_lib/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/video_writer.py` & `media-processing-lib-0.63/media_processing_lib/video/video_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib/video/writer/opencv/writer.py` & `media-processing-lib-0.63/media_processing_lib/video/writer/opencv/writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/media_processing_lib.egg-info/SOURCES.txt` & `media-processing-lib-0.63/media_processing_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/resources/OpenSans-Bold.ttf` & `media-processing-lib-0.63/resources/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.62/setup.py` & `media-processing-lib-0.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
 
 name = "media-processing-lib"
-version = "0.62"
+version = "0.63"
 description = "Media processing library for video, audio and images."
 url = "https://gitlab.com/mihaicristianpirvu/media-processing-lib"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

