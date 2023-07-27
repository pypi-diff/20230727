# Comparing `tmp/PyDynamic-2.4.0.tar.gz` & `tmp/PyDynamic-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamic-2.4.0.tar", last modified: Mon Mar 20 08:38:12 2023, max compression
+gzip compressed data, was "PyDynamic-2.4.1.tar", last modified: Thu Jul 27 13:55:00 2023, max compression
```

## Comparing `PyDynamic-2.4.0.tar` & `PyDynamic-2.4.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11826 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10323 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7650 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/licence.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py310.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11396 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py310.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py37.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10941 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py37.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py38.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11721 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py38.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py39.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11636 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements-py39.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/dev-requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/environment.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1137 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/requirements-py310.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/requirements-py37.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/requirements-py38.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/requirements-py39.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/requirements.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2311 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/requirements/upgrade_dependencies.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4507 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.115261 PyDynamic-2.4.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2023-03-20 08:38:09.000000 PyDynamic-2.4.0/src/PyDynamic/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic/deconvolution/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/deconvolution/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2422 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/deconvolution/fit_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1785 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/demonstrate_fit_som.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3457 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)   256616 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50594 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50623 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     6197 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1268 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/examples/working_with_signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic/identification/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/identification/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1034 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/identification/fit_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      847 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/identification/fit_transfer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/src/PyDynamic/misc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5838 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/SecondOrderSystem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1884 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/filterstuff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7847 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/impinvar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7217 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/noise.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8724 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/testsignals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23151 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/misc/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/src/PyDynamic/model_estimation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/model_estimation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39343 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/model_estimation/fit_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9530 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/model_estimation/fit_transfer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9972 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.123261 PyDynamic-2.4.0/src/PyDynamic/uncertainty/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17787 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/interpolate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/interpolation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39807 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_DFT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14351 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_DWT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27932 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_MonteCarlo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6282 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_convolution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26281 2023-03-20 08:36:54.000000 PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-20 08:38:12.119261 PyDynamic-2.4.0/src/PyDynamic.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11826 2023-03-20 08:38:12.000000 PyDynamic-2.4.0/src/PyDynamic.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-03-20 08:38:12.000000 PyDynamic-2.4.0/src/PyDynamic.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-20 08:38:12.000000 PyDynamic-2.4.0/src/PyDynamic.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-03-20 08:38:12.000000 PyDynamic-2.4.0/src/PyDynamic.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-03-20 08:38:12.000000 PyDynamic-2.4.0/src/PyDynamic.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.976739 PyDynamic-2.4.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11826 2023-07-27 13:55:00.976739 PyDynamic-2.4.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10323 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7650 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/licence.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.968739 PyDynamic-2.4.1/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py310.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11393 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py310.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py37.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10997 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py37.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py38.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11774 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py38.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py39.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11675 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements-py39.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/dev-requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/environment.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1165 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/requirements-py310.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/requirements-py37.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/requirements-py38.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/requirements-py39.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/requirements.txt
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2311 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/requirements/upgrade_dependencies.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-07-27 13:55:00.980739 PyDynamic-2.4.1/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5827 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.964739 PyDynamic-2.4.1/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.968739 PyDynamic-2.4.1/src/PyDynamic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2023-07-27 13:54:58.000000 PyDynamic-2.4.1/src/PyDynamic/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.968739 PyDynamic-2.4.1/src/PyDynamic/deconvolution/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/deconvolution/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2422 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/deconvolution/fit_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.968739 PyDynamic-2.4.1/src/PyDynamic/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1785 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/demonstrate_fit_som.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.972739 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3457 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)   256616 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50594 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50623 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     6197 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/examples/working_with_signals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.972739 PyDynamic-2.4.1/src/PyDynamic/identification/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/identification/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1034 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/identification/fit_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      847 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/identification/fit_transfer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.976739 PyDynamic-2.4.1/src/PyDynamic/misc/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5838 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/SecondOrderSystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1884 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/filterstuff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7847 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/impinvar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7217 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/noise.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8724 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/testsignals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23151 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/misc/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.976739 PyDynamic-2.4.1/src/PyDynamic/model_estimation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/model_estimation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39343 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/model_estimation/fit_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9530 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/model_estimation/fit_transfer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9972 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/signals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.976739 PyDynamic-2.4.1/src/PyDynamic/uncertainty/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17787 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/interpolate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/interpolation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39847 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_DFT.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14351 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_DWT.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27932 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_MonteCarlo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6282 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_convolution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26281 2023-07-27 13:53:42.000000 PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-27 13:55:00.968739 PyDynamic-2.4.1/src/PyDynamic.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11826 2023-07-27 13:55:00.000000 PyDynamic-2.4.1/src/PyDynamic.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-07-27 13:55:00.000000 PyDynamic-2.4.1/src/PyDynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-27 13:55:00.000000 PyDynamic-2.4.1/src/PyDynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-07-27 13:55:00.000000 PyDynamic-2.4.1/src/PyDynamic.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-07-27 13:55:00.000000 PyDynamic-2.4.1/src/PyDynamic.egg-info/top_level.txt
```

### Comparing `PyDynamic-2.4.0/PKG-INFO` & `PyDynamic-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PyDynamic
-Version: 2.4.0
+Version: 2.4.1
 Summary: A software package for the analysis of dynamic measurements
 Home-page: https://ptb-m4d.github.io/PyDynamic/
 Author: Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, Martin Weber
 Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN
-Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.0/PyDynamic-2.4.0.tar.gz
-Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.0/
-Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.0/
+Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.1/PyDynamic-2.4.1.tar.gz
+Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.1/
+Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.1/
 Project-URL: Tracker, https://github.com/PTB-M4D/PyDynamic/issues
 Keywords: measurement uncertainty,dynamic measurements,metrology,GUM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.0 Summary: A software
+Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.1 Summary: A software
 package for the analysis of dynamic measurements Home-page: https://ptb-
 m4d.github.io/PyDynamic/ Author: Sascha EichstÃ¤dt, Maximilian Gruber, BjÃ¶rn
 Ludwig, Thomas Bruns, Martin Weber Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/
