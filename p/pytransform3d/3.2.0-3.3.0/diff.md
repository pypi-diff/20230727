# Comparing `tmp/pytransform3d-3.2.0.tar.gz` & `tmp/pytransform3d-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransform3d-3.2.0.tar", last modified: Wed May 24 12:11:41 2023, max compression
+gzip compressed data, was "pytransform3d-3.3.0.tar", last modified: Thu Jul 27 08:03:27 2023, max compression
```

## Comparing `pytransform3d-3.2.0.tar` & `pytransform3d-3.3.0.tar`

### file list

```diff
@@ -1,81 +1,271 @@
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1653 2023-01-12 22:48:31.000000 pytransform3d-3.2.0/LICENSE
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       58 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/MANIFEST.in
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8884 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/README.md
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.793366 pytransform3d-3.2.0/pytransform3d/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       61 2023-05-24 12:06:02.000000 pytransform3d-3.2.0/pytransform3d/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21369 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/batch_rotations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2257 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/batch_rotations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11534 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/camera.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1268 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/camera.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3898 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/coordinates.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      462 2021-08-07 17:17:14.000000 pytransform3d-3.2.0/pytransform3d/coordinates.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13372 2022-02-11 10:41:03.000000 pytransform3d-3.2.0/pytransform3d/editor.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.797366 pytransform3d-3.2.0/pytransform3d/plot_utils/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      829 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10111 2022-12-22 19:37:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1692 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2606 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      373 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21851 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2656 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.797366 pytransform3d-3.2.0/pytransform3d/rotations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9185 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      407 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_constants.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    62106 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/rotations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7054 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_conversions.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3444 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      356 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8686 2022-02-11 10:43:44.000000 pytransform3d-3.2.0/pytransform3d/rotations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      683 2021-06-06 09:06:24.000000 pytransform3d-3.2.0/pytransform3d/rotations/_plot.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7689 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      718 2023-01-12 22:48:31.000000 pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5201 2022-02-11 10:41:03.000000 pytransform3d-3.2.0/pytransform3d/rotations/_rotors.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      748 2021-06-06 09:06:24.000000 pytransform3d-3.2.0/pytransform3d/rotations/_rotors.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5045 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/rotations/_slerp.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      688 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/rotations/_slerp.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4236 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      393 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_testing.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16625 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1736 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_utils.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19380 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/trajectories.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1618 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/trajectories.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19965 2023-05-24 12:05:13.000000 pytransform3d-3.2.0/pytransform3d/transform_manager.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2213 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/transform_manager.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/pytransform3d/transformations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3834 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    32766 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/transformations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2892 2021-05-23 13:02:30.000000 pytransform3d-3.2.0/pytransform3d/transformations/_conversions.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5540 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      517 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6006 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      360 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5945 2021-05-06 20:16:10.000000 pytransform3d-3.2.0/pytransform3d/transformations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      632 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_plot.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3489 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_random.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      406 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_random.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6100 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/transformations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      509 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_testing.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7271 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      952 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13510 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      888 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_utils.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17158 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/uncertainty.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1320 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/uncertainty.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28330 2022-12-22 19:37:52.000000 pytransform3d-3.2.0/pytransform3d/urdf.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3345 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/urdf.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/pytransform3d/visualizer/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      708 2023-02-11 17:57:50.000000 pytransform3d-3.2.0/pytransform3d/visualizer/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    37882 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5704 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_artists.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23163 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_figure.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4235 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_figure.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.793366 pytransform3d-3.2.0/pytransform3d.egg-info/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2620 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/SOURCES.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/dependency_links.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      158 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/requires.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       14 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/top_level.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      272 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/setup.cfg
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1399 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/setup.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.177996 pytransform3d-3.3.0/.circleci/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1151 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/.circleci/config.yml
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      388 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/.coveragerc
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.177996 pytransform3d-3.3.0/.github/
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.177996 pytransform3d-3.3.0/.github/workflows/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1345 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      143 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/.gitignore
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      460 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/.travis.yml
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      548 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/CITATION.cff
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3706 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/CONTRIBUTING.md
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1653 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/LICENSE
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       58 2023-04-27 13:57:59.000000 pytransform3d-3.3.0/MANIFEST.in
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9545 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/PKG-INFO
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     8872 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/README.md
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.177996 pytransform3d-3.3.0/doc/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6852 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/Makefile
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6724 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/make.bat
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.181995 pytransform3d-3.3.0/doc/source/
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.185995 pytransform3d-3.3.0/doc/source/_static/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    74598 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/accelerate_cylinder.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   253480 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/active_passive.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    98976 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/active_passive.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   848240 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/animation_dynamics.gif
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1445677 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/animation_kuka.gif
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  3522512 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/animation_nao.gif
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    93411 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/camera.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    14603 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/camera.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    60149 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/concatenate_uncertain_transforms.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13423 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_camera.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    11621 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_camera.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    30474 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_plane.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    14200 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_plane.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    49907 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_ship.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    20087 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/conventions_ship.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    30102 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/cylinders.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    36252 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/example_plot_box.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    82328 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/example_plot_screw.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3316 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/frame.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4744 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/frame.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    31386 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/graph.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   131501 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/kuka_trajectories.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     8257 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/doc/source/_static/logo.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    29356 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/doc/source/_static/logo.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   259797 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/photogrammetry.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2004 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/position.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3765 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/position.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13264 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/rotation.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    12056 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/rotation.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   219371 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/rotations.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    30270 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/rotations.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    79691 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/rotations_axis_angle.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17723 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/screw_axis.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13281 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/screw_axis.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17155 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/doc/source/_static/tf-trafo-over-time.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    88915 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/transform_graph.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     8523 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/transform_graph.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    61580 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/transform_manager_mesh.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    43212 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/transformation_modeling.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    19836 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_static/transformation_modeling.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   301497 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/transformations.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    68865 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/transformations.svg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    15998 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/translation.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7143 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/_static/translation.svg
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.185995 pytransform3d-3.3.0/doc/source/_templates/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      670 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_templates/class.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      811 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_templates/class_without_inherited.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      191 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/_templates/function.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      392 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/animations.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    19341 2023-07-27 07:32:04.000000 pytransform3d-3.3.0/doc/source/api.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2051 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/camera.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4630 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/conf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7878 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/euler_angles.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2830 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/doc/source/index.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1828 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/doc/source/install.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     8951 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/introduction.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    19616 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/rotations.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2186 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/transform_manager.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    16828 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/transformation_ambiguities.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1957 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/transformation_modeling.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2535 2023-07-27 07:32:04.000000 pytransform3d-3.3.0/doc/source/transformation_over_time.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    11969 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/doc/source/transformations.rst
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.185995 pytransform3d-3.3.0/examples/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      123 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/README.rst
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.185995 pytransform3d-3.3.0/examples/animations/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       43 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/animations/README.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3878 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/animations/animate_angle_axis_interpolation.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2274 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/animations/animate_quaternion_integration.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3884 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/animations/animate_quaternion_interpolation.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1044 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/animations/animate_rotation.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1440 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/animations/animate_trajectory.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.185995 pytransform3d-3.3.0/examples/apps/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       33 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/apps/README.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      843 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/apps/app_transformation_editor.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.189995 pytransform3d-3.3.0/examples/plots/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       37 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/plots/README.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      825 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_axis_angle.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1158 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_axis_angle_from_two_vectors.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      923 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_bivector.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      939 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_box.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      945 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_camera_3d.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1372 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_camera_projection.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1965 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_camera_trajectory.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1958 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_camera_with_image.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1076 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/plots/plot_collision_objects.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1022 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_compare_rotations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3610 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_concatenate_uncertain_transforms.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3080 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_convention_rotation_global_local.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      960 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_cylinder.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3443 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_dual_quaternion_interpolation.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      970 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_euler_angles.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1108 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_frames.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3096 2023-07-27 07:32:04.000000 pytransform3d-3.3.0/examples/plots/plot_interpolation_for_transform_manager.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2018 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_invert_uncertain_transform.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      843 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_matrix_from_two_vectors.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      779 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_mesh.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4324 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_pose_fusion.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      770 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_pose_trajectory.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      659 2023-02-28 08:50:26.000000 pytransform3d-3.3.0/examples/plots/plot_quaternion_integrate.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1897 2023-02-28 08:50:29.000000 pytransform3d-3.3.0/examples/plots/plot_quaternion_slerp.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1970 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_random_geometries.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      848 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_robot.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1414 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_rotate_cylinder.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1335 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_sample_rotations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      498 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_sample_transforms.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1707 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_screw.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      425 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_sphere.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1106 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_spheres.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      948 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_spherical_grid.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1955 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_straight_line_path.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      408 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_transform.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      833 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_transform_concatenation.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1106 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_transform_manager.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2673 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_urdf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1076 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/plots/plot_urdf_with_meshes.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      420 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/plots/plot_vector.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.189995 pytransform3d-3.3.0/examples/visualizations/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       35 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/visualizations/README.rst
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5960 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/examples/visualizations/render_urdf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1229 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_add_remove_artist.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      362 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_basis.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      559 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_box.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1016 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_camera_3d.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      342 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_capsule.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      332 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_cone.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      775 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_cylinder.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6095 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_ee_wrench.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      335 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_ellipsoid.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      830 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_mesh.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      728 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_basis.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2186 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_cylinder_with_wrench.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      822 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_line.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1431 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_robot.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1281 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_trajectory.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1381 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_moving_urdf_with_meshes.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      649 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_plane.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9180 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/examples/visualizations/vis_probabilistic_robot_kinematics.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      514 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_scatter.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      297 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_sphere.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2317 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_urdf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1143 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_urdf_with_meshes.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      422 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/examples/visualizations/vis_vector.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1263 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/manifest.xml
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.189995 pytransform3d-3.3.0/paper/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    79384 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/paper/app_transformation_editor.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2698 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/paper/paper.bib
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5775 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/paper/paper.md
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    40547 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/paper/plot_transform_manager.png
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    41667 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/paper/plot_urdf.png
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       61 2023-07-27 07:58:12.000000 pytransform3d-3.3.0/pytransform3d/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    21369 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/batch_rotations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2257 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/batch_rotations.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    11534 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/camera.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1268 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/camera.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3898 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/coordinates.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      462 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/coordinates.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13372 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/editor.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d/plot_utils/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      829 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    10111 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_artists.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1692 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_artists.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2606 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_layout.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      373 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_layout.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    21851 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_plot_functions.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2656 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/plot_utils/_plot_functions.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d/rotations/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9185 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      407 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_constants.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    62106 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/pytransform3d/rotations/_conversions.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7054 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/_conversions.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3444 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/_jacobians.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      356 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/_jacobians.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     8686 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_plot.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      683 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_plot.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7689 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/pytransform3d/rotations/_quaternion_operations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      718 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_quaternion_operations.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5201 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_rotors.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      748 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_rotors.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5045 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_slerp.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      688 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_slerp.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4236 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_testing.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      393 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/rotations/_testing.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    16625 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/_utils.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1736 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/rotations/_utils.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d/test/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    16996 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/test/test_batch_rotations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3213 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/test/test_camera.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3386 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/test/test_coordinates.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6412 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/test/test_plot_utils.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    78642 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/pytransform3d/test/test_rotations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    11538 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/test/test_trajectories.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    14300 2023-07-27 07:44:30.000000 pytransform3d-3.3.0/pytransform3d/test/test_transform_manager.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    34584 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/test/test_transformations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7263 2023-04-27 13:57:59.000000 pytransform3d-3.3.0/pytransform3d/test/test_uncertainty.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    31924 2023-07-20 12:18:17.000000 pytransform3d-3.3.0/pytransform3d/test/test_urdf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    19380 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/trajectories.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1618 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/trajectories.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d/transform_manager/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      639 2023-07-27 07:32:04.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6688 2023-07-27 07:36:27.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_temporal_transform_manager.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2342 2023-07-27 07:32:04.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_temporal_transform_manager.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9334 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_transform_graph_base.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1838 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_transform_graph_base.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    12608 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_transform_manager.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1975 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/transform_manager/_transform_manager.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/pytransform3d/transformations/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3834 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    32766 2023-04-27 13:57:59.000000 pytransform3d-3.3.0/pytransform3d/transformations/_conversions.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2892 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_conversions.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5540 2023-06-26 07:32:49.000000 pytransform3d-3.3.0/pytransform3d/transformations/_dual_quaternion_operations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      517 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_dual_quaternion_operations.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6006 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_jacobians.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      360 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_jacobians.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5945 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_plot.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      632 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_plot.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3489 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_random.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      406 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_random.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6100 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_testing.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      509 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_testing.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7271 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_transform_operations.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      952 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_transform_operations.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13510 2023-04-04 09:14:31.000000 pytransform3d-3.3.0/pytransform3d/transformations/_utils.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      888 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/transformations/_utils.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17158 2023-04-27 13:57:59.000000 pytransform3d-3.3.0/pytransform3d/uncertainty.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1320 2023-04-27 13:57:59.000000 pytransform3d-3.3.0/pytransform3d/uncertainty.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    28937 2023-07-20 12:15:56.000000 pytransform3d-3.3.0/pytransform3d/urdf.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3347 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/urdf.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/pytransform3d/visualizer/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      708 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/pytransform3d/visualizer/__init__.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    38633 2023-07-20 14:53:02.000000 pytransform3d-3.3.0/pytransform3d/visualizer/_artists.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5804 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/visualizer/_artists.pyi
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    23376 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/visualizer/_figure.py
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4293 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/pytransform3d/visualizer/_figure.pyi
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.193995 pytransform3d-3.3.0/pytransform3d.egg-info/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9545 2023-07-27 08:03:27.000000 pytransform3d-3.3.0/pytransform3d.egg-info/PKG-INFO
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9029 2023-07-27 08:03:27.000000 pytransform3d-3.3.0/pytransform3d.egg-info/SOURCES.txt
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)        1 2023-07-27 08:03:27.000000 pytransform3d-3.3.0/pytransform3d.egg-info/dependency_links.txt
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      143 2023-07-27 08:03:27.000000 pytransform3d-3.3.0/pytransform3d.egg-info/requires.txt
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       14 2023-07-27 08:03:27.000000 pytransform3d-3.3.0/pytransform3d.egg-info/top_level.txt
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       49 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/requirements.txt
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      272 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/setup.cfg
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1353 2023-07-20 11:59:37.000000 pytransform3d-3.3.0/setup.py
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.177996 pytransform3d-3.3.0/test/
+drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-07-27 08:03:27.197995 pytransform3d-3.3.0/test/test_data/
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6284 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/cone.stl
+-rwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)       65 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/reconstruction_camera_matrix.csv
+-rwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)    58765 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/reconstruction_odometry.csv
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3131 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/robot_with_visuals.urdf
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   378684 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/scan.stl
+-rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      933 2023-02-10 09:20:21.000000 pytransform3d-3.3.0/test/test_data/simple_mechanism.urdf
```

### Comparing `pytransform3d-3.2.0/LICENSE` & `pytransform3d-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/PKG-INFO` & `pytransform3d-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.2.0
+Version: 3.3.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -38,16 +38,15 @@
 * tight coupling with matplotlib to quickly visualize (or animate)
   transformations
 * the TransformManager which manages complex chains of transformations
   (with export to graph visualization as PNG, additionally requires pydot)
 * the TransformEditor which allows to modify transformations graphically
   (additionally requires PyQt4/5)
 * the UrdfTransformManager which is able to load transformations from
