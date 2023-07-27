# Comparing `tmp/imgviz-1.7.2.tar.gz` & `tmp/imgviz-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgviz-1.7.2.tar", last modified: Tue Feb 14 18:15:31 2023, max compression
+gzip compressed data, was "imgviz-1.7.3.tar", last modified: Thu Jul 27 01:59:17 2023, max compression
```

## Comparing `imgviz-1.7.2.tar` & `imgviz-1.7.3.tar`

### file list

```diff
@@ -1,87 +1,99 @@
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.345416 imgviz-1.7.2/
--rw-r--r--   0 wkentaro   (501) staff       (20)     1075 2023-02-14 15:59:37.000000 imgviz-1.7.2/LICENSE
--rw-r--r--   0 wkentaro   (501) staff       (20)       75 2023-02-14 15:59:37.000000 imgviz-1.7.2/MANIFEST.in
--rw-r--r--   0 wkentaro   (501) staff       (20)     5314 2023-02-14 18:15:31.345496 imgviz-1.7.2/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     4434 2023-02-14 18:08:28.000000 imgviz-1.7.2/README.md
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.334464 imgviz-1.7.2/imgviz/
--rw-r--r--   0 wkentaro   (501) staff       (20)      816 2023-02-14 18:15:02.000000 imgviz-1.7.2/imgviz/__init__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.335928 imgviz-1.7.2/imgviz/_io/
--rw-r--r--   0 wkentaro   (501) staff       (20)      292 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/__init__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.336479 imgviz-1.7.2/imgviz/_io/_pyglet/
--rw-r--r--   0 wkentaro   (501) staff       (20)       92 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/_pyglet/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      244 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/_pyglet/base.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     9010 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/_io/_pyglet/pyglet_imshow.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      184 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/_pyglet/pyglet_run.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      842 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/_io/base.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      856 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/_io/opencv.py
--rw-r--r--   0 wkentaro   (501) staff       (20)       86 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/pil.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      661 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/_io/pyplot.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2031 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/centerize.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     5274 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/color.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.336606 imgviz-1.7.2/imgviz/data/
--rw-r--r--   0 wkentaro   (501) staff       (20)      158 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/__init__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.339038 imgviz-1.7.2/imgviz/data/arc2017/
--rw-r--r--   0 wkentaro   (501) staff       (20)      839 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/data/arc2017/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      827 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/arc2017/camera_info.yaml
--rw-r--r--   0 wkentaro   (501) staff       (20)      595 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/arc2017/class_names.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)   715747 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/arc2017/data.npz
--rw-r--r--   0 wkentaro   (501) staff       (20)  2849434 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/arc2017/res4.npz
--rw-r--r--   0 wkentaro   (501) staff       (20)    51017 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/arc2017/rgb.jpg
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.339216 imgviz-1.7.2/imgviz/data/kitti/
--rw-r--r--   0 wkentaro   (501) staff       (20)      699 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/data/kitti/__init__.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.339366 imgviz-1.7.2/imgviz/data/kitti/odometry/
--rw-r--r--   0 wkentaro   (501) staff       (20)   728871 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/kitti/odometry/00.txt
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.340002 imgviz-1.7.2/imgviz/data/lena/
--rw-r--r--   0 wkentaro   (501) staff       (20)      198 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/data/lena/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)   473831 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/lena/lena.png
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.341802 imgviz-1.7.2/imgviz/data/middlebury/
--rw-r--r--   0 wkentaro   (501) staff       (20)     1071 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/data/middlebury/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)  2457612 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/middlebury/grove3.flo
--rw-r--r--   0 wkentaro   (501) staff       (20)   604275 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/middlebury/grove3.png
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.342858 imgviz-1.7.2/imgviz/data/voc/
--rw-r--r--   0 wkentaro   (501) staff       (20)      621 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/data/voc/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      146 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/voc/class_names.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)   436248 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/voc/data.npz
--rw-r--r--   0 wkentaro   (501) staff       (20)    42712 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/data/voc/rgb.jpg
--rw-r--r--   0 wkentaro   (501) staff       (20)     3040 2023-02-14 18:08:58.000000 imgviz-1.7.2/imgviz/depth.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.344079 imgviz-1.7.2/imgviz/draw/
--rw-r--r--   0 wkentaro   (501) staff       (20)      582 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/draw/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1513 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/circle.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      765 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/ellipse.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      551 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/line.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1471 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/rectangle.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2062 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/star.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2067 2023-02-14 18:11:03.000000 imgviz-1.7.2/imgviz/draw/text.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     4161 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/text_in_rectangle.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1453 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/draw/triangle.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      381 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/dtype.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.344323 imgviz-1.7.2/imgviz/external/
--rw-r--r--   0 wkentaro   (501) staff       (20)        0 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/external/__init__.py
--rw-r--r--   0 wkentaro   (501) staff       (20)    69582 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/external/transformations.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2792 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/flow.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     4241 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/instances.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     6940 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/label.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     2405 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/nchannel.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1550 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/normalize.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     3481 2023-02-14 16:45:21.000000 imgviz-1.7.2/imgviz/resize.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     3662 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/tile.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1573 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/trajectory.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      303 2023-02-14 15:59:37.000000 imgviz-1.7.2/imgviz/utils.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.335225 imgviz-1.7.2/imgviz.egg-info/
--rw-r--r--   0 wkentaro   (501) staff       (20)     5314 2023-02-14 18:15:31.000000 imgviz-1.7.2/imgviz.egg-info/PKG-INFO
--rw-r--r--   0 wkentaro   (501) staff       (20)     1672 2023-02-14 18:15:31.000000 imgviz-1.7.2/imgviz.egg-info/SOURCES.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        1 2023-02-14 18:15:31.000000 imgviz-1.7.2/imgviz.egg-info/dependency_links.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)       92 2023-02-14 18:15:31.000000 imgviz-1.7.2/imgviz.egg-info/requires.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)        7 2023-02-14 18:15:31.000000 imgviz-1.7.2/imgviz.egg-info/top_level.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)      156 2023-02-14 15:59:37.000000 imgviz-1.7.2/pyproject.toml
--rw-r--r--   0 wkentaro   (501) staff       (20)      151 2023-02-14 15:59:37.000000 imgviz-1.7.2/requirements.txt
--rw-r--r--   0 wkentaro   (501) staff       (20)      232 2023-02-14 18:15:31.345764 imgviz-1.7.2/setup.cfg
--rw-r--r--   0 wkentaro   (501) staff       (20)     4302 2023-02-14 15:59:37.000000 imgviz-1.7.2/setup.py
-drwxr-xr-x   0 wkentaro   (501) staff       (20)        0 2023-02-14 18:15:31.345278 imgviz-1.7.2/tests/
--rw-r--r--   0 wkentaro   (501) staff       (20)      624 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_centerize.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      252 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_depth.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      256 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_flow.py
--rw-r--r--   0 wkentaro   (501) staff       (20)     1200 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_label.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      574 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_resize.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      404 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_tile.py
--rw-r--r--   0 wkentaro   (501) staff       (20)      203 2023-02-14 15:59:37.000000 imgviz-1.7.2/tests/test_trajectory.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.902986 imgviz-1.7.3/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1075 2022-11-10 04:15:53.000000 imgviz-1.7.3/LICENSE
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       75 2022-11-10 04:15:53.000000 imgviz-1.7.3/MANIFEST.in
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     6547 2023-07-27 01:59:17.902986 imgviz-1.7.3/PKG-INFO
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     4434 2023-03-23 13:59:59.000000 imgviz-1.7.3/README.md
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.874986 imgviz-1.7.3/imgviz/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      816 2023-07-27 01:57:50.000000 imgviz-1.7.3/imgviz/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.874986 imgviz-1.7.3/imgviz/_io/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      292 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/_io/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.874986 imgviz-1.7.3/imgviz/_io/_pyglet/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       92 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/_io/_pyglet/__init__.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      244 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/_io/_pyglet/base.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     9432 2023-07-27 01:57:47.000000 imgviz-1.7.3/imgviz/_io/_pyglet/pyglet_imshow.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      184 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/_io/_pyglet/pyglet_run.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      842 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/_io/base.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      856 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/_io/opencv.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       86 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/_io/pil.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      661 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/_io/pyplot.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2031 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/centerize.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     5274 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/color.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.874986 imgviz-1.7.3/imgviz/data/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      158 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.878986 imgviz-1.7.3/imgviz/data/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      303 2023-03-23 13:57:41.000000 imgviz-1.7.3/imgviz/data/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.882986 imgviz-1.7.3/imgviz/data/arc2017/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      839 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/data/arc2017/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.882986 imgviz-1.7.3/imgviz/data/arc2017/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1107 2023-03-24 13:51:35.000000 imgviz-1.7.3/imgviz/data/arc2017/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      827 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/arc2017/camera_info.yaml
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      595 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/arc2017/class_names.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)   715747 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/arc2017/data.npz
+-rw-r--r--   0 mujin     (1000) mujin     (1000)  2849434 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/arc2017/res4.npz
+-rw-r--r--   0 mujin     (1000) mujin     (1000)    51017 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/arc2017/rgb.jpg
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.886986 imgviz-1.7.3/imgviz/data/kitti/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      699 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/data/kitti/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.886986 imgviz-1.7.3/imgviz/data/kitti/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1019 2023-03-24 13:51:35.000000 imgviz-1.7.3/imgviz/data/kitti/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.886986 imgviz-1.7.3/imgviz/data/kitti/odometry/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)   728871 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/kitti/odometry/00.txt
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.886986 imgviz-1.7.3/imgviz/data/lena/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      198 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/data/lena/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.886986 imgviz-1.7.3/imgviz/data/lena/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      440 2023-03-24 13:51:35.000000 imgviz-1.7.3/imgviz/data/lena/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mujin     (1000) mujin     (1000)   473831 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/lena/lena.png
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.894986 imgviz-1.7.3/imgviz/data/middlebury/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1071 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/data/middlebury/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.894986 imgviz-1.7.3/imgviz/data/middlebury/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1041 2023-03-24 13:51:35.000000 imgviz-1.7.3/imgviz/data/middlebury/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mujin     (1000) mujin     (1000)  2457612 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/middlebury/grove3.flo
+-rw-r--r--   0 mujin     (1000) mujin     (1000)   604275 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/middlebury/grove3.png
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.898986 imgviz-1.7.3/imgviz/data/voc/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      621 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/data/voc/__init__.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.898986 imgviz-1.7.3/imgviz/data/voc/__pycache__/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      895 2023-03-24 13:51:35.000000 imgviz-1.7.3/imgviz/data/voc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      146 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/voc/class_names.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)   436248 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/voc/data.npz
+-rw-r--r--   0 mujin     (1000) mujin     (1000)    42712 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/data/voc/rgb.jpg
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     3040 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/depth.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.898986 imgviz-1.7.3/imgviz/draw/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      582 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/draw/__init__.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1513 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/circle.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      765 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/ellipse.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      551 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/draw/line.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1471 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/rectangle.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2062 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/star.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2067 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/draw/text.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     4161 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/text_in_rectangle.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1453 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/draw/triangle.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      381 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/dtype.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.898986 imgviz-1.7.3/imgviz/external/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)        0 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/external/__init__.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)    69582 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/external/transformations.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2792 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/flow.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     4241 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/instances.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     6940 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/label.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     2405 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/nchannel.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1550 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/normalize.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     3481 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/resize.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     3662 2022-11-20 23:55:37.000000 imgviz-1.7.3/imgviz/tile.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1573 2023-03-23 13:59:59.000000 imgviz-1.7.3/imgviz/trajectory.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      303 2022-11-10 04:15:53.000000 imgviz-1.7.3/imgviz/utils.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.874986 imgviz-1.7.3/imgviz.egg-info/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     6547 2023-07-27 01:59:17.000000 imgviz-1.7.3/imgviz.egg-info/PKG-INFO
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1994 2023-07-27 01:59:17.000000 imgviz-1.7.3/imgviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)        1 2023-07-27 01:59:17.000000 imgviz-1.7.3/imgviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)       92 2023-07-27 01:59:17.000000 imgviz-1.7.3/imgviz.egg-info/requires.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)        7 2023-07-27 01:59:17.000000 imgviz-1.7.3/imgviz.egg-info/top_level.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      156 2022-11-10 04:15:53.000000 imgviz-1.7.3/pyproject.toml
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      151 2022-11-10 04:15:53.000000 imgviz-1.7.3/requirements.txt
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      232 2023-07-27 01:59:17.902986 imgviz-1.7.3/setup.cfg
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     4302 2022-11-20 23:55:37.000000 imgviz-1.7.3/setup.py
+drwxr-xr-x   0 mujin     (1000) mujin     (1000)        0 2023-07-27 01:59:17.902986 imgviz-1.7.3/tests/
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      624 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_centerize.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      252 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_depth.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      256 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_flow.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)     1200 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_label.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      574 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_resize.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      404 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_tile.py
+-rw-r--r--   0 mujin     (1000) mujin     (1000)      203 2022-11-10 04:15:53.000000 imgviz-1.7.3/tests/test_trajectory.py
```

### Comparing `imgviz-1.7.2/LICENSE` & `imgviz-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/PKG-INFO` & `imgviz-1.7.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: imgviz
-Version: 1.7.2
-Summary: Image Visualization Tools
-Home-page: http://github.com/wkentaro/imgviz
-Author: Kentaro Wada
-Author-email: www.kentaro.wada@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: all
-License-File: LICENSE
-
 <!-- DO NOT EDIT THIS FILE MANUALLY. This file is generated by generate_readme.py. -->
 
 <h1 align="center">
   imgviz
 </h1>
 
 <h4 align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: imgviz Version: 1.7.2 Summary: Image Visualization