-download/v2.4.0/PyDynamic-2.4.0.tar.gz Project-URL: Documentation, https://
-pydynamic.readthedocs.io/en/v2.4.0/ Project-URL: Source, https://github.com/
-PTB-M4D/PyDynamic/tree/v2.4.0/ Project-URL: Tracker, https://github.com/PTB-
+download/v2.4.1/PyDynamic-2.4.1.tar.gz Project-URL: Documentation, https://
+pydynamic.readthedocs.io/en/v2.4.1/ Project-URL: Source, https://github.com/
+PTB-M4D/PyDynamic/tree/v2.4.1/ Project-URL: Tracker, https://github.com/PTB-
 M4D/PyDynamic/issues Keywords: measurement uncertainty,dynamic
 measurements,metrology,GUM Platform: UNKNOWN Classifier: Development Status ::
 4 - Beta Classifier: Topic :: Utilities Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: GNU Lesser
 General Public License v3 or later (LGPLv3+) Classifier: Programming Language
```

### Comparing `PyDynamic-2.4.0/README.md` & `PyDynamic-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/licence.txt` & `PyDynamic-2.4.1/licence.txt`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/requirements/dev-requirements-py310.txt` & `PyDynamic-2.4.1/requirements/dev-requirements-py310.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,82 +4,81 @@
 #
 #    pip-compile --output-file=requirements/dev-requirements-py310.txt requirements/dev-requirements-py310.in
 #
 -e file:.
     # via -r requirements/dev-requirements.in
 alabaster==0.7.13
     # via sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   hypothesis
     #   jsonschema
-    #   pytest
-babel==2.11.0
+babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via nbconvert
-black[jupyter]==23.1.0
+black[jupyter]==23.3.0
     # via -r requirements/dev-requirements.in
 bleach==6.0.0
     # via
     #   nbconvert
     #   readme-renderer
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
 chardet==5.1.0
     # via tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
-contourpy==1.0.7
+contourpy==1.1.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==39.0.1
+cryptography==41.0.1
     # via secretstorage
 cycler==0.11.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.6
     # via virtualenv
@@ -88,63 +87,64 @@
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
+    #   anyio
     #   hypothesis
     #   pytest
 executing==1.2.0
     # via stack-data
-fastjsonschema==2.16.2
+fastjsonschema==2.17.1
     # via nbformat
-filelock==3.9.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-fonttools==4.38.0
+fonttools==4.40.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via
     #   -c requirements/requirements-py310.txt
     #   uncertainties
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via python-semantic-release
-hypothesis==6.68.1
+hypothesis==6.80.0
     # via -r requirements/dev-requirements.in
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
 iniconfig==2.0.0
     # via pytest
-invoke==1.7.3
+invoke==2.1.3
     # via python-semantic-release
-ipykernel==6.21.2
+ipykernel==6.23.3
     # via
     #   -r requirements/dev-requirements.in
     #   nbclassic
     #   notebook
-ipython==8.10.0
+ipython==8.14.0
     # via
     #   -r requirements/dev-requirements.in
     #   black
     #   ipykernel
 ipython-genutils==0.2.0
     # via
     #   nbclassic
@@ -164,279 +164,280 @@
     #   jupyter-server
     #   myst-parser
     #   nbclassic
     #   nbconvert
     #   nbsphinx
     #   notebook
     #   sphinx
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   nbformat
-jupyter-client==8.0.2
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
-jupyter-core==5.2.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.2.1
+jupyter-server==2.7.0
     # via
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab-pygments==0.2.2
     # via nbconvert
-keyring==23.13.1
+keyring==24.2.0
     # via twine
 kiwisolver==1.4.4
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-markdown-it-py==2.1.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-mpmath==1.2.1
+mpmath==1.3.0
     # via
     #   -c requirements/requirements-py310.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
-myst-parser==0.18.1
+myst-parser==2.0.0
     # via -r requirements/dev-requirements.in
-nbclassic==0.5.1
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.2
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.2.9
+nbconvert==7.6.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbsphinx
     #   notebook
-nbformat==5.7.3
+nbformat==5.9.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
     #   notebook
-nbsphinx==0.8.12
+nbsphinx==0.9.2
     # via -r requirements/dev-requirements.in
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-notebook==6.5.2
+notebook==6.5.4
     # via pydynamic
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-numpy==1.24.2
+numpy==1.25.0
     # via
     #   -c requirements/requirements-py310.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-packaging==23.0
+overrides==7.3.1
+    # via jupyter-server
+packaging==23.1
     # via
     #   -c requirements/requirements-py310.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==1.5.3
+pandas==2.0.3
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
 pkginfo==1.9.6
     # via twine
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-pyproject-api==1.5.0
+pyproject-api==1.5.2
     # via tox
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements/dev-requirements.in
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/dev-requirements.in
 pytest-custom-exit-code==0.3.0
     # via -r requirements/dev-requirements.in
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements-py310.txt
     #   jupyter-client
     #   matplotlib
     #   pandas
-python-gitlab==3.13.0
+python-gitlab==3.15.0
     # via python-semantic-release
-python-json-logger==2.0.6
+python-json-logger==2.0.7
     # via jupyter-events
-python-semantic-release==7.33.1
+python-semantic-release==7.34.6
     # via -r requirements/dev-requirements.in
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -c requirements/requirements-py310.txt
-    #   babel
     #   pandas
 pywavelets==1.4.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 pyyaml==6.0
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.0.0
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   python-gitlab
     #   python-semantic-release
     #   requests-oauthlib
     #   requests-toolbelt
     #   sphinx
     #   tweepy
     #   twine
 requests-oauthlib==1.3.1
     # via tweepy
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via
     #   python-gitlab
     #   twine
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-scipy==1.10.0
+scipy==1.11.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   -c requirements/requirements-py310.txt
@@ -448,41 +449,42 @@
     # via gitdb
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==6.2.1
     # via
     #   -r requirements/dev-requirements.in
     #   myst-parser
     #   nbsphinx
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.2.0
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements/dev-requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
-sympy==1.11.1
+sympy==1.12
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
@@ -490,36 +492,36 @@
     #   notebook
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 tinycss2==1.2.1
     # via nbconvert
-tokenize-rt==5.0.0
+tokenize-rt==5.1.0
     # via black
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.11.6
+tomlkit==0.11.8
     # via python-semantic-release
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.5
+tox==4.6.3
     # via -r requirements/dev-requirements.in
-tqdm==4.64.1
+tqdm==4.65.0
     # via twine
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
@@ -529,42 +531,41 @@
     #   matplotlib-inline
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
     #   notebook
-tweepy==4.12.1
+tweepy==4.14.0
     # via -r requirements/dev-requirements.in
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.5.0
-    # via myst-parser
+tzdata==2023.3
+    # via
+    #   -c requirements/requirements-py310.txt
+    #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py310.txt
     #   time-series-buffer
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==1.26.14
+urllib3==2.0.3
     # via
     #   requests
     #   twine
-virtualenv==20.19.0
+virtualenv==20.23.1
     # via tox
 wcwidth==0.2.6
     # via prompt-toolkit
-webcolors==1.12
+webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.1
     # via jupyter-server
-wheel==0.38.4
+wheel==0.40.0
     # via python-semantic-release
-zipp==3.13.0
+zipp==3.15.0
     # via importlib-metadata
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `PyDynamic-2.4.0/requirements/dev-requirements-py37.txt` & `PyDynamic-2.4.1/requirements/dev-requirements-py37.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,72 +4,71 @@
 #
 #    pip-compile --output-file=requirements/dev-requirements-py37.txt requirements/dev-requirements-py37.in
 #
 -e file:.
     # via -r requirements/dev-requirements.in
 alabaster==0.7.13
     # via sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   hypothesis
     #   jsonschema
