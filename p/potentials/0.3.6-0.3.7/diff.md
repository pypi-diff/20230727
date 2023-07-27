# Comparing `tmp/potentials-0.3.6.tar.gz` & `tmp/potentials-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\potentials\dist\.tmp-6b0tjit8\potentials-0.3.6.tar", last modified: Tue Apr 18 20:20:19 2023, max compression
+gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\potentials\dist\.tmp-9rpwyh_2\potentials-0.3.7.tar", last modified: Thu Jul 27 17:47:00 2023, max compression
```

## Comparing `potentials-0.3.6.tar` & `potentials-0.3.7.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/
--rw-rw-rw-   0        0        0     2776 2020-07-21 17:56:46.000000 potentials-0.3.6/LICENSE.TXT
--rw-rw-rw-   0        0        0      160 2022-06-01 17:13:54.000000 potentials-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4243 2023-04-18 20:20:19.000000 potentials-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2021-09-14 15:58:47.000000 potentials-0.3.6/README.rst
--rw-rw-rw-   0        0        0     3083 2023-04-04 19:01:01.000000 potentials-0.3.6/UPDATES.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/Database/
--rw-rw-rw-   0        0        0    14382 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/__init__.py
--rw-rw-rw-   0        0        0    15046 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_action.py
--rw-rw-rw-   0        0        0    18665 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_citation.py
--rw-rw-rw-   0        0        0    11655 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_faq.py
--rw-rw-rw-   0        0        0    14818 2023-04-04 15:40:25.000000 potentials-0.3.6/potentials/Database/_kim_potential.py
--rw-rw-rw-   0        0        0    42725 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_lammps_potential.py
--rw-rw-rw-   0        0        0    17183 2023-04-04 17:08:21.000000 potentials-0.3.6/potentials/Database/_potential.py
--rw-rw-rw-   0        0        0    24254 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_record.py
--rw-rw-rw-   0        0        0    10620 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_related_models.py
--rw-rw-rw-   0        0        0    12559 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_request.py
--rw-rw-rw-   0        0        0    11603 2023-03-24 17:02:24.000000 potentials-0.3.6/potentials/Database/_widgets.py
--rw-rw-rw-   0        0        0     1228 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/load_database.py
--rw-rw-rw-   0        0        0     9996 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Settings.py
--rw-rw-rw-   0        0        0        5 2023-04-04 17:52:48.000000 potentials-0.3.6/potentials/VERSION
--rw-rw-rw-   0        0        0      727 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/buildrecord/
--rw-rw-rw-   0        0        0      107 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/buildrecord/__init__.py
--rw-rw-rw-   0        0        0     1359 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/build_lammps_potential.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/
--rw-rw-rw-   0        0        0     6135 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EamBuilder.py
--rw-rw-rw-   0        0        0     5551 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EimBuilder.py
--rw-rw-rw-   0        0        0     5916 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/KimBuilder.py
--rw-rw-rw-   0        0        0     6212 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py
--rw-rw-rw-   0        0        0    13157 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PairBuilder.py
--rw-rw-rw-   0        0        0     6210 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py
--rw-rw-rw-   0        0        0    19230 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py
--rw-rw-rw-   0        0        0      315 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/paramfile/
--rw-rw-rw-   0        0        0    51311 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAM.py
--rw-rw-rw-   0        0        0    55972 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAMAlloy.py
--rw-rw-rw-   0        0        0    57842 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAMFS.py
--rw-rw-rw-   0        0        0      192 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/paramfile/__init__.py
--rw-rw-rw-   0        0        0     6747 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/converters.py
--rw-rw-rw-   0        0        0     2188 2022-09-19 13:36:46.000000 potentials-0.3.6/potentials/paramfile/load_eam.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/record/
--rw-rw-rw-   0        0        0    13706 2023-04-07 14:29:04.000000 potentials-0.3.6/potentials/record/Action.py
--rw-rw-rw-   0        0        0     7400 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Artifact.py
--rw-rw-rw-   0        0        0    21924 2023-04-04 16:04:52.000000 potentials-0.3.6/potentials/record/BasePotentialLAMMPS.py
--rw-rw-rw-   0        0        0    11669 2023-04-03 20:05:11.000000 potentials-0.3.6/potentials/record/Citation.py
--rw-rw-rw-   0        0        0     5378 2023-04-03 20:06:44.000000 potentials-0.3.6/potentials/record/FAQ.py
--rw-rw-rw-   0        0        0    12748 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Implementation.py
--rw-rw-rw-   0        0        0     5258 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Link.py
--rw-rw-rw-   0        0        0     5363 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Parameter.py
--rw-rw-rw-   0        0        0    17400 2023-04-04 17:06:29.000000 potentials-0.3.6/potentials/record/Potential.py
--rw-rw-rw-   0        0        0    25778 2023-04-04 15:19:25.000000 potentials-0.3.6/potentials/record/PotentialLAMMPS.py
--rw-rw-rw-   0        0        0    36541 2023-04-04 16:09:47.000000 potentials-0.3.6/potentials/record/PotentialLAMMPSKIM.py
--rw-rw-rw-   0        0        0    11939 2023-04-03 20:24:30.000000 potentials-0.3.6/potentials/record/Request.py
--rw-rw-rw-   0        0        0      655 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/tools/
--rw-rw-rw-   0        0        0      446 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/tools/__pycache__/
--rw-rw-rw-   0        0        0      543 2022-03-31 22:26:25.000000 potentials-0.3.6/potentials/tools/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1173 2019-07-31 19:39:47.000000 potentials-0.3.6/potentials/tools/__pycache__/aslist.cpython-37.pyc
--rw-rw-rw-   0        0        0     7975 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/atomic_info.cpython-37.pyc
--rw-rw-rw-   0        0        0   152808 2021-08-03 17:29:36.000000 potentials-0.3.6/potentials/tools/__pycache__/atomicdata.cpython-37.pyc
--rw-rw-rw-   0        0        0     1399 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/numderivative.cpython-37.pyc
--rw-rw-rw-   0        0        0     1546 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/parse_authors.cpython-37.pyc
--rw-rw-rw-   0        0        0      601 2020-07-23 20:51:50.000000 potentials-0.3.6/potentials/tools/__pycache__/screen_input.cpython-37.pyc
--rw-rw-rw-   0        0        0     1610 2019-12-28 16:49:05.000000 potentials-0.3.6/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc
--rw-rw-rw-   0        0        0    11550 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/atomic_info.py
--rw-rw-rw-   0        0        0   132864 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/atomicdata.csv
--rw-rw-rw-   0        0        0     1448 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/numderivative.py
--rw-rw-rw-   0        0        0     2200 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/parse_authors.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsd/
--rw-rw-rw-   0        0        0     9468 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Action.xsd
--rw-rw-rw-   0        0        0     3699 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Citation.xsd
--rw-rw-rw-   0        0        0      448 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/xsd/FAQ.xsd
--rw-rw-rw-   0        0        0    16696 2022-07-22 17:55:47.000000 potentials-0.3.6/potentials/xsd/Potential.xsd
--rw-rw-rw-   0        0        0     5944 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Request.xsd
--rw-rw-rw-   0        0        0        0 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsd/__pycache__/
--rw-rw-rw-   0        0        0      164 2022-07-25 16:45:13.000000 potentials-0.3.6/potentials/xsd/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1318 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/artifact.xsd
--rw-rw-rw-   0        0        0     3982 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/implementation.xsd
--rw-rw-rw-   0        0        0     1316 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/link.xsd
--rw-rw-rw-   0        0        0      667 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/parameter.xsd
--rw-rw-rw-   0        0        0     5499 2022-07-25 16:28:26.000000 potentials-0.3.6/potentials/xsd/potential_LAMMPS.xsd
--rw-rw-rw-   0        0        0     1718 2022-07-25 16:28:08.000000 potentials-0.3.6/potentials/xsd/potential_LAMMPS_KIM.xsd
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsl/
--rw-rw-rw-   0        0        0      891 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Action.xsl
--rw-rw-rw-   0        0        0     3657 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Citation.xsl
--rw-rw-rw-   0        0        0      583 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/FAQ.xsl
--rw-rw-rw-   0        0        0    10387 2022-10-03 14:26:23.000000 potentials-0.3.6/potentials/xsl/Potential.xsl
--rw-rw-rw-   0        0        0     1759 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Request.xsl
--rw-rw-rw-   0        0        0        0 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsl/__pycache__/
--rw-rw-rw-   0        0        0      164 2021-08-09 15:09:12.000000 potentials-0.3.6/potentials/xsl/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      584 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/artifact.xsl
--rw-rw-rw-   0        0        0     5446 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/implementation.xsl
--rw-rw-rw-   0        0        0      580 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/link.xsl
--rw-rw-rw-   0        0        0      582 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/parameter.xsl
--rw-rw-rw-   0        0        0     2203 2022-07-22 20:07:25.000000 potentials-0.3.6/potentials/xsl/potential_LAMMPS.xsl
--rw-rw-rw-   0        0        0     2218 2022-07-25 16:04:25.000000 potentials-0.3.6/potentials/xsl/potential_LAMMPS_KIM.xsl
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/
--rw-rw-rw-   0        0        0     4243 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3360 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-02-04 15:07:00.000000 potentials-0.3.6/potentials.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-03-31 22:10:53.000000 potentials-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 20:20:19.000000 potentials-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-04-04 18:08:19.000000 potentials-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/tests/
--rw-rw-rw-   0        0        0        0 2022-10-03 14:26:23.000000 potentials-0.3.6/tests/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/
+-rw-rw-rw-   0        0        0     2776 2020-07-21 17:56:46.000000 potentials-0.3.7/LICENSE.TXT
+-rw-rw-rw-   0        0        0      160 2022-06-01 17:13:54.000000 potentials-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4296 2023-07-27 17:47:00.000000 potentials-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2021-09-14 15:58:47.000000 potentials-0.3.7/README.rst
+-rw-rw-rw-   0        0        0     3346 2023-07-26 14:09:10.000000 potentials-0.3.7/UPDATES.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/Database/
+-rw-rw-rw-   0        0        0    14382 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/__init__.py
+-rw-rw-rw-   0        0        0    15046 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_action.py
+-rw-rw-rw-   0        0        0    18665 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_citation.py
+-rw-rw-rw-   0        0        0    11655 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_faq.py
+-rw-rw-rw-   0        0        0    14818 2023-04-04 15:40:25.000000 potentials-0.3.7/potentials/Database/_kim_potential.py
+-rw-rw-rw-   0        0        0    42725 2023-07-27 15:58:41.000000 potentials-0.3.7/potentials/Database/_lammps_potential.py
+-rw-rw-rw-   0        0        0    17183 2023-04-04 17:08:21.000000 potentials-0.3.7/potentials/Database/_potential.py
+-rw-rw-rw-   0        0        0    24254 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_record.py
+-rw-rw-rw-   0        0        0    10620 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_related_models.py
+-rw-rw-rw-   0        0        0    12559 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/_request.py
+-rw-rw-rw-   0        0        0    11603 2023-03-24 17:02:24.000000 potentials-0.3.7/potentials/Database/_widgets.py
+-rw-rw-rw-   0        0        0     1228 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Database/load_database.py
+-rw-rw-rw-   0        0        0     9996 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/Settings.py
+-rw-rw-rw-   0        0        0        5 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/VERSION
+-rw-rw-rw-   0        0        0      914 2023-07-27 16:00:12.000000 potentials-0.3.7/potentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/buildrecord/
+-rw-rw-rw-   0        0        0      107 2022-03-31 22:10:53.000000 potentials-0.3.7/potentials/buildrecord/__init__.py
+-rw-rw-rw-   0        0        0     1359 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/build_lammps_potential.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/
+-rw-rw-rw-   0        0        0     6135 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/EamBuilder.py
+-rw-rw-rw-   0        0        0     5551 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/EimBuilder.py
+-rw-rw-rw-   0        0        0     5916 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/KimBuilder.py
+-rw-rw-rw-   0        0        0     6212 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py
+-rw-rw-rw-   0        0        0    13157 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/PairBuilder.py
+-rw-rw-rw-   0        0        0     6210 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py
+-rw-rw-rw-   0        0        0    19230 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py
+-rw-rw-rw-   0        0        0      315 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/paramfile/
+-rw-rw-rw-   0        0        0    30487 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/paramfile/ADP.py
+-rw-rw-rw-   0        0        0    51311 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/paramfile/EAM.py
+-rw-rw-rw-   0        0        0    55972 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/paramfile/EAMAlloy.py
+-rw-rw-rw-   0        0        0    57842 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/paramfile/EAMFS.py
+-rw-rw-rw-   0        0        0      232 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/paramfile/__init__.py
+-rw-rw-rw-   0        0        0     8548 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/paramfile/converters.py
+-rw-rw-rw-   0        0        0     2399 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/paramfile/load_eam.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/record/
+-rw-rw-rw-   0        0        0    13885 2023-05-31 16:11:38.000000 potentials-0.3.7/potentials/record/Action.py
+-rw-rw-rw-   0        0        0     7687 2023-05-31 16:15:27.000000 potentials-0.3.7/potentials/record/Artifact.py
+-rw-rw-rw-   0        0        0    21961 2023-07-26 14:09:10.000000 potentials-0.3.7/potentials/record/BasePotentialLAMMPS.py
+-rw-rw-rw-   0        0        0    11838 2023-05-31 16:15:21.000000 potentials-0.3.7/potentials/record/Citation.py
+-rw-rw-rw-   0        0        0     5557 2023-05-31 16:15:18.000000 potentials-0.3.7/potentials/record/FAQ.py
+-rw-rw-rw-   0        0        0    12998 2023-05-31 16:15:13.000000 potentials-0.3.7/potentials/record/Implementation.py
+-rw-rw-rw-   0        0        0     5571 2023-05-31 16:15:08.000000 potentials-0.3.7/potentials/record/Link.py
+-rw-rw-rw-   0        0        0     5613 2023-05-31 16:15:03.000000 potentials-0.3.7/potentials/record/Parameter.py
+-rw-rw-rw-   0        0        0    17569 2023-05-31 16:14:44.000000 potentials-0.3.7/potentials/record/Potential.py
+-rw-rw-rw-   0        0        0    27194 2023-05-31 16:14:39.000000 potentials-0.3.7/potentials/record/PotentialLAMMPS.py
+-rw-rw-rw-   0        0        0    36720 2023-05-31 16:14:33.000000 potentials-0.3.7/potentials/record/PotentialLAMMPSKIM.py
+-rw-rw-rw-   0        0        0    11993 2023-05-31 16:14:29.000000 potentials-0.3.7/potentials/record/Request.py
+-rw-rw-rw-   0        0        0      655 2022-03-31 22:10:53.000000 potentials-0.3.7/potentials/record/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/tools/
+-rw-rw-rw-   0        0        0      446 2022-03-31 22:10:53.000000 potentials-0.3.7/potentials/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/tools/__pycache__/
+-rw-rw-rw-   0        0        0      543 2022-03-31 22:26:25.000000 potentials-0.3.7/potentials/tools/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1173 2019-07-31 19:39:47.000000 potentials-0.3.7/potentials/tools/__pycache__/aslist.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7975 2022-05-25 17:25:42.000000 potentials-0.3.7/potentials/tools/__pycache__/atomic_info.cpython-37.pyc
+-rw-rw-rw-   0        0        0   152808 2021-08-03 17:29:36.000000 potentials-0.3.7/potentials/tools/__pycache__/atomicdata.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1399 2022-05-25 17:25:42.000000 potentials-0.3.7/potentials/tools/__pycache__/numderivative.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1546 2022-05-25 17:25:42.000000 potentials-0.3.7/potentials/tools/__pycache__/parse_authors.cpython-37.pyc
+-rw-rw-rw-   0        0        0      601 2020-07-23 20:51:50.000000 potentials-0.3.7/potentials/tools/__pycache__/screen_input.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1610 2019-12-28 16:49:05.000000 potentials-0.3.7/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc
+-rw-rw-rw-   0        0        0    11550 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/tools/atomic_info.py
+-rw-rw-rw-   0        0        0   132864 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/tools/atomicdata.csv
+-rw-rw-rw-   0        0        0     1448 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/tools/numderivative.py
+-rw-rw-rw-   0        0        0     2200 2022-05-23 16:10:08.000000 potentials-0.3.7/potentials/tools/parse_authors.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/xsd/
+-rw-rw-rw-   0        0        0     9468 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/Action.xsd
+-rw-rw-rw-   0        0        0     3699 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/Citation.xsd
+-rw-rw-rw-   0        0        0      448 2022-03-31 22:10:53.000000 potentials-0.3.7/potentials/xsd/FAQ.xsd
+-rw-rw-rw-   0        0        0    16696 2022-07-22 17:55:47.000000 potentials-0.3.7/potentials/xsd/Potential.xsd
+-rw-rw-rw-   0        0        0     5944 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/Request.xsd
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/xsd/__pycache__/
+-rw-rw-rw-   0        0        0      164 2022-07-25 16:45:13.000000 potentials-0.3.7/potentials/xsd/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1318 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/artifact.xsd
+-rw-rw-rw-   0        0        0     3982 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/implementation.xsd
+-rw-rw-rw-   0        0        0     1316 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/link.xsd
+-rw-rw-rw-   0        0        0      667 2021-08-03 11:09:29.000000 potentials-0.3.7/potentials/xsd/parameter.xsd
+-rw-rw-rw-   0        0        0     5499 2022-07-25 16:28:26.000000 potentials-0.3.7/potentials/xsd/potential_LAMMPS.xsd
+-rw-rw-rw-   0        0        0     1718 2022-07-25 16:28:08.000000 potentials-0.3.7/potentials/xsd/potential_LAMMPS_KIM.xsd
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/xsl/
+-rw-rw-rw-   0        0        0      891 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/Action.xsl
+-rw-rw-rw-   0        0        0     3657 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/Citation.xsl
+-rw-rw-rw-   0        0        0      583 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/FAQ.xsl
+-rw-rw-rw-   0        0        0    10387 2022-10-03 14:26:23.000000 potentials-0.3.7/potentials/xsl/Potential.xsl
+-rw-rw-rw-   0        0        0     1759 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/Request.xsl
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials/xsl/__pycache__/
+-rw-rw-rw-   0        0        0      164 2021-08-09 15:09:12.000000 potentials-0.3.7/potentials/xsl/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      584 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/artifact.xsl
+-rw-rw-rw-   0        0        0     5446 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/implementation.xsl
+-rw-rw-rw-   0        0        0      580 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/link.xsl
+-rw-rw-rw-   0        0        0      582 2021-08-03 11:09:30.000000 potentials-0.3.7/potentials/xsl/parameter.xsl
+-rw-rw-rw-   0        0        0     2203 2022-07-22 20:07:25.000000 potentials-0.3.7/potentials/xsl/potential_LAMMPS.xsl
+-rw-rw-rw-   0        0        0     2218 2022-07-25 16:04:25.000000 potentials-0.3.7/potentials/xsl/potential_LAMMPS_KIM.xsl
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/potentials.egg-info/
+-rw-rw-rw-   0        0        0     4296 2023-07-27 17:46:59.000000 potentials-0.3.7/potentials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3388 2023-07-27 17:46:59.000000 potentials-0.3.7/potentials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:46:59.000000 potentials-0.3.7/potentials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-02-04 15:07:00.000000 potentials-0.3.7/potentials.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      121 2023-07-27 17:46:59.000000 potentials-0.3.7/potentials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 17:46:59.000000 potentials-0.3.7/potentials.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-03-31 22:10:53.000000 potentials-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:47:00.000000 potentials-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1798 2023-07-27 17:45:11.000000 potentials-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:47:00.000000 potentials-0.3.7/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-03 14:26:23.000000 potentials-0.3.7/tests/test_settings.py
```

### Comparing `potentials-0.3.6/LICENSE.TXT` & `potentials-0.3.7/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/PKG-INFO` & `potentials-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: potentials
-Version: 0.3.6
+Version: 0.3.7
 Summary: API database tools for accessing the NIST Interatomic Potentials Repository: explore and download interatomic potentials and computed properties.
 Home-page: https://github.com/usnistgov/potentials
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,interatomic potential,force field
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
 
 ==========
 potentials
 ==========