-Tools Home-page: http://github.com/wkentaro/imgviz Author: Kentaro Wada Author-
-email: www.kentaro.wada@gmail.com License: MIT Classifier: Development Status
-:: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 2.7 Classifier: Programming Language ::
-Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Provides-Extra: all License-File: LICENSE
                              ****** imgviz ******
                        *** Image Visualization Tools ***
    [https://img.shields.io/pypi/v/imgviz.svg] [https://img.shields.io/pypi/
    pyversions/imgviz.svg] [https://github.com/wkentaro/imgviz/workflows/ci/
                        badge.svg] [Documentation_Status]
     Documentation | Installation | Getting_Started | Examples | C++_Version
```

### Comparing `imgviz-1.7.2/imgviz/__init__.py` & `imgviz-1.7.3/imgviz/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 
 from . import _io as io
 from . import data
 from . import draw
 from .centerize import centerize
 from .color import asgray
 from .color import asrgb
```

### Comparing `imgviz-1.7.2/imgviz/_io/_pyglet/pyglet_imshow.py` & `imgviz-1.7.3/imgviz/_io/_pyglet/pyglet_imshow.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     image = _convert_to_imagedata(images[index])
     sprite = pyglet.sprite.Sprite(image)
 
     def _post_image_update():
         filename = images[window.index].filename
         _centerize_sprite_in_window(sprite, window)