-    #   pytest
-babel==2.11.0
+babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via nbconvert
-black[jupyter]==23.1.0
+black[jupyter]==23.3.0
     # via -r requirements/dev-requirements.in
 bleach==6.0.0
     # via
     #   nbconvert
     #   readme-renderer
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
 chardet==5.1.0
     # via tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==39.0.1
+cryptography==41.0.1
     # via secretstorage
 cycler==0.11.0
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.6
     # via virtualenv
@@ -80,64 +79,66 @@
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
 entrypoints==0.4
     # via jupyter-client
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
+    #   anyio
     #   hypothesis
     #   pytest
-fastjsonschema==2.16.2
+fastjsonschema==2.17.1
     # via nbformat
-filelock==3.9.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 fonttools==4.38.0
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
 future==0.18.3
     # via
     #   -c requirements/requirements-py37.txt
     #   uncertainties
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via python-semantic-release
-hypothesis==6.68.1
+hypothesis==6.79.4
     # via -r requirements/dev-requirements.in
 idna==3.4
     # via
     #   anyio
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
     # via
+    #   attrs
     #   click
     #   jsonschema
     #   keyring
     #   nbconvert
     #   nbformat
     #   pluggy
     #   pytest
     #   sphinx
     #   tox
     #   twine
     #   virtualenv
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via
     #   jsonschema
     #   keyring
 iniconfig==2.0.0
     # via pytest
-invoke==1.7.3
+invoke==2.1.3
     # via python-semantic-release
 ipykernel==6.16.2
     # via
     #   -r requirements/dev-requirements.in
     #   nbclassic
     #   notebook
 ipython==7.34.0
@@ -180,102 +181,102 @@
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
-jupyter-server==1.23.5
+jupyter-server==1.24.0
     # via
     #   nbclassic
     #   notebook-shim
 jupyterlab-pygments==0.2.2
     # via nbconvert
-keyring==23.13.1
+keyring==24.1.1
     # via twine
 kiwisolver==1.4.4
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
 matplotlib==3.5.3
     # via
     #   -c requirements/requirements-py37.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.3.5
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-mpmath==1.2.1
+mpmath==1.3.0
     # via
     #   -c requirements/requirements-py37.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
-myst-parser==0.18.1
+myst-parser==1.0.0
     # via -r requirements/dev-requirements.in
-nbclassic==0.5.1
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.2
+nbclient==0.7.4
     # via nbconvert
-nbconvert==7.2.9
+nbconvert==7.6.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbsphinx
     #   notebook
-nbformat==5.7.3
+nbformat==5.8.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
     #   notebook
-nbsphinx==0.8.12
+nbsphinx==0.9.2
     # via -r requirements/dev-requirements.in
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclassic
     #   notebook
-notebook==6.5.2
+notebook==6.5.4
     # via pydynamic
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
 numpy==1.21.6
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-packaging==23.0
+packaging==23.1
     # via
     #   -c requirements/requirements-py37.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   matplotlib
     #   nbconvert
@@ -288,131 +289,131 @@
     # via
     #   -c requirements/requirements-py37.txt
     #   pydynamic
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
 pkginfo==1.9.6
     # via twine
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via
     #   black
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   -c requirements/requirements-py37.txt
     #   matplotlib
-pyproject-api==1.5.0
+pyproject-api==1.5.2
     # via tox
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements/dev-requirements.in
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/dev-requirements.in
 pytest-custom-exit-code==0.3.0
     # via -r requirements/dev-requirements.in
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements-py37.txt
     #   jupyter-client
     #   matplotlib
     #   pandas
-python-gitlab==3.13.0
+python-gitlab==3.15.0
     # via python-semantic-release
-python-semantic-release==7.33.1
+python-semantic-release==7.34.6
     # via -r requirements/dev-requirements.in
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -c requirements/requirements-py37.txt
     #   babel
     #   pandas
 pywavelets==1.3.0
     # via
     #   -c requirements/requirements-py37.txt
     #   pydynamic
 pyyaml==6.0
     # via myst-parser
-pyzmq==25.0.0
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   python-gitlab
     #   python-semantic-release
     #   requests-oauthlib
     #   requests-toolbelt
     #   sphinx
     #   tweepy
     #   twine
 requests-oauthlib==1.3.1
     # via tweepy
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via
     #   python-gitlab
     #   twine
 rfc3986==2.0.0
     # via twine
 scipy==1.7.3
     # via
     #   -c requirements/requirements-py37.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   -c requirements/requirements-py37.txt