```

### Comparing `potentials-0.3.6/README.rst` & `potentials-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/UPDATES.rst` & `potentials-0.3.7/UPDATES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Updates
 =======
 
+0.3.7
+-----
+
+- Record objects are updated allowing for each to be assigned a default
+  database object from which record methods can retrieve additional database
+  content as needed.
+- A new parameter file builder tool has been added for ADP potentials.
+
 0.3.6
 -----
 
 - Code adjustments related to yabadaba 0.2.0 updates to Query handling.
   The parameters supported by query operations can now be viewed with
   querydoc.
```

### Comparing `potentials-0.3.6/potentials/Database/__init__.py` & `potentials-0.3.7/potentials/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_action.py` & `potentials-0.3.7/potentials/Database/_action.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_citation.py` & `potentials-0.3.7/potentials/Database/_citation.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_faq.py` & `potentials-0.3.7/potentials/Database/_faq.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_kim_potential.py` & `potentials-0.3.7/potentials/Database/_kim_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_lammps_potential.py` & `potentials-0.3.7/potentials/Database/_lammps_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_potential.py` & `potentials-0.3.7/potentials/Database/_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_record.py` & `potentials-0.3.7/potentials/Database/_record.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_related_models.py` & `potentials-0.3.7/potentials/Database/_related_models.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_request.py` & `potentials-0.3.7/potentials/Database/_request.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/_widgets.py` & `potentials-0.3.7/potentials/Database/_widgets.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Database/load_database.py` & `potentials-0.3.7/potentials/Database/load_database.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/Settings.py` & `potentials-0.3.7/potentials/Settings.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/build_lammps_potential.py` & `potentials-0.3.7/potentials/buildrecord/build_lammps_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EamBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/EamBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EimBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/EimBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/KimBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/KimBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PairBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/PairBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py` & `potentials-0.3.7/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/paramfile/EAM.py` & `potentials-0.3.7/potentials/paramfile/EAM.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/paramfile/EAMAlloy.py` & `potentials-0.3.7/potentials/paramfile/EAMAlloy.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/paramfile/EAMFS.py` & `potentials-0.3.7/potentials/paramfile/EAMFS.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/paramfile/converters.py` & `potentials-0.3.7/potentials/paramfile/converters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Union
 
 # https://numpy.org/
 import numpy as np
 
 # Local imports
 from ..tools import aslist