-  [URDF](https://wiki.ros.org/urdf) files (additionally requires
-  beautifulsoup4)
+  [URDF](https://wiki.ros.org/urdf) files (additionally requires lxml)
 * a matplotlib-like interface to Open3D's visualizer to display and animate
   geometries and transformations (additionally requires Open3D)
 
 pytransform3d is used in various domains, for example:
 
 * specifying motions of a robot
 * learning robot movements from human demonstration
```

### Comparing `pytransform3d-3.2.0/README.md` & `pytransform3d-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 * tight coupling with matplotlib to quickly visualize (or animate)
   transformations
 * the TransformManager which manages complex chains of transformations
   (with export to graph visualization as PNG, additionally requires pydot)
 * the TransformEditor which allows to modify transformations graphically
   (additionally requires PyQt4/5)
 * the UrdfTransformManager which is able to load transformations from
-  [URDF](https://wiki.ros.org/urdf) files (additionally requires
-  beautifulsoup4)
+  [URDF](https://wiki.ros.org/urdf) files (additionally requires lxml)
 * a matplotlib-like interface to Open3D's visualizer to display and animate
   geometries and transformations (additionally requires Open3D)
 
 pytransform3d is used in various domains, for example:
 
 * specifying motions of a robot
 * learning robot movements from human demonstration
```

### Comparing `pytransform3d-3.2.0/pytransform3d/batch_rotations.py` & `pytransform3d-3.3.0/pytransform3d/batch_rotations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/batch_rotations.pyi` & `pytransform3d-3.3.0/pytransform3d/batch_rotations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/camera.py` & `pytransform3d-3.3.0/pytransform3d/camera.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/camera.pyi` & `pytransform3d-3.3.0/pytransform3d/camera.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/coordinates.py` & `pytransform3d-3.3.0/pytransform3d/coordinates.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/editor.py` & `pytransform3d-3.3.0/pytransform3d/editor.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/__init__.py` & `pytransform3d-3.3.0/pytransform3d/plot_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.py` & `pytransform3d-3.3.0/pytransform3d/plot_utils/_artists.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.pyi` & `pytransform3d-3.3.0/pytransform3d/plot_utils/_artists.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.py` & `pytransform3d-3.3.0/pytransform3d/plot_utils/_layout.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.py` & `pytransform3d-3.3.0/pytransform3d/plot_utils/_plot_functions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.pyi` & `pytransform3d-3.3.0/pytransform3d/plot_utils/_plot_functions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/__init__.py` & `pytransform3d-3.3.0/pytransform3d/rotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_conversions.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_conversions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_conversions.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_conversions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_plot.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_plot.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_plot.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_quaternion_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_quaternion_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_rotors.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_rotors.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_rotors.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_rotors.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_slerp.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_slerp.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_slerp.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_slerp.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_testing.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_utils.py` & `pytransform3d-3.3.0/pytransform3d/rotations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/rotations/_utils.pyi` & `pytransform3d-3.3.0/pytransform3d/rotations/_utils.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/trajectories.py` & `pytransform3d-3.3.0/pytransform3d/trajectories.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/trajectories.pyi` & `pytransform3d-3.3.0/pytransform3d/trajectories.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transform_manager.py` & `pytransform3d-3.3.0/pytransform3d/visualizer/_figure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,573 +1,738 @@
-"""Manage complex chains of transformations.
-
-See :doc:`transform_manager` for more information.
-"""
+"""Figure based on Open3D's visualizer."""
 import numpy as np
-import scipy.sparse as sp
-from scipy.sparse import csgraph
-try:  # pragma: no cover
-    import pydot
-    PYDOT_AVAILABLE = True
-except ImportError:
-    PYDOT_AVAILABLE = False
-from .transformations import (check_transform, invert_transform, concat,
-                              plot_transform)
-
-
-class TransformManager(object):
-    """Manage transformations between frames.
-
-    This is a simplified version of `ROS tf <http://wiki.ros.org/tf>`_ that
-    ignores the temporal aspect. A user can register transformations. The
-    shortest path between all frames will be computed internally which enables
-    us to provide transforms for any connected frames.
-
-    Suppose we know the transformations A2B, D2C, and B2C. The transform
-    manager can compute any transformation between the frames A, B, C and D.
-    For example, you can request the transformation that represents frame D in
-    frame A. The transformation manager will automatically concatenate the
-    transformations D2C, C2B, and B2A, where C2B and B2A are obtained by
-    inverting B2C and A2B respectively.
-
-    .. warning::
-
-        It is possible to introduce inconsistencies in the transformation
-        manager. Adding A2B and B2A with inconsistent values will result in
-        an invalid state because inconsistencies will not be checked. It seems
-        to be trivial in this simple case but can be computationally complex
-        for large graphs. You can check the consistency explicitly with
-        :func:`TransformManager.check_consistency`.
-
-    The TransformManager does not directly support serialization because
-    we don't want to decide for a specific format. However, it allows
-    conversion to a dict with only primitive types that is serializable,
-    for instance, as JSON. If a more compact format is required, binary
-    formats like msgpack can be used. Use :func:`TransformManager.to_dict`
-    and :func:`TransformManager.from_dict` for this purpose.
+import open3d as o3d
+from .. import rotations as pr
+from .. import transformations as pt
+from .. import trajectories as ptr
+from ._artists import (Line3D, PointCollection3D, Vector3D, Frame, Trajectory,
+                       Camera, Box, Sphere, Cylinder, Mesh, Ellipsoid, Capsule,
+                       Cone, Plane, Graph)
+
+
+class Figure:
+    """The top level container for all the plot elements.
+
+    You can close the visualizer with the keys `escape` or `q`.
 
     Parameters
     ----------
-    strict_check : bool, optional (default: True)
-        Raise a ValueError if the transformation matrix is not numerically
-        close enough to a real transformation matrix. Otherwise we print a
-        warning.
-
-    check : bool, optional (default: True)
-        Check if transformation matrices are valid and requested nodes exist,
-        which might significantly slow down some operations.
+    window_name : str, optional (default: Open3D)
+        Window title name.
+
+    width : int, optional (default: 1920)
+        Width of the window.
+
+    height : int, optional (default: 1080)
+        Height of the window.
+
+    with_key_callbacks : bool, optional (default: False)
+        Creates a visualizer that allows to register callbacks
+        for keys.
     """
-    def __init__(self, strict_check=True, check=True):
-        self.strict_check = strict_check
-        self.check = check
+    def __init__(self, window_name="Open3D", width=1920, height=1080,
+                 with_key_callbacks=False):
+        if with_key_callbacks:
+            self.visualizer = o3d.visualization.VisualizerWithKeyCallback()
+        else:
+            self.visualizer = o3d.visualization.Visualizer()
+        self.visualizer.create_window(
+            window_name=window_name, width=width, height=height)
 
-        self.transforms = {}
-        self.nodes = []
+    def add_geometry(self, geometry):
+        """Add geometry to visualizer.
 
-        # A pair (self.i[n], self.j[n]) represents indices of connected nodes
-        self.i = []
-        self.j = []
-        # We have to store the index n associated to a transformation to be
-        # able to remove the transformation later
-        self.transform_to_ij_index = {}
-        # Connection information as sparse matrix
-        self.connections = sp.csr_matrix((0, 0))
+        Parameters
+        ----------
+        geometry : Geometry
+            Open3D geometry.
+        """
+        self.visualizer.add_geometry(geometry)
 
-        # Result of shortest path algorithm:
-        # distance matrix (distance is the number of transformations)
-        self.dist = np.empty(0)
-        self.predecessors = np.empty(0, dtype=np.int32)
+    def _remove_geometry(self, geometry):
+        """Remove geometry to visualizer.
 
-        self._cached_shortest_paths = {}
+        .. warning::
 
-    def add_transform(self, from_frame, to_frame, A2B):
-        """Register a transformation.
+            This function is not public because the interface of the
+            underlying visualizer might change in the future causing the
+            signature of this function to change as well.
 
         Parameters
         ----------
-        from_frame : Hashable
-            Name of the frame for which the transformation is added in the
-            to_frame coordinate system
+        geometry : Geometry
+            Open3D geometry.
+        """
+        self.visualizer.remove_geometry(geometry)
 
-        to_frame : Hashable
-            Name of the frame in which the transformation is defined
+    def update_geometry(self, geometry):
+        """Indicate that geometry has been updated.
 
-        A2B : array-like, shape (4, 4)
-            Homogeneous matrix that represents the transformation from
-            'from_frame' to 'to_frame'
+        Parameters
+        ----------
+        geometry : Geometry
+            Open3D geometry.
+        """
+        self.visualizer.update_geometry(geometry)
 
-        Returns
-        -------
-        self : TransformManager
-            This object for chaining
+    def remove_artist(self, artist):
+        """Remove artist from visualizer.
+
+        Parameters
+        ----------
+        artist : Artist
+            Artist that should be removed from this figure.
         """
-        if self.check:
-            A2B = check_transform(A2B, strict_check=self.strict_check)
-        if from_frame not in self.nodes:
-            self.nodes.append(from_frame)
-        if to_frame not in self.nodes:
-            self.nodes.append(to_frame)
+        for g in artist.geometries:
+            self._remove_geometry(g)
 
-        transform_key = (from_frame, to_frame)
+    def set_line_width(self, line_width):
+        """Set render option line width.
 
-        recompute_shortest_path = False
-        if transform_key not in self.transforms:
-            ij_index = len(self.i)
-            self.i.append(self.nodes.index(from_frame))
-            self.j.append(self.nodes.index(to_frame))
-            self.transform_to_ij_index[transform_key] = ij_index
-            recompute_shortest_path = True
+        Note: this feature does not work in Open3D's visualizer at the
+        moment.
 
-        self.transforms[transform_key] = A2B
+        Parameters
+        ----------
+        line_width : float
+            Line width.
+        """
+        self.visualizer.get_render_option().line_width = line_width
+        self.visualizer.update_renderer()
+
+    def set_zoom(self, zoom):
+        """Set zoom.
+
+        Parameters
+        ----------
+        zoom : float
+            Zoom of the visualizer.
+        """
+        self.visualizer.get_view_control().set_zoom(zoom)
+
+    def animate(self, callback, n_frames, loop=False, fargs=()):
+        """Make animation with callback.
+
+        Parameters
+        ----------
+        callback : callable
+            Callback that will be called in a loop to update geometries.
+            The first input of the function will be the current frame
+            index from [0, `n_frames`). Further arguments can be given as
+            `fargs`. The function should return one artist object or a
+            list of artists that have been updated.
+
+        n_frames : int
+            Total number of frames.
 
-        if recompute_shortest_path:
-            self._recompute_shortest_path()
+        loop : bool, optional (default: False)
+            Run callback in an infinite loop.
 
-        return self
+        fargs : list, optional (default: [])
+            Arguments that will be passed to the callback.
 
-    def remove_transform(self, from_frame, to_frame):
-        """Remove a transformation.
+        Raises
+        ------
+        RuntimeError
+            When callback does not return any artists
+        """
+        initialized = False
+        window_open = True
+        while window_open and (loop or not initialized):
+            for i in range(n_frames):
+                drawn_artists = callback(i, *fargs)
+
+                if drawn_artists is None:
+                    raise RuntimeError(
+                        "The animation function must return a "
+                        "sequence of Artist objects.")
+                try:
+                    drawn_artists = [a for a in drawn_artists]
+                except TypeError:
+                    drawn_artists = [drawn_artists]
+
+                for a in drawn_artists:
+                    for geometry in a.geometries:
+                        self.update_geometry(geometry)
+
+                window_open = self.visualizer.poll_events()
+                if not window_open:
+                    break
+                self.visualizer.update_renderer()
+            initialized = True
 
-        Nothing happens if there is no such transformation.
+    def view_init(self, azim=-60, elev=30):
+        """Set the elevation and azimuth of the axes.
 
         Parameters
         ----------
-        from_frame : Hashable
-            Name of the frame for which the transformation is added in the
-            to_frame coordinate system
+        azim : float, optional (default: -60)
+            Azimuth angle in the x,y plane in degrees.
+
+        elev : float, optional (default: 30)
+            Elevation angle in the z plane.
+        """
+        vc = self.visualizer.get_view_control()
+        pcp = vc.convert_to_pinhole_camera_parameters()
+        distance = np.linalg.norm(pcp.extrinsic[:3, 3])
+        R_azim_elev_0_world2camera = np.array([
+            [0, 1, 0],
+            [0, 0, -1],
+            [-1, 0, 0]])
+        R_azim_elev_0_camera2world = R_azim_elev_0_world2camera.T
+        # azimuth and elevation are defined in world frame
+        R_azim = pr.active_matrix_from_angle(2, np.deg2rad(azim))
+        R_elev = pr.active_matrix_from_angle(1, np.deg2rad(-elev))
+        R_elev_azim_camera2world = R_azim.dot(R_elev).dot(
+            R_azim_elev_0_camera2world)
+        pcp.extrinsic = pt.transform_from(  # world2camera
+            R=R_elev_azim_camera2world.T,
+            p=[0, 0, distance])
+        vc.convert_from_pinhole_camera_parameters(pcp)
 
-        to_frame : Hashable
-            Name of the frame in which the transformation is defined
+    def plot(self, P, c=(0, 0, 0)):
+        """Plot line.
+
+        Parameters
+        ----------
+        P : array-like, shape (n_points, 3)
+            Points of which the line consists.
+
+        c : array-like, shape (n_points - 1, 3) or (3,), optional (default: black)
+            Color can be given as individual colors per line segment or
+            as one color for each segment. A color is represented by 3
+            values between 0 and 1 indicate representing red, green, and
+            blue respectively.
 
         Returns
         -------
-        self : TransformManager
-            This object for chaining
+        line : Line3D
+            New line.
         """
-        transform_key = (from_frame, to_frame)
-        if transform_key in self.transforms:
-            del self.transforms[transform_key]
-            ij_index = self.transform_to_ij_index[transform_key]
-            del self.transform_to_ij_index[transform_key]
-            self.transform_to_ij_index = dict(
-                (k, v if v < ij_index else v - 1)
-                for k, v in self.transform_to_ij_index.items())
-            del self.i[ij_index]
-            del self.j[ij_index]
-            self._recompute_shortest_path()
-        return self
-
-    def _recompute_shortest_path(self):
-        n_nodes = len(self.nodes)
-        self.connections = sp.csr_matrix(
-            (np.zeros(len(self.i)), (self.i, self.j)),
-            shape=(n_nodes, n_nodes))
-        self.dist, self.predecessors = csgraph.shortest_path(
-            self.connections, unweighted=True, directed=False, method="D",
-            return_predecessors=True)
-        self._cached_shortest_paths.clear()
+        line3d = Line3D(P, c)
+        line3d.add_artist(self)
+        return line3d
 
-    def has_frame(self, frame):
-        """Check if frame has been registered.
+    def scatter(self, P, s=0.05, c=None):
+        """Plot collection of points.
 
         Parameters
         ----------
-        frame : Hashable
-            Frame name
+        P : array, shape (n_points, 3)
+            Points
+
+        s : float, optional (default: 0.05)
+            Scaling of the spheres that will be drawn.
+
+        c : array-like, shape (3,) or (n_points, 3), optional (default: black)
+            A color is represented by 3 values between 0 and 1 indicate
+            representing red, green, and blue respectively.
 
         Returns
         -------
-        has_frame : bool
-            Frame is registered
+        point_collection : PointCollection3D
+            New point collection.
         """
-        return frame in self.nodes
+        point_collection = PointCollection3D(P, s, c)
+        point_collection.add_artist(self)
+        return point_collection
 
-    def get_transform(self, from_frame, to_frame):
-        """Request a transformation.
+    def plot_vector(self, start=np.zeros(3), direction=np.array([1, 0, 0]),
+                    c=(0, 0, 0)):
+        """Plot vector.
 
         Parameters
         ----------
-        from_frame : Hashable
-            Name of the frame for which the transformation is requested in the
-            to_frame coordinate system
+        start : array-like, shape (3,), optional (default: [0, 0, 0])
+            Start of the vector
+
+        direction : array-like, shape (3,), optional (default: [1, 0, 0])
+            Direction of the vector
 
-        to_frame : Hashable
-            Name of the frame in which the transformation is defined
+        c : array-like, shape (3,), optional (default: black)
+            A color is represented by 3 values between 0 and 1 indicate
+            representing red, green, and blue respectively.
 
         Returns
         -------
-        A2B : array-like, shape (4, 4)
-            Homogeneous matrix that represents the transformation from
-            'from_frame' to 'to_frame'
+        vector : Vector3D
+            New vector.
+        """
+        vector3d = Vector3D(start, direction, c)
+        vector3d.add_artist(self)
+        return vector3d
 
-        Raises
-        ------
-        KeyError
-            If one of the frames is unknown or there is no connection between
-            them
-        """
-        if self.check:
-            if from_frame not in self.nodes:
-                raise KeyError("Unknown frame '%s'" % from_frame)
-            if to_frame not in self.nodes:
-                raise KeyError("Unknown frame '%s'" % to_frame)
-
-        if (from_frame, to_frame) in self.transforms:
-            return self.transforms[(from_frame, to_frame)]
-
-        if (to_frame, from_frame) in self.transforms:
-            return invert_transform(
-                self.transforms[(to_frame, from_frame)],
-                strict_check=self.strict_check, check=self.check)
-
-        i = self.nodes.index(from_frame)
-        j = self.nodes.index(to_frame)
-        if not np.isfinite(self.dist[i, j]):
-            raise KeyError("Cannot compute path from frame '%s' to "
-                           "frame '%s'." % (from_frame, to_frame))
-
-        path = self._shortest_path(i, j)
-        return self._path_transform(path)
-
-    def _shortest_path(self, i, j):
-        if (i, j) in self._cached_shortest_paths:
-            return self._cached_shortest_paths[(i, j)]
-
-        path = []
-        k = i
-        while k != -9999:
-            path.append(self.nodes[k])
-            k = self.predecessors[j, k]
-        self._cached_shortest_paths[(i, j)] = path
-        return path
-
-    def _path_transform(self, path):
-        A2B = np.eye(4)
-        for from_f, to_f in zip(path[:-1], path[1:]):
-            A2B = concat(A2B, self.get_transform(from_f, to_f),
-                         strict_check=self.strict_check, check=self.check)
-        return A2B
-
-    def plot_frames_in(self, frame, ax=None, s=1.0, ax_s=1, show_name=True,
-                       whitelist=None, **kwargs):  # pragma: no cover
-        """Plot all frames in a given reference frame.
-
-        Note that frames that cannot be connected to the reference frame are
-        omitted.
+    def plot_basis(self, R=None, p=np.zeros(3), s=1.0, strict_check=True):
+        """Plot basis.
 
         Parameters
         ----------
-        frame : Hashable
-            Reference frame
+        R : array-like, shape (3, 3), optional (default: I)
+            Rotation matrix, each column contains a basis vector
 
-        ax : Matplotlib 3d axis, optional (default: None)
-            If the axis is None, a new 3d axis will be created
+        p : array-like, shape (3,), optional (default: [0, 0, 0])
+            Offset from the origin
 
         s : float, optional (default: 1)
             Scaling of the frame that will be drawn
 
-        ax_s : float, optional (default: 1)
-            Scaling of the new matplotlib 3d axis
+        strict_check : bool, optional (default: True)
+            Raise a ValueError if the rotation matrix is not numerically
+            close enough to a real rotation matrix. Otherwise we print a
+            warning.
+
+        Returns
+        -------
+        Frame : frame
+            New frame.
+        """
+        if R is None:
+            R = np.eye(3)
+        R = pr.check_matrix(R, strict_check=strict_check)
+
+        frame = Frame(pt.transform_from(R=R, p=p), s=s)
+        frame.add_artist(self)
+
+        return frame
 
-        show_name : bool, optional (default: True)
-            Print node names
+    def plot_transform(self, A2B=None, s=1.0, name=None, strict_check=True):
+        """Plot coordinate frame.
 
-        whitelist : list, optional (default: None)
-            Frames that must be plotted
+        Parameters
+        ----------
+        A2B : array-like, shape (4, 4)
+            Transform from frame A to frame B
 
-        kwargs : dict, optional (default: {})
-            Additional arguments for the plotting functions, e.g. alpha
+        s : float, optional (default: 1)
+            Length of basis vectors
+
+        name : str, optional (default: None)
+            Name of the frame
+
+        strict_check : bool, optional (default: True)
+            Raise a ValueError if the transformation matrix is not
+            numerically close enough to a real transformation matrix.
+            Otherwise we print a warning.
 
         Returns
         -------
-        ax : Matplotlib 3d axis
-            New or old axis
-
-        Raises
-        ------
-        KeyError
-            If the frame is unknown
+        Frame : frame
+            New frame.
         """
-        if frame not in self.nodes:
-            raise KeyError("Unknown frame '%s'" % frame)
+        if A2B is None:
+            A2B = np.eye(4)
+        A2B = pt.check_transform(A2B, strict_check=strict_check)
 
-        nodes = self._whitelisted_nodes(whitelist)
+        frame = Frame(A2B, name, s)
+        frame.add_artist(self)
 
-        for node in nodes:
-            try:
-                node2frame = self.get_transform(node, frame)
-                name = node if show_name else None
-                ax = plot_transform(
-                    ax, node2frame, s, ax_s, name,
-                    strict_check=self.strict_check, **kwargs)
-            except KeyError:
-                pass  # Frame is not connected to the reference frame
-        return ax
+        return frame
 
-    def plot_connections_in(self, frame, ax=None, ax_s=1, whitelist=None,
-                            **kwargs):  # pragma: no cover
-        """Plot direct frame connections in a given reference frame.
+    def plot_trajectory(self, P, n_frames=10, s=1.0, c=(0, 0, 0)):
+        """Trajectory of poses.
 
-        A line between each pair of frames for which a direct transformation
-        is known will be plotted. Direct means that either A2B or B2A has been
-        added to the transformation manager.
+        Parameters
+        ----------
+        P : array-like, shape (n_steps, 7), optional (default: None)
+            Sequence of poses represented by positions and quaternions in
+            the order (x, y, z, w, vx, vy, vz) for each step
+
+        n_frames : int, optional (default: 10)
+            Number of frames that should be plotted to indicate the
+            rotation
+
+        s : float, optional (default: 1)
+            Scaling of the frames that will be drawn
 
-        Note that frames that cannot be connected to the reference frame are
-        omitted.
+        c : array-like, shape (3,), optional (default: black)
+            A color is represented by 3 values between 0 and 1 indicate
+            representing red, green, and blue respectively.
+
+        Returns
+        -------
+        trajectory : Trajectory
+            New trajectory.
+        """
+        H = ptr.matrices_from_pos_quat(P)
+        trajectory = Trajectory(H, n_frames, s, c)
+        trajectory.add_artist(self)
+        return trajectory
+
+    def plot_sphere(self, radius=1.0, A2B=np.eye(4), resolution=20, c=None):
+        """Plot sphere.
 
         Parameters
         ----------
-        frame : Hashable
-            Reference frame
+        radius : float, optional (default: 1)
+            Radius of the sphere
 
-        ax : Matplotlib 3d axis, optional (default: None)
-            If the axis is None, a new 3d axis will be created
-
-        ax_s : float, optional (default: 1)
-            Scaling of the new matplotlib 3d axis
+        A2B : array-like, shape (4, 4)
+            Transform from frame A to frame B
 
-        whitelist : list, optional (default: None)
-            Both frames of a connection must be in the whitelist to plot the
-            connection
+        resolution : int, optional (default: 20)
+            The resolution of the sphere. The longitudes will be split into
+            resolution segments (i.e. there are resolution + 1 latitude
+            lines including the north and south pole). The latitudes will
+            be split into 2 * resolution segments (i.e. there are
+            2 * resolution longitude lines.)
 
-        kwargs : dict, optional (default: {})
-            Additional arguments for the plotting functions, e.g. alpha
+        c : array-like, shape (3,), optional (default: None)
+            Color
 
         Returns
         -------
-        ax : Matplotlib 3d axis
-            New or old axis
-
-        Raises
-        ------
-        KeyError
-            If the frame is unknown
+        sphere : Sphere
+            New sphere.
         """
-        if frame not in self.nodes:
-            raise KeyError("Unknown frame '%s'" % frame)
+        sphere = Sphere(radius, A2B, resolution, c)
+        sphere.add_artist(self)
+        return sphere
 
-        if ax is None:
-            from .plot_utils import make_3d_axis
-            ax = make_3d_axis(ax_s)
+    def plot_box(self, size=np.ones(3), A2B=np.eye(4), c=None):
+        """Plot box.
 
-        nodes = self._whitelisted_nodes(whitelist)
+        Parameters
+        ----------
+        size : array-like, shape (3,), optional (default: [1, 1, 1])
+            Size of the box per dimension
 
-        if "c" not in kwargs and "color" not in kwargs:
-            kwargs["color"] = "black"
+        A2B : array-like, shape (4, 4), optional (default: I)
+            Center of the box
 
-        for frame_names in self.transforms:
-            from_frame, to_frame = frame_names
-            if from_frame in nodes and to_frame in nodes:
-                try:
-                    from2ref = self.get_transform(from_frame, frame)
-                    to2ref = self.get_transform(to_frame, frame)
-                    ax.plot(
-                        (from2ref[0, 3], to2ref[0, 3]),
-                        (from2ref[1, 3], to2ref[1, 3]),
-                        (from2ref[2, 3], to2ref[2, 3]),
-                        **kwargs
-                    )
-                except KeyError:
-                    pass  # Frame is not connected to the reference frame
+        c : array-like, shape (3,), optional (default: None)
+            Color
 
-        return ax
+        Returns
+        -------
+        box : Box
+            New box.
+        """
+        box = Box(size, A2B, c)
+        box.add_artist(self)
+        return box
 
-    def _whitelisted_nodes(self, whitelist):
-        """Get whitelisted nodes.
+    def plot_cylinder(self, length=2.0, radius=1.0, A2B=np.eye(4),
+                      resolution=20, split=4, c=None):
+        """Plot cylinder.
 
         Parameters
         ----------
-        whitelist : list or None
-            Whitelist of frames
+        length : float, optional (default: 1)
+            Length of the cylinder.
+
+        radius : float, optional (default: 1)
+            Radius of the cylinder.
+
+        A2B : array-like, shape (4, 4)
+            Pose of the cylinder. The position corresponds to the center of the
+            line segment and the z-axis to the direction of the line segment.
+
+        resolution : int, optional (default: 20)
+            The circle will be split into resolution segments
+
+        split : int, optional (default: 4)
+            The height will be split into split segments
+
+        c : array-like, shape (3,), optional (default: None)
+            Color
 
         Returns
         -------
-        nodes : set
-            Existing whitelisted nodes
-
-        Raises
-        ------
-        KeyError
-            Will be raised if an unknown node is in the whitelist.
+        cylinder : Cylinder
+            New cylinder.
         """
-        nodes = set(self.nodes)
-        if whitelist is not None:
-            whitelist = set(whitelist)
-            nodes = nodes.intersection(whitelist)
-            nonwhitlisted_nodes = whitelist.difference(nodes)
-            if nonwhitlisted_nodes:
-                raise KeyError("Whitelist contains unknown nodes: '%s'"
-                               % nonwhitlisted_nodes)
-        return nodes
-
-    def check_consistency(self):
-        """Check consistency of the known transformations.
-
-        The complexity of this is between :math:`O(n^2)` and :math:`O(n^3)`,
-        where :math:`n` is the number of nodes. In graphs where each pair of
-        nodes is directly connected the complexity is :math:`O(n^2)`. In graphs
-        that are actually paths, the complexity is :math:`O(n^3)`.
+        cylinder = Cylinder(length, radius, A2B, resolution, split, c)
+        cylinder.add_artist(self)
+        return cylinder
+
+    def plot_mesh(self, filename, A2B=np.eye(4), s=np.ones(3), c=None):
+        """Plot mesh.
+
+        Parameters
+        ----------
+        filename : str
+            Path to mesh file
+
+        A2B : array-like, shape (4, 4)
+            Center of the mesh
+
+        s : array-like, shape (3,), optional (default: [1, 1, 1])
+            Scaling of the mesh that will be drawn
+
+        c : array-like, shape (n_vertices, 3) or (3,), optional (default: None)
+            Color(s)
 
         Returns
         -------
-        consistent : bool
-            Is the graph consistent, i.e. is A2B always the same as the inverse
-            of B2A?
-        """
-        consistent = True
-        for node1 in self.nodes:
-            for node2 in self.nodes:
-                try:
-                    node1_to_node2 = self.get_transform(node1, node2)
-                    node2_to_node1 = self.get_transform(node2, node1)
-                    node1_to_node2_inv = invert_transform(
-                        node2_to_node1, strict_check=self.strict_check,
-                        check=self.check)
-                    consistent = consistent and np.allclose(node1_to_node2,
-                                                            node1_to_node2_inv)
-                except KeyError:
-                    pass  # Frames are not connected
-        return consistent
+        mesh : Mesh
+            New mesh.
+        """
+        mesh = Mesh(filename, A2B, s, c)
+        mesh.add_artist(self)
+        return mesh
+
+    def plot_ellipsoid(self, radii=np.ones(3), A2B=np.eye(4), resolution=20,
+                       c=None):
+        """Plot ellipsoid.
+
+        Parameters
+        ----------
+        radii : array-like, shape (3,)
+            Radii along the x-axis, y-axis, and z-axis of the ellipsoid.
 
-    def connected_components(self):
-        """Get number of connected components.
+        A2B : array-like, shape (4, 4)
+            Transform from frame A to frame B
+
+        resolution : int, optional (default: 20)
+            The resolution of the ellipsoid. The longitudes will be split into
+            resolution segments (i.e. there are resolution + 1 latitude
+            lines including the north and south pole). The latitudes will
+            be split into 2 * resolution segments (i.e. there are
+            2 * resolution longitude lines.)
 
-        If the number is larger than 1 there will be frames without
-        connections.
+        c : array-like, shape (3,), optional (default: None)
+            Color
 
         Returns
         -------
-        n_connected_components : int
-            Number of connected components.
+        ellipsoid : Ellipsoid
+            New ellipsoid.
         """
-        return csgraph.connected_components(
-            self.connections, directed=False, return_labels=False)
+        ellipsoid = Ellipsoid(radii, A2B, resolution, c)
+        ellipsoid.add_artist(self)
+        return ellipsoid
 
-    def write_png(self, filename, prog=None):  # pragma: no cover
-        """Create PNG from dot graph of the transformations.
+    def plot_capsule(self, height=1, radius=1, A2B=np.eye(4), resolution=20,
+                     c=None):
+        """Plot capsule.
 
-        .. warning::
+        A capsule is the volume covered by a sphere moving along a line
+        segment.
+
+        Parameters
+        ----------
+        height : float, optional (default: 1)
+            Height of the capsule along its z-axis.
+
+        radius : float, optional (default: 1)
+            Radius of the capsule.
+
+        A2B : array-like, shape (4, 4)
+            Pose of the capsule. The position corresponds to the center of the
+            line segment and the z-axis to the direction of the line segment.
+
+        resolution : int, optional (default: 20)
+            The resolution of the capsule. The longitudes will be split into
+            resolution segments (i.e. there are resolution + 1 latitude lines
+            including the north and south pole). The latitudes will be split
+            into 2 * resolution segments (i.e. there are 2 * resolution
+            longitude lines.)
+
+        c : array-like, shape (3,), optional (default: None)
+            Color
 
-            Note that this method requires the Python package pydot and an
-            existing installation of graphviz on your system.
+        Returns
+        -------
+        capsule : Capsule
+            New capsule.
+        """
+        capsule = Capsule(height, radius, A2B, resolution, c)
+        capsule.add_artist(self)
+        return capsule
+
+    def plot_cone(self, height=1, radius=1, A2B=np.eye(4), resolution=20,
+                  c=None):
+        """Plot cone.
 
         Parameters
         ----------
-        filename : str
-            Name of the output file. Should end with '.png'.
+        height : float, optional (default: 1)
+            Height of the cone along its z-axis.
 
-        prog : str, optional (default: dot)
-            Name of GraphViz executable that can be found in the `$PATH` or
-            absolute path to GraphViz executable. Possible options are, for
-            example, 'dot', 'twopi', 'neato', 'circo', 'fdp', 'sfdp'.
+        radius : float, optional (default: 1)
+            Radius of the cone.
 
-        Raises
-        ------
-        ImportError
-            If pydot is not available
+        A2B : array-like, shape (4, 4)
+            Pose of the cone.
+
+        resolution : int, optional (default: 20)
+            The circle will be split into resolution segments.
+
+        c : array-like, shape (3,), optional (default: None)
+            Color
+
+        Returns
+        -------
+        cone : Cone
+            New cone.
         """
-        if not PYDOT_AVAILABLE:
-            raise ImportError("pydot must be installed to use this feature.")
+        cone = Cone(height, radius, A2B, resolution, c)
+        cone.add_artist(self)
+        return cone
 
-        graph = pydot.Dot(graph_type="graph")
-        frame_color = "#dd3322"
-        connection_color = "#d0d0ff"
-
-        for frame in self.nodes:
-            node = pydot.Node(
-                _dot_display_name(frame), style="filled",
-                fillcolor=frame_color, shape="egg")
-            graph.add_node(node)
-        for frames, A2B in self.transforms.items():
-            frame_a, frame_b = frames
-            connection_name = "%s to %s\n%s" % (
-                _dot_display_name(frame_a), _dot_display_name(frame_b),
-                str(np.round(A2B, 3)))
-            node = pydot.Node(
-                connection_name, style="filled", fillcolor=connection_color,
-                shape="note")
-            graph.add_node(node)
-            a_name = _dot_display_name(frame_a)
-            a_edge = pydot.Edge(connection_name, a_name, penwidth=3)
-            graph.add_edge(a_edge)
-            b_name = _dot_display_name(frame_b)
-            b_edge = pydot.Edge(connection_name, b_name, penwidth=3)
-            graph.add_edge(b_edge)
-
-        graph.write_png(filename, prog=prog)
-
-    def to_dict(self):
-        """Convert the transform manager to a dict that is serializable.
-
-        Returns
-        -------
-        tm_dict : dict
-            Serializable dict.
-        """
-        return {
-            "class": self.__class__.__name__,
-            "strict_check": self.strict_check,
-            "check": self.check,
-            "transforms": [(k, v.ravel().tolist())
-                           for k, v in self.transforms.items()],
-            "nodes": self.nodes,
-            "i": self.i,
-            "j": self.j,
-            "transform_to_ij_index": list(self.transform_to_ij_index.items()),
-            "connections": {
-                "data": self.connections.data.tolist(),
-                "indices": self.connections.indices.tolist(),
-                "indptr": self.connections.indptr.tolist()
-            },
-            "dist": self.dist.tolist(),
-            "predecessors": self.predecessors.tolist()
-        }
-
-    @staticmethod
-    def from_dict(tm_dict):
-        """Create transform manager from dict.
+    def plot_plane(self, normal=np.array([0.0, 0.0, 1.0]), d=None,
+                   point_in_plane=None, s=1.0, c=None):
+        """Plot plane.
 
         Parameters
         ----------
-        tm_dict : dict
-            Serializable dict.
+        normal : array-like, shape (3,), optional (default: [0, 0, 1])
+            Plane normal.
+
+        d : float, optional (default: None)
+            Distance to origin in Hesse normal form.
+
+        point_in_plane : array-like, shape (3,), optional (default: None)
+            Point in plane.
+
+        s : float, optional (default: 1)
+            Scaling of the plane that will be drawn.
+
+        c : array-like, shape (3,), optional (default: None)
+            Color.
 
         Returns
         -------
+        plane : Plane
+            New plane.
+        """
+        plane = Plane(normal, d, point_in_plane, s, c)
+        plane.add_artist(self)
+        return plane
+
+    def plot_graph(
+            self, tm, frame, show_frames=False, show_connections=False,
+            show_visuals=False, show_collision_objects=False,
+            show_name=False, whitelist=None,
+            convex_hull_of_collision_objects=False, s=1.0):
+        """Plot graph of connected frames.
+
+        Parameters
+        ----------
         tm : TransformManager
-            Deserialized transform manager.
+            Representation of the graph
+
+        frame : str
+            Name of the base frame in which the graph will be displayed
+
+        show_frames : bool, optional (default: False)
+            Show coordinate frames
+
+        show_connections : bool, optional (default: False)
+            Draw lines between frames of the graph
+
+        show_visuals : bool, optional (default: False)
+            Show visuals that are stored in the graph
+
+        show_collision_objects : bool, optional (default: False)
+            Show collision objects that are stored in the graph
+
+        show_name : bool, optional (default: False)
+            Show names of frames
+
+        whitelist : list, optional (default: all)
+            List of frames that should be displayed
+
+        convex_hull_of_collision_objects : bool, optional (default: False)
+            Show convex hull of collision objects.
+
+        s : float, optional (default: 1)
+            Scaling of the frames that will be drawn
+
+        Returns
+        -------
+        graph : Graph
+            New graph.
         """
-        strict_check = tm_dict.get("strict_check")
-        check = tm_dict.get("check")
-        tm = TransformManager(strict_check=strict_check, check=check)
-        tm.set_transform_manager_state(tm_dict)
-        return tm
-
-    def set_transform_manager_state(self, tm_dict):
-        """Set state of transform manager from dict.
+        graph = Graph(tm, frame, show_frames, show_connections,
+                      show_visuals, show_collision_objects, show_name,
+                      whitelist, convex_hull_of_collision_objects, s)
+        graph.add_artist(self)
+        return graph
+
+    def plot_camera(self, M, cam2world=None, virtual_image_distance=1,
+                    sensor_size=(1920, 1080), strict_check=True):
+        """Plot camera in world coordinates.
+
+        This function is inspired by Blender's camera visualization. It will
+        show the camera center, a virtual image plane, and the top of the
+        virtual image plane.
+
+        Parameters
+        ----------
+        M : array-like, shape (3, 3)
+            Intrinsic camera matrix that contains the focal lengths on the
+            diagonal and the center of the the image in the last column. It
+            does not matter whether values are given in meters or pixels as
+            long as the unit is the same as for the sensor size.
+
+        cam2world : array-like, shape (4, 4), optional (default: I)
+            Transformation matrix of camera in world frame. We assume that the
+            position is given in meters.
+
+        virtual_image_distance : float, optional (default: 1)
+            Distance from pinhole to virtual image plane that will be
+            displayed. We assume that this distance is given in meters. The
+            unit has to be consistent with the unit of the position in
+            cam2world.
+
+        sensor_size : array-like, shape (2,), optional (default: [1920, 1080])
+            Size of the image sensor: (width, height). It does not matter
+            whether values are given in meters or pixels as long as the unit is
+            the same as for the sensor size.
+
+        strict_check : bool, optional (default: True)
+            Raise a ValueError if the transformation matrix is not numerically
+            close enough to a real transformation matrix. Otherwise we print a
+            warning.
+
+        Returns
+        -------
+        camera : Camera
+            New camera.
+        """
+        camera = Camera(M, cam2world, virtual_image_distance, sensor_size,
+                        strict_check)
+        camera.add_artist(self)
+        return camera
+
+    def save_image(self, filename):
+        """Save rendered image to file.
 
         Parameters
         ----------
-        tm_dict : dict
-            Serializable dict.
-        """
-        transforms = tm_dict.get("transforms")
-        self.transforms = dict([
-            (tuple(k), np.array(v).reshape(4, 4)) for k, v in transforms])
-        self.nodes = tm_dict.get("nodes")
-        self.i = tm_dict.get("i")
-        self.j = tm_dict.get("j")
-        self.transform_to_ij_index = dict(
-            [(tuple(k), v) for k, v in tm_dict.get("transform_to_ij_index")])
-        connections = tm_dict.get("connections")
-        self.connections = sp.csr_matrix((
-            connections["data"], connections["indices"],
-            connections["indptr"]))
-        n_nodes = len(self.nodes)
-        dist = np.array(tm_dict.get("dist"))
-        self.dist = dist.reshape(n_nodes, n_nodes)
-        predecessors = np.array(tm_dict.get("predecessors"), dtype=np.int32)
-        self.predecessors = predecessors.reshape(n_nodes, n_nodes)
+        filename : str
+            Path to file in which the rendered image should be stored
+        """
+        self.visualizer.capture_screen_image(filename, True)
 
+    def show(self):
+        """Display the figure window."""
+        self.visualizer.run()
+        self.visualizer.destroy_window()
 
-def _dot_display_name(name):  # pragma: no cover
-    return name.replace("/", "")
+
+def figure(window_name="Open3D", width=1920, height=1080,
+           with_key_callbacks=False):
+    """Create a new figure.
+
+    Parameters
+    ----------
+    window_name : str, optional (default: Open3D)
+        Window title name.
+
+    width : int, optional (default: 1920)
+        Width of the window.
+
+    height : int, optional (default: 1080)
+        Height of the window.
+
+    with_key_callbacks : bool, optional (default: False)
+        Creates a visualizer that allows to register callbacks
+        for keys.
+
+    Returns
+    -------
+    figure : Figure
+        New figure.
+    """
+    return Figure(window_name, width, height, with_key_callbacks)
```

### Comparing `pytransform3d-3.2.0/pytransform3d/transform_manager.pyi` & `pytransform3d-3.3.0/pytransform3d/transform_manager/_transform_manager.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+from typing import Dict, Tuple, List, Union, Set, Hashable, Any
+
 import numpy as np
 import numpy.typing as npt
-import scipy.sparse as sp
 from mpl_toolkits.mplot3d import Axes3D
-from typing import Dict, Tuple, List, Union, Set, Hashable, Any
 
+from ._transform_graph_base import TransformGraphBase
+
+
+PYDOT_AVAILABLE: bool
 
-class TransformManager(object):
-    strict_check: bool
-    check: bool
-    transforms: Dict[Tuple[Hashable, Hashable], np.ndarray]
-    nodes: List[Hashable]
-    i: List[int]
-    j: List[int]
-    transform_to_ij_index = Dict[Tuple[Hashable, Hashable], int]
-    connections: sp.csr_matrix
-    dist: np.ndarray
-    predecessors: np.ndarray
-    _cached_shortest_paths: Dict[Tuple[int, int], List[Hashable]]
+
+class TransformManager(TransformGraphBase):
+    _transforms: Dict[Tuple[Hashable, Hashable], np.ndarray]
 
     def __init__(self, strict_check: bool = ..., check: bool = ...): ...
 
-    def add_transform(self, from_frame: Hashable, to_frame: Hashable,
-                      A2B: np.ndarray) -> "TransformManager": ...
+    @property
+    def transforms(self) -> Dict[Tuple[Hashable, Hashable], np.ndarray]: ...
+
+    def _check_transform(self, A2B: npt.ArrayLike) -> np.ndarray: ...
+
+    def _transform_available(self, key: Tuple[Hashable, Hashable]) -> bool: ...
 
-    def remove_transform(
-            self, from_frame: Hashable,
-            to_frame: Hashable) -> "TransformManager": ...
+    def _set_transform(self, key: Tuple[Hashable, Hashable], A2B: Any): ...
 
-    def has_frame(self, frame: Hashable) -> bool: ...
+    def _get_transform(self, key: Tuple[Hashable, Hashable]) -> Any: ...
+
+    def _del_transform(self, key: Tuple[Hashable, Hashable]): ...
+
+    def add_transform(self, from_frame: Hashable, to_frame: Hashable,
+                      A2B: np.ndarray) -> "TransformManager": ...
 
     def get_transform(self, from_frame: Hashable,
                       to_frame: Hashable) -> np.ndarray: ...
 
     def plot_frames_in(
             self, frame: Hashable, ax: Union[None, Axes3D] = ...,
             s: float = ..., ax_s: float = ..., show_name: bool = ...,
@@ -42,25 +44,15 @@
             ax_s: float = ...,
             whitelist: Union[List[Hashable], None] = ...,
             **kwargs) -> Axes3D: ...
 
     def _whitelisted_nodes(
             self, whitelist: Union[None, List[Hashable]]) -> Set[Hashable]: ...
 
-    def check_consistency(self) -> bool: ...
-
-    def connected_components(self) -> int: ...
-
     def write_png(self, filename: str, prog: Union[str, None] = ...): ...
 
-    def _recompute_shortest_path(self): ...
-
-    def _shortest_path(self, i: int, j: int) -> List[str]: ...
-
-    def _path_transform(self, path: List[Hashable]) -> np.ndarray: ...
-
     def to_dict(self) -> Dict[str, Any]: ...
 
     @staticmethod
     def from_dict(tm_dict: Dict[str, Any]) -> "TransformManager": ...
 
     def set_transform_manager_state(self, tm_dict: Dict[str, Any]): ...
```

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/__init__.py` & `pytransform3d-3.3.0/pytransform3d/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_conversions.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_conversions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_conversions.pyi` & `pytransform3d-3.3.0/pytransform3d/transformations/_conversions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_dual_quaternion_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.pyi` & `pytransform3d-3.3.0/pytransform3d/transformations/_dual_quaternion_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_plot.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_plot.pyi` & `pytransform3d-3.3.0/pytransform3d/transformations/_plot.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_random.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_random.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_testing.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_transform_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.pyi` & `pytransform3d-3.3.0/pytransform3d/transformations/_transform_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_utils.py` & `pytransform3d-3.3.0/pytransform3d/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/transformations/_utils.pyi` & `pytransform3d-3.3.0/pytransform3d/transformations/_utils.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/uncertainty.py` & `pytransform3d-3.3.0/pytransform3d/uncertainty.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/uncertainty.pyi` & `pytransform3d-3.3.0/pytransform3d/uncertainty.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/urdf.py` & `pytransform3d-3.3.0/pytransform3d/urdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Load transformations from URDF files.
 
 See :doc:`transform_manager` for more information.
 """
 import os
 import numpy as np
 import warnings
-from bs4 import BeautifulSoup
+from lxml import etree
 from .transform_manager import TransformManager
 from .transformations import transform_from, concat
 from .rotations import (
     active_matrix_from_extrinsic_roll_pitch_yaw, matrix_from_axis_angle,
     norm_vector)
 
 
@@ -19,15 +19,15 @@
     URDF is the `Unified Robot Description Format <http://wiki.ros.org/urdf>`_.
     URDF allows to define joints between links that can be rotated about one
     axis. This transformation manager allows to set the joint angles after
     joints have been added or loaded from an URDF.
 
     .. warning::
 
-        Note that this module requires the Python package beautifulsoup4.
+        Note that this module requires the Python package lxml.
 
     .. note::
 
         Joint angles must be given in radians.
 
     Parameters
     ----------
@@ -322,38 +322,46 @@
         Joints of the robot
 
     Raises
     ------
     UrdfException
         If URDF is not valid
     """
-    urdf = BeautifulSoup(urdf_xml, "xml")
+    # lxml does not allow whitespaces in the beginning
+    urdf_xml = urdf_xml.strip()
+    # lxml complains about unicode strings that start with unicode encoding
+    # declaration. Hence, we have to convert them to bytes first.
+    urdf_xml = bytes(urdf_xml.encode("utf-8"))
+    try:
+        root = etree.XML(urdf_xml, parser=etree.XMLParser(recover=True))
+    except etree.XMLSyntaxError:
+        raise UrdfException("Invalid XML.")
 
     # URDF XML schema:
     # https://github.com/ros/urdfdom/blob/master/xsd/urdf.xsd
 
-    robot = urdf.find("robot")
-    if robot is None:
+    if root.tag != "robot":
         raise UrdfException("Robot tag is missing.")
 
-    if not robot.has_attr("name"):
+    tree = etree.ElementTree(root)
+
+    if "name" not in root.attrib:
         raise UrdfException("Attribute 'name' is missing in robot tag.")
 
-    robot_name = robot["name"]
+    robot_name = root.attrib["name"]
 
-    materials = dict([
-        _parse_material(material)
-        for material in robot.findAll("material", recursive=False)])
+    materials = dict([_parse_material(material)
+                      for material in tree.findall("material")])
 
     links = [_parse_link(link, materials, mesh_path, package_dir, strict_check)
-             for link in robot.findAll("link", recursive=False)]
+             for link in tree.findall("link")]
 
     link_names = [link.name for link in links]
     joints = [_parse_joint(joint, link_names, strict_check)
-              for joint in robot.findAll("joint", recursive=False)]
+              for joint in tree.findall("joint")]
 
     return robot_name, links, joints
 
 
 def initialize_urdf_transform_manager(tm, robot_name, links, joints):
     """Initializes transform manager from previously parsed URDF data.
 
@@ -374,41 +382,41 @@
     tm.add_transform(links[0].name, robot_name, np.eye(4))
     _add_links(tm, links)
     _add_joints(tm, joints)
 
 
 def _parse_material(material):
     """Parse material."""
-    if not material.has_attr("name"):
+    if "name" not in material.attrib:
         raise UrdfException("Material name is missing.")
-    colors = material.findAll("color")
+    colors = material.findall("color")
     if len(colors) not in [0, 1]:
         raise UrdfException("More than one color is not allowed.")
     if len(colors) == 1:
         color = _parse_color(colors[0])
     else:
         color = None
     # TODO texture is currently ignored
-    return material["name"], color
+    return material.attrib["name"], color
 
 
 def _parse_color(color):
     """Parse color."""
-    if not color.has_attr("rgba"):
+    if "rgba" not in color.attrib:
         raise UrdfException("Attribute 'rgba' of color tag is missing.")
-    return np.fromstring(color["rgba"], sep=" ")
+    return np.fromstring(color.attrib["rgba"], sep=" ")
 
 
 def _parse_link(link, materials, mesh_path, package_dir, strict_check):
     """Create link."""
-    if not link.has_attr("name"):
+    if "name" not in link.attrib:
         raise UrdfException("Link name is missing.")
 
     result = Link()
-    result.name = link["name"]
+    result.name = link.attrib["name"]
 
     visuals, visual_transforms = _parse_link_children(
         link, "visual", materials, mesh_path, package_dir, strict_check)
     result.visuals = visuals
     result.transforms.extend(visual_transforms)
 
     collision_objects, collision_object_transforms = _parse_link_children(
@@ -427,47 +435,48 @@
 
     return result
 
 
 def _parse_link_children(link, child_type, materials, mesh_path, package_dir,
                          strict_check):
     """Parse collision objects or visuals."""
-    children = link.findAll(child_type)
+    children = link.findall(child_type)
     shape_objects = []
     transforms = []
     for i, child in enumerate(children):
-        if child.has_attr("name"):
-            name = "%s:%s/%s" % (child_type, link["name"], child["name"])
+        if "name" in child.attrib:
+            name = "%s:%s/%s" % (child_type, link.attrib["name"],
+                                 child.attrib["name"])
         else:
-            name = "%s:%s/%s" % (child_type, link["name"], i)
+            name = "%s:%s/%s" % (child_type, link.attrib["name"], i)
 
         color = None
         if child_type == "visual":
             material = child.find("material")
             if material is not None:
                 material_name, color = _parse_material(material)
                 if color is None and material_name in materials:
                     color = materials[material_name]
 
         child2link = _parse_origin(child, strict_check)
-        transforms.append((name, link["name"], child2link))
+        transforms.append((name, link.attrib["name"], child2link))
 
         shape_objects.extend(_parse_geometry(
             child, name, color, mesh_path, package_dir))
     return shape_objects, transforms
 
 
 def _parse_geometry(child, name, color, mesh_path, package_dir):
     """Parse geometric primitives (box, cylinder, sphere) or meshes."""
     geometry = child.find("geometry")
     if geometry is None:
         raise UrdfException("Missing geometry tag in link '%s'" % name)
     result = []
     for shape_type in ["box", "cylinder", "sphere", "mesh"]:
-        shapes = geometry.findAll(shape_type)
+        shapes = geometry.findall(shape_type)
         Cls = shape_classes[shape_type]
         for shape in shapes:
             shape_object = Cls(
                 name, mesh_path=mesh_path, package_dir=package_dir,
                 color=color)
             shape_object.parse(shape)
             result.append(shape_object)
@@ -476,133 +485,133 @@
 
 def _parse_origin(entry, strict_check):
     """Parse transformation."""
     origin = entry.find("origin")
     translation = np.zeros(3)
     rotation = np.eye(3)
     if origin is not None:
-        if origin.has_attr("xyz"):
-            translation = np.fromstring(origin["xyz"], sep=" ")
-        if origin.has_attr("rpy"):
-            roll_pitch_yaw = np.fromstring(origin["rpy"], sep=" ")
+        if "xyz" in origin.attrib:
+            translation = np.fromstring(origin.attrib["xyz"], sep=" ")
+        if "rpy" in origin.attrib:
+            roll_pitch_yaw = np.fromstring(origin.attrib["rpy"], sep=" ")
             # URDF and KDL use the active convention for rotation matrices.
             # For more details on how the URDF parser handles the
             # conversion from Euler angles, see this blog post:
             # https://orbitalstation.wordpress.com/tag/quaternion/
             rotation = active_matrix_from_extrinsic_roll_pitch_yaw(
                 roll_pitch_yaw)
     return transform_from(
         rotation, translation, strict_check=strict_check)
 
 
 def _parse_mass(inertial):
     """Parse link mass."""
     mass = inertial.find("mass")
-    if mass is not None and mass.has_attr("value"):
-        result = float(mass["value"])
+    if mass is not None and "value" in mass.attrib:
+        result = float(mass.attrib["value"])
     else:
         result = 0.0
     return result
 
 
 def _parse_inertia(inertial):
     """Parse inertia matrix."""
     inertia = inertial.find("inertia")
 
     result = np.zeros((3, 3))
     if inertia is None:
         return result
 
-    if inertia.has_attr("ixx"):
-        result[0, 0] = float(inertia["ixx"])
-    if inertia.has_attr("ixy"):
-        ixy = float(inertia["ixy"])
+    if "ixx" in inertia.attrib:
+        result[0, 0] = float(inertia.attrib["ixx"])
+    if "ixy" in inertia.attrib:
+        ixy = float(inertia.attrib["ixy"])
         result[0, 1] = ixy
         result[1, 0] = ixy
-    if inertia.has_attr("ixz"):
-        ixz = float(inertia["ixz"])
+    if "ixz" in inertia.attrib:
+        ixz = float(inertia.attrib["ixz"])
         result[0, 2] = ixz
         result[2, 0] = ixz
-    if inertia.has_attr("iyy"):
-        result[1, 1] = float(inertia["iyy"])
-    if inertia.has_attr("iyz"):
-        iyz = float(inertia["iyz"])
+    if "iyy" in inertia.attrib:
+        result[1, 1] = float(inertia.attrib["iyy"])
+    if "iyz" in inertia.attrib:
+        iyz = float(inertia.attrib["iyz"])
         result[1, 2] = iyz
         result[2, 1] = iyz
-    if inertia.has_attr("izz"):
-        result[2, 2] = float(inertia["izz"])
+    if "izz" in inertia.attrib:
+        result[2, 2] = float(inertia.attrib["izz"])
     return result
 
 
 def _parse_joint(joint, link_names, strict_check):
     """Create joint object."""
     j = Joint()
 
-    if not joint.has_attr("name"):
+    if "name" not in joint.attrib:
         raise UrdfException("Joint name is missing.")
-    j.joint_name = joint["name"]
+    j.joint_name = joint.attrib["name"]
 
-    if not joint.has_attr("type"):
+    if "type" not in joint.attrib:
         raise UrdfException("Joint type is missing in joint '%s'."
                             % j.joint_name)
 
     parent = joint.find("parent")
     if parent is None:
         raise UrdfException("No parent specified in joint '%s'"
                             % j.joint_name)
-    if not parent.has_attr("link"):
+    if "link" not in parent.attrib:
         raise UrdfException("No parent link name given in joint '%s'."
                             % j.joint_name)
-    j.parent = parent["link"]
+    j.parent = parent.attrib["link"]
     if j.parent not in link_names:
         raise UrdfException("Parent link '%s' of joint '%s' is not "
                             "defined." % (j.parent, j.joint_name))
 
     child = joint.find("child")
     if child is None:
         raise UrdfException("No child specified in joint '%s'"
                             % j.joint_name)
-    if not child.has_attr("link"):
+    if "link" not in child.attrib:
         raise UrdfException("No child link name given in joint '%s'."
                             % j.joint_name)
-    j.child = child["link"]
+    j.child = child.attrib["link"]
     if j.child not in link_names:
         raise UrdfException("Child link '%s' of joint '%s' is not "
                             "defined." % (j.child, j.joint_name))
 
-    j.joint_type = joint["type"]
+    j.joint_type = joint.attrib["type"]
 
     if j.joint_type in ["planar", "floating"]:
         raise UrdfException("Unsupported joint type '%s'" % j.joint_type)
     if j.joint_type not in ["revolute", "continuous", "prismatic",
                             "fixed"]:
         raise UrdfException("Joint type '%s' is not allowed in a URDF "
                             "document." % j.joint_type)
 
     j.child2parent = _parse_origin(joint, strict_check)
 
     j.joint_axis = np.array([1, 0, 0])
     if j.joint_type in ["revolute", "continuous", "prismatic"]:
         axis = joint.find("axis")
-        if axis is not None and axis.has_attr("xyz"):
-            j.joint_axis = np.fromstring(axis["xyz"], sep=" ")
+        if axis is not None and "xyz" in axis.attrib:
+            j.joint_axis = np.fromstring(axis.attrib["xyz"], sep=" ")
 
     j.limits = _parse_limits(joint)
     return j
 
 
 def _parse_limits(joint):
     """Parse joint limits."""
     limit = joint.find("limit")
     lower, upper = float("-inf"), float("inf")
     if limit is not None:
-        if limit.has_attr("lower"):
-            lower = float(limit["lower"])
-        if limit.has_attr("upper"):
-            upper = float(limit["upper"])
+        if "lower" in limit.attrib:
+            lower = float(limit.attrib["lower"])
+        if "upper" in limit.attrib:
+            upper = float(limit.attrib["upper"])
     return lower, upper
 
 
 def _add_links(tm, links):
     """Add previously parsed links.
 
     Parameters
@@ -748,16 +757,16 @@
     """Geometrical object: box."""
     def __init__(self, frame, mesh_path, package_dir, color):
         super(Box, self).__init__(frame, mesh_path, package_dir, color)
         self.size = np.zeros(3)
 
     def parse(self, xml):
         """Parse box size."""
-        if xml.has_attr("size"):
-            self.size[:] = np.fromstring(xml["size"], sep=" ")
+        if "size" in xml.attrib:
+            self.size[:] = np.fromstring(xml.attrib["size"], sep=" ")
 
     def plot(self, tm, frame, ax=None, alpha=0.3, wireframe=True,
              convex_hull=True):  # pragma: no cover
         """Plot box."""
         A2B = tm.get_transform(self.frame, frame)
         color = self.color if self.color is not None else "k"
         from .plot_utils import plot_box
@@ -769,17 +778,17 @@
     """Geometrical object: sphere."""
     def __init__(self, frame, mesh_path, package_dir, color):
         super(Sphere, self).__init__(frame, mesh_path, package_dir, color)
         self.radius = 0.0
 
     def parse(self, xml):
         """Parse sphere radius."""
-        if not xml.has_attr("radius"):
+        if "radius" not in xml.attrib:
             raise UrdfException("Sphere has no radius.")
-        self.radius = float(xml["radius"])
+        self.radius = float(xml.attrib["radius"])
 
     def plot(self, tm, frame, ax=None, alpha=0.3, wireframe=True,
              convex_hull=True):  # pragma: no cover
         """Plot sphere."""
         center = tm.get_transform(self.frame, frame)[:3, 3]
         color = self.color if self.color is not None else "k"
         from .plot_utils import plot_sphere
@@ -793,20 +802,20 @@
     def __init__(self, frame, mesh_path, package_dir, color):
         super(Cylinder, self).__init__(frame, mesh_path, package_dir, color)
         self.radius = 0.0
         self.length = 0.0
 
     def parse(self, xml):
         """Parse cylinder radius and length."""
-        if not xml.has_attr("radius"):
+        if "radius" not in xml.attrib:
             raise UrdfException("Cylinder has no radius.")
-        self.radius = float(xml["radius"])
-        if not xml.has_attr("length"):
+        self.radius = float(xml.attrib["radius"])
+        if "length" not in xml.attrib:
             raise UrdfException("Cylinder has no length.")
-        self.length = float(xml["length"])
+        self.length = float(xml.attrib["length"])
 
     def plot(self, tm, frame, ax=None, alpha=0.3, wireframe=True,
              convex_hull=True):  # pragma: no cover
         """Plot cylinder."""
         A2B = tm.get_transform(self.frame, frame)
         color = self.color if self.color is not None else "k"
         from .plot_utils import plot_cylinder
@@ -823,24 +832,25 @@
         self.scale = np.ones(3)
 
     def parse(self, xml):
         """Parse mesh filename and scale."""
         if self.mesh_path is None and self.package_dir is None:
             self.filename = None
         else:
-            if not xml.has_attr("filename"):
+            if "filename" not in xml.attrib:
                 raise UrdfException("Mesh has no filename.")
             if self.mesh_path is not None:
-                self.filename = os.path.join(self.mesh_path, xml["filename"])
+                self.filename = os.path.join(
+                    self.mesh_path, xml.attrib["filename"])
             else:
                 assert self.package_dir is not None
-                self.filename = xml["filename"].replace(
+                self.filename = xml.attrib["filename"].replace(
                     "package://", self.package_dir)
-            if xml.has_attr("scale"):
-                self.scale = np.fromstring(xml["scale"], sep=" ")
+            if "scale" in xml.attrib:
+                self.scale = np.fromstring(xml.attrib["scale"], sep=" ")
 
     def plot(self, tm, frame, ax=None, alpha=0.3, wireframe=True,
              convex_hull=True):  # pragma: no cover
         """Plot mesh."""
         from .plot_utils import plot_mesh
         A2B = tm.get_transform(self.frame, frame)
         color = self.color if self.color is not None else "k"
```

### Comparing `pytransform3d-3.2.0/pytransform3d/urdf.pyi` & `pytransform3d-3.3.0/pytransform3d/urdf.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from typing import Dict, Tuple, List, Union, Type, Hashable
 import numpy as np
 import numpy.typing as npt
 from mpl_toolkits.mplot3d import Axes3D
-from bs4.element import Tag
+from lxml.etree import Element
 from .transform_manager import TransformManager
-from typing import Dict, Tuple, List, Any, Union, Type, Hashable
 
 
 class UrdfTransformManager(TransformManager):
     _joints: Dict[str, Tuple[Hashable, Hashable, np.ndarray, np.ndarray,
                              Tuple[float, float], str]]
     collision_objects: List[Geometry]
     visuals: List[Geometry]
@@ -68,15 +68,15 @@
     mesh_path: Union[None, str]
     package_dir: Union[None, str]
     color: npt.ArrayLike
 
     def __init__(self, frame: str, mesh_path: Union[None, str],
                  package_dir: Union[None, str], color: str): ...
 
-    def parse(self, xml: Tag): ...
+    def parse(self, xml: Element): ...
 
     def plot(self, tm: UrdfTransformManager, frame: Hashable,
              ax: Union[None, Axes3D] = ..., alpha: float = ...,
              wireframe: bool = ..., convex_hull: bool = ...): ...
 
 
 class Box(Geometry):
```

### Comparing `pytransform3d-3.2.0/pytransform3d/visualizer/__init__.py` & `pytransform3d-3.3.0/pytransform3d/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.2.0/pytransform3d/visualizer/_artists.py` & `pytransform3d-3.3.0/pytransform3d/visualizer/_artists.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,17 +544,25 @@
         Center of the mesh
 
     s : array-like, shape (3,), optional (default: [1, 1, 1])
         Scaling of the mesh that will be drawn
 
     c : array-like, shape (n_vertices, 3) or (3,), optional (default: None)
         Color(s)
+
+    convex_hull : bool, optional (default: False)
+        Compute convex hull of mesh.
     """
-    def __init__(self, filename, A2B=np.eye(4), s=np.ones(3), c=None):
-        self.mesh = o3d.io.read_triangle_mesh(filename)
+    def __init__(self, filename, A2B=np.eye(4), s=np.ones(3), c=None,
+                 convex_hull=False):
+        mesh = o3d.io.read_triangle_mesh(filename)
+        if convex_hull:
+            self.mesh = mesh.compute_convex_hull()[0]
+        else:
+            self.mesh = mesh
         self.mesh.vertices = o3d.utility.Vector3dVector(
             np.asarray(self.mesh.vertices) * s)
         self.mesh.compute_vertex_normals()
         if c is not None:
             n_vertices = len(self.mesh.vertices)
             colors = np.zeros((n_vertices, 3))
             colors[:] = c
@@ -1046,27 +1054,33 @@
 
     show_name : bool, optional (default: False)
         Show names of frames
 
     whitelist : list, optional (default: all)
         List of frames that should be displayed
 
+    convex_hull_of_collision_objects : bool, optional (default: False)
+        Show convex hull of collision objects.
+
     s : float, optional (default: 1)
         Scaling of the frames that will be drawn
     """
     def __init__(self, tm, frame, show_frames=False, show_connections=False,
                  show_visuals=False, show_collision_objects=False,
-                 show_name=False, whitelist=None, s=1.0):
+                 show_name=False, whitelist=None,
+                 convex_hull_of_collision_objects=False, s=1.0):
         self.tm = tm
         self.frame = frame
         self.show_frames = show_frames
         self.show_connections = show_connections
         self.show_visuals = show_visuals
         self.show_collision_objects = show_collision_objects
         self.whitelist = whitelist
+        self.convex_hull_of_collision_objects = \
+            convex_hull_of_collision_objects
         self.s = s
 
         if self.frame not in self.tm.nodes:
             raise KeyError("Unknown frame '%s'" % self.frame)
 
         self.nodes = list(sorted(self.tm._whitelisted_nodes(whitelist)))
 
@@ -1097,15 +1111,16 @@
         self.visuals = {}
         if show_visuals and hasattr(self.tm, "visuals"):
             self.visuals.update(_objects_to_artists(self.tm.visuals))
         self.collision_objects = {}
         if show_collision_objects and hasattr(
                 self.tm, "collision_objects"):
             self.collision_objects.update(
-                _objects_to_artists(self.tm.collision_objects))
+                _objects_to_artists(self.tm.collision_objects,
+                                    convex_hull_of_collision_objects))
 
         self.set_data()
 
     def set_data(self):
         """Indicate that data has been updated."""
         if self.show_frames:
             for node in self.nodes:
@@ -1157,22 +1172,25 @@
         for obj in self.visuals.values():
             geometries += obj.geometries
         for obj in self.collision_objects.values():
             geometries += obj.geometries
         return geometries
 
 
-def _objects_to_artists(objects):
+def _objects_to_artists(objects, convex_hull=False):
     """Convert geometries from URDF to artists.
 
     Parameters
     ----------
     objects : list of Geometry
         Objects parsed from URDF.
 
+    convex_hull : bool, optional (default: False)
+        Compute convex hull for each object.
+
     Returns
     -------
     artists : dict
         Mapping from frame names to artists.
     """
     artists = {}
     for obj in objects:
@@ -1186,12 +1204,13 @@
                 artist = Sphere(radius=obj.radius, c=color)
             elif isinstance(obj, urdf.Box):
                 artist = Box(obj.size, c=color)
             elif isinstance(obj, urdf.Cylinder):
                 artist = Cylinder(obj.length, obj.radius, c=color)
             else:
                 assert isinstance(obj, urdf.Mesh)
-                artist = Mesh(obj.filename, s=obj.scale, c=color)
+                artist = Mesh(obj.filename, s=obj.scale, c=color,
+                              convex_hull=convex_hull)
             artists[obj.frame] = artist
         except RuntimeError as e:
             warnings.warn(str(e))
     return artists
```

### Comparing `pytransform3d-3.2.0/pytransform3d/visualizer/_artists.pyi` & `pytransform3d-3.3.0/pytransform3d/visualizer/_artists.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,16 @@
 
     @property
     def geometries(self) -> List[o3d.geometry.Geometry3D]: ...
 
 
 class Mesh(Artist):
     def __init__(self, filename: str, A2B: npt.ArrayLike = ...,
-                 s: npt.ArrayLike = ..., c: Union[None, npt.ArrayLike] = ...): ...
+                 s: npt.ArrayLike = ..., c: Union[None, npt.ArrayLike] = ...,
+                 convex_hull: bool = ...): ...
 
     def set_data(self, A2B: npt.ArrayLike): ...
 
     @property
     def geometries(self) -> List[o3d.geometry.Geometry3D]: ...
 
 
@@ -175,15 +176,16 @@
 
 
 class Graph(Artist):
     def __init__(
             self, tm: TransformManager, frame: str, show_frames: bool = ...,
             show_connections: bool = ..., show_visuals: bool = ...,
             show_collision_objects: bool = ..., show_name: bool = ...,
-            whitelist: Union[None, List[str]] = ..., s: float = ...): ...
+            whitelist: Union[None, List[str]] = ...,
+            convex_hull_of_collision_objects: bool = ..., s: float = ...): ...
 
     def set_data(self): ...
 
     @property
     def geometries(self) -> List[o3d.geometry.Geometry3D]: ...
```

### Comparing `pytransform3d-3.2.0/pytransform3d/visualizer/_figure.pyi` & `pytransform3d-3.3.0/pytransform3d/visualizer/_figure.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,15 @@
             s: float = ..., c: Union[None, npt.ArrayLike] = ...) -> Plane: ...
 
     def plot_graph(
             self, tm: TransformManager, frame: str, show_frames: bool = ...,
             show_connections: bool = ..., show_visuals: bool = ...,
             show_collision_objects: bool = ..., show_name: bool = ...,
             whitelist: Union[None, List[str]] = ...,
+            convex_hull_of_collision_objects: bool = ...,
             s: float = ...) -> Graph: ...
 
     def plot_camera(
             self, M: npt.ArrayLike,
             cam2world: Union[None, npt.ArrayLike] = ...,
             virtual_image_distance: float = ...,
             sensor_size: npt.ArrayLike = ...,
```

### Comparing `pytransform3d-3.2.0/pytransform3d.egg-info/PKG-INFO` & `pytransform3d-3.3.0/pytransform3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.2.0
+Version: 3.3.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -38,16 +38,15 @@
 * tight coupling with matplotlib to quickly visualize (or animate)
   transformations
 * the TransformManager which manages complex chains of transformations
   (with export to graph visualization as PNG, additionally requires pydot)
 * the TransformEditor which allows to modify transformations graphically
   (additionally requires PyQt4/5)
 * the UrdfTransformManager which is able to load transformations from
-  [URDF](https://wiki.ros.org/urdf) files (additionally requires
-  beautifulsoup4)
+  [URDF](https://wiki.ros.org/urdf) files (additionally requires lxml)
 * a matplotlib-like interface to Open3D's visualizer to display and animate
   geometries and transformations (additionally requires Open3D)
 
 pytransform3d is used in various domains, for example:
 
 * specifying motions of a robot
 * learning robot movements from human demonstration
```

### Comparing `pytransform3d-3.2.0/setup.py` & `pytransform3d-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,15 @@
               "License :: OSI Approved :: BSD License",
               "Operating System :: OS Independent",
               "Topic :: Scientific/Engineering :: Mathematics",
               "Topic :: Scientific/Engineering :: Visualization",
           ],
           license='BSD-3-Clause',
           packages=find_packages(),
-          install_requires=["numpy", "scipy", "matplotlib", "lxml",
-                            "beautifulsoup4"],
+          install_requires=["numpy", "scipy", "matplotlib", "lxml"],
           extras_require={
               "all": ["pydot", "trimesh", "open3d"],
               "doc": ["numpydoc", "sphinx", "sphinx-gallery",
                       "sphinx-bootstrap-theme"],
               "test": ["pytest", "pytest-cov"]
           }
           )
```