@@ -422,31 +423,32 @@
     # via gitdb
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==5.3.0
     # via
     #   -r requirements/dev-requirements.in
     #   myst-parser
     #   nbsphinx
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.2.0
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements/dev-requirements.in
 sphinxcontrib-applehelp==1.0.2
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.0
     # via sphinx
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
@@ -470,27 +472,27 @@
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.11.6
+tomlkit==0.11.8
     # via python-semantic-release
 tornado==6.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.5
+tox==4.6.3
     # via -r requirements/dev-requirements.in
-tqdm==4.64.1
+tqdm==4.65.0
     # via twine
 traitlets==5.9.0
     # via
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
@@ -498,54 +500,55 @@
     #   matplotlib-inline
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
     #   notebook
-tweepy==4.12.1
+tweepy==4.14.0
     # via -r requirements/dev-requirements.in
 twine==3.8.0
     # via python-semantic-release
 typed-ast==1.5.4
     # via black
-typing-extensions==4.5.0
+typing-extensions==4.7.0
     # via
     #   -c requirements/requirements-py37.txt
     #   anyio
     #   argon2-cffi
     #   black
     #   gitpython
     #   importlib-metadata
     #   jsonschema
     #   kiwisolver
     #   markdown-it-py
     #   myst-parser
     #   platformdirs
+    #   python-gitlab
     #   tox
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py37.txt
     #   time-series-buffer
-urllib3==1.26.14
+urllib3==2.0.3
     # via
     #   requests
     #   twine
-virtualenv==20.19.0
+virtualenv==20.23.1
     # via tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.1
     # via jupyter-server
-wheel==0.38.4
+wheel==0.40.0
     # via python-semantic-release
-zipp==3.13.0
+zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `PyDynamic-2.4.0/requirements/dev-requirements-py38.txt` & `PyDynamic-2.4.1/requirements/dev-requirements-py38.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,82 +4,81 @@
 #
 #    pip-compile --output-file=requirements/dev-requirements-py38.txt requirements/dev-requirements-py38.in
 #
 -e file:.
     # via -r requirements/dev-requirements.in
 alabaster==0.7.13
     # via sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   hypothesis
     #   jsonschema
-    #   pytest
-babel==2.11.0
+babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via nbconvert
-black[jupyter]==23.1.0
+black[jupyter]==23.3.0
     # via -r requirements/dev-requirements.in
 bleach==6.0.0
     # via
     #   nbconvert
     #   readme-renderer
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
 chardet==5.1.0
     # via tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
-contourpy==1.0.7
+contourpy==1.1.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==39.0.1
+cryptography==41.0.1
     # via secretstorage
 cycler==0.11.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.6
     # via virtualenv
@@ -88,72 +87,73 @@
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
+    #   anyio
     #   hypothesis
     #   pytest
 executing==1.2.0
     # via stack-data
-fastjsonschema==2.16.2
+fastjsonschema==2.17.1
     # via nbformat
-filelock==3.9.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-fonttools==4.38.0
+fonttools==4.40.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via
     #   -c requirements/requirements-py38.txt
     #   uncertainties
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via python-semantic-release
-hypothesis==6.68.1
+hypothesis==6.80.0
     # via -r requirements/dev-requirements.in
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
     # via
     #   jupyter-client
     #   keyring
     #   nbconvert
     #   sphinx
     #   twine
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via
     #   -c requirements/requirements-py38.txt
     #   jsonschema
     #   keyring
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-invoke==1.7.3
+invoke==2.1.3
     # via python-semantic-release
-ipykernel==6.21.2
+ipykernel==6.23.3
     # via
     #   -r requirements/dev-requirements.in
     #   nbclassic
     #   notebook
-ipython==8.10.0
+ipython==8.12.2
     # via
     #   -r requirements/dev-requirements.in
     #   black
     #   ipykernel
 ipython-genutils==0.2.0
     # via
     #   nbclassic
@@ -173,281 +173,283 @@
     #   jupyter-server
     #   myst-parser
     #   nbclassic
     #   nbconvert
     #   nbsphinx
     #   notebook
     #   sphinx
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   nbformat
-jupyter-client==8.0.2
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
-jupyter-core==5.2.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.2.1
+jupyter-server==2.7.0
     # via
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab-pygments==0.2.2
     # via nbconvert
-keyring==23.13.1
+keyring==24.2.0
     # via twine
 kiwisolver==1.4.4
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-markdown-it-py==2.1.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-mpmath==1.2.1
+mpmath==1.3.0
     # via
     #   -c requirements/requirements-py38.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
-myst-parser==0.18.1
+myst-parser==2.0.0
     # via -r requirements/dev-requirements.in
-nbclassic==0.5.1
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.2
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.2.9
+nbconvert==7.6.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbsphinx
     #   notebook
-nbformat==5.7.3
+nbformat==5.9.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
     #   notebook
-nbsphinx==0.8.12
+nbsphinx==0.9.2
     # via -r requirements/dev-requirements.in
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-notebook==6.5.2
+notebook==6.5.4
     # via pydynamic
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-numpy==1.24.2
+numpy==1.24.4
     # via
     #   -c requirements/requirements-py38.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-packaging==23.0
+overrides==7.3.1
+    # via jupyter-server
+packaging==23.1
     # via
     #   -c requirements/requirements-py38.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==1.5.3
+pandas==2.0.3
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
 pkginfo==1.9.6
     # via twine
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-pyproject-api==1.5.0
+pyproject-api==1.5.2
     # via tox
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements/dev-requirements.in
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/dev-requirements.in
 pytest-custom-exit-code==0.3.0
     # via -r requirements/dev-requirements.in
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements-py38.txt
     #   jupyter-client
     #   matplotlib
     #   pandas
-python-gitlab==3.13.0
+python-gitlab==3.15.0
     # via python-semantic-release
-python-json-logger==2.0.6
+python-json-logger==2.0.7
     # via jupyter-events
-python-semantic-release==7.33.1
+python-semantic-release==7.34.6
     # via -r requirements/dev-requirements.in
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -c requirements/requirements-py38.txt
     #   babel
     #   pandas
 pywavelets==1.4.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 pyyaml==6.0
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.0.0
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   python-gitlab
     #   python-semantic-release
     #   requests-oauthlib
     #   requests-toolbelt
     #   sphinx
     #   tweepy
     #   twine
 requests-oauthlib==1.3.1
     # via tweepy
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via
     #   python-gitlab
     #   twine
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-scipy==1.10.0
+scipy==1.10.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   -c requirements/requirements-py38.txt
@@ -459,41 +461,42 @@
     # via gitdb
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==6.2.1
     # via
     #   -r requirements/dev-requirements.in
     #   myst-parser
     #   nbsphinx
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.2.0
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements/dev-requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
-sympy==1.11.1
+sympy==1.12
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
@@ -501,36 +504,36 @@
     #   notebook
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 tinycss2==1.2.1
     # via nbconvert
-tokenize-rt==5.0.0
+tokenize-rt==5.1.0
     # via black
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.11.6
+tomlkit==0.11.8
     # via python-semantic-release
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.5
+tox==4.6.3
     # via -r requirements/dev-requirements.in
-tqdm==4.64.1
+tqdm==4.65.0
     # via twine
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
@@ -540,47 +543,48 @@
     #   matplotlib-inline
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
     #   notebook
-tweepy==4.12.1
+tweepy==4.14.0
     # via -r requirements/dev-requirements.in
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.5.0
+typing-extensions==4.7.0
     # via
     #   black
-    #   myst-parser
+    #   ipython
+tzdata==2023.3
+    # via
+    #   -c requirements/requirements-py38.txt
+    #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py38.txt
     #   time-series-buffer
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==1.26.14
+urllib3==2.0.3
     # via
     #   requests
     #   twine
-virtualenv==20.19.0
+virtualenv==20.23.1
     # via tox
 wcwidth==0.2.6
     # via prompt-toolkit
-webcolors==1.12
+webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.1
     # via jupyter-server
-wheel==0.38.4
+wheel==0.40.0
     # via python-semantic-release
-zipp==3.13.0
+zipp==3.15.0
     # via
     #   -c requirements/requirements-py38.txt
     #   importlib-metadata
     #   importlib-resources
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `PyDynamic-2.4.0/requirements/dev-requirements-py39.txt` & `PyDynamic-2.4.1/requirements/dev-requirements-py39.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,82 +4,81 @@
 #
 #    pip-compile --output-file=requirements/dev-requirements-py39.txt requirements/dev-requirements-py39.in
 #
 -e file:.
     # via -r requirements/dev-requirements.in
 alabaster==0.7.13
     # via sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   hypothesis
     #   jsonschema