-from . import EAM, EAMAlloy, EAMFS
+from . import EAM, EAMAlloy, EAMFS, ADP
 
 def eam_to_eam_alloy(eam: Union[str, io.IOBase, EAM, list],
                      symbol: Union[str, list],
                      numr: Optional[int] = None,
                      cutoffr: Optional[float] = None,
                      deltar: Optional[float] = None,
                      numrho: Optional[int] = None,
@@ -190,8 +190,64 @@
             fs.set_rho_r(symbolpair, table=alloy.rho_r(symbol))
     
         # Copy over r*phi(r)
         for symbol2 in alloy.symbols[:i+1]:
             symbolpair = [symbol, symbol2]
             fs.set_rphi_r(symbolpair, table=alloy.rphi_r(symbolpair))
     
-    return fs
+    return fs
+
+def eam_alloy_to_adp(alloy: EAMAlloy) -> ADP:
+    """
+    Converts a parameter file in the eam/alloy format to the adp format.
+    NOTE: the u(r) and w(r) tables are automatically set to all zeros.
+    
+    Parameters
+    ----------
+    alloy : path, file-like object, or potentials.paramfile.EAMAlloy
+        A parameter file in the LAMMPS pair_style eam/alloy setfl format.
+    
+    Returns
+    -------
+    potentials.paramfile.ADP
+        The eam/alloy setfl parameter file converted and combined into an
+        adp setfl file representation.
+    """
+    # Load parameter file
+    if not isinstance(alloy, EAMAlloy):
+        alloy = EAMAlloy(alloy)
+    
+    # Initialize fs object
+    adp = ADP()
+    
+    # Copy over header
+    adp.header = alloy.header
+
+    # Copy over r
+    adp.set_r(num=alloy.numr, cutoff=alloy.cutoffr, delta=alloy.deltar)
+
+    # Copy over rho
+    adp.set_rho(num=alloy.numrho, cutoff=alloy.cutoffrho, delta=alloy.deltarho)
+    
+    for i, symbol in enumerate(alloy.symbols):
+        
+        # Copy over symbol info
+        adp.set_symbol_info(**alloy.symbol_info(symbol))
+    
+    for i, symbol in enumerate(alloy.symbols):
+        
+        # Copy over F(rho)
+        adp.set_F_rho(symbol, table=alloy.F_rho(symbol))
+        
+        # Copy over rho(r)
+        adp.set_rho_r(symbol, table=alloy.rho_r(symbol))
+    
+        # Copy over r*phi(r)
+        for symbol2 in alloy.symbols[:i+1]:
+            symbolpair = [symbol, symbol2]
+            adp.set_rphi_r(symbolpair, table=alloy.rphi_r(symbolpair))
+            
+            # Set u(r) and w(r) to all zeros
+            adp.set_u_r(symbolpair, table=np.zeros_like(adp.r))
+            adp.set_w_r(symbolpair, table=np.zeros_like(adp.r))
+    
+    return adp
```

### Comparing `potentials-0.3.6/potentials/paramfile/load_eam.py` & `potentials-0.3.7/potentials/paramfile/load_eam.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # coding: utf-8
 # Standard libraries
 import io
 from typing import Optional, Union
 
 # Local imports
-from . import EAM, EAMAlloy, EAMFS
+from . import EAM, EAMAlloy, EAMFS, ADP
 
 def load_eam(f: Union[str, io.IOBase],
-             style: Optional[str] = None) -> Union[EAM, EAMAlloy, EAMFS]:
+             style: Optional[str] = None) -> Union[EAM, EAMAlloy, EAMFS, ADP]:
     """
     Loads a LAMMPS-compatible EAM parameter file.
     
     Parameters
     ----------
     f : path-like object or file-like object
         The parameter file to read in, either as a file path or as an open
         file-like object.
     style : str, optional
         The parameter file format.  'eam' will load funcfl files for the LAMMPS
         eam pair_style.  'eam/alloy' or 'alloy' will load setfl files for the
         LAMMPS eam/alloy pair_style.  'eam/fs' or 'fs' will load setfl files for
-        the eam/fs pair_style.  If not given, will attempt to load the file
-        using the different styles.
+        the eam/fs pair_style.  'ap' will load setfl files for the adp pair_style.
+        If not given, will attempt to load the file using the different styles.
         
     Returns
     -------
-    EAM, EAMAlloy or EAMFS
+    EAM, EAMAlloy, EAMFS or ADP
         The loaded parameter file content.
     """
     
     # Shortcut to classes for known styles
     if style == 'eam':
         return EAM(f)
     elif style == 'eam/alloy' or style == 'alloy':
         return EAMAlloy(f)
     elif style == 'eam/fs' or style == 'fs':
         return EAMFS(f)
