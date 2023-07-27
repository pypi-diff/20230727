# Comparing `tmp/pyfmrheo-0.1.0.tar.gz` & `tmp/pyfmrheo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmrheo-0.1.0.tar", last modified: Wed Jul 26 19:26:36 2023, max compression
+gzip compressed data, was "pyfmrheo-0.1.1.tar", last modified: Thu Jul 27 11:24:44 2023, max compression
```

## Comparing `pyfmrheo-0.1.0.tar` & `pyfmrheo-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.438665 pyfmrheo-0.1.0/
--rw-rw-rw-   0        0        0     1097 2023-07-26 18:07:23.000000 pyfmrheo-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      676 2023-07-26 19:26:36.439665 pyfmrheo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/README.md
--rw-rw-rw-   0        0        0      298 2023-07-26 18:38:53.000000 pyfmrheo-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      830 2023-07-26 19:26:36.445667 pyfmrheo-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.264625 pyfmrheo-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.285631 pyfmrheo-0.1.0/src/pyfmrheo/
--rw-rw-rw-   0        0        0       68 2023-07-26 18:08:53.000000 pyfmrheo-0.1.0/src/pyfmrheo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.370649 pyfmrheo-0.1.0/src/pyfmrheo/models/
--rw-rw-rw-   0        0        0      271 2023-07-26 18:36:55.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/__init__.py
--rw-rw-rw-   0        0        0     5535 2023-07-26 18:18:46.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/bec.py
--rw-rw-rw-   0        0        0     9653 2023-07-26 18:18:56.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/calibration.py
--rw-rw-rw-   0        0        0     3335 2023-07-26 18:19:02.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/double_powerlaw.py
--rw-rw-rw-   0        0        0     2759 2023-07-26 18:19:35.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/drag_sphere_model.py
--rw-rw-rw-   0        0        0      817 2023-07-26 18:19:38.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/geom_coeffs.py
--rw-rw-rw-   0        0        0     7596 2023-07-26 18:19:45.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/hertz.py
--rw-rw-rw-   0        0        0     6587 2023-07-26 18:19:49.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/rheology.py
--rw-rw-rw-   0        0        0     3145 2023-07-26 18:20:12.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/sader.py
--rw-rw-rw-   0        0        0     4393 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/sho.py
--rw-rw-rw-   0        0        0     3358 2023-07-26 18:20:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/sine.py
--rw-rw-rw-   0        0        0    12839 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/models/ting.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.422661 pyfmrheo-0.1.0/src/pyfmrheo/routines/
--rw-rw-rw-   0        0        0     3480 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/HertzFit.py
--rw-rw-rw-   0        0        0     4673 2023-04-26 10:18:29.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/MicrorheologyFFT.py
--rw-rw-rw-   0        0        0     6127 2023-04-26 10:18:54.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/MicrorheologySine.py
--rw-rw-rw-   0        0        0     1157 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/NonContactCal.py
--rw-rw-rw-   0        0        0     1186 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/PiezoCharacterization.py
--rw-rw-rw-   0        0        0     6517 2023-04-26 10:16:42.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/TingFit.py
--rw-rw-rw-   0        0        0     3603 2023-07-26 18:21:24.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/ViscousDragSteps.py
--rw-rw-rw-   0        0        0      215 2023-07-26 18:11:29.000000 pyfmrheo-0.1.0/src/pyfmrheo/routines/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.435664 pyfmrheo-0.1.0/src/pyfmrheo/utils/
--rw-rw-rw-   0        0        0       61 2023-07-26 18:11:49.000000 pyfmrheo-0.1.0/src/pyfmrheo/utils/__init__.py
--rw-rw-rw-   0        0        0     3382 2023-07-26 18:37:05.000000 pyfmrheo-0.1.0/src/pyfmrheo/utils/force_curves.py
--rw-rw-rw-   0        0        0     3733 2023-03-10 20:19:23.000000 pyfmrheo-0.1.0/src/pyfmrheo/utils/signal_processing.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:26:36.303635 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/
--rw-rw-rw-   0        0        0      676 2023-07-26 19:26:36.000000 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-26 19:26:36.000000 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:26:36.000000 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-26 19:26:36.000000 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 19:26:36.000000 pyfmrheo-0.1.0/src/pyfmrheo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2023-07-26 18:07:23.000000 pyfmrheo-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1098 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-07-27 11:21:44.000000 pyfmrheo-0.1.1/README.md
+-rw-rw-rw-   0        0        0      298 2023-07-27 11:23:13.000000 pyfmrheo-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      830 2023-07-27 11:24:44.239221 pyfmrheo-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.926586 pyfmrheo-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.966590 pyfmrheo-0.1.1/src/pyfmrheo/
+-rw-rw-rw-   0        0        0       68 2023-07-26 18:08:53.000000 pyfmrheo-0.1.1/src/pyfmrheo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.126607 pyfmrheo-0.1.1/src/pyfmrheo/models/
+-rw-rw-rw-   0        0        0      271 2023-07-26 18:36:55.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/__init__.py
+-rw-rw-rw-   0        0        0     5535 2023-07-26 18:18:46.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/bec.py
+-rw-rw-rw-   0        0        0     9653 2023-07-26 18:18:56.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/calibration.py
+-rw-rw-rw-   0        0        0     3335 2023-07-26 18:19:02.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/double_powerlaw.py
+-rw-rw-rw-   0        0        0     2759 2023-07-26 18:19:35.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/drag_sphere_model.py
+-rw-rw-rw-   0        0        0      817 2023-07-26 18:19:38.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/geom_coeffs.py
+-rw-rw-rw-   0        0        0     7596 2023-07-26 18:19:45.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/hertz.py
+-rw-rw-rw-   0        0        0     6587 2023-07-26 18:19:49.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/rheology.py
+-rw-rw-rw-   0        0        0     3145 2023-07-26 18:20:12.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sader.py
+-rw-rw-rw-   0        0        0     4393 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sho.py
+-rw-rw-rw-   0        0        0     3358 2023-07-26 18:20:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/sine.py
+-rw-rw-rw-   0        0        0    12839 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/models/ting.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.207218 pyfmrheo-0.1.1/src/pyfmrheo/routines/
+-rw-rw-rw-   0        0        0     3480 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/HertzFit.py
+-rw-rw-rw-   0        0        0     4673 2023-04-26 10:18:29.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologyFFT.py
+-rw-rw-rw-   0        0        0     6127 2023-04-26 10:18:54.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologySine.py
+-rw-rw-rw-   0        0        0     1157 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/NonContactCal.py
+-rw-rw-rw-   0        0        0     1186 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/PiezoCharacterization.py
+-rw-rw-rw-   0        0        0     6517 2023-04-26 10:16:42.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/TingFit.py
+-rw-rw-rw-   0        0        0     3603 2023-07-26 18:21:24.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/ViscousDragSteps.py
+-rw-rw-rw-   0        0        0      215 2023-07-26 18:11:29.000000 pyfmrheo-0.1.1/src/pyfmrheo/routines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:44.231221 pyfmrheo-0.1.1/src/pyfmrheo/utils/
+-rw-rw-rw-   0        0        0       61 2023-07-26 18:11:49.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/__init__.py
+-rw-rw-rw-   0        0        0     3382 2023-07-26 18:37:05.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/force_curves.py
+-rw-rw-rw-   0        0        0     3733 2023-03-10 20:19:23.000000 pyfmrheo-0.1.1/src/pyfmrheo/utils/signal_processing.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:24:43.998594 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/
+-rw-rw-rw-   0        0        0     1098 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 11:24:43.000000 pyfmrheo-0.1.1/src/pyfmrheo.egg-info/top_level.txt
```

### Comparing `pyfmrheo-0.1.0/LICENSE` & `pyfmrheo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/setup.cfg` & `pyfmrheo-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6d72 6865 6f0d 0a76 6572   = pyfmrheo..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 0d0a 6175  sion = 0.1.0..au
+00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 6175  sion = 0.1.1..au
 00000030: 7468 6f72 203d 204a 6176 6965 7220 4c6f  thor = Javier Lo
 00000040: 7065 7a20 416c 6f6e 736f 0d0a 6175 7468  pez Alonso..auth
 00000050: 6f72 5f65 6d61 696c 203d 206a 6c61 2e6c  or_email = jla.l
 00000060: 6f70 657a 2e31 3840 676d 6169 6c2e 636f  opez.18@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2070 7974 686f 6e20 7061 636b 6167   A python packag
 00000090: 6520 746f 2070 6572 666f 726d 2061 6e61  e to perform ana
```

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/bec.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/bec.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/calibration.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/calibration.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/double_powerlaw.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/double_powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/drag_sphere_model.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/drag_sphere_model.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/geom_coeffs.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/geom_coeffs.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/hertz.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/hertz.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/rheology.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/rheology.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/sader.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/sader.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/sho.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/sho.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/sine.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/sine.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/models/ting.py` & `pyfmrheo-0.1.1/src/pyfmrheo/models/ting.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/HertzFit.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/HertzFit.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/MicrorheologyFFT.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologyFFT.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/MicrorheologySine.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/MicrorheologySine.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/NonContactCal.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/NonContactCal.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/PiezoCharacterization.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/PiezoCharacterization.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/TingFit.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/TingFit.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/routines/ViscousDragSteps.py` & `pyfmrheo-0.1.1/src/pyfmrheo/routines/ViscousDragSteps.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/utils/force_curves.py` & `pyfmrheo-0.1.1/src/pyfmrheo/utils/force_curves.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo/utils/signal_processing.py` & `pyfmrheo-0.1.1/src/pyfmrheo/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `pyfmrheo-0.1.0/src/pyfmrheo.egg-info/SOURCES.txt` & `pyfmrheo-0.1.1/src/pyfmrheo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