-    #   pytest
-babel==2.11.0
+babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via nbconvert
-black[jupyter]==23.1.0
+black[jupyter]==23.3.0
     # via -r requirements/dev-requirements.in
 bleach==6.0.0
     # via
     #   nbconvert
     #   readme-renderer
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
 chardet==5.1.0
     # via tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.2
+comm==0.1.3
     # via ipykernel
-contourpy==1.0.7
+contourpy==1.1.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==39.0.1
+cryptography==41.0.1
     # via secretstorage
 cycler==0.11.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.6
     # via virtualenv
@@ -88,70 +87,71 @@
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
+    #   anyio
     #   hypothesis
     #   pytest
 executing==1.2.0
     # via stack-data
-fastjsonschema==2.16.2
+fastjsonschema==2.17.1
     # via nbformat
-filelock==3.9.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-fonttools==4.38.0
+fonttools==4.40.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via
     #   -c requirements/requirements-py39.txt
     #   uncertainties
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via python-semantic-release
-hypothesis==6.68.1
+hypothesis==6.80.0
     # via -r requirements/dev-requirements.in
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
     # via
     #   jupyter-client
     #   keyring
     #   nbconvert
     #   sphinx
     #   twine
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-invoke==1.7.3
+invoke==2.1.3
     # via python-semantic-release
-ipykernel==6.21.2
+ipykernel==6.23.3
     # via
     #   -r requirements/dev-requirements.in
     #   nbclassic
     #   notebook
-ipython==8.10.0
+ipython==8.14.0
     # via
     #   -r requirements/dev-requirements.in
     #   black
     #   ipykernel
 ipython-genutils==0.2.0
     # via
     #   nbclassic
@@ -171,279 +171,280 @@
     #   jupyter-server
     #   myst-parser
     #   nbclassic
     #   nbconvert
     #   nbsphinx
     #   notebook
     #   sphinx
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   nbformat
-jupyter-client==8.0.2
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
-jupyter-core==5.2.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.2.1
+jupyter-server==2.7.0
     # via
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab-pygments==0.2.2
     # via nbconvert
-keyring==23.13.1
+keyring==24.2.0
     # via twine
 kiwisolver==1.4.4
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-markdown-it-py==2.1.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-mpmath==1.2.1
+mpmath==1.3.0
     # via
     #   -c requirements/requirements-py39.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
-myst-parser==0.18.1
+myst-parser==2.0.0
     # via -r requirements/dev-requirements.in
-nbclassic==0.5.1
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.2
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.2.9
+nbconvert==7.6.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbsphinx
     #   notebook
-nbformat==5.7.3
+nbformat==5.9.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
     #   notebook
-nbsphinx==0.8.12
+nbsphinx==0.9.2
     # via -r requirements/dev-requirements.in
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-notebook==6.5.2
+notebook==6.5.4
     # via pydynamic
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-numpy==1.24.2
+numpy==1.25.0
     # via
     #   -c requirements/requirements-py39.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-packaging==23.0
+overrides==7.3.1
+    # via jupyter-server
+packaging==23.1
     # via
     #   -c requirements/requirements-py39.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==1.5.3
+pandas==2.0.3
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 pkginfo==1.9.6
     # via twine