+    elif style == 'adp':
+        return ADP(f)
     elif style is not None:
         raise ValueError('Unknown style')
     
     # Check if f is a file
     if hasattr(f, 'readlines'):
         closefile = False
     else:
@@ -68,10 +70,15 @@
         return obj
     
     # Test if eam/fs
     obj = test_style(f, EAMFS)
     if obj is not None:
         return obj
     
+    # Test if adp
+    obj = test_style(f, ADP)
+    if obj is not None:
+        return obj
+
     if closefile:
         f.close()
     raise ValueError('Failed to load as any known style')
```

### Comparing `potentials-0.3.6/potentials/record/Action.py` & `potentials-0.3.7/potentials/record/Action.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,26 +145,29 @@
     Class for representing Action records that document changes to the
     Interatomic Potentials Repository.
     """
 
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         date : str or datetime.date, optional
             The date to assign to the record.
         type : str, optional
             The Action type to assign to the record.
         potentials : list, optional
             Potential or model contents for Potential records to associate
             with the action.
@@ -173,15 +176,15 @@
         """
         # Set default values
         self.type = 'new posting'
         self.__potentials = []
         self.date = datetime.date.today()
         self.comment = None
 
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'Action'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/Artifact.py` & `potentials-0.3.7/potentials/record/Artifact.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,33 +17,38 @@
     """
     Class for describing artifacts (files accessible online). Note that this is
     meant as a component class for other record objects.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes an Artifact object to describe a file accessible online
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The name to assign to the record.  Not used by this class.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
+            Not used by this class.
         filename : str, optional
             The name of the file without path information.
         label : str, optional
             A short description label.
         url : str, optional
             URL for file where downloaded, if available.
         """
         assert name is None, 'name is not used by this class'