-        window.set_caption(filename)
+        window.set_caption("{} {}/{}".format(filename, window.index + 1, len(images)))
         print(
             filename,
             "{}/{}".format(window.index + 1, len(images)),
             file=sys.stderr,
         )
 
     _post_image_update()
@@ -232,20 +232,29 @@
 
     display = pyglet.canvas.Display()
     screen = display.get_default_screen()
 
     max_window_width = int(round(screen.width * 0.75))
     max_window_height = int(round(screen.height * 0.75))
 
+    # try to fit the image into the screen
     if aspect_ratio > 1:  # width > height
+        window_width = max_window_width
+        window_height = int(round(window_width / aspect_ratio))
+    else:
         window_height = max_window_height
         window_width = int(round(window_height * aspect_ratio))
-    else:
+
+    # if still too large, shrink it
+    if window_width > max_window_width:
         window_width = max_window_width
         window_height = int(round(window_width / aspect_ratio))
+    if window_height > max_window_height:
+        window_height = max_window_height
+        window_width = int(round(window_height * aspect_ratio))
 
     window = pyglet.window.Window(
         width=window_width,
         height=window_height,
         caption=caption,
     )
     return window
```

### Comparing `imgviz-1.7.2/imgviz/_io/base.py` & `imgviz-1.7.3/imgviz/_io/base.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/_io/opencv.py` & `imgviz-1.7.3/imgviz/_io/opencv.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/_io/pyplot.py` & `imgviz-1.7.3/imgviz/_io/pyplot.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/centerize.py` & `imgviz-1.7.3/imgviz/centerize.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/color.py` & `imgviz-1.7.3/imgviz/color.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/__init__.py` & `imgviz-1.7.3/imgviz/data/arc2017/__init__.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/camera_info.yaml` & `imgviz-1.7.3/imgviz/data/arc2017/camera_info.yaml`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/class_names.txt` & `imgviz-1.7.3/imgviz/data/arc2017/class_names.txt`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/data.npz` & `imgviz-1.7.3/imgviz/data/arc2017/data.npz`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/res4.npz` & `imgviz-1.7.3/imgviz/data/arc2017/res4.npz`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/arc2017/rgb.jpg` & `imgviz-1.7.3/imgviz/data/arc2017/rgb.jpg`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/kitti/__init__.py` & `imgviz-1.7.3/imgviz/data/kitti/__init__.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/kitti/odometry/00.txt` & `imgviz-1.7.3/imgviz/data/kitti/odometry/00.txt`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/lena/lena.png` & `imgviz-1.7.3/imgviz/data/lena/lena.png`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/middlebury/__init__.py` & `imgviz-1.7.3/imgviz/data/middlebury/__init__.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/middlebury/grove3.flo` & `imgviz-1.7.3/imgviz/data/middlebury/grove3.flo`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/middlebury/grove3.png` & `imgviz-1.7.3/imgviz/data/middlebury/grove3.png`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/voc/__init__.py` & `imgviz-1.7.3/imgviz/data/voc/__init__.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/voc/data.npz` & `imgviz-1.7.3/imgviz/data/voc/data.npz`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/data/voc/rgb.jpg` & `imgviz-1.7.3/imgviz/data/voc/rgb.jpg`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/depth.py` & `imgviz-1.7.3/imgviz/depth.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/__init__.py` & `imgviz-1.7.3/imgviz/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/circle.py` & `imgviz-1.7.3/imgviz/draw/circle.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/ellipse.py` & `imgviz-1.7.3/imgviz/draw/ellipse.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/line.py` & `imgviz-1.7.3/imgviz/draw/line.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/rectangle.py` & `imgviz-1.7.3/imgviz/draw/rectangle.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/star.py` & `imgviz-1.7.3/imgviz/draw/star.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/text.py` & `imgviz-1.7.3/imgviz/draw/text.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/text_in_rectangle.py` & `imgviz-1.7.3/imgviz/draw/text_in_rectangle.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/draw/triangle.py` & `imgviz-1.7.3/imgviz/draw/triangle.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/external/transformations.py` & `imgviz-1.7.3/imgviz/external/transformations.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/flow.py` & `imgviz-1.7.3/imgviz/flow.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/instances.py` & `imgviz-1.7.3/imgviz/instances.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/label.py` & `imgviz-1.7.3/imgviz/label.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/nchannel.py` & `imgviz-1.7.3/imgviz/nchannel.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/normalize.py` & `imgviz-1.7.3/imgviz/normalize.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/resize.py` & `imgviz-1.7.3/imgviz/resize.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/tile.py` & `imgviz-1.7.3/imgviz/tile.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz/trajectory.py` & `imgviz-1.7.3/imgviz/trajectory.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/imgviz.egg-info/PKG-INFO` & `imgviz-1.7.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgviz
-Version: 1.7.2
+Version: 1.7.3
 Summary: Image Visualization Tools
 Home-page: http://github.com/wkentaro/imgviz
 Author: Kentaro Wada
 Author-email: www.kentaro.wada@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -37,24 +37,24 @@
   <a href="https://pypi.org/project/imgviz"><img src="https://img.shields.io/pypi/pyversions/imgviz.svg"></a>
   <a href="https://github.com/wkentaro/imgviz/actions"><img src="https://github.com/wkentaro/imgviz/workflows/ci/badge.svg"></a>
   <a href="https://imgviz.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/imgviz/badge/?version=latest" alt="Documentation Status" /></a>
 </div>
 
 <div align="center">
   <a href="https://imgviz.readthedocs.io/en/latest/?badge=latest"><b>Documentation</b></a> |
-  <a href="#installation"><b>Installation</b></a> |
-  <a href="#getting-started"><b>Getting Started</b></a> |
-  <a href="#examples"><b>Examples</b></a> |
+  <a href="https://github.com/wkentaro/imgviz/blob/main/#installation?raw=true"><b>Installation</b></a> |
+  <a href="https://github.com/wkentaro/imgviz/blob/main/#getting-started"><b>Getting Started</b></a> |
+  <a href="https://github.com/wkentaro/imgviz/blob/main/#examples"><b>Examples</b></a> |
   <a href="https://github.com/wkentaro/imgviz-cpp"><b>C++ Version</b></a>
 </div>
 
 <br/>
 
 <div align="center">
-  <img src=".readme/getting_started.jpg" width="95%">
+  <img src="https://github.com/wkentaro/imgviz/blob/main/.readme/getting_started.jpg?raw=true" width="95%">
 </div>
 
 ## Installation
 
 ```bash
 pip install imgviz
 