-platformdirs==3.0.0
+platformdirs==3.8.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-pyproject-api==1.5.0
+pyproject-api==1.5.2
     # via tox
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements/dev-requirements.in
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements/dev-requirements.in
 pytest-custom-exit-code==0.3.0
     # via -r requirements/dev-requirements.in
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements-py39.txt
     #   jupyter-client
     #   matplotlib
     #   pandas
-python-gitlab==3.13.0
+python-gitlab==3.15.0
     # via python-semantic-release
-python-json-logger==2.0.6
+python-json-logger==2.0.7
     # via jupyter-events
-python-semantic-release==7.33.1
+python-semantic-release==7.34.6
     # via -r requirements/dev-requirements.in
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -c requirements/requirements-py39.txt
-    #   babel
     #   pandas
 pywavelets==1.4.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 pyyaml==6.0
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.0.0
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   python-gitlab
     #   python-semantic-release
     #   requests-oauthlib
     #   requests-toolbelt
     #   sphinx
     #   tweepy
     #   twine
 requests-oauthlib==1.3.1
     # via tweepy
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via
     #   python-gitlab
     #   twine
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-scipy==1.10.0
+scipy==1.11.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   -c requirements/requirements-py39.txt
@@ -455,41 +456,42 @@
     # via gitdb
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==6.2.1
     # via
     #   -r requirements/dev-requirements.in
     #   myst-parser
     #   nbsphinx
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.2.0
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements/dev-requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
-sympy==1.11.1
+sympy==1.12
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
@@ -497,36 +499,36 @@
     #   notebook
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 tinycss2==1.2.1
     # via nbconvert
-tokenize-rt==5.0.0
+tokenize-rt==5.1.0
     # via black
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.11.6
+tomlkit==0.11.8
     # via python-semantic-release
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.5
+tox==4.6.3
     # via -r requirements/dev-requirements.in
-tqdm==4.64.1
+tqdm==4.65.0
     # via twine
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
@@ -536,47 +538,48 @@
     #   matplotlib-inline
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
     #   notebook
-tweepy==4.12.1
+tweepy==4.14.0
     # via -r requirements/dev-requirements.in
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.5.0
+typing-extensions==4.7.0
     # via
     #   black
-    #   myst-parser
+    #   ipython
+tzdata==2023.3
+    # via
+    #   -c requirements/requirements-py39.txt
+    #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py39.txt
     #   time-series-buffer
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==1.26.14
+urllib3==2.0.3
     # via
     #   requests
     #   twine
-virtualenv==20.19.0
+virtualenv==20.23.1
     # via tox
 wcwidth==0.2.6
     # via prompt-toolkit
-webcolors==1.12
+webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.1
     # via jupyter-server
-wheel==0.38.4
+wheel==0.40.0
     # via python-semantic-release
-zipp==3.13.0
+zipp==3.15.0
     # via
     #   -c requirements/requirements-py39.txt
     #   importlib-metadata
     #   importlib-resources
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `PyDynamic-2.4.0/requirements/requirements-py310.txt` & `PyDynamic-2.4.1/requirements/requirements-py38.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/requirements-py310.txt
+#    pip-compile --output-file=requirements/requirements-py38.txt
 #
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-fonttools==4.38.0
+fonttools==4.40.0
     # via matplotlib
 future==0.18.3
     # via uncertainties
+importlib-resources==5.12.0
+    # via matplotlib
 kiwisolver==1.4.4
     # via matplotlib
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via PyDynamic (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-numpy==1.24.2
+numpy==1.24.4
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.0
+packaging==23.1
     # via matplotlib
-pandas==1.5.3
+pandas==2.0.3
     # via PyDynamic (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pywavelets==1.4.1
     # via PyDynamic (setup.py)
-scipy==1.10.0
+scipy==1.10.1
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
-sympy==1.11.1
+sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `PyDynamic-2.4.0/requirements/requirements-py37.txt` & `PyDynamic-2.4.1/requirements/requirements-py37.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,45 +10,45 @@
     # via matplotlib
 future==0.18.3
     # via uncertainties
 kiwisolver==1.4.4
     # via matplotlib
 matplotlib==3.5.3
     # via PyDynamic (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
 numpy==1.21.6
     # via
     #   PyDynamic (setup.py)
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.0
+packaging==23.1
     # via matplotlib
 pandas==1.3.5
     # via PyDynamic (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pywavelets==1.3.0
     # via PyDynamic (setup.py)
 scipy==1.7.3
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
 sympy==1.10.1
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
-typing-extensions==4.5.0
+typing-extensions==4.7.0
     # via kiwisolver
 uncertainties==3.1.7
     # via time-series-buffer