-        super().__init__(model=model, name=name, **kwargs)
+        assert database is None, 'database is not used by this class'
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'artifact'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/BasePotentialLAMMPS.py` & `potentials-0.3.7/potentials/record/BasePotentialLAMMPS.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,28 @@
 
 class BasePotentialLAMMPS(Record):
     """
     Base parent class for PotentialLAMMPS objects
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
-                 name: Optional[str] = None):
+                 name: Optional[str] = None,
+                 database = None):
         """
         Initializes an instance and loads content from a data model.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The record name to use.  If not given, this will be set to the
             potential's id.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         **kwargs : any, optional
             Any other keyword parameters supported by the child class.
         """
         # Check if base class is initialized directly
         if self.__module__ == __name__:
             raise TypeError("don't use base class")
 
@@ -56,84 +59,83 @@
         self._symbols = []
         self._masses = []
         self._charges = []
         self._pair_style = None
         self._allsymbols = False
         self._status = None
 
-
         # Pass parameters to load
-        super().__init__(model, name=name)
-        
+        super().__init__(model, name=name, database=database)
+
     @property
     def id(self) -> str:
         """str : Human-readable identifier for the LAMMPS implementation."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._id
-    
+
     @property
     def key(self) -> str:
         """str : uuid hash-key for the LAMMPS implementation."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._key
-    
+
     @property
     def url(self):
         """str : URL for an online copy of the record."""
         return self._url
 
     @property
     def potid(self) -> str:
         """str : Human-readable identifier for the potential model."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._potid