@@ -108,51 +108,51 @@
     [rgb, depthviz, labelviz, maskviz, insviz],
     shape=(1, 5),
     border=(255, 255, 255),
     border_width=5,
 )
 ```
 
-## [Examples](examples)
+## [Examples](https://github.com/wkentaro/imgviz/blob/main/examples)
 
 <table>
 	<tr>
-		<td><pre><a href="examples/centerize.py">examples/centerize.py</a></pre></td>
-		<td><img src="examples/.readme/centerize.jpg" width="53.333333333333336%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/centerize.py">examples/centerize.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/centerize.jpg?raw=true" width="53.333333333333336%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/depth2rgb.py">examples/depth2rgb.py</a></pre></td>
-		<td><img src="examples/.readme/depth2rgb.jpg" width="78.16091954022988%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/depth2rgb.py">examples/depth2rgb.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/depth2rgb.jpg?raw=true" width="78.16091954022988%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/draw.py">examples/draw.py</a></pre></td>
-		<td><img src="examples/.readme/draw.jpg" width="37.79047619047619%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/draw.py">examples/draw.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/draw.jpg?raw=true" width="37.79047619047619%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/flow2rgb.py">examples/flow2rgb.py</a></pre></td>
-		<td><img src="examples/.readme/flow2rgb.jpg" width="52.21052631578947%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/flow2rgb.py">examples/flow2rgb.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/flow2rgb.jpg?raw=true" width="52.21052631578947%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/instances2rgb.py">examples/instances2rgb.py</a></pre></td>
-		<td><img src="examples/.readme/instances2rgb.jpg" width="66.35451505016722%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/instances2rgb.py">examples/instances2rgb.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/instances2rgb.jpg?raw=true" width="66.35451505016722%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/label2rgb.py">examples/label2rgb.py</a></pre></td>
-		<td><img src="examples/.readme/label2rgb.jpg" width="76.01532567049807%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/label2rgb.py">examples/label2rgb.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/label2rgb.jpg?raw=true" width="76.01532567049807%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/nchannel2rgb.py">examples/nchannel2rgb.py</a></pre></td>
-		<td><img src="examples/.readme/nchannel2rgb.jpg" width="52.21052631578947%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/nchannel2rgb.py">examples/nchannel2rgb.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/nchannel2rgb.jpg?raw=true" width="52.21052631578947%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/plot_trajectory.py">examples/plot_trajectory.py</a></pre></td>
-		<td><img src="examples/.readme/plot_trajectory.jpg" width="26.86868686868687%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/plot_trajectory.py">examples/plot_trajectory.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/plot_trajectory.jpg?raw=true" width="26.86868686868687%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/resize.py">examples/resize.py</a></pre></td>
-		<td><img src="examples/.readme/resize.jpg" width="47.238095238095234%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/resize.py">examples/resize.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/resize.jpg?raw=true" width="47.238095238095234%" /></td>
 	</tr>
 	<tr>
-		<td><pre><a href="examples/tile.py">examples/tile.py</a></pre></td>
-		<td><img src="examples/.readme/tile.jpg" width="35.812274368231044%" /></td>
+		<td><pre><a href="https://github.com/wkentaro/imgviz/blob/main/examples/tile.py">examples/tile.py</a></pre></td>
+		<td><img src="https://github.com/wkentaro/imgviz/blob/main/examples/.readme/tile.jpg?raw=true" width="35.812274368231044%" /></td>
 	</tr>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imgviz Version: 1.7.2 Summary: Image Visualization
+Metadata-Version: 2.1 Name: imgviz Version: 1.7.3 Summary: Image Visualization
 Tools Home-page: http://github.com/wkentaro/imgviz Author: Kentaro Wada Author-
 email: www.kentaro.wada@gmail.com License: MIT Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
@@ -13,15 +13,16 @@
                              ****** imgviz ******
                        *** Image Visualization Tools ***
    [https://img.shields.io/pypi/v/imgviz.svg] [https://img.shields.io/pypi/
    pyversions/imgviz.svg] [https://github.com/wkentaro/imgviz/workflows/ci/
                        badge.svg] [Documentation_Status]
     Documentation | Installation | Getting_Started | Examples | C++_Version
 
-                         [.readme/getting_started.jpg]
+            [https://github.com/wkentaro/imgviz/blob/main/.readme/
+                         getting_started.jpg?raw=true]
 ## Installation ```bash pip install imgviz # there are optional dependencies
 like skimage, below installs all. pip install imgviz[all] ``` ## Dependencies -
 [matplotlib](https://pypi.org/project/matplotlib) - [numpy](https://pypi.org/
 project/numpy) - [Pillow>=5.3.0](https://pypi.org/project/Pillow) - [PyYAML]
 (https://pypi.org/project/PyYAML) ## Getting Started ```python #
 getting_started.py import imgviz # sample data of rgb, depth, class label and
 instance masks data = imgviz.data.arc2017() rgb = data["rgb"] gray =