```

### Comparing `PyDynamic-2.4.0/requirements/requirements-py38.txt` & `PyDynamic-2.4.1/requirements/requirements-py39.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/requirements-py38.txt
+#    pip-compile --output-file=requirements/requirements-py39.txt
 #
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-fonttools==4.38.0
+fonttools==4.40.0
     # via matplotlib
 future==0.18.3
     # via uncertainties
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via matplotlib
 kiwisolver==1.4.4
     # via matplotlib
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via PyDynamic (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-numpy==1.24.2
+numpy==1.25.0
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.0
+packaging==23.1
     # via matplotlib
-pandas==1.5.3
+pandas==2.0.3
     # via PyDynamic (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pywavelets==1.4.1
     # via PyDynamic (setup.py)
-scipy==1.10.0
+scipy==1.11.1
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
-sympy==1.11.1
+sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
-zipp==3.13.0
+zipp==3.15.0
     # via importlib-resources
```

### Comparing `PyDynamic-2.4.0/requirements/requirements-py39.txt` & `PyDynamic-2.4.1/requirements/requirements-py310.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/requirements-py39.txt
+#    pip-compile --output-file=requirements/requirements-py310.txt
 #
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
-fonttools==4.38.0
+fonttools==4.40.0
     # via matplotlib
 future==0.18.3
     # via uncertainties
-importlib-resources==5.10.2
-    # via matplotlib
 kiwisolver==1.4.4
     # via matplotlib
-matplotlib==3.7.0
+matplotlib==3.7.1
     # via PyDynamic (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-numpy==1.24.2
+numpy==1.25.0
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.0
+packaging==23.1
     # via matplotlib
-pandas==1.5.3
+pandas==2.0.3
     # via PyDynamic (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pywavelets==1.4.1
     # via PyDynamic (setup.py)
-scipy==1.10.0
+scipy==1.11.1
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
-sympy==1.11.1
+sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
-zipp==3.13.0
-    # via importlib-resources
```

### Comparing `PyDynamic-2.4.0/requirements/upgrade_dependencies.sh` & `PyDynamic-2.4.1/requirements/upgrade_dependencies.sh`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/setup.cfg` & `PyDynamic-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/setup.py` & `PyDynamic-2.4.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,127 @@
 """Install PyDynamic in Python path and provide all packaging metadata."""
 import codecs
 import os
 from os import path
+from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 
 def get_readme():
     """Get README.md's content"""
     this_directory = path.abspath(path.dirname(__file__))
-    with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
-        return f.read()
+    with open(path.join(this_directory, "README.md"), encoding="utf-8") as file:
+        return file.read()
 
 
-def read(rel_path):
+def get_version(rel_path: str) -> str:
+    """Extract __version__ variable's value from a file's content"""
+    for line in read_file_content(rel_path).splitlines():
+        if line.startswith("__version__"):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    raise RuntimeError("Unable to find version string.")
+
+
+def read_file_content(rel_path: str) -> str:
+    """Extract a file's content and provide a variable to access it"""
     here = path.abspath(path.dirname(__file__))
-    with codecs.open(path.join(here, rel_path), "r") as fp:
-        return fp.read()
+    with codecs.open(path.join(here, rel_path), "r") as file:
+        return file.read()
 
 
 class Tweet(Command):
+    """Handle the tweeting on executing setup.py tweet"""
+
+    _filename: str
 
-    filename: str
+    _consumer_key: str
+    _consumer_secret: str
+    _access_token: str
+    _access_token_secret: str
+    _twitter_api_auth_handle = None
 
-    description = "Send new tweets to the Twitter API to announce releases"
+    description: str = "Send new tweets to the Twitter API to announce releases"
 
-    user_options = [("filename=", "f", "filename containing the tweet")]
+    user_options: List[Tuple[str, str, str]] = [
+        ("filename=", "f", "filename containing the tweet")
+    ]
 
     def initialize_options(self):
-        self.filename = "tweet.txt"
+        """Set filename to default value"""
+        self._filename = "tweet.txt"
 
     def finalize_options(self):
-        if self.filename is None:
+        """React to invalid circumstance that no filename is set"""
+        if self._filename is None:
             raise RuntimeError("Parameter --filename is missing")
 
     def run(self):
-        import tweepy
+        """Actually organize and conduct the tweeting"""
+        from tweepy import Client
 
-        def _tweet():
-            _get_twitter_api_handle().update_status(read_tweet_from_file())
+        def set_twitter_api_secrets_from_environment():
+            self._consumer_key = os.getenv("CONSUMER_KEY")
+            self._consumer_secret = os.getenv("CONSUMER_SECRET")
+            self._access_token = os.getenv("ACCESS_TOKEN")
+            self._access_token_secret = os.getenv("ACCESS_TOKEN_SECRET")
 
-        def _get_twitter_api_handle():
-            return tweepy.API(_get_twitter_api_auth_handle())
+        def set_twitter_api_auth_handle():
+            self._twitter_api_auth_handle = raise_error_or_retrieve_handle()
 
-        def _get_twitter_api_auth_handle():
+        def raise_error_or_retrieve_handle() -> Client:
             try:
-                auth = tweepy.OAuthHandler(
-                    os.getenv("consumer_key"), os.getenv("consumer_secret")
-                )
-                auth.set_access_token(
-                    os.getenv("access_token"), os.getenv("access_token_secret")
-                )
-                return auth
-            except TypeError as e:
-                if "Consumer key must be" in str(e):
+                return initialize_twitter_api_auth_handle()
+            except TypeError as type_error_message:
+                if "must be string or bytes" in str(type_error_message):
                     raise ValueError(
-                        "ValueError: Environment variables 'consumer_key', "
-                        "'consumer_secret', 'access_token' and 'access_token_secret' "
+                        "ValueError: Environment variables 'CONSUMER_KEY', "
+                        "'CONSUMER_SECRET', 'ACCESS_TOKEN' and 'ACCESS_TOKEN_SECRET' "
                         "have to be set."
                     )
+                raise TypeError from type_error_message
 
-        def read_tweet_from_file() -> str:
-            with open(self.filename, "r") as f:
-                content: str = f.read()
-            return content
+        def initialize_twitter_api_auth_handle() -> Client:
+            return Client(
+                consumer_key=self._consumer_key,
+                consumer_secret=self._consumer_secret,
+                access_token=self._access_token,
+                access_token_secret=self._access_token_secret,
+            )
 
-        _tweet()
+        def tweet():
+            self._twitter_api_auth_handle.create_tweet(text=read_tweet_from_file())
 
+        def read_tweet_from_file() -> str:
+            with open(self._filename, "r", encoding="utf-8") as file:
+                content: str = file.read()
+            return content
 
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith("__version__"):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find version string.")
+        set_twitter_api_secrets_from_environment()
+        set_twitter_api_auth_handle()
+        tweet()
 
 
 current_release_version = get_version("src/PyDynamic/__init__.py")
 
 setup(
     name="PyDynamic",
     version=current_release_version,
     description="A software package for the analysis of dynamic measurements",
     long_description=get_readme(),
     long_description_content_type="text/markdown",
     url="https://ptb-m4d.github.io/PyDynamic/",
-    download_url="https://github.com/PTB-M4D/PyDynamic/releases/download/v{0}/"
-    "PyDynamic-{0}.tar.gz".format(current_release_version),
-    author="Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, "
-    "Martin Weber",
+    download_url=(
+        f"https://github.com/PTB-M4D/PyDynamic/releases/download/"
+        f"v{current_release_version}/PyDynamic-{current_release_version}.tar.gz"
+    ),
+    author=(
+        "Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, Martin Weber"
+    ),
     author_email="sascha.eichstaedt@ptb.de",
     keywords="measurement uncertainty, dynamic measurements, metrology, GUM",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     project_urls={
         "Documentation": f"https://pydynamic.readthedocs.io/en/"
```

### Comparing `PyDynamic-2.4.0/src/PyDynamic/__init__.py` & `PyDynamic-2.4.1/src/PyDynamic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. seealso::
 
    - `initial project website <https://www.euramet.org/research-innovation/search
      -research-projects/details/project/standards-and-software-to-maximise-end-user
      -uptake-of-nmi-calibrations-of-dynamic-force-torque-and/>`_
    - `GitHub website <https://www.github.com/PTB-M4D/PyDynamic>`_
 """
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 __all__ = [
     "LSFIR",
     "LSIIR",
     "fit_som",
     "FreqResp2RealImag",
     "GUM_DFT",
```

### Comparing `PyDynamic-2.4.0/src/PyDynamic/deconvolution/__init__.py` & `PyDynamic-2.4.1/src/PyDynamic/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/deconvolution/fit_filter.py` & `PyDynamic-2.4.1/src/PyDynamic/deconvolution/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/demonstrate_fit_som.py` & `PyDynamic-2.4.1/src/PyDynamic/examples/demonstrate_fit_som.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py` & `PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat` & `PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat` & `PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat` & `PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py` & `PyDynamic-2.4.1/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/examples/working_with_signals.py` & `PyDynamic-2.4.1/src/PyDynamic/examples/working_with_signals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/identification/fit_filter.py` & `PyDynamic-2.4.1/src/PyDynamic/identification/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/identification/fit_transfer.py` & `PyDynamic-2.4.1/src/PyDynamic/identification/fit_transfer.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/SecondOrderSystem.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/SecondOrderSystem.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/__init__.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/filterstuff.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/filterstuff.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/impinvar.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/impinvar.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/noise.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/noise.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/testsignals.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/testsignals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/misc/tools.py` & `PyDynamic-2.4.1/src/PyDynamic/misc/tools.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/model_estimation/__init__.py` & `PyDynamic-2.4.1/src/PyDynamic/model_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/model_estimation/fit_filter.py` & `PyDynamic-2.4.1/src/PyDynamic/model_estimation/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/model_estimation/fit_transfer.py` & `PyDynamic-2.4.1/src/PyDynamic/model_estimation/fit_transfer.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/signals.py` & `PyDynamic-2.4.1/src/PyDynamic/signals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/__init__.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/interpolate.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/interpolate.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/interpolation.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/interpolation.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_DFT.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_DFT.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,17 @@
     # calculate blocks of uncertainty matrix
     if len(UF.shape) == 2:
         RR = UF[:N_in, :N_in]
         RI = UF[:N_in, N_in:]
         II = UF[N_in:, N_in:]
         # propagate uncertainties
         Ux = np.dot(Cc, np.dot(RR, Cc.T))
-        Ux += 2 * np.dot(Cc, np.dot(RI, Cs.T))
+        term2 = np.dot(Cc, np.dot(RI, Cs.T))
+        Ux += term2
+        Ux += term2.T
         Ux += np.dot(Cs, np.dot(II, Cs.T))
     else:
         RR = UF[:N_in]
         II = UF[N_in:]
         Ux = np.dot(Cc, _prod(RR, Cc.T)) + np.dot(Cs, _prod(II, Cs.T))
 
     if returnC:
```

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_DWT.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_DWT.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_MonteCarlo.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_convolution.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_convolution.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic/uncertainty/propagate_filter.py` & `PyDynamic-2.4.1/src/PyDynamic/uncertainty/propagate_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.0/src/PyDynamic.egg-info/PKG-INFO` & `PyDynamic-2.4.1/src/PyDynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PyDynamic
-Version: 2.4.0
+Version: 2.4.1
 Summary: A software package for the analysis of dynamic measurements
 Home-page: https://ptb-m4d.github.io/PyDynamic/
 Author: Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, Martin Weber
 Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN
-Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.0/PyDynamic-2.4.0.tar.gz
-Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.0/
-Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.0/
+Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.1/PyDynamic-2.4.1.tar.gz
+Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.1/
+Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.1/
 Project-URL: Tracker, https://github.com/PTB-M4D/PyDynamic/issues
 Keywords: measurement uncertainty,dynamic measurements,metrology,GUM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.0 Summary: A software
+Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.1 Summary: A software
 package for the analysis of dynamic measurements Home-page: https://ptb-
 m4d.github.io/PyDynamic/ Author: Sascha EichstÃ¤dt, Maximilian Gruber, BjÃ¶rn
 Ludwig, Thomas Bruns, Martin Weber Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/
-download/v2.4.0/PyDynamic-2.4.0.tar.gz Project-URL: Documentation, https://
-pydynamic.readthedocs.io/en/v2.4.0/ Project-URL: Source, https://github.com/
-PTB-M4D/PyDynamic/tree/v2.4.0/ Project-URL: Tracker, https://github.com/PTB-
+download/v2.4.1/PyDynamic-2.4.1.tar.gz Project-URL: Documentation, https://
+pydynamic.readthedocs.io/en/v2.4.1/ Project-URL: Source, https://github.com/
+PTB-M4D/PyDynamic/tree/v2.4.1/ Project-URL: Tracker, https://github.com/PTB-
 M4D/PyDynamic/issues Keywords: measurement uncertainty,dynamic
 measurements,metrology,GUM Platform: UNKNOWN Classifier: Development Status ::
 4 - Beta Classifier: Topic :: Utilities Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: GNU Lesser
 General Public License v3 or later (LGPLv3+) Classifier: Programming Language
```

### Comparing `PyDynamic-2.4.0/src/PyDynamic.egg-info/SOURCES.txt` & `PyDynamic-2.4.1/src/PyDynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