-    
+
     @property
     def potkey(self) -> str:
         """str : uuid hash-key for the potential model."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._potkey
-    
+
     @property
     def poturl(self):
         """str : URL for an online copy of the record."""
         return self._poturl
 
     @property
     def units(self) -> str:
         """str : LAMMPS units option."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._units
-    
+
     @property
     def atom_style(self) -> str:
         """str : LAMMPS atom_style option."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._atom_style
-    
+
     @property
     def symbols(self) -> list:
         """list of str : All atom-model symbols."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._symbols
-    
+
     @property
     def pair_style(self) -> str:
         """str : LAMMPS pair_style option."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._pair_style
-    
+
     @property
     def allsymbols(self) -> bool:
         """bool : indicates if all model symbols must be listed."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._allsymbols
 
@@ -144,15 +146,15 @@
             raise AttributeError('No model information loaded')
         return self._status
 
     @property
     def pot_dir(self):
         """str : The directory containing files associated with a given potential."""
         return self.__pot_dir
-    
+
     @pot_dir.setter
     def pot_dir(self, value: str):
         self.__pot_dir = str(value)
 
     @property
     def artifacts(self) -> list:
         """list : The list of file artifacts for the potential including download URLs."""
@@ -183,18 +185,18 @@
         Returns
         -------
         num_downloaded : int
             The number of artifacts downloaded.
         num_skipped : int
             The number of artifacts not downloaded.
         """
-        
+
         if pot_dir is not None:
             self.pot_dir = pot_dir
-        
+
         num_downloaded = 0
         num_skipped = 0
         if len(self.artifacts) > 0:
             if not Path(self.pot_dir).is_dir():
                 Path(self.pot_dir).mkdir(parents=True)
 
             for artifact in self.artifacts:
@@ -229,15 +231,15 @@
         self._id = pot['id']
         try:
             self.name
         except AttributeError:
             self.name = self.id
 
         self._key = pot['key']
-        self._url = pot.get('key', None)
+        self._url = pot.get('url', None)
         try:
             self._potid = pot['potential']['id']
         except (KeyError, TypeError):
             self._potid = None
         try:
             self._potkey = pot['potential']['key']
         except (KeyError, TypeError):
@@ -285,25 +287,25 @@
         Returns
         -------
         list
             The updated list.
         """
         # Convert symbols to a list if needed
         symbols = aslist(symbols)
-        
+
         # Check that all symbols are set
         for symbol in symbols:
             assert symbol is not None, 'symbols list incomplete: found None value'
-        
+
         # Add missing symbols if potential's allsymbols is True
         if self.allsymbols:
             for symbol in self.symbols:
                 if symbol not in symbols:
                     symbols.append(symbol)
-        
+
         return symbols
 
     def elements(self,
                  symbols: Union[str, list, None] = None) -> list:
         """
         Returns a list of element names associated with atom-model symbols.
         
@@ -317,24 +319,24 @@
         -------
         list of str
             The str element symbols corresponding to the atom-model symbols.
         """
         # Return all elements if symbols is None
         if symbols is None:
             return self._elements
-        
+
         # Normalize symbols
         symbols = self.normalize_symbols(symbols)
-        
+
         # Get all matching elements
         elements = []
         for symbol in symbols:
             i = self.symbols.index(symbol)
             elements.append(self._elements[i])
-        
+
         return elements
 
     def masses(self,
                symbols: Union[str, list, None] = None,
                prompt: bool = False) -> list:
         """
         Returns a list of atomic/ionic masses associated with atom-model
@@ -358,24 +360,24 @@
 
         # Use all symbols if symbols is None
         if symbols is None:
             symbols = self.symbols
         else:
             # Normalize symbols
             symbols = self.normalize_symbols(symbols)
-        
+
         # Get all matching masses
         masses = []
         for symbol in symbols:
             i = self.symbols.index(symbol)
             if self._masses[i] is None:
                 masses.append(atomic_mass(self._elements[i], prompt=prompt))
             else:
                 masses.append(self._masses[i])
-        
+
         return masses
 
     def charges(self,
                 symbols: Union[str, list, None] = None) -> list:
         """
         Returns a list of atomic charges associated with atom-model symbols.
         Will have a None value if not assigned.
@@ -393,21 +395,21 @@
         """
         # Use all symbols if symbols is None
         if symbols is None:
             symbols = self.symbols
         else:
             # Normalize symbols
             symbols = self.normalize_symbols(symbols)
-        
+
         # Get all matching charges
         charges = []
         for symbol in symbols:
             i = self.symbols.index(symbol)
             charges.append(self._charges[i])
-        
+
         return charges
 
     def metadata(self) -> dict:
         """
         Generates a dict of simple metadata values associated with the record.
         Useful for quickly comparing records and for building pandas.DataFrames
         for multiple records of the same style.