@@ -33,18 +34,29 @@
 data["labels"] masks = data["masks"] == 1 captions = [data["class_names"][l]
 for l in labels] maskviz = imgviz.instances2rgb(gray, masks=masks,
 labels=labels, captions=captions) # tile instance masks insviz = [(rgb * m[:,
 :, None])[b[0] : b[2], b[1] : b[3]] for b, m in zip(bboxes, masks)] insviz =
 imgviz.tile(imgs=insviz, border=(255, 255, 255)) insviz = imgviz.resize(insviz,
 height=rgb.shape[0]) # tile visualization tiled = imgviz.tile( [rgb, depthviz,
 labelviz, maskviz, insviz], shape=(1, 5), border=(255, 255, 255),
-border_width=5, ) ``` ## [Examples](examples)
-examples/centerize.py       [examples/.readme/centerize.jpg]
-examples/depth2rgb.py       [examples/.readme/depth2rgb.jpg]
-examples/draw.py            [examples/.readme/draw.jpg]
-examples/flow2rgb.py        [examples/.readme/flow2rgb.jpg]
-examples/instances2rgb.py   [examples/.readme/instances2rgb.jpg]
-examples/label2rgb.py       [examples/.readme/label2rgb.jpg]
-examples/nchannel2rgb.py    [examples/.readme/nchannel2rgb.jpg]
-examples/plot_trajectory.py [examples/.readme/plot_trajectory.jpg]
-examples/resize.py          [examples/.readme/resize.jpg]
-examples/tile.py            [examples/.readme/tile.jpg]
+border_width=5, ) ``` ## [Examples](https://github.com/wkentaro/imgviz/blob/
+main/examples)
+examples/centerize.py       [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/centerize.jpg?raw=true]
+examples/depth2rgb.py       [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/depth2rgb.jpg?raw=true]
+examples/draw.py            [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/draw.jpg?raw=true]
+examples/flow2rgb.py        [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/flow2rgb.jpg?raw=true]
+examples/instances2rgb.py   [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/instances2rgb.jpg?raw=true]
+examples/label2rgb.py       [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/label2rgb.jpg?raw=true]
+examples/nchannel2rgb.py    [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/nchannel2rgb.jpg?raw=true]
+examples/plot_trajectory.py [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/plot_trajectory.jpg?raw=true]
+examples/resize.py          [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/resize.jpg?raw=true]
+examples/tile.py            [https://github.com/wkentaro/imgviz/blob/main/
+                            examples/.readme/tile.jpg?raw=true]
```

### Comparing `imgviz-1.7.2/imgviz.egg-info/SOURCES.txt` & `imgviz-1.7.3/imgviz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,31 +30,37 @@
 imgviz/_io/pil.py
 imgviz/_io/pyplot.py
 imgviz/_io/_pyglet/__init__.py
 imgviz/_io/_pyglet/base.py
 imgviz/_io/_pyglet/pyglet_imshow.py
 imgviz/_io/_pyglet/pyglet_run.py
 imgviz/data/__init__.py