```

### Comparing `potentials-0.3.6/potentials/record/Citation.py` & `potentials-0.3.7/potentials/record/Citation.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,33 +24,35 @@
     """
     Class for representing Citation metadata records.
     """
 
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
-        
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         """
         # Set default values
         self.__bib = {}
         self.bib['note'] = ''
 
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'Citation'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/FAQ.py` & `potentials-0.3.7/potentials/record/FAQ.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,30 +16,33 @@
     """
     Class for representing FAQ records that document the FAQs for the NIST
     Interatomic Potentials Repository.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         """
         self.__question = None
         self.__answer = None
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'FAQ'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/Implementation.py` & `potentials-0.3.7/potentials/record/Implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,25 @@
     """
     Class for representing Implementation metadata records. . Note that this is
     meant as a component class for other record objects.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The name to assign to the record.  Not used by this class.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         type : str, optional
             Describes the format for the implementation.
         key : str, optional
             The UUID4 key to assign to the implementation.
         id : str, optional
             The unique id to assign to the implementation.
         status : str, optional
@@ -48,15 +51,16 @@
             Any Artifact objects or data to associate with the implementation.
         parameters : list, optional
             Any Parameter objects or data to associate with the implementation.
         links : list, optional
             Any Link objects or data to associate with the implementation.
         """
         assert name is None, 'name is not used by this class'
-        super().__init__(model=model, name=name, **kwargs)
+        assert database is None, 'database is not used by this class'
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'implementation'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/Link.py` & `potentials-0.3.7/potentials/record/Link.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,38 @@
 class Link(Record):
     """
     Class for describing website link
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Link object providing a hyperlink to content. Note that
         this is meant as a component class for other record objects.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The name to assign to the record.  Not used by this class.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         url : str, optional
             URL for the link.
         label : str, optional
             A short description label.
         linktext : str, optional
             The text for the link, i.e. what gets clicked on.
         """
-        super().__init__(model=model, name=name, **kwargs)
+        assert name is None, 'name is not used by this class'
+        assert database is None, 'database is not used by this class'
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'link'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/Parameter.py` & `potentials-0.3.7/potentials/record/Parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,37 @@
     """
     Class for describing parameter values. Note that this is
     meant as a component class for other record objects.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Parameter object to describe parameter values.
 
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The name to assign to the record.  Not used by this class.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         paramname : str, optional
             The name of the parameter or string parameter line.
         value : float, optional
             The value of the parameter.
         unit : str, optional
             Units associated with value.
         """
         assert name is None, 'name is not used by this class'
-        super().__init__(model=model, name=name, **kwargs)
+        assert database is None, 'database is not used by this class'
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'parameter'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/Potential.py` & `potentials-0.3.7/potentials/record/Potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,41 +21,43 @@
     """
     Class for representing Potential metadata records.
     """
 
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
-        
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         """
         # Set default values
         self.url = None
         self.elements = None
         self.key = None
         self.othername = None
         self.fictional = False
         self.modelname = None
         self.notes = None
         self.recorddate = datetime.date.today()
         self.__citations = []
         self.__implementations = []
 
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'Potential'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/PotentialLAMMPS.py` & `potentials-0.3.7/potentials/record/PotentialLAMMPS.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,31 +24,34 @@
     """
     Class for building LAMMPS input lines from a potential-LAMMPS data model.
     """
     
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  pot_dir: Optional[str] = None):
         """
         Initializes an instance and loads content from a data model.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The record name to use.  If not given, this will be set to the
             potential's id.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         pot_dir : str, optional
             The path to a directory containing any artifacts associated with
             the potential.  Default value is None, which assumes any required
             files will be in the working directory when LAMMPS is executed.
         """
-        super().__init__(model=model, name=name)
+        super().__init__(model=model, name=name, database=database)
         if pot_dir is not None:
             self.pot_dir = pot_dir
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'potential_LAMMPS'
@@ -633,8 +636,40 @@
         # Set pair_info
         info += '\n'
         info += self.pair_info(symbols=symbols, masses=masses, prompt=prompt,
                                comments=comments)
 
         return info
 
-    
+    def get_file(self,
+                 filename: Union[str, Path],
+                 localroot: Union[str, Path, None] = None):
+        """
+        Retrieves a file either locally or from the record's tar archive.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The name/path for the file.  For local files, this is taken
+            relative to localroot.  For files in the tar archive, this is taken
+            relative to the tar's root directory which is always named for the
+            record, i.e., {self.name}/{filename}.
+        localroot : str, Path or None, optional
+            The local root directory that filename (if it exists) is relative
+            to.  The default value of None will use the pot_dir directory.
+        
+        Raises
+        ------
+        ValueError
+            If filename exists in the tar but is not a file.
+
+        Returns
+        -------
+        io.IOBase
+            A file-like object in binary read mode that allows for the file
+            contents to be read.
+        """
+        # Set default root path
+        if localroot is None:
+            localroot = self.pot_dir
+
+        return super().get_file(filename, localroot)
```

### Comparing `potentials-0.3.6/potentials/record/PotentialLAMMPSKIM.py` & `potentials-0.3.7/potentials/record/PotentialLAMMPSKIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,28 +23,31 @@
     """
     Class for building LAMMPS input lines from a potential-LAMMPS-KIM data model.
     """
     
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  id: Optional[str] = None, 
                  potkey: Optional[str] = None,
                  potid: Optional[str] = None,
                  symbolset: Union[str, list, None] = None):
         """
         Initializes an instance and loads content from a data model.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The record name to use.  If not given, this will be set to the
             potential's id.
+        database : yabadaba.Database, optional
+            Allows for a default database to be associated with the record.
         id : str, optional
             The full KIM model id indicating the version to use.  If not given,
             then the newest known version will be used.
         potkey : str, optional
             Specifies which potential (by potkey value) to use.  Only important
             if the kim model is associated with multiple potential entries.
             This controls which symbols are available.
@@ -56,15 +59,15 @@
             Specifies which potential (by symbols value) to use.  Only important
             if the kim model is associated with multiple potential entries.
             If potkey or potid is not given, then the first potential entry
             found with all listed symbols will be selected.
         """
 
         # Call super with only name
-        super().__init__(model=None, name=name)
+        super().__init__(model=None, name=name, database=database)
 
         # Call load_model if needed
         if model is not None:
             self.load_model(model=model, name=name, id=id, potkey=potkey,
                             potid=potid, symbolset=symbolset)
         
         elif id is not None:
```

### Comparing `potentials-0.3.6/potentials/record/Request.py` & `potentials-0.3.7/potentials/record/Request.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     """
     Class for representing Request records that are associated with user
     requests to the NIST Interatomic Potentials Repository for new potentials.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
@@ -135,15 +136,15 @@
             the elemental system being requested.
         """
         # Set default values
         self.__systems = []
         self.date = datetime.date.today()
         self.comment = None
 
-        super().__init__(model=model, name=name, **kwargs)
+        super().__init__(model=model, name=name, database=database, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'Request'
 
     @property
```

### Comparing `potentials-0.3.6/potentials/record/__init__.py` & `potentials-0.3.7/potentials/record/__init__.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/__init__.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/aslist.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/aslist.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/atomic_info.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/atomic_info.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/atomicdata.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/atomicdata.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/numderivative.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/numderivative.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/parse_authors.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/parse_authors.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/screen_input.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/screen_input.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc` & `potentials-0.3.7/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/atomic_info.py` & `potentials-0.3.7/potentials/tools/atomic_info.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/atomicdata.csv` & `potentials-0.3.7/potentials/tools/atomicdata.csv`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/numderivative.py` & `potentials-0.3.7/potentials/tools/numderivative.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/tools/parse_authors.py` & `potentials-0.3.7/potentials/tools/parse_authors.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/Action.xsd` & `potentials-0.3.7/potentials/xsd/Action.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/Citation.xsd` & `potentials-0.3.7/potentials/xsd/Citation.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/Potential.xsd` & `potentials-0.3.7/potentials/xsd/Potential.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/Request.xsd` & `potentials-0.3.7/potentials/xsd/Request.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/artifact.xsd` & `potentials-0.3.7/potentials/xsd/artifact.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/implementation.xsd` & `potentials-0.3.7/potentials/xsd/implementation.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/link.xsd` & `potentials-0.3.7/potentials/xsd/link.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/parameter.xsd` & `potentials-0.3.7/potentials/xsd/parameter.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/potential_LAMMPS.xsd` & `potentials-0.3.7/potentials/xsd/potential_LAMMPS.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsd/potential_LAMMPS_KIM.xsd` & `potentials-0.3.7/potentials/xsd/potential_LAMMPS_KIM.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/Action.xsl` & `potentials-0.3.7/potentials/xsl/Action.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/Citation.xsl` & `potentials-0.3.7/potentials/xsl/Citation.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/FAQ.xsl` & `potentials-0.3.7/potentials/xsl/FAQ.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/Potential.xsl` & `potentials-0.3.7/potentials/xsl/Potential.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/Request.xsl` & `potentials-0.3.7/potentials/xsl/Request.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/artifact.xsl` & `potentials-0.3.7/potentials/xsl/artifact.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/implementation.xsl` & `potentials-0.3.7/potentials/xsl/implementation.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/link.xsl` & `potentials-0.3.7/potentials/xsl/link.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/parameter.xsl` & `potentials-0.3.7/potentials/xsl/parameter.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/potential_LAMMPS.xsl` & `potentials-0.3.7/potentials/xsl/potential_LAMMPS.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials/xsl/potential_LAMMPS_KIM.xsl` & `potentials-0.3.7/potentials/xsl/potential_LAMMPS_KIM.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.6/potentials.egg-info/PKG-INFO` & `potentials-0.3.7/potentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: potentials
-Version: 0.3.6
+Version: 0.3.7
 Summary: API database tools for accessing the NIST Interatomic Potentials Repository: explore and download interatomic potentials and computed properties.
 Home-page: https://github.com/usnistgov/potentials
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,interatomic potential,force field
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
 
 ==========
 potentials
 ==========
```

### Comparing `potentials-0.3.6/potentials.egg-info/SOURCES.txt` & `potentials-0.3.7/potentials.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 potentials/buildrecord/potential_LAMMPS/EimBuilder.py
 potentials/buildrecord/potential_LAMMPS/KimBuilder.py
 potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py
 potentials/buildrecord/potential_LAMMPS/PairBuilder.py
 potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py
 potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py
 potentials/buildrecord/potential_LAMMPS/__init__.py
+potentials/paramfile/ADP.py
 potentials/paramfile/EAM.py
 potentials/paramfile/EAMAlloy.py
 potentials/paramfile/EAMFS.py
 potentials/paramfile/__init__.py
 potentials/paramfile/converters.py
 potentials/paramfile/load_eam.py
 potentials/record/Action.py
```

### Comparing `potentials-0.3.6/setup.py` & `potentials-0.3.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,18 @@
         'API database tools for accessing the NIST Interatomic Potentials Repository:',
         'explore and download interatomic potentials and computed properties.']),
     long_description = getreadme(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Physics'
     ],
     keywords = [
         'atom',
         'atomic',
         'atomistic',
         'molecular dynamics',
@@ -46,12 +47,12 @@
         'matplotlib',
         'pandas',
         'requests',
         'habanero',
         'bibtexparser',
         'ipywidgets',
         'cdcs',
-        'yabadaba>=0.2.0'
+        'yabadaba>=0.2.1'
     ],
     include_package_data = True,
     zip_safe = False
 )
```