+imgviz/data/__pycache__/__init__.cpython-39.pyc
 imgviz/data/arc2017/__init__.py
 imgviz/data/arc2017/camera_info.yaml
 imgviz/data/arc2017/class_names.txt
 imgviz/data/arc2017/data.npz
 imgviz/data/arc2017/res4.npz
 imgviz/data/arc2017/rgb.jpg
+imgviz/data/arc2017/__pycache__/__init__.cpython-39.pyc
 imgviz/data/kitti/__init__.py
+imgviz/data/kitti/__pycache__/__init__.cpython-39.pyc
 imgviz/data/kitti/odometry/00.txt
 imgviz/data/lena/__init__.py
 imgviz/data/lena/lena.png
+imgviz/data/lena/__pycache__/__init__.cpython-39.pyc
 imgviz/data/middlebury/__init__.py
 imgviz/data/middlebury/grove3.flo
 imgviz/data/middlebury/grove3.png
+imgviz/data/middlebury/__pycache__/__init__.cpython-39.pyc
 imgviz/data/voc/__init__.py
 imgviz/data/voc/class_names.txt
 imgviz/data/voc/data.npz
 imgviz/data/voc/rgb.jpg
+imgviz/data/voc/__pycache__/__init__.cpython-39.pyc
 imgviz/draw/__init__.py
 imgviz/draw/circle.py
 imgviz/draw/ellipse.py
 imgviz/draw/line.py
 imgviz/draw/rectangle.py
 imgviz/draw/star.py
 imgviz/draw/text.py
```

### Comparing `imgviz-1.7.2/setup.py` & `imgviz-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/tests/test_centerize.py` & `imgviz-1.7.3/tests/test_centerize.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/tests/test_label.py` & `imgviz-1.7.3/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `imgviz-1.7.2/tests/test_resize.py` & `imgviz-1.7.3/tests/test_resize.py`

 * *Files identical despite different names*

