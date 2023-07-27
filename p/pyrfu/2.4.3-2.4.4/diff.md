# Comparing `tmp/pyrfu-2.4.3.tar.gz` & `tmp/pyrfu-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfu-2.4.3.tar", last modified: Fri Jun 16 10:56:01 2023, max compression
+gzip compressed data, was "pyrfu-2.4.4.tar", last modified: Thu Jul 27 14:08:27 2023, max compression
```

## Comparing `pyrfu-2.4.3.tar` & `pyrfu-2.4.4.tar`

### file list

```diff
@@ -1,348 +1,314 @@
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.228027 pyrfu-2.4.3/
--rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.3/.flake8
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.459838 pyrfu-2.4.3/.github/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.507865 pyrfu-2.4.3/.github/workflows/
--rw-r--r--   0 louisr     (501) staff       (20)      570 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.github/workflows/flake8.yml
--rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 louisr     (501) staff       (20)      588 2023-06-09 14:46:12.000000 pyrfu-2.4.3/.github/workflows/pylint.yml
--rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.3/.gitignore
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.517289 pyrfu-2.4.3/.idea/
--rw-r--r--   0 louisr     (501) staff       (20)      294 2023-06-14 09:44:52.000000 pyrfu-2.4.3/.idea/aws.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.518921 pyrfu-2.4.3/.idea/codeStyles/
--rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.521263 pyrfu-2.4.3/.idea/inspectionProfiles/
--rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/vcs.xml
--rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
--rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-06-09 14:43:25.000000 pyrfu-2.4.3/.pre-commit-config.yaml
--rwxr-xr-x   0 louisr     (501) staff       (20)       83 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.readthedocs.yml
--rw-r--r--   0 louisr     (501) staff       (20)     2972 2023-04-20 14:38:38.000000 pyrfu-2.4.3/CONTRIBUTING.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.3/LICENSE.txt
--rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.3/MANIFEST.in
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-16 10:56:01.227157 pyrfu-2.4.3/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     6490 2023-06-09 10:13:58.000000 pyrfu-2.4.3/README.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.546892 pyrfu-2.4.3/docs/
--rw-r--r--   0 louisr     (501) staff       (20)      640 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/Makefile
--rw-r--r--   0 louisr     (501) staff       (20)      341 2023-04-21 12:45:20.000000 pyrfu-2.4.3/docs/environment.yml
--rw-r--r--   0 louisr     (501) staff       (20)      785 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/make.bat
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.569847 pyrfu-2.4.3/docs/source/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.572840 pyrfu-2.4.3/docs/source/_static/
--rw-r--r--   0 louisr     (501) staff       (20)    18615 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/_static/logo-pyrfu.png
--rw-r--r--   0 louisr     (501) staff       (20)     2011 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/_static/logo-pyrfu.svg
--rw-r--r--   0 louisr     (501) staff       (20)     8992 2023-06-09 14:50:39.000000 pyrfu-2.4.3/docs/source/conf.py
--rw-r--r--   0 louisr     (501) staff       (20)      372 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/contributing.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1091 2023-06-14 09:19:39.000000 pyrfu-2.4.3/docs/source/examples.rst
--rw-r--r--   0 louisr     (501) staff       (20)      192 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/getting_started.rst
--rw-r--r--   0 louisr     (501) staff       (20)      618 2023-04-21 13:33:36.000000 pyrfu-2.4.3/docs/source/index.rst
--rw-r--r--   0 louisr     (501) staff       (20)       72 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/modules.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1283 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/quick-overview.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.468931 pyrfu-2.4.3/examples/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.574300 pyrfu-2.4.3/examples/00_overview/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.586051 pyrfu-2.4.3/examples/00_overview/.ipynb_checkpoints/
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.3/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.3/examples/00_overview/quick-overview.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.662376 pyrfu-2.4.3/examples/01_mms/
--rw-r--r--   0 louisr     (501) staff       (20)   281483 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_b_e_j.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   564517 2023-06-09 09:46:23.000000 pyrfu-2.4.3/examples/01_mms/example_mms_ebfields.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   371521 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_edr_signatures.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   411079 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_eis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   108423 2023-06-08 16:35:41.000000 pyrfu-2.4.3/examples/01_mms/example_mms_electron_psd.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   432503 2023-06-09 14:51:47.000000 pyrfu-2.4.3/examples/01_mms/example_mms_feeps.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   184196 2023-06-08 15:51:52.000000 pyrfu-2.4.3/examples/01_mms/example_mms_hpca.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   279733 2023-06-08 16:35:41.000000 pyrfu-2.4.3/examples/01_mms/example_mms_ohmslaw.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   353737 2023-06-08 16:40:22.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_deflux.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   450116 2023-06-09 09:46:14.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_distributions.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   634316 2023-06-09 09:42:51.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_pad.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   445067 2023-06-08 15:50:47.000000 pyrfu-2.4.3/examples/01_mms/example_mms_polarizationanalysis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   242849 2023-06-09 07:50:56.000000 pyrfu-2.4.3/examples/01_mms/example_mms_reduced_electron_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   424890 2023-06-09 09:16:19.000000 pyrfu-2.4.3/examples/01_mms/example_mms_reduced_ion_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   205591 2023-06-09 11:46:23.000000 pyrfu-2.4.3/examples/01_mms/example_mms_walen_test.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.666315 pyrfu-2.4.3/examples/02_dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)    51819 2023-06-09 11:47:26.000000 pyrfu-2.4.3/examples/02_dispersion/example_dispersion_one_fluid.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)     3072 2023-06-16 10:53:10.000000 pyrfu-2.4.3/pyproject.toml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.668295 pyrfu-2.4.3/pyrfu/
--rw-r--r--   0 louisr     (501) staff       (20)      334 2023-06-16 10:53:10.000000 pyrfu-2.4.3/pyrfu/__init__.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.689255 pyrfu-2.4.3/pyrfu/__pycache__/
--rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.695429 pyrfu-2.4.3/pyrfu/dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)    10001 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/disp_surf_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3487 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/one_fluid_dispersion.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.700442 pyrfu-2.4.3/pyrfu/lp/
--rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/photo_current.py
--rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/thermal_current.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.894309 pyrfu-2.4.3/pyrfu/mms/
--rw-r--r--   0 louisr     (501) staff       (20)     6045 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.3/pyrfu/mms/ancillary.json
--rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/calculate_epsilon.py
--rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     2280 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/copy_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     2195 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/copy_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/correct_edp_probe_timing.py
--rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1093 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     2558 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/def2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1631 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dft_time_shift.py
--rw-r--r--   0 louisr     (501) staff       (20)     5503 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/download_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     7477 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/download_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dpf2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     3166 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dsl2gse.py
--rw-r--r--   0 louisr     (501) staff       (20)     3041 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dsl2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_proton_correction.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     4590 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_skymap_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_spec_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/estimate_phase_speed.py
--rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_active_eyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.3/pyrfu/mms/feeps_bad_data.json
--rw-r--r--   0 louisr     (501) staff       (20)     1697 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_correct_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     3354 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_energy_table.py
--rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_flat_field_corrections.py
--rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pitch_angles.py
--rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_remove_bad_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_remove_sun.py
--rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_sector_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_split_integral_ch.py
--rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/fft_bandpass.py
--rw-r--r--   0 louisr     (501) staff       (20)    11773 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/fk_power_spectrum_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     9081 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     4726 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_eis_allt.py
--rw-r--r--   0 louisr     (501) staff       (20)     4496 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_feeps_alleyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     2525 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6173 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_hpca_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     7052 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_pitch_angle_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)    11195 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_calc_anodes.py
--rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     5663 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1620 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_spin_sum.py
--rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/lh_wave_analysis.py
--rw-r--r--   0 louisr     (501) staff       (20)     6789 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/list_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     4230 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/list_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2770 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/load_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2860 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/load_brst_segments.py
--rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/make_model_kappa.py
--rw-r--r--   0 louisr     (501) staff       (20)     7022 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/make_model_rq.py
--rw-r--r--   0 louisr     (501) staff       (20)     7043 2023-06-16 10:48:31.000000 pyrfu-2.4.3/pyrfu/mms/make_model_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)    25074 2023-05-15 20:42:21.000000 pyrfu-2.4.3/pyrfu/mms/mms_keys.json
--rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/probe_align_times.py
--rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd2def.py
--rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd2dpf.py
--rw-r--r--   0 louisr     (501) staff       (20)    18467 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     3307 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd_rebin.py
--rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/read_feeps_sector_masks_csv.py
--rw-r--r--   0 louisr     (501) staff       (20)     8942 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     5397 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_edist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     2034 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_idist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     3131 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_imoms_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/rotate_tensor.py
--rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/scpot2ne.py
--rw-r--r--   0 louisr     (501) staff       (20)      945 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/spectr_to_dataset.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.939657 pyrfu-2.4.3/pyrfu/mms/sun/
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3854 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/tokenize.py
--rw-r--r--   0 louisr     (501) staff       (20)     3248 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_elim.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)    11440 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     8287 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     2487 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_to_e64.py
--rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/whistler_b2e.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.946049 pyrfu-2.4.3/pyrfu/models/
--rw-r--r--   0 louisr     (501) staff       (20)      347 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     2810 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/igrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/models/igrf13coeffs.csv
--rw-r--r--   0 louisr     (501) staff       (20)     6085 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/magnetopause_normal.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.988558 pyrfu-2.4.3/pyrfu/plot/
--rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/add_position.py
--rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/annotate_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)      935 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/colorbar.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.989836 pyrfu-2.4.3/pyrfu/plot/logo/
--rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
--rw-r--r--   0 louisr     (501) staff       (20)     1108 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/make_labels.py
--rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/mms_pl_config.py
--rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/pl_scatter_matrix.py
--rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/pl_tx.py
--rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_clines.py
--rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1431 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_line.py
--rw-r--r--   0 louisr     (501) staff       (20)     3646 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_reduced_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)    11634 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_sitl_overview.py
--rw-r--r--   0 louisr     (501) staff       (20)     4627 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_spectr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_surf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/span_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/zoom.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.210364 pyrfu-2.4.3/pyrfu/pyrf/
--rw-r--r--   0 louisr     (501) staff       (20)     5552 2023-06-10 21:31:59.000000 pyrfu-2.4.3/pyrfu/pyrf/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1963 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/autocorr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2651 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/average_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1156 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/avg_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_grad.py
--rw-r--r--   0 louisr     (501) staff       (20)     4188 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_j.py
--rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_k.py
--rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2080 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_ag.py
--rw-r--r--   0 louisr     (501) staff       (20)     1422 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_agyro.py
--rw-r--r--   0 louisr     (501) staff       (20)     1850 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_dng.py
--rw-r--r--   0 louisr     (501) staff       (20)      591 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_dt.py
--rw-r--r--   0 louisr     (501) staff       (20)      614 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_fs.py
--rw-r--r--   0 louisr     (501) staff       (20)     1809 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_sqrtq.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cart2sph.py
--rw-r--r--   0 louisr     (501) staff       (20)     1929 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cart2sph_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1570 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cdfepoch2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1746 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/compress_cwt.py
--rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/convert_fac.py
--rw-r--r--   0 louisr     (501) staff       (20)     6502 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/corr_deriv.py
--rw-r--r--   0 louisr     (501) staff       (20)    10401 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cotrans.py
--rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cross.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/date_str.py
--rw-r--r--   0 louisr     (501) staff       (20)      821 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      842 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642ttns.py
--rw-r--r--   0 louisr     (501) staff       (20)      694 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642unix.py
--rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dec_par_perp.py
--rw-r--r--   0 louisr     (501) staff       (20)     2871 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dist_append.py
--rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dot.py
--rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dynamic_press.py
--rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/e_vxb.py
--rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/eb_nrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    36446 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ebsp.py
--rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/edb.py
--rw-r--r--   0 louisr     (501) staff       (20)      593 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/end.py
--rw-r--r--   0 louisr     (501) staff       (20)     3009 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/estimate.py
--rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/extend_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     3736 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/filt.py
--rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/find_closest.py
--rw-r--r--   0 louisr     (501) staff       (20)     3795 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/get_omni_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/gradient.py
--rw-r--r--   0 louisr     (501) staff       (20)      987 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/gse2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     2401 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/histogram.py
--rw-r--r--   0 louisr     (501) staff       (20)     3159 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/histogram2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/increments.py
--rw-r--r--   0 louisr     (501) staff       (20)    18234 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/int_sph_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     2024 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/integrate.py
--rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iplasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)      585 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso2unix.py
--rw-r--r--   0 louisr     (501) staff       (20)      875 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime.py
--rw-r--r--   0 louisr     (501) staff       (20)      626 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012timevec.py
--rw-r--r--   0 louisr     (501) staff       (20)      999 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/l_shell.py
--rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/lowpass.py
--rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/match_phibe_dir.py
--rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/match_phibe_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2153 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean.py
--rw-r--r--   0 louisr     (501) staff       (20)     2391 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean_field.py
--rw-r--r--   0 louisr     (501) staff       (20)     2231 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/medfilt.py
--rw-r--r--   0 louisr     (501) staff       (20)     2362 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/median_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/movmean.py
--rw-r--r--   0 louisr     (501) staff       (20)     4661 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mva.py
--rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/new_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/norm.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/normalize.py
--rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_1d.py
--rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     3593 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pid_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/plasma_beta.py
--rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/plasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/poynting_flux.py
--rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pres_anis.py
--rw-r--r--   0 louisr     (501) staff       (20)     2958 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pvi.py
--rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pvi_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/read_cdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     2017 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/remove_repeated_points.py
--rw-r--r--   0 louisr     (501) staff       (20)     8891 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/resample.py
--rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_models_parameters.json
--rw-r--r--   0 louisr     (501) staff       (20)    15259 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_normal.py
--rw-r--r--   0 louisr     (501) staff       (20)     9264 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_parameters.py
--rw-r--r--   0 louisr     (501) staff       (20)     1651 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/solid_angle.py
--rw-r--r--   0 louisr     (501) staff       (20)      910 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/sph2cart.py
--rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/st_diff.py
--rw-r--r--   0 louisr     (501) staff       (20)      568 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/start.py
--rw-r--r--   0 louisr     (501) staff       (20)     1857 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/struct_func.py
--rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/t_eval.py
--rw-r--r--   0 louisr     (501) staff       (20)     3716 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/time_clip.py
--rw-r--r--   0 louisr     (501) staff       (20)     1163 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/timevec2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)     1501 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/trace.py
--rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/pyrf/transformation_indices.json
--rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_append.py
--rw-r--r--   0 louisr     (501) staff       (20)      956 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_scalar.py
--rw-r--r--   0 louisr     (501) staff       (20)     3043 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_tensor_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      672 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_time.py
--rw-r--r--   0 louisr     (501) staff       (20)     1022 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_vec_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      928 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ttns2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)      718 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/unix2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/vht.py
--rw-r--r--   0 louisr     (501) staff       (20)     1683 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wave_fft.py
--rw-r--r--   0 louisr     (501) staff       (20)     6301 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wavelet.py
--rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wavepolarize_means.py
--rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/waverage.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.218252 pyrfu-2.4.3/pyrfu/solo/
--rw-r--r--   0 louisr     (501) staff       (20)      373 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/solo/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     1109 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     4619 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/read_lfr_density.py
--rw-r--r--   0 louisr     (501) staff       (20)     8224 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/read_tnr.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.221674 pyrfu-2.4.3/pyrfu/tests/
--rw-r--r--   0 louisr     (501) staff       (20)      210 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/tests/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1553 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/tests/test_pyrf.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.688013 pyrfu-2.4.3/pyrfu.egg-info/
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     9550 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/SOURCES.txt
--rw-r--r--   0 louisr     (501) staff       (20)        1 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/dependency_links.txt
--rw-r--r--   0 louisr     (501) staff       (20)      235 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/requires.txt
--rw-r--r--   0 louisr     (501) staff       (20)       30 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/top_level.txt
--rw-r--r--   0 louisr     (501) staff       (20)     2691 2023-06-09 14:45:06.000000 pyrfu-2.4.3/requirements.txt
--rw-r--r--   0 louisr     (501) staff       (20)       38 2023-06-16 10:56:01.228197 pyrfu-2.4.3/setup.cfg
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.479079 pyrfu-2.4.3/venv/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.223550 pyrfu-2.4.3/venv/bin/
--rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.3/venv/bin/activate_this.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.539250 pyrfu-2.4.4/
+-rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.4/.flake8
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.627836 pyrfu-2.4.4/.github/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.667641 pyrfu-2.4.4/.github/workflows/
+-rw-r--r--   0 louisr     (501) staff       (20)      625 2023-07-21 11:39:19.000000 pyrfu-2.4.4/.github/workflows/flake8.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      643 2023-07-21 11:38:43.000000 pyrfu-2.4.4/.github/workflows/pylint.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.4/.gitignore
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.672539 pyrfu-2.4.4/.idea/
+-rw-r--r--   0 louisr     (501) staff       (20)      294 2023-07-27 10:47:39.000000 pyrfu-2.4.4/.idea/aws.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.673963 pyrfu-2.4.4/.idea/codeStyles/
+-rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.676057 pyrfu-2.4.4/.idea/inspectionProfiles/
+-rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/vcs.xml
+-rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
+-rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-07-21 10:56:15.000000 pyrfu-2.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 louisr     (501) staff       (20)     2237 2023-07-21 11:09:58.000000 pyrfu-2.4.4/CONTRIBUTING.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.4/LICENSE.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.4/MANIFEST.in
+-rw-r--r--   0 louisr     (501) staff       (20)     8802 2023-07-27 14:08:27.538152 pyrfu-2.4.4/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)     6429 2023-07-21 11:27:45.000000 pyrfu-2.4.4/README.rst
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.678747 pyrfu-2.4.4/docs/
+-rw-r--r--   0 louisr     (501) staff       (20)      658 2023-07-21 12:01:16.000000 pyrfu-2.4.4/docs/Makefile
+-rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-07-21 11:17:04.000000 pyrfu-2.4.4/docs/conf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3034 2023-07-27 14:06:50.000000 pyrfu-2.4.4/pyproject.toml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.680045 pyrfu-2.4.4/pyrfu/
+-rw-r--r--   0 louisr     (501) staff       (20)      334 2023-07-27 14:06:50.000000 pyrfu-2.4.4/pyrfu/__init__.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.685728 pyrfu-2.4.4/pyrfu/__pycache__/
+-rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.689203 pyrfu-2.4.4/pyrfu/dispersion/
+-rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10001 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/disp_surf_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3487 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/one_fluid_dispersion.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.693595 pyrfu-2.4.4/pyrfu/lp/
+-rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/photo_current.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/thermal_current.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.108832 pyrfu-2.4.4/pyrfu/mms/
+-rw-r--r--   0 louisr     (501) staff       (20)     6045 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.4/pyrfu/mms/ancillary.json
+-rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/calculate_epsilon.py
+-rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2280 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/copy_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2195 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/copy_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/correct_edp_probe_timing.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1093 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2558 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/def2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1631 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dft_time_shift.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5503 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/download_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7477 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/download_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dpf2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3166 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dsl2gse.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3041 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dsl2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_proton_correction.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4590 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_skymap_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_spec_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/estimate_phase_speed.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_active_eyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.4/pyrfu/mms/feeps_bad_data.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1697 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_correct_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3350 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/feeps_energy_table.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_flat_field_corrections.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pitch_angles.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_remove_bad_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_remove_sun.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_sector_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_split_integral_ch.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/fft_bandpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11773 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/fk_power_spectrum_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9972 2023-07-27 14:04:04.000000 pyrfu-2.4.4/pyrfu/mms/get_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4726 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_eis_allt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4496 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_feeps_alleyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2524 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6176 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_hpca_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7054 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_pitch_angle_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11323 2023-07-27 14:04:04.000000 pyrfu-2.4.4/pyrfu/mms/get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_calc_anodes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5663 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1620 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_spin_sum.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/lh_wave_analysis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6789 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/list_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4230 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/list_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2795 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/load_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2860 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/load_brst_segments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/make_model_kappa.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7022 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/make_model_rq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7039 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/make_model_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    25195 2023-07-21 11:00:36.000000 pyrfu-2.4.4/pyrfu/mms/mms_keys.json
+-rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/probe_align_times.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/psd2def.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/psd2dpf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18460 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/psd_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3343 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/psd_rebin.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/read_feeps_sector_masks_csv.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8942 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5397 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_edist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2034 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_idist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3131 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_imoms_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/rotate_tensor.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/scpot2ne.py
+-rw-r--r--   0 louisr     (501) staff       (20)      945 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/spectr_to_dataset.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.161895 pyrfu-2.4.4/pyrfu/mms/sun/
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3866 2023-07-21 11:03:34.000000 pyrfu-2.4.4/pyrfu/mms/tokenize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3248 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_elim.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11440 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8287 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2487 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_to_e64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/whistler_b2e.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.167242 pyrfu-2.4.4/pyrfu/models/
+-rw-r--r--   0 louisr     (501) staff       (20)      347 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/models/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2810 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/models/igrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/models/igrf13coeffs.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     6038 2023-07-21 11:40:35.000000 pyrfu-2.4.4/pyrfu/models/magnetopause_normal.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.191429 pyrfu-2.4.4/pyrfu/plot/
+-rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/add_position.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/annotate_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)      935 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/colorbar.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.192622 pyrfu-2.4.4/pyrfu/plot/logo/
+-rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
+-rw-r--r--   0 louisr     (501) staff       (20)     1108 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/make_labels.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/mms_pl_config.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/pl_scatter_matrix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/pl_tx.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_clines.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1431 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_line.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3646 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_reduced_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11753 2023-07-21 11:05:55.000000 pyrfu-2.4.4/pyrfu/plot/plot_sitl_overview.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4627 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_spectr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_surf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/span_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/zoom.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.523202 pyrfu-2.4.4/pyrfu/pyrf/
+-rw-r--r--   0 louisr     (501) staff       (20)     5552 2023-07-27 14:06:41.000000 pyrfu-2.4.4/pyrfu/pyrf/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2078 2023-07-21 22:14:58.000000 pyrfu-2.4.4/pyrfu/pyrf/autocorr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2651 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/average_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1489 2023-07-22 21:41:45.000000 pyrfu-2.4.4/pyrfu/pyrf/avg_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_grad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4196 2023-07-21 10:45:02.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_j.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_k.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2510 2023-07-21 20:18:55.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_ag.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1842 2023-07-21 20:22:06.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_agyro.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2270 2023-07-21 20:51:36.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_dng.py
+-rw-r--r--   0 louisr     (501) staff       (20)      738 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_dt.py
+-rw-r--r--   0 louisr     (501) staff       (20)      761 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_fs.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2233 2023-07-21 21:02:32.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_sqrtq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-07-27 14:06:45.000000 pyrfu-2.4.4/pyrfu/pyrf/cart2sph.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1929 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/cart2sph_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1723 2023-07-21 20:27:19.000000 pyrfu-2.4.4/pyrfu/pyrf/cdfepoch2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1746 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/compress_cwt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/convert_fac.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6502 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/corr_deriv.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10371 2023-07-21 21:07:03.000000 pyrfu-2.4.4/pyrfu/pyrf/cotrans.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/cross.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/date_str.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1118 2023-07-21 21:18:32.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      842 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642ttns.py
+-rw-r--r--   0 louisr     (501) staff       (20)      694 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dec_par_perp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2394 2023-07-27 14:03:26.000000 pyrfu-2.4.4/pyrfu/pyrf/dist_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dot.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dynamic_press.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/e_vxb.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/eb_nrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    36446 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ebsp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/edb.py
+-rw-r--r--   0 louisr     (501) staff       (20)      593 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/end.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3009 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/estimate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/extend_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3736 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/filt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/find_closest.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3795 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/get_omni_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/gradient.py
+-rw-r--r--   0 louisr     (501) staff       (20)      987 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/gse2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2401 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/histogram.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3155 2023-07-21 10:34:50.000000 pyrfu-2.4.4/pyrfu/pyrf/histogram2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/increments.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18234 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/int_sph_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2024 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/integrate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iplasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)      585 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso2unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)      875 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime.py
+-rw-r--r--   0 louisr     (501) staff       (20)      626 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1061 2023-07-21 12:04:40.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012timevec.py
+-rw-r--r--   0 louisr     (501) staff       (20)      999 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/l_shell.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/lowpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/match_phibe_dir.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/match_phibe_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2153 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2387 2023-07-21 10:33:13.000000 pyrfu-2.4.4/pyrfu/pyrf/mean_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mean_field.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2231 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/medfilt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2358 2023-07-21 10:33:35.000000 pyrfu-2.4.4/pyrfu/pyrf/median_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/movmean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4661 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mva.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8345 2023-07-21 11:08:11.000000 pyrfu-2.4.4/pyrfu/pyrf/mva_gui.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/new_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/norm.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/normalize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-07-21 10:34:07.000000 pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_1d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3593 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pid_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/plasma_beta.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/plasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/poynting_flux.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pres_anis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2958 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pvi.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pvi_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/read_cdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2017 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/remove_repeated_points.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8816 2023-07-21 12:05:30.000000 pyrfu-2.4.4/pyrfu/pyrf/resample.py
+-rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_models_parameters.json
+-rw-r--r--   0 louisr     (501) staff       (20)    15200 2023-07-21 12:11:34.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_normal.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9264 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_parameters.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1651 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/solid_angle.py
+-rw-r--r--   0 louisr     (501) staff       (20)      910 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/sph2cart.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/st_diff.py
+-rw-r--r--   0 louisr     (501) staff       (20)      794 2023-07-22 21:11:20.000000 pyrfu-2.4.4/pyrfu/pyrf/start.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1857 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/struct_func.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/t_eval.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3716 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/time_clip.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1163 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/timevec2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10280 2023-06-20 16:59:32.000000 pyrfu-2.4.4/pyrfu/pyrf/timing_gui.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1625 2023-07-22 21:23:02.000000 pyrfu-2.4.4/pyrfu/pyrf/trace.py
+-rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/pyrf/transformation_indices.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1224 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_scalar.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3943 2023-07-22 20:48:02.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1320 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_tensor_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      672 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_time.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1279 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_vec_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      928 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ttns2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)      718 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/unix2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/vht.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1683 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wave_fft.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6301 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wavelet.py
+-rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wavepolarize_means.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/waverage.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.531292 pyrfu-2.4.4/pyrfu/solo/
+-rw-r--r--   0 louisr     (501) staff       (20)      373 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/solo/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1109 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4619 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/read_lfr_density.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8224 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/read_tnr.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.534360 pyrfu-2.4.4/pyrfu/tests/
+-rw-r--r--   0 louisr     (501) staff       (20)      210 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/tests/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)    21319 2023-07-22 21:43:35.000000 pyrfu-2.4.4/pyrfu/tests/test_pyrf.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.684740 pyrfu-2.4.4/pyrfu.egg-info/
+-rw-r--r--   0 louisr     (501) staff       (20)     8802 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)     8434 2023-07-27 14:08:26.000000 pyrfu-2.4.4/pyrfu.egg-info/SOURCES.txt
+-rw-r--r--   0 louisr     (501) staff       (20)        1 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/dependency_links.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      193 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/requires.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       27 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/top_level.txt
+-rw-r--r--   0 louisr     (501) staff       (20)     1557 2023-07-21 11:26:29.000000 pyrfu-2.4.4/requirements.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       38 2023-07-27 14:08:27.539491 pyrfu-2.4.4/setup.cfg
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.634536 pyrfu-2.4.4/venv/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.536132 pyrfu-2.4.4/venv/bin/
+-rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.4/venv/bin/activate_this.py
```

### Comparing `pyrfu-2.4.3/.github/workflows/flake8.yml` & `pyrfu-2.4.4/.github/workflows/flake8.yml`

 * *Files 27% similar despite different names*

```diff
@@ -13,12 +13,13 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        python -m pip install -r docs/requirements.txt
         python -m pip install -r requirements.txt
         pip install flake8
     - name: check_flake8
       run: |
         flake8 $(git ls-files '*.py')
```

### Comparing `pyrfu-2.4.3/.github/workflows/publish-to-pypi.yml` & `pyrfu-2.4.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/.github/workflows/pylint.yml` & `pyrfu-2.4.4/.github/workflows/pylint.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,12 +13,13 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        python -m pip install -r docs/requirements.txt
         python -m pip install -r requirements.txt
         pip install pylint
     - name: pylint
       run: |
         pylint --rcfile=pyproject.toml $(git ls-files '*.py')
```

### Comparing `pyrfu-2.4.3/.idea/inspectionProfiles/Project_Default.xml` & `pyrfu-2.4.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml` & `pyrfu-2.4.4/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/.pre-commit-config.yaml` & `pyrfu-2.4.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
   - repo: https://github.com/ambv/black
-    rev: "23.3.0"
+    rev: "23.7.0"
     hooks:
       - id: black
         language_version: python3.9
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.7.0
     hooks:
       - id: nbqa-black
```

### Comparing `pyrfu-2.4.3/CONTRIBUTING.rst` & `pyrfu-2.4.4/CONTRIBUTING.rst`

 * *Files 19% similar despite different names*

```diff
@@ -19,36 +19,16 @@
 --------------
 Prefer if possible Python>=3.8 since there are major dependencies that do not support
 older python versions.
 
 
 Coding style
 ------------
-Stick as much as possible to
-`PEP8 <https://www.python.org/dev/peps/pep-0008/>`__ for general
-guidelines in term of coding conventions and to
-`PEP257 <https://www.python.org/dev/peps/pep-0257/>`__ for typical
-docstring conventions. You can also have a look to `Python
-anti-pattern <https://docs.quantifiedcode.com/python-anti-patterns/>`__.
-
-Main guidelines from PEP8
--------------------------
-PEP8 coding conventions are:
-
--  Use 4 spaces per indentation level.
--  Limit all lines to a maximum of 100 characters.
--  Separate top-level function and class definitions with two blank
-   lines.
--  Make sure that all variables are used.
--  Imports should be grouped in the following order:
-
-    -  Standard library imports.
-    -  Related third party imports.
-    -  Local application/library specific imports.
-    -  A blank line between each group of imports.
+The pyrfu package uses the `Black code style <https://black.readthedocs
+.io/en/stable/the_black_code_style/current_style.html>`__ .
 
 Use Linters
 ------------
 Linters are tools for static code quality checker. For instance, you can
 use the following tools to test conformity with the common pythonic
 standards:
 
@@ -61,15 +41,15 @@
 All these linters can be simply installed with pip. Further details
 on the functionnalities can be found
 `here <http://books.agiliq.com/projects/essential-python-tools/en/latest/linters.html>`__
 or `there <https://realpython.com/python-code-quality/>`__.
 Also, a lot of features can also be provided natively or by installing
 plugins with your IDE (PyCharm, Spyder, Eclipse, etc.).
 
-To be accepted to ``pyrfu`` every new code as to get a pylint score higher than 9/10.
+To be accepted to ``pyrfu`` every new code as to get a pylint score of 10/10.
 
 Documentation
 -------------
 Documentation of all the files must be done in-line using Sphinx_.
 The doxtring as to follow the numpydoc_ style
 
 .. _Sphinx: http://www.sphinx-doc.org/en/master/
```

### Comparing `pyrfu-2.4.3/LICENSE.txt` & `pyrfu-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/PKG-INFO` & `pyrfu-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -211,15 +211,14 @@
 - `matplotlib <https://matplotlib.org>`_ >=3.5.2
 - `numba <http://numba.pydata.org>`_ >=0.54.1
 - `numpy <https://www.numpy.org>`_ >=1.20.3
 - `pandas <https://pandas.pydata.org/>`_ >=1.3.4
 - `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
 - `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
 - `scipy <https://scipy.org>`_ >=1.7.3
-- `Sphinx <https://www.sphinx-doc.org/en/master/>`_ >=4.3.0
 - `tqdm <https://tqdm.github.io/>`_ >=4.62.3
 - `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
 
 
 Testing dependencies are:
 
 - `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
```

### Comparing `pyrfu-2.4.3/README.rst` & `pyrfu-2.4.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,14 @@
 - `matplotlib <https://matplotlib.org>`_ >=3.5.2
 - `numba <http://numba.pydata.org>`_ >=0.54.1
 - `numpy <https://www.numpy.org>`_ >=1.20.3
 - `pandas <https://pandas.pydata.org/>`_ >=1.3.4
 - `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
 - `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
 - `scipy <https://scipy.org>`_ >=1.7.3
-- `Sphinx <https://www.sphinx-doc.org/en/master/>`_ >=4.3.0
 - `tqdm <https://tqdm.github.io/>`_ >=4.62.3
 - `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
 
 
 Testing dependencies are:
 
 - `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
```

### Comparing `pyrfu-2.4.3/docs/Makefile` & `pyrfu-2.4.4/docs/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    =
-SPHINXBUILD   = sphinx-build
-SOURCEDIR     = source
+SPHINXBUILD   = python -m sphinx
+SPHINXPROJ    = pyrfu
+SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(ALLSPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `pyrfu-2.4.3/docs/source/conf.py` & `pyrfu-2.4.4/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,86 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
 # Built-in imports
 import os
-import shutil
 import sys
 
 # 3rd party imports
 import pydata_sphinx_theme
 
 # -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, "/Users/louisr/Documents/PhD/irfu-python/pyrfu")
-
-examples_source = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), "..", "..", "examples"),
-)
-examples_dest = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), "examples"),
-)
-
-"""
-def setup(app):
-    sphinxcontrib.apidoc.setup(
-        [
-            "-f",  # Overwrite existing files
-            "-T",  # Create table of contents
-            "-e",  # Give modules their own pages
-            "-o",  # Output the files to:
-            "./_autogen/",  # Output Directory
-            "./../../pyrfu",  # Main Module directory
-        ],
-    )
-
-
-if os.path.exists(examples_dest):
-    shutil.rmtree(examples_dest)
-os.mkdir(examples_dest)
-
-for root, dirs, files in os.walk(examples_source):
-    for dr in dirs:
-        os.mkdir(
-            os.path.join(root.replace(examples_source, examples_dest), dr),
-        )
-    for fil in files:
-        if os.path.splitext(fil)[1] in [".ipynb", ".md", ".rst"]:
-            source_filename = os.path.join(root, fil)
-            dest_filename = source_filename.replace(
-                examples_source,
-                examples_dest,
-            )
-            shutil.copyfile(source_filename, dest_filename)
-
-"""
-
-
-if os.path.exists(examples_dest):
-    shutil.rmtree(examples_dest)
-os.mkdir(examples_dest)
-
-for root, dirs, files in os.walk(examples_source):
-    for dr in dirs:
-        os.mkdir(os.path.join(root.replace(examples_source, examples_dest), dr))
-    for fil in files:
-        if os.path.splitext(fil)[1] in [".ipynb", ".md", ".rst"]:
-            source_filename = os.path.join(root, fil)
-            dest_filename = source_filename.replace(examples_source, examples_dest)
-            shutil.copyfile(source_filename, dest_filename)
-
-
-sys.path.insert(0, os.path.abspath("../.."))
-
-# -- Project information -----------------------------------------------------
-
-project = "pyrfu"
-author = "Louis Richard"
-# copyright = f"2019–{datetime.utcnow().year}, {author}"
-
+src_path = os.path.abspath("..")
+sys.path.insert(0, src_path)
+os.environ["PYTHONPATH"] = src_path
 
 # -- General configuration ---------------------------------------------------
+autosummary_generate = True
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
 # ones.
 
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinx.ext.autosectionlabel",
+    "sphinx.ext.autosummary",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.coverage",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
+    "sphinx_gallery.load_style",
+    "sphinx_codeautolink",
     "sphinxcontrib.apidoc",
     "sphinx.ext.todo",
     "nbsphinx",
-    #  "sphinx_gallery.gen_gallery"
+    "sphinx_copybutton",
+    "numpydoc",
 ]
 
 
+apidoc_module_dir = "../pyrfu"
+apidoc_output_dir = "dev"
+apidoc_excluded_paths = ["tests", "*/tests/", "*/*/tests/", "*/*/*/tests"]
+apidoc_separate_modules = True
+apidoc_module_first = True
+
+# autosectionlabel_prefix_document = True
+codeautolink_custom_blocks = {
+    "python3": None,
+    "pycon3": "sphinx_codeautolink.clean_pycon",
+}
+
+nbsphinx_execute_arguments = [
+    "--InlineBackend.figure_formats={'svg', 'pdf'}",
+    "--InlineBackend.rc=figure.dpi=96",
+]
+
+nbsphinx_execute = "never"
+
+nbsphinx_thumbnails = {}
+
+mathjax3_config = {
+    "tex": {"tags": "ams", "useLabelIds": True},
+}
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
-source_suffix = [".rst", ".md"]
+source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
+# General information about the project.
+project = "pyrfu"
+author = "Louis Richard"
+
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
 
@@ -133,36 +91,32 @@
     "_build",
     "Thumbs.db",
     ".DS_Store",
     "**.ipynb_checkpoints",
     "examples/**/README.md",
 ]
 
-autodoc_mock_imports = ["numba", "sfs"]
+numpydoc_show_class_members = False
 
-# -- Options for HTML output -------------------------------------------------
+# The name of the Pygments (syntax highlighting) style to use.
+# pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = True
+
+# -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-# html_theme = "alabaster"
+# html_theme = 'sphinx_rtd_theme'
 html_theme = pydata_sphinx_theme.__name__
-# html_theme = "sphinx_rtd_theme"
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-
 
-# Add any paths that contain custom themes here, relative to this directory.
-# html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
@@ -183,85 +137,82 @@
 #
 html_logo = "_static/logo-pyrfu.png"
 
 # The name of an image file (relative to this directory) to use as a favicon of
 # the docs.  This file should be a Windows icon file (.ico) being 16x16 or
 # 32x32 pixels large.
 
-
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "pyrfudoc"
 
 
-# -- Options for LaTeX output ------------------------------------------------
+# -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
-    # The paper size ("letterpaper" or "a4paper").
+    # The paper size ('letterpaper' or 'a4paper').
     #
-    # "papersize": "letterpaper",
-    # The font size ("10pt", "11pt" or "12pt").
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
     #
-    # "pointsize": "10pt",
+    # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
     #
-    # "preamble": "",
+    # 'preamble': '',
     # Latex figure (float) alignment
     #
-    # "figure_align": "htbp",
+    # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         master_doc,
         "pyrfu.tex",
-        "pyrfu Documentation",
+        "Python Space Physics (RymdFysik) Utilities Documentation",
         "Louis Richard",
         "manual",
     ),
 ]
 
-
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "pyrfu", "pyrfu Documentation", [author], 1)]
-
+man_pages = [
+    (
+        master_doc,
+        "pyrfu",
+        "Python Space Physics (RymdFysik) Utilities Documentation",
+        [author],
+        1,
+    )
+]
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
         "pyrfu",
-        "pyrfu Documentation",
+        "Python Space Physics (RymdFysik) Utilities Documentation",
         author,
         "pyrfu",
-        "One line description of project.",
+        "Python routines to work with space data, particularly with MMS data. "
+        "Also some general plasma routines.",
         "Miscellaneous",
     ),
 ]
 
-
-# -- Extension configuration -------------------------------------------------
-
-# -- Options for todo extension ----------------------------------------------
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = True
-
-
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
 epub_title = project
 
 # The unique identifier of the text. This can be a ISBN number
 # or the project homepage.
@@ -272,21 +223,18 @@
 #
 # epub_uid = ""
 
 # A list of files that should not be packed into the epub file.
 epub_exclude_files = ["search.html"]
 
 
-# -- Extension configuration -------------------------------------------------
-
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "xarray": ("http://xarray.pydata.org/en/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/", None),
+    "matplotlib": ("https://matplotlib.org/stable/", None),
 }
 
-apidoc_module_dir = "../../pyrfu"
-apidoc_output_dir = "_generated"
-apidoc_excluded_paths = ["tests", "*/tests/", "*/*/tests/", "*/*/*/tests"]
-apidoc_separate_modules = True
+autodoc_mock_imports = ["numba", "sfs"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfu-2.4.3/pyproject.toml` & `pyrfu-2.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel==0.38.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfu"
-version = "2.4.3"
+version = "2.4.4"
 description = "Python Space Physics (RymdFysik) Utilities"
 readme = "README.rst"
 authors = [{ name = "Louis RICHARD", email = "louir@irfu.se" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Other Environment",
@@ -36,19 +36,17 @@
 dependencies = [
     "cdflib>=1.0.4",
     "geopack>=1.0.9",
     "matplotlib>=3.5.2",
     "numba>=0.54.1",
     "numpy>=1.20.3",
     "pandas>=1.3.4",
-    "pydata-sphinx-theme>=0.13.0",
     "python-dateutil>=2.8.2",
     "requests>=2.26.0",
     "scipy>=1.7.3",
-    "Sphinx>=4.3.0",
     "tqdm>=4.62.3",
     "xarray>=0.20.1",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "pip-tools"]
@@ -107,20 +105,21 @@
 """
 ignore = """
     ancillary.json,
     config.json,
     feeps_bad_data.json,
     igrf13coeffs.csv,
     mms_keys.json,
-    transformation_indices.json
+    transformation_indices.json,
+    test_pyrf.py
 """
 ignored-modules = "scipy,cdflib"
 
 [tool.bumpver]
-current_version = "2.4.3"
+current_version = "2.4.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyrfu-2.4.3/pyrfu/__pycache__/__init__.cpython-38.pyc` & `pyrfu-2.4.4/pyrfu/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/dispersion/disp_surf_calc.py` & `pyrfu-2.4.4/pyrfu/dispersion/disp_surf_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/dispersion/one_fluid_dispersion.py` & `pyrfu-2.4.4/pyrfu/dispersion/one_fluid_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/lp/__init__.py` & `pyrfu-2.4.4/pyrfu/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/lp/photo_current.py` & `pyrfu-2.4.4/pyrfu/lp/photo_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/lp/thermal_current.py` & `pyrfu-2.4.4/pyrfu/lp/thermal_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/__init__.py` & `pyrfu-2.4.4/pyrfu/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/ancillary.json` & `pyrfu-2.4.4/pyrfu/mms/ancillary.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/calculate_epsilon.py` & `pyrfu-2.4.4/pyrfu/mms/calculate_epsilon.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/copy_files.py` & `pyrfu-2.4.4/pyrfu/mms/copy_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/copy_files_ancillary.py` & `pyrfu-2.4.4/pyrfu/mms/copy_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/correct_edp_probe_timing.py` & `pyrfu-2.4.4/pyrfu/mms/correct_edp_probe_timing.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/db_get_ts.py` & `pyrfu-2.4.4/pyrfu/mms/db_get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/db_get_variable.py` & `pyrfu-2.4.4/pyrfu/mms/db_get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/db_init.py` & `pyrfu-2.4.4/pyrfu/mms/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/def2psd.py` & `pyrfu-2.4.4/pyrfu/mms/def2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/dft_time_shift.py` & `pyrfu-2.4.4/pyrfu/mms/dft_time_shift.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/download_ancillary.py` & `pyrfu-2.4.4/pyrfu/mms/download_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/download_data.py` & `pyrfu-2.4.4/pyrfu/mms/download_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/dpf2psd.py` & `pyrfu-2.4.4/pyrfu/mms/dpf2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/dsl2gse.py` & `pyrfu-2.4.4/pyrfu/mms/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/dsl2gsm.py` & `pyrfu-2.4.4/pyrfu/mms/dsl2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_ang_ang.py` & `pyrfu-2.4.4/pyrfu/mms/eis_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_pad.py` & `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_skymap.py` & `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_spec.py` & `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_moments.py` & `pyrfu-2.4.4/pyrfu/mms/eis_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_omni.py` & `pyrfu-2.4.4/pyrfu/mms/eis_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_pad.py` & `pyrfu-2.4.4/pyrfu/mms/eis_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_pad_combine_sc.py` & `pyrfu-2.4.4/pyrfu/mms/eis_pad_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_pad_spinavg.py` & `pyrfu-2.4.4/pyrfu/mms/eis_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_proton_correction.py` & `pyrfu-2.4.4/pyrfu/mms/eis_proton_correction.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_skymap.py` & `pyrfu-2.4.4/pyrfu/mms/eis_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_skymap_combine_sc.py` & `pyrfu-2.4.4/pyrfu/mms/eis_skymap_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_spec_combine_sc.py` & `pyrfu-2.4.4/pyrfu/mms/eis_spec_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/eis_spin_avg.py` & `pyrfu-2.4.4/pyrfu/mms/eis_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/estimate_phase_speed.py` & `pyrfu-2.4.4/pyrfu/mms/estimate_phase_speed.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_active_eyes.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_active_eyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_bad_data.json` & `pyrfu-2.4.4/pyrfu/mms/feeps_bad_data.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_correct_energies.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_correct_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_energy_table.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_energy_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,16 @@
     Returns
     -------
     out : list
         Energy table.
 
     Notes
     -----
-    Bad eyes are replaced by NaNs.
-    Different original energy tables are used depending on if the sensor head
-    is 6-8 (ions) or not (electrons) :
+    Bad eyes are replaced by NaNs. Different original energy tables are used
+    depending on if the sensor head is 6-8 (ions) or not (electrons) :
         * Electron Eyes: 1, 2, 3, 4, 5, 9, 10, 11, 12
         * Ion Eyes: 6, 7, 8
 
     """
 
     if 6 <= sensor_id <= 8:
         mms_energies = [
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_flat_field_corrections.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_flat_field_corrections.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_omni.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_pad.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_pad_spinavg.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_pitch_angles.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_pitch_angles.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_remove_bad_data.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_remove_bad_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_remove_sun.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_remove_sun.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_sector_spec.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_sector_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_spin_avg.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/feeps_split_integral_ch.py` & `pyrfu-2.4.4/pyrfu/mms/feeps_split_integral_ch.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/fft_bandpass.py` & `pyrfu-2.4.4/pyrfu/mms/fft_bandpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/fk_power_spectrum_4sc.py` & `pyrfu-2.4.4/pyrfu/mms/fk_power_spectrum_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_data.py` & `pyrfu-2.4.4/pyrfu/mms/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     Index of MMS spacecraft
 
     >>> ic = 1
 
     Load magnetic field from FGM
 
-    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint_brst, ic)
+    >>> b_xyz = mms.get_data("b_gse_fgm_brst_l2", tint_brst, ic)
 
     """
 
     mms_id = str(mms_id)
 
     var, cdf_name = _var_and_cdf_name(var_str, mms_id)
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_dist.py` & `pyrfu-2.4.4/pyrfu/mms/get_dist.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,25 +114,25 @@
 
         except TypeError:
             pass
 
     return out
 
 
-def get_dist(file_path, cdf_name, tint):
+def get_dist(file_path, cdf_name, tint: list = None):
     r"""Read field named cdf_name in file and convert to velocity distribution
     function.
 
     Parameters
     ----------
     file_path : str
         Path of the cdf file.
     cdf_name : str
         Name of the target variable in the cdf file.
-    tint : list of str
+    tint : list of str, Optional
         Time interval.
 
     Returns
     -------
     out : xarray.Dataset
         Time series of the velocity distribution function if the target
         specie in the selected time interval.
@@ -146,16 +146,34 @@
     elif "_des_" in cdf_name:
         specie = "electrons"
     else:
         raise AttributeError(
             "Couldn't get the particle species from file name!!",
         )
 
-    tint_org = tint
-    tint = extend_tint(tint, [-1, 1])
+    # Check time interval type
+    # Check time interval
+    if tint is None:
+        tint = ["1995-10-06T18:50:00.000000000", "2200-10-06T18:50:00.000000000"]
+    elif isinstance(tint, (np.ndarray, list)):
+        if isinstance(tint[0], np.datetime64):
+            tint = datetime642iso8601(np.array(tint))
+        elif isinstance(tint[0], str):
+            tint = iso86012datetime64(
+                np.array(tint),
+            )  # to make sure it is ISO8601 ok!!
+            tint = datetime642iso8601(np.array(tint))
+        else:
+            raise TypeError("Values must be in datetime64, or str!!")
+    else:
+        raise TypeError("tint must be array_like!!")
+
+    # Extend time interval by 1s and convert time interval to epochs
+    tint_org = tint.copy()
+    tint = extend_tint(tint, [-1.0, 1.0])
     tint = list(datetime642iso8601(iso86012datetime64(np.array(tint))))
     tint = np.stack(list(map(cdfepoch.parse, tint)))
 
     with CDF(file_path) as file:
         # Get the relevant CDF file information (zVariables)
         cdf_infos = file.cdf_info()
         z_vars = cdf_infos.zVariables
@@ -236,15 +254,16 @@
                     energy1 = energy[0, :]
             else:
                 energy0 = file.varget(en0_name)
                 energy1 = file.varget(en1_name)
 
             # Overwrite energy to make sure that energy0 and energy1
             # are used instead
-            energy = None
+            energy = np.tile(energy0, (len(step_table), 1))
+            energy[step_table == 1] = np.tile(energy1, (int(np.sum(step_table)), 1))
 
         elif tmmode == "fast":
             if energy.ndim == 1:
                 energy0 = energy
                 energy1 = energy
             elif energy.shape[0] == 1:
                 energy0 = energy[0, :]
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_eis_allt.py` & `pyrfu-2.4.4/pyrfu/mms/get_eis_allt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_feeps_alleyes.py` & `pyrfu-2.4.4/pyrfu/mms/get_feeps_alleyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_feeps_omni.py` & `pyrfu-2.4.4/pyrfu/mms/get_feeps_omni.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Set to True to follow the loading. Default is True.
     data_path : str, Optional
         Path of MMS data. Default uses `pyrfu.mms.mms_config.py`
     spin_avg : bool, Optional
         Spin average the omni-directional flux. Default is False.
 
     Returns
-    --------
+    -------
     flux_omni : xarray.DataArray
         Energy spectrum of the target data unit for the target specie in omni
         direction.
 
     See Also
     --------
     pyrfu.mms.get_feeps_alleyes, pyrfu.mms.feeps_remove_bad_data,
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_hpca_dist.py` & `pyrfu-2.4.4/pyrfu/mms/get_hpca_dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,28 +90,29 @@
     return out_dphi
 
 
 def get_hpca_dist(inp, azimuth):
     r"""Returns pseudo-3D particle data structures containing mms hpca data
     for use with spd_slice2d.
 
-    Paramters
-    ---------
+    Parameters
+    ----------
     inp : xarray.DataArray
         HPCA ion spec
     azimuth : xarray.DataArray
         Azimuthal angles.
 
     Returns
     -------
     out : dict
         HPCA distribution
 
 
     """
+
     # check if the time series is monotonic to avoid doing incorrect
     # calculations when there's a problem with the CDF files
     time_data = azimuth.time.data
 
     n_mono = np.where(time_data[1:] <= time_data[:-1])
     assert len(n_mono[0]) == 0, "non-monotonic data found in the Epoch_Angles"
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_pitch_angle_dist.py` & `pyrfu-2.4.4/pyrfu/mms/get_pitch_angle_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         Time interval for closeup.
 
     Returns
     -------
     pad : xarray.DataArray
         Particle pitch angle distribution
 
-    Other Paramters
-    ---------------
+    Other Parameters
+    ----------------
     angles : int or float or list of ndarray
         User defined angles.
     meanorsum : {'mean', 'sum', 'sum_weighted'}
         Method.
 
     Examples
     --------
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_ts.py` & `pyrfu-2.4.4/pyrfu/mms/get_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,36 +170,38 @@
                     pass
 
         out["attrs"] = _get_depend_attributes(file, depend_key)
 
     return out
 
 
-def get_ts(file_path, cdf_name, tint):
+def get_ts(file_path, cdf_name, tint: list = None):
     r"""Reads field named cdf_name in file and convert to time series.
 
     Parameters
     ----------
     file_path : str
         Path of the cdf file.
     cdf_name : str
         Name of the target variable in the cdf file.
-    tint : list of str
+    tint : list of str, Optional
         Time interval.
 
     Returns
     -------
     out : xarray.DataArray
         Time series of the target variable in the selected time interval.
 
     """
 
     # Check time interval type
     # Check time interval
-    if isinstance(tint, (np.ndarray, list)):
+    if tint is None:
+        tint = ["1995-10-06T18:50:00.000000000", "2200-10-06T18:50:00.000000000"]
+    elif isinstance(tint, (np.ndarray, list)):
         if isinstance(tint[0], np.datetime64):
             tint = datetime642iso8601(np.array(tint))
         elif isinstance(tint[0], str):
             tint = iso86012datetime64(
                 np.array(tint),
             )  # to make sure it is ISO8601 ok!!
             tint = datetime642iso8601(np.array(tint))
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/get_variable.py` & `pyrfu-2.4.4/pyrfu/mms/get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/hpca_calc_anodes.py` & `pyrfu-2.4.4/pyrfu/mms/hpca_calc_anodes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/hpca_energies.py` & `pyrfu-2.4.4/pyrfu/mms/hpca_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/hpca_pad.py` & `pyrfu-2.4.4/pyrfu/mms/hpca_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/hpca_spin_sum.py` & `pyrfu-2.4.4/pyrfu/mms/hpca_spin_sum.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/lh_wave_analysis.py` & `pyrfu-2.4.4/pyrfu/mms/lh_wave_analysis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/list_files.py` & `pyrfu-2.4.4/pyrfu/mms/list_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/list_files_ancillary.py` & `pyrfu-2.4.4/pyrfu/mms/list_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/load_ancillary.py` & `pyrfu-2.4.4/pyrfu/mms/load_ancillary.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,12 +100,12 @@
         rows.columns = anc_dict[product]["columns_names"]
 
         data_frame_dict[i] = rows[:][start_idx:end_idx]
 
     data_frame = data_frame_dict[0]
 
     for k in list(data_frame_dict.keys())[1:]:
-        data_frame = data_frame.append(data_frame_dict[k])
+        data_frame = pd.concat([data_frame, data_frame_dict[k]], ignore_index=True)
 
     data_frame = data_frame.sort_values(by="time").set_index(["time"])
 
     return data_frame.to_xarray()
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/load_brst_segments.py` & `pyrfu-2.4.4/pyrfu/mms/load_brst_segments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/make_model_kappa.py` & `pyrfu-2.4.4/pyrfu/mms/make_model_kappa.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/make_model_rq.py` & `pyrfu-2.4.4/pyrfu/mms/make_model_rq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/make_model_vdf.py` & `pyrfu-2.4.4/pyrfu/mms/make_model_vdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,15 @@
     Returns
     -------
     model_vdf : xarray.Dataset
         Distribution function in the same format as vdf.
 
     See also
     --------
-    pyrfu.mms.calculate_epsilon : Calculates epsilon parameter using model
-    distribution.
+    pyrfu.mms.calculate_epsilon : Calculates epsilon parameter using model distribution.
 
     Examples
     --------
     >>> from pyrfu.mms import get_data, make_model_vdf
 
     Define time interval
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/mms_keys.json` & `pyrfu-2.4.4/pyrfu/mms/mms_keys.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'edp'": "{'hmfe_dsl_edp_brst_l2': OrderedDict([('dtype', 'hmfe'), ('cdf_name', "*

 * *          "'edp_hmfe_dsl_brst_l2')])}"}*

```diff
@@ -112,14 +112,18 @@
             "cdf_name": "edp_dce_fast_l2a",
             "dtype": "dce2d"
         },
         "e_ssc_edp_slow_l2a": {
             "cdf_name": "edp_dce_slow_l2a",
             "dtype": "dce2d"
         },
+        "hmfe_dsl_edp_brst_l2": {
+            "cdf_name": "edp_hmfe_dsl_brst_l2",
+            "dtype": "hmfe"
+        },
         "phase_edp_fast_l2a": {
             "cdf_name": "edp_phase_fast_l2a",
             "dtype": "dce2d"
         },
         "phase_edp_slow_l2a": {
             "cdf_name": "edp_phase_slow_l2a",
             "dtype": "dce2d"
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/probe_align_times.py` & `pyrfu-2.4.4/pyrfu/mms/probe_align_times.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/psd2def.py` & `pyrfu-2.4.4/pyrfu/mms/psd2def.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/psd2dpf.py` & `pyrfu-2.4.4/pyrfu/mms/psd2dpf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/psd_moments.py` & `pyrfu-2.4.4/pyrfu/mms/psd_moments.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     ----------
     vdf : xarray.Dataset
         3D skymap velocity distribution.
     sc_pot : xarray.DataArray
         Time series of the spacecraft potential.
 
     Returns
-    --------
+    -------
     n_psd : xarray.DataArray
         Time series of the number density (1rst moment).
     v_psd : xarray.DataArray
         Time series of the bulk velocity (2nd moment).
     p_psd : xarray.DataArray
         Time series of the pressure tensor (3rd moment).
     p2_psd : xarray.DataArray
@@ -205,19 +205,19 @@
         ensure that the same number of points are integrated over.
     no_sc_pot : bool
         Set to 1 to set spacecraft potential to zero. Calculates moments
         without correcting for spacecraft potential.
     en_channels : array_like
         Set energy channels to integrate over [min max]; min and max between
         must be between 1 and 32.
-    partial_moments : ndarray or xarray.DataArray
-        Use a binary array (or DataArray) (pmomsarr) to select which psd
-        points are used in the moments calculation. pmomsarr must be a
-        binary array (1s and 0s, 1s correspond to points used). Array (or
-        data of Dataarray) must be the same size as vdf.data.
+    partial_moments : numpy.ndarray or xarray.DataArray
+        Use a binary array to select which psd points are used in the moments
+        calculation. `partial_moments` must be a binary array (1s and 0s,
+        1s correspond to points used). Array (or data of Dataarray) must be the same
+        size as vdf.data.
     inner_electron : {"on", "off"}
         inner_electrontron potential for electron moments.
 
     Examples
     --------
     >>> from pyrfu import mms
 
@@ -244,15 +244,15 @@
 
     # [eV] sc_pot + w_inner_electron for electron moments calculation
     w_inner_electron = 3.5
 
     vdf.data.data *= 1e12
 
     # Check if data is fast or burst resolution
-    field_name = vdf.attrs["FIELDNAM"]
+    field_name = vdf.data.attrs["FIELDNAM"]
 
     if "brst" in field_name:
         is_brst_data = True
         logging.info("Burst resolution data is used")
     elif "fast" in field_name:
         is_brst_data = False
         logging.info("Fast resolution data is used")
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/psd_rebin.py` & `pyrfu-2.4.4/pyrfu/mms/psd_rebin.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 
     Parameters
     ----------
     vdf : xarray.Dataset
         Time series of the particle distribution.
     phi : xarray.DataArray
         Time series of the phi angles.
-    energy0 : xarray.DataArray or ndarray
+    energy0 : xarray.DataArray or numpy.ndarray
         Energy table 0.
-    energy1 : xarray.DataArray or ndarray
+    energy1 : xarray.DataArray or numpy.ndarray
         Energy table 1.
     step_table : xarray.DataArray
         Time series of the stepping table between energies (burst).
 
     Returns
     -------
-    time_r : ndarray
+    time_r : numpy.ndarray
         Revised time steps.
-    vdf_r : ndarray
+    vdf_r : numpy.ndarray
         Rebinned particle distribution.
-    energy_r : ndarray
+    energy_r : numpy.ndarray
         Revised energy table.
-    phi_r : ndarray
+    phi_r : numpy.ndarray
         Time series of the recalculated phi angle.
 
     Notes
     -----
     I'm assuming no gaps in the burst data interval. If there is a gap use
     time_clip before running. To be updated later.
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/read_feeps_sector_masks_csv.py` & `pyrfu-2.4.4/pyrfu/mms/read_feeps_sector_masks_csv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/reduce.py` & `pyrfu-2.4.4/pyrfu/mms/reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/remove_edist_background.py` & `pyrfu-2.4.4/pyrfu/mms/remove_edist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/remove_idist_background.py` & `pyrfu-2.4.4/pyrfu/mms/remove_idist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/remove_imoms_background.py` & `pyrfu-2.4.4/pyrfu/mms/remove_imoms_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/rotate_tensor.py` & `pyrfu-2.4.4/pyrfu/mms/rotate_tensor.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/scpot2ne.py` & `pyrfu-2.4.4/pyrfu/mms/scpot2ne.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/spectr_to_dataset.py` & `pyrfu-2.4.4/pyrfu/mms/spectr_to_dataset.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/tokenize.py` & `pyrfu-2.4.4/pyrfu/mms/tokenize.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     "partve",
     "qi",
     "errqi",
     "qe",
     "errqe",
     "b",
     "e",
+    "hmfe",
     "e2d",
     "es12",
     "es34",
 ]
 
 all_params_tensors = [
     "pi",
```

### Comparing `pyrfu-2.4.3/pyrfu/mms/vdf_elim.py` & `pyrfu-2.4.4/pyrfu/mms/vdf_elim.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/vdf_omni.py` & `pyrfu-2.4.4/pyrfu/mms/vdf_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/vdf_projection.py` & `pyrfu-2.4.4/pyrfu/mms/vdf_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/vdf_reduce.py` & `pyrfu-2.4.4/pyrfu/mms/vdf_reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/vdf_to_e64.py` & `pyrfu-2.4.4/pyrfu/mms/vdf_to_e64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/mms/whistler_b2e.py` & `pyrfu-2.4.4/pyrfu/mms/whistler_b2e.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/models/igrf.py` & `pyrfu-2.4.4/pyrfu/models/igrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/models/igrf13coeffs.csv` & `pyrfu-2.4.4/pyrfu/models/igrf13coeffs.csv`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/models/magnetopause_normal.py` & `pyrfu-2.4.4/pyrfu/models/magnetopause_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,15 @@
     r_gsm,
     b_z_imf,
     p_sw,
     model: str = "mp_shue1997",
     m_alfven: float = 4.0,
 ):
     r"""Computes the distance and normal vector to the magnetopause for
-    Shue et al., 1997 or Shue et al., 1998 model. Or bow shock for
-    Farris & Russell 1994 model.
+    [1]_ or [2]_ model. Or bow shock for [3]_ model.
 
     Parameters
     ----------
     r_gsm : array_like
         GSM position in Re (if more than 3 values assumes that 1st is time).
     b_z_imf : float
         IMF Bz in nT.
```

### Comparing `pyrfu-2.4.3/pyrfu/plot/__init__.py` & `pyrfu-2.4.4/pyrfu/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/add_position.py` & `pyrfu-2.4.4/pyrfu/plot/add_position.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/annotate_heatmap.py` & `pyrfu-2.4.4/pyrfu/plot/annotate_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/colorbar.py` & `pyrfu-2.4.4/pyrfu/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg` & `pyrfu-2.4.4/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/make_labels.py` & `pyrfu-2.4.4/pyrfu/plot/make_labels.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/mms_pl_config.py` & `pyrfu-2.4.4/pyrfu/plot/mms_pl_config.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/pl_scatter_matrix.py` & `pyrfu-2.4.4/pyrfu/plot/pl_scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/pl_tx.py` & `pyrfu-2.4.4/pyrfu/plot/pl_tx.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_ang_ang.py` & `pyrfu-2.4.4/pyrfu/plot/plot_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_clines.py` & `pyrfu-2.4.4/pyrfu/plot/plot_clines.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_heatmap.py` & `pyrfu-2.4.4/pyrfu/plot/plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_line.py` & `pyrfu-2.4.4/pyrfu/plot/plot_line.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_magnetosphere.py` & `pyrfu-2.4.4/pyrfu/plot/plot_magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_projection.py` & `pyrfu-2.4.4/pyrfu/plot/plot_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_reduced_2d.py` & `pyrfu-2.4.4/pyrfu/plot/plot_reduced_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_sitl_overview.py` & `pyrfu-2.4.4/pyrfu/plot/plot_sitl_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,26 +342,28 @@
 
 
 def plot_sitl_overview(
     tint_brst,
     title,
     mms_id: int = 2,
     data_path: str = "/Volumes/mms",
-    fig_path: str = "figures",
+    fig_path: str = "./figures",
 ):
     r"""Creates overview plot from SITL selections.
 
-    Paramters
-    ---------
+    Parameters
+    ----------
     tint_brst : list
         Time interval selected.
     mms_id : int, Optional
         Spacecraft index. Default is 1.
     data_path : str, Optional
-        Path to MMS data. Default is /Volumes/
+        Path to MMS data. Default is the one defined in pyrfu.mms.config.json
+    fig_path : str, Optional
+        Path to save the figures. Default is ./figures
 
     Returns
     -------
     fig : matplotlib.figure
         Figure.
     axs : list
         All axes.
```

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_spectr.py` & `pyrfu-2.4.4/pyrfu/plot/plot_spectr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/plot_surf.py` & `pyrfu-2.4.4/pyrfu/plot/plot_surf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/span_tint.py` & `pyrfu-2.4.4/pyrfu/plot/span_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/plot/zoom.py` & `pyrfu-2.4.4/pyrfu/plot/zoom.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/__init__.py` & `pyrfu-2.4.4/pyrfu/pyrf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/average_vdf.py` & `pyrfu-2.4.4/pyrfu/pyrf/average_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/avg_4sc.py` & `pyrfu-2.4.4/pyrfu/pyrf/avg_4sc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+# 3rd party imports
+import xarray as xr
+
 # Local imports
 from .calc_fs import calc_fs
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
@@ -40,12 +43,22 @@
     Spacecraft indices
 
     >>> b_mms = [get_data("B_gse_fgm_srvy_l2", tint, i) for i in range(1, 5)]
     >>> b_xyz = avg_4sc(b_mms)
 
     """
 
-    b_list = [resample(b, b_list[0], f_s=calc_fs(b_list[0])) for b in b_list]
+    # Check input type
+    assert isinstance(b_list, list), "b_list must be a list"
+
+    b_list_r = []
+
+    for b in b_list:
+        if isinstance(b, xr.DataArray):
+            b_list_r.append(resample(b, b_list[0], f_s=calc_fs(b_list[0])))
+        else:
+            raise TypeError("elements of b_list must be xarray.DataArray")
 
+    # Average the resamples time series
     b_avg = sum(b_list) / len(b_list)
 
     return b_avg
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/c_4_grad.py` & `pyrfu-2.4.4/pyrfu/pyrf/c_4_grad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/c_4_j.py` & `pyrfu-2.4.4/pyrfu/pyrf/c_4_j.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def c_4_j(r_list, b_list):
     r"""Calculate current density :math:`J` from using 4
-    spacecraft technique [4]_, the divergence of the magnetic field
+    spacecraft technique [1]_, the divergence of the magnetic field
     :math:`\nabla . B`, magnetic field at the center of
     mass of the tetrahedron, :math:`J \times B`
     force, part of the divergence of stress associated with
     curvature :math:`\nabla.T_{shear}` and gradient of
     the magnetic pressure :math:`\nabla P_b`. Where :
 
     .. math::
@@ -33,15 +33,15 @@
         J \times B = \nabla.T_{shear} + \nabla P_b
 
         \nabla.T_{shear} = \frac{(B.\nabla) B}{\mu_0}
 
         \nabla P_b = \nabla \frac{B^2}{2\mu_0}
 
     The divergence of the magnetic field is current density units as
-    it shows the error on the estimation of the current density [5]_ .
+    it shows the error on the estimation of the current density [2]_ .
 
     Parameters
     ----------
     r_list : list of xarray.DataArray
         Time series of the spacecraft position [km].
     b_list : list of xarray.DataArray
         Time series of the magnetic field [nT].
@@ -69,20 +69,20 @@
     pyrfu.pyrf.c_4_k : Calculates reciprocal vectors in barycentric
                             coordinates.
     pyrfu.pyrf.c_4_grad : Calculate gradient of physical field using 4
                             spacecraft technique.
 
     References
     ----------
-    .. [4]	Dunlop, M. W., A. Balogh, K.-H. Glassmeier, and P. Robert
+    .. [1]	Dunlop, M. W., A. Balogh, K.-H. Glassmeier, and P. Robert
             (2002a), Four-point Cluster application of magnetic field
             analysis tools: The Curl- ometer, J. Geophys. Res.,
             107(A11), 1384, doi : https://doi.org/10.1029/2001JA005088.
 
-    .. [5]	Robert, P., et al. (1998), Accuracy of current determination,
+    .. [2]	Robert, P., et al. (1998), Accuracy of current determination,
             in Analysis Methods for Multi-Spacecraft Data, edited by G.
             Paschmann and P. W. Daly, pp. 395–418, Int. Space Sci. Inst.,
             Bern. url : http://www.issibern.ch/forads/sr-001-16.pdf
 
     Examples
     --------
     >>> import numpy as np
@@ -94,21 +94,20 @@
 
     Spacecraft indices
 
     >>> mms_list = np.arange(1,5)
 
     Load magnetic field and spacecraft position
 
-    >>> b_mms = [mms.get_data("B_gse_fgm_srvy_l2", tint, i) for i in mms_list]
-    >>> r_mms = [mms.get_data("R_gse", tint, i) for i in mms_list]
+    >>> b_mms = [mms.get_data("b_gse_fgm_srvy_l2", tint, i) for i in mms_list]
+    >>> r_mms = [mms.get_data("r_gse_mec_srvy_l2", tint, i) for i in mms_list]
 
     Compute current density, divergence of b, etc. using curlometer technique
 
-    >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms,
-    b_mms)
+    >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
 
     """
 
     mu0 = constants.mu_0
 
     b_avg = 1e-9 * avg_4sc(b_list)
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/c_4_k.py` & `pyrfu-2.4.4/pyrfu/pyrf/c_4_k.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/c_4_v.py` & `pyrfu-2.4.4/pyrfu/pyrf/c_4_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/calc_ag.py` & `pyrfu-2.4.4/pyrfu/pyrf/calc_ag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
+
+# Local imports
+from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -63,20 +67,28 @@
 
     Compute agyrotropy coefficient
 
     >>> ag_e, ag_cr_e = pyrf.calc_ag(p_fac_e_pp)
 
     """
 
+    # Check input type
+    assert isinstance(p_xyz, xr.DataArray), "p_xyz must be a xarray.DataArray"
+
+    # Check import shape
+    message = "p_xyz must be a time series of a tensor"
+    assert p_xyz.data.ndim == 3 and p_xyz.shape[1] == 3 and p_xyz.shape[2] == 3, message
+
     # Diagonal and off-diagonal terms
-    p_11, p_22, _ = [p_xyz[:, 0, 0], p_xyz[:, 1, 1], p_xyz[:, 2, 2]]
-    p_12, p_13, p_23 = [p_xyz[:, 0, 1], p_xyz[:, 0, 2], p_xyz[:, 1, 2]]
+    p_11, p_22, _ = [p_xyz.data[:, 0, 0], p_xyz.data[:, 1, 1], p_xyz.data[:, 2, 2]]
+    p_12, p_13, p_23 = [p_xyz.data[:, 0, 1], p_xyz.data[:, 0, 2], p_xyz.data[:, 1, 2]]
 
     det_p = p_11 * (p_22**2 - p_23**2)
     det_p -= p_12 * (p_12 * p_22 - p_23 * p_13)
     det_p += p_13 * (p_12 * p_23 - p_22 * p_13)
 
     det_g = p_11 * p_22**2
 
     agyrotropy = np.abs(det_p - det_g) / (det_p + det_g)
+    agyrotropy = ts_scalar(p_xyz.time.data, agyrotropy)
 
     return agyrotropy
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/calc_agyro.py` & `pyrfu-2.4.4/pyrfu/pyrf/calc_agyro.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
+
+# Local imports
+from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -54,13 +58,21 @@
 
     Compute agyrotropy coefficient
 
     >>> agyro_e = pyrf.calc_agyro(p_fac_e_qq)
 
     """
 
+    # Check input type
+    assert isinstance(p_xyz, xr.DataArray), "p_xyz must be a xarray.DataArray"
+
+    # Check import shape
+    message = "p_xyz must be a time series of a tensor"
+    assert p_xyz.data.ndim == 3 and p_xyz.shape[1] == 3 and p_xyz.shape[2] == 3, message
+
     # Parallel and perpendicular components
-    p_perp_1, p_perp_2 = [p_xyz[:, 1, 1], p_xyz[:, 2, 2]]
+    p_perp_1, p_perp_2 = [p_xyz.data[:, 1, 1], p_xyz.data[:, 2, 2]]
 
-    agyro = np.abs(p_perp_1 - p_perp_2) / (p_perp_1 + p_perp_2)
+    agyrotropy = np.abs(p_perp_1 - p_perp_2) / (p_perp_1 + p_perp_2)
+    agyrotropy = ts_scalar(p_xyz.time.data, agyrotropy)
 
-    return agyro
+    return agyrotropy
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/calc_dng.py` & `pyrfu-2.4.4/pyrfu/pyrf/calc_dng.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
+
+# Local imports
+from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -61,17 +65,26 @@
 
     Compute agyrotropy coefficient
 
     >>> d_ng_e = pyrf.calc_dng(p_fac_e_pp)
 
     """
 
+    # Check input type
+    assert isinstance(p_xyz, xr.DataArray), "p_xyz must be a xarray.DataArray"
+
+    # Check import shape
+    message = "p_xyz must be a time series of a tensor"
+    assert p_xyz.data.ndim == 3 and p_xyz.shape[1] == 3 and p_xyz.shape[2] == 3, message
+
     # Parallel and perpendicular components
-    p_para, p_perp = [p_xyz[:, 0, 0], (p_xyz[:, 1, 1] + p_xyz[:, 2, 2]) / 2]
+    p_para = p_xyz.data[:, 0, 0]
+    p_perp = (p_xyz.data[:, 1, 1] + p_xyz.data[:, 2, 2]) / 2
 
     # Off-diagonal terms
-    p_12, p_13, p_23 = [p_xyz[:, 0, 1], p_xyz[:, 0, 2], p_xyz[:, 1, 2]]
+    p_12, p_13, p_23 = [p_xyz.data[:, 0, 1], p_xyz.data[:, 0, 2], p_xyz.data[:, 1, 2]]
 
     d_ng = np.sqrt(8 * (p_12**2 + p_13**2 + p_23**2))
     d_ng /= p_para + 2 * p_perp
+    d_ng = ts_scalar(p_xyz.time.data, d_ng)
 
     return d_ng
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/calc_dt.py` & `pyrfu-2.4.4/pyrfu/pyrf/calc_dt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def calc_dt(inp):
     r"""Computes time step of the input time series.
 
     Parameters
     ----------
-    inp : xarray.DataArray
+    inp : xarray.DataArray or xarray.Dataset
         Time series of the input variable.
 
     Returns
     -------
     out : float
         Time step in seconds.
 
     """
 
+    message = "Input must be a time series"
+    assert isinstance(inp, (xr.Dataset, xr.DataArray)), message
+
     out = np.median(np.diff(inp.time.data)).astype(np.float64) * 1e-9
 
     return out
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/calc_sqrtq.py` & `pyrfu-2.4.4/pyrfu/pyrf/calc_sqrtq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
+
+# Local imports
+from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -60,17 +64,26 @@
 
     Compute agyrotropy coefficient
 
     >>> sqrt_q_e = pyrf.calc_sqrtq(p_fac_e_pp)
 
     """
 
+    # Check input type
+    assert isinstance(p_xyz, xr.DataArray), "p_xyz must be a xarray.DataArray"
+
+    # Check import shape
+    message = "p_xyz must be a time series of a tensor"
+    assert p_xyz.data.ndim == 3 and p_xyz.shape[1] == 3 and p_xyz.shape[2] == 3, message
+
     # Parallel and perpendicular components
-    p_para, p_perp = [p_xyz[:, 0, 0], (p_xyz[:, 1, 1] + p_xyz[:, 2, 2]) / 2]
+    p_para = p_xyz.data[:, 0, 0]
+    p_perp = (p_xyz.data[:, 1, 1] + p_xyz.data[:, 2, 2]) / 2
 
     # Off-diagonal terms
-    p_12, p_13, p_23 = [p_xyz[:, 0, 1], p_xyz[:, 0, 2], p_xyz[:, 1, 2]]
+    p_12, p_13, p_23 = [p_xyz.data[:, 0, 1], p_xyz.data[:, 0, 2], p_xyz.data[:, 1, 2]]
 
     sqrt_q = np.sqrt(p_12**2 + p_13**2 + p_23**2)
     sqrt_q /= np.sqrt(p_perp**2 + 2 * p_perp * p_para)
+    sqrt_q = ts_scalar(p_xyz.time.data, sqrt_q)
 
     return sqrt_q
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/cart2sph.py` & `pyrfu-2.4.4/pyrfu/pyrf/cart2sph.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/cart2sph_ts.py` & `pyrfu-2.4.4/pyrfu/pyrf/cart2sph_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/cdfepoch2datetime64.py` & `pyrfu-2.4.4/pyrfu/pyrf/cdfepoch2datetime64.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,23 +61,27 @@
 
 
 def cdfepoch2datetime64(epochs):
     r"""Converts CDF epochs to numpy.datetime64 with nanosecond precision.
 
     Parameters
     ----------
-    epochs : array_like
+    epochs : float or int or array_like
         CDF epochs to convert.
 
     Returns
     -------
     times : numpy.ndarray
         Array of times in datetime64([ns]).
 
     """
 
+    # Check input type
+    message = "epochs must be array_like"
+    assert isinstance(epochs, (float, int, list, np.ndarray)), message
+
     times = cdfepoch.breakdown(epochs)
     times = np.transpose(np.atleast_2d(times))
 
     times = _compose_date(*times).astype("datetime64[ns]")
 
     return times
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/compress_cwt.py` & `pyrfu-2.4.4/pyrfu/pyrf/compress_cwt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/convert_fac.py` & `pyrfu-2.4.4/pyrfu/pyrf/convert_fac.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/corr_deriv.py` & `pyrfu-2.4.4/pyrfu/pyrf/corr_deriv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/cotrans.py` & `pyrfu-2.4.4/pyrfu/pyrf/cotrans.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         else:
             transf_mat_out = np.matmul(transf_mat, transf_mat_out)
 
     return transf_mat_out
 
 
 def cotrans(inp, flag, hapgood: bool = True):
-    r"""Coordinate transformation GE0/GEI/GSE/GSM/SM/MAG
+    r"""Coordinate transformation GE0/GEI/GSE/GSM/SM/MAG as described in [1]_
 
     Parameters
     ----------
     inp : xarray.DataArray or ndarray
         Time series of the input field.
     flag : str
         Coordinates transformation "{coord1}>{coord2}", where coord1 and
@@ -191,24 +191,21 @@
 
     If the original coordinates is not in the meta
 
     >>> b_gsm = cotrans(b_gse, 'GSE>GSM')
 
     Compute the dipole direction in GSE
 
-    >>> dipole = cotrans(b_gse.time,
-    'dipoledirectiongse')
+    >>> dipole = cotrans(b_gse.time, 'dipoledirectiongse')
 
 
     References
     ----------
-    .. [17]     Hapgood 1997 (corrected version of Hapgood 1992) Planet.Space
-                Sci..Vol. 40, No. 5. pp. 71l - 717, 1992
-
-    .. [18]     USNO - AA 2011 & 2012
+    .. [1]  Hapgood 1997 (corrected version of Hapgood 1992) Planet.Space Sci..Vol.
+            40, No. 5. pp. 71l - 717, 1992
 
     """
 
     if ">" in flag:
         ref_syst_in, ref_syst_out = flag.split(">")
     else:
         ref_syst_in, ref_syst_out = [None, flag.lower()]
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/cross.py` & `pyrfu-2.4.4/pyrfu/pyrf/cross.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/date_str.py` & `pyrfu-2.4.4/pyrfu/pyrf/date_str.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/datetime2iso8601.py` & `pyrfu-2.4.4/pyrfu/pyrf/datetime2iso8601.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
+import datetime
+
+import numpy as np
 import pandas as pd
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
@@ -23,18 +26,24 @@
     Returns
     -------
     tt2000 : str
         Time in TT20000 iso_8601 format.
 
     """
 
-    if isinstance(time, list):
+    # Check input type
+    message = "time must be array_like or datetime.datetime"
+    assert isinstance(time, (list, np.ndarray, datetime.datetime)), message
+
+    if isinstance(time, (np.ndarray, list)):
         return list(map(datetime2iso8601, time))
 
+    assert isinstance(time, datetime.datetime), "time datetime.datetime"
+
     time_datetime = pd.Timestamp(time)
 
     # Convert to string
     datetime_str = time_datetime.strftime("%Y-%m-%dT%H:%M:%S.%f")
 
-    tt2000 = f"{datetime_str}{time_datetime.nanosecond:03d}"
+    time_iso8601 = f"{datetime_str}{time_datetime.nanosecond:03d}"
 
-    return tt2000
+    return time_iso8601
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/datetime642iso8601.py` & `pyrfu-2.4.4/pyrfu/pyrf/datetime642iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/datetime642ttns.py` & `pyrfu-2.4.4/pyrfu/pyrf/datetime642ttns.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/datetime642unix.py` & `pyrfu-2.4.4/pyrfu/pyrf/datetime642unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/dec_par_perp.py` & `pyrfu-2.4.4/pyrfu/pyrf/dec_par_perp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/dist_append.py` & `pyrfu-2.4.4/pyrfu/pyrf/dist_append.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,45 +76,28 @@
             [
                 inp0.attrs["delta_energy_minus"].data,
                 inp1.attrs["delta_energy_minus"].data,
             ],
         )
         glob_attrs["delta_energy_minus"] = delta_energy_minus
 
-    # Energy
-    if inp0.attrs["tmmode"] == "brst":
-        step_table = np.hstack(
-            [inp0.attrs["esteptable"], inp1.attrs["esteptable"]],
-        )
-
-        out = ts_skymap(
-            time,
-            data,
-            None,
-            phi,
-            theta,
-            energy0=inp0.energy0,
-            energy1=inp0.energy1,
-            esteptable=step_table,
-            attrs=data_attrs,
-            coords_attrs=coords_attrs,
-            glob_attrs=glob_attrs,
-        )
+    step_table = np.hstack(
+        [inp0.attrs["esteptable"], inp1.attrs["esteptable"]],
+    )
 
-    else:
-        energy = np.vstack([inp0.energy.data, inp1.energy.data])
+    energy = np.vstack([inp0.energy.data, inp1.energy.data])
 
-        out = ts_skymap(
-            time,
-            data,
-            energy,
-            phi,
-            theta,
-            energy0=inp0.energy0,
-            energy1=inp0.energy1,
-            esteptable=np.ones(energy.shape[0]),
-            attrs=data_attrs,
-            coords_attrs=coords_attrs,
-            glob_attrs=glob_attrs,
-        )
+    out = ts_skymap(
+        time,
+        data,
+        energy,
+        phi,
+        theta,
+        energy0=inp0.energy0,
+        energy1=inp0.energy1,
+        esteptable=step_table,
+        attrs=data_attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
 
     return out
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/dot.py` & `pyrfu-2.4.4/pyrfu/pyrf/dot.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/dynamic_press.py` & `pyrfu-2.4.4/pyrfu/pyrf/dynamic_press.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/e_vxb.py` & `pyrfu-2.4.4/pyrfu/pyrf/e_vxb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/eb_nrf.py` & `pyrfu-2.4.4/pyrfu/pyrf/eb_nrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ebsp.py` & `pyrfu-2.4.4/pyrfu/pyrf/ebsp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/edb.py` & `pyrfu-2.4.4/pyrfu/pyrf/edb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/end.py` & `pyrfu-2.4.4/pyrfu/pyrf/end.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/estimate.py` & `pyrfu-2.4.4/pyrfu/pyrf/estimate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/extend_tint.py` & `pyrfu-2.4.4/pyrfu/pyrf/extend_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/filt.py` & `pyrfu-2.4.4/pyrfu/pyrf/filt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/find_closest.py` & `pyrfu-2.4.4/pyrfu/pyrf/find_closest.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/get_omni_data.py` & `pyrfu-2.4.4/pyrfu/pyrf/get_omni_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/gradient.py` & `pyrfu-2.4.4/pyrfu/pyrf/gradient.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/gse2gsm.py` & `pyrfu-2.4.4/pyrfu/pyrf/gse2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/histogram.py` & `pyrfu-2.4.4/pyrfu/pyrf/histogram.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/histogram2d.py` & `pyrfu-2.4.4/pyrfu/pyrf/histogram2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
 
     Compute magnitude of B and J
 
     >>> b_mag = pyrf.norm(b_xyz)
     >>> j_mag = pyrf.norm(j_xyz)
 
-    Histogram of |J| vs |B|
+    Histogram of J vs B
 
     >>> h2d_b_j = pyrf.histogram2d(b_mag, j_mag)
 
     """
 
     # resample inp2 with respect to inp1
     if len(inp2) != len(inp1):
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/increments.py` & `pyrfu-2.4.4/pyrfu/pyrf/increments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/int_sph_dist.py` & `pyrfu-2.4.4/pyrfu/pyrf/int_sph_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/integrate.py` & `pyrfu-2.4.4/pyrfu/pyrf/integrate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/iplasma_calc.py` & `pyrfu-2.4.4/pyrfu/pyrf/iplasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/iso2unix.py` & `pyrfu-2.4.4/pyrfu/pyrf/iso2unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime.py` & `pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime64.py` & `pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/iso86012timevec.py` & `pyrfu-2.4.4/pyrfu/pyrf/iso86012timevec.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __status__ = "Prototype"
 
 
 def iso86012timevec(time):
     r"""Convert ISO 8601 time string into time vector.
 
     Parameters
-    ---------
+    ----------
     time : str
         Time in ISO 8601 format YYYY-MM-DDThh:mm:ss.mmmuuunnn.
 
     Returns
     -------
     time_vec : list
         Time vector.
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/l_shell.py` & `pyrfu-2.4.4/pyrfu/pyrf/l_shell.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/lowpass.py` & `pyrfu-2.4.4/pyrfu/pyrf/lowpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/magnetosphere.py` & `pyrfu-2.4.4/pyrfu/pyrf/magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/match_phibe_dir.py` & `pyrfu-2.4.4/pyrfu/pyrf/match_phibe_dir.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/match_phibe_v.py` & `pyrfu-2.4.4/pyrfu/pyrf/match_phibe_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/mean.py` & `pyrfu-2.4.4/pyrfu/pyrf/mean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/mean_bins.py` & `pyrfu-2.4.4/pyrfu/pyrf/mean_bins.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
 
     Compute magnitude of B and J
 
     >>> b_mag = pyrf.norm(b_xyz)
     >>> j_mag = pyrf.norm(j_xyz)
 
-    Mean value of |J| for 10 bins of |B|
+    Mean value of J for 10 bins of B
 
     >>> m_b_j = pyrf.mean_bins(b_mag, j_mag)
 
     """
 
     if inp1 is None:
         inp1 = inp0
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/mean_field.py` & `pyrfu-2.4.4/pyrfu/pyrf/mean_field.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/medfilt.py` & `pyrfu-2.4.4/pyrfu/pyrf/medfilt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/median_bins.py` & `pyrfu-2.4.4/pyrfu/pyrf/median_bins.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
 
     Compute magnitude of B and J
 
     >>> b_mag = pyrf.norm(b_xyz)
     >>> j_mag = pyrf.norm(j_xyz)
 
-    Median value of |J| for 10 bins of |B|
+    Median value of J for 10 bins of B
 
     >>> med_b_j = pyrf.mean_bins(b_mag, j_mag)
 
     """
 
     x_sort = np.sort(inp0.data)
     x_edge = np.linspace(x_sort[0], x_sort[-1], bins + 1)
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/movmean.py` & `pyrfu-2.4.4/pyrfu/pyrf/movmean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/mva.py` & `pyrfu-2.4.4/pyrfu/pyrf/mva.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/new_xyz.py` & `pyrfu-2.4.4/pyrfu/pyrf/new_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/norm.py` & `pyrfu-2.4.4/pyrfu/pyrf/norm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/normalize.py` & `pyrfu-2.4.4/pyrfu/pyrf/normalize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_1d.py` & `pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     Returns
     -------
     opt_n_x : int
         Number of bins that minimizes the cost function.
 
     References
     ----------
-    _[1]    Rudemo, M. (1982) Empirical Choice of Histograms and Kernel Density
+    .. [1]  Rudemo, M. (1982) Empirical Choice of Histograms and Kernel Density
             Estimators. Scandinavian Journal of Statistics, 9, 65-78.
 
-    _[2]    Shimazaki H. and Shinomoto S., A method for selecting the bin size
+    .. [2]  Shimazaki H. and Shinomoto S., A method for selecting the bin size
             of a time histogram Neural Computation (2007) Vol. 19(6), 1503-1527
     """
 
     x_min, x_max = [np.min(x.data), np.max(x.data)]
 
     # #of Bins
     ns_x = np.arange(n_min, n_max)
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_2d.py` & `pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/pid_4sc.py` & `pyrfu-2.4.4/pyrfu/pyrf/pid_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/plasma_beta.py` & `pyrfu-2.4.4/pyrfu/pyrf/plasma_beta.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/plasma_calc.py` & `pyrfu-2.4.4/pyrfu/pyrf/plasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/poynting_flux.py` & `pyrfu-2.4.4/pyrfu/pyrf/poynting_flux.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/pres_anis.py` & `pyrfu-2.4.4/pyrfu/pyrf/pres_anis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/psd.py` & `pyrfu-2.4.4/pyrfu/pyrf/psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/pvi.py` & `pyrfu-2.4.4/pyrfu/pyrf/pvi.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/pvi_4sc.py` & `pyrfu-2.4.4/pyrfu/pyrf/pvi_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/read_cdf.py` & `pyrfu-2.4.4/pyrfu/pyrf/read_cdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/remove_repeated_points.py` & `pyrfu-2.4.4/pyrfu/pyrf/remove_repeated_points.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/resample.py` & `pyrfu-2.4.4/pyrfu/pyrf/resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,18 +269,14 @@
         Points above STD*THRESH are disregarded for averaging
 
     Returns
     -------
     out : xarray.DataArray
         Resampled input to the reference time line using the selected method.
 
-    TODO
-    ----
-    Make the resampling VDF (xarray.Dataset) compliant.
-
 
     Examples
     --------
     >>> from pyrfu import mms, pyrf
 
     Time interval
 
@@ -288,16 +284,16 @@
 
     Spacecraft index
 
     >>> mms_id = 1
 
     Load magnetic field and electric field
 
-    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_fast_l2", tint, mms_id)
+    >>> b_xyz = mms.get_data("e_gse_fgm_srvy_l2", tint, mms_id)
+    >>> e_xyz = mms.get_data("e_gse_edp_fast_l2", tint, mms_id)
 
     Resample magnetic field to electric field sampling
 
     >>> b_xyz = pyrf.resample(b_xyz, e_xyz)
 
     """
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/shock_models_parameters.json` & `pyrfu-2.4.4/pyrfu/pyrf/shock_models_parameters.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/shock_normal.py` & `pyrfu-2.4.4/pyrfu/pyrf/shock_normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,20 @@
         Hash table with:
             * b_u : Upstream magnetic field (nT).
             * b_d : Downstream magnetic field.
             * v_u : Upstream plasma bulk velocity (km/s).
             * v_d : Downstream plasma bulk velocity.
             * n_u : Upstream number density (cm^-3).
             * n_d : Downstream number density.
-        Optional:
             * r_xyz : Spacecraft position in time series format of 1x3 vector. Optional.
             * d2u : Down-to-up, is 1 or -1. Optional.
             * dt_f : Time duration of shock foot (s). Optional.
             * f_cp : Reflected ion gyrofrequency (Hz). Optional.
-            * n : Number of Monte Carlo particles used in determining errorbars.
-            Optional, default is 100.
+            * n : Number of Monte Carlo particles. Optional, default is 100.
+
     leq90 : bool, Optional
         Force angles to be less than 90 (default). For leq90 = 0, angles can be between
         0 and 180 deg. For time series input and quasi-perp shocks,leq90 = 0 is
         recommended.
 
     Returns
     -------
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/shock_parameters.py` & `pyrfu-2.4.4/pyrfu/pyrf/shock_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/solid_angle.py` & `pyrfu-2.4.4/pyrfu/pyrf/solid_angle.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/sph2cart.py` & `pyrfu-2.4.4/pyrfu/pyrf/sph2cart.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/st_diff.py` & `pyrfu-2.4.4/pyrfu/pyrf/st_diff.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/start.py` & `pyrfu-2.4.4/pyrfu/pyrf/start.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party import
 import numpy as np
+import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -23,10 +24,16 @@
     Returns
     -------
     out : float
         Value of the first time in the desired format.
 
     """
 
+    # Check input type
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+
+    # Make sure this is a time series
+    assert list(inp.dims)[0] == "time", "inp must be a time series"
+
     out = inp.time.data[0].astype(np.int64) * 1e-9
 
     return out
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/struct_func.py` & `pyrfu-2.4.4/pyrfu/pyrf/struct_func.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/t_eval.py` & `pyrfu-2.4.4/pyrfu/pyrf/t_eval.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/time_clip.py` & `pyrfu-2.4.4/pyrfu/pyrf/time_clip.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/timevec2iso8601.py` & `pyrfu-2.4.4/pyrfu/pyrf/timevec2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/trace.py` & `pyrfu-2.4.4/pyrfu/pyrf/trace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
+# Local imports
+from .ts_scalar import ts_scalar
+
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
@@ -48,24 +51,20 @@
 
     Compute scalar temperature
 
     >>> t_i = pyrf.trace(t_xyzfac_i)
 
     """
 
-    inp_data = inp.data
-    out_data = inp_data[:, 0, 0] + inp_data[:, 1, 1] + inp_data[:, 2, 2]
+    # Check input type
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
 
-    # Attributes
-    attrs = inp.attrs
+    # Check that inp is a tensor
+    message = "inp must be a time series of a tensor"
+    assert inp.ndim == 3 and inp.shape[1] == 3 and inp.shape[1] == 3, message
 
-    # Change tensor order from 2 (matrix) to 0 (scalar)
-    attrs["TENSOR_ORDER"] = 0
+    out_data = inp.data[:, 0, 0] + inp.data[:, 1, 1] + inp.data[:, 2, 2]
 
-    out = xr.DataArray(
-        out_data,
-        coords=[inp.time.data],
-        dims=["time"],
-        attrs=attrs,
-    )
+    # Construct time series
+    out = ts_scalar(inp.time.data, out_data, inp.attrs)
 
     return out
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/transformation_indices.json` & `pyrfu-2.4.4/pyrfu/pyrf/transformation_indices.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ts_append.py` & `pyrfu-2.4.4/pyrfu/pyrf/ts_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ts_scalar.py` & `pyrfu-2.4.4/pyrfu/pyrf/ts_scalar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
+import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
@@ -13,31 +14,36 @@
 
 
 def ts_scalar(time, data, attrs: dict = None):
     r"""Create a time series containing a 0th order tensor
 
     Parameters
     ----------
-    time : ndarray
+    time : numpy.ndarray
         Array of times.
-    data : ndarray
+    data : numpy.ndarray
         Data corresponding to the time list.
     attrs : dict, Optional
         Attributes of the data list.
 
     Returns
     -------
     out : xarray.DataArray
         0th order tensor time series.
 
     """
 
+    # Check input type
+    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
+    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
+
+    # Check input shape must be (n, )
     assert data.ndim == 1, "Input must be a scalar"
     assert len(time) == len(data), "Time and data must have the same length"
 
-    if attrs is None:
+    if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
     out = xr.DataArray(data, coords=[time[:]], dims="time", attrs=attrs)
     out.attrs["TENSOR_ORDER"] = 0
 
     return out
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ts_tensor_xyz.py` & `pyrfu-2.4.4/pyrfu/pyrf/ts_tensor_xyz.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
+import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
@@ -27,18 +28,23 @@
     Returns
     -------
     out : xarray.DataArray
         2nd order tensor time series.
 
     """
 
+    # Check input type
+    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
+    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
+
+    # Check input shape must be (n, 3, 3)
     assert data.ndim == 3 and data.shape[1:] == (3, 3)
     assert len(time) == len(data), "Time and data must have the same length"
 
-    if attrs is None:
+    if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
     out = xr.DataArray(
         data,
         coords=[time[:], ["x", "y", "z"], ["x", "y", "z"]],
         dims=["time", "comp_h", "comp_v"],
         attrs=attrs,
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ts_time.py` & `pyrfu-2.4.4/pyrfu/pyrf/ts_time.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ts_vec_xyz.py` & `pyrfu-2.4.4/pyrfu/pyrf/ts_vec_xyz.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
+import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
@@ -27,18 +28,23 @@
     Returns
     -------
     out : xarray.DataArray
         1st order tensor time series.
 
     """
 
+    # Check input type
+    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
+    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
+
+    # Check input shape must be (n, 3)
     assert data.ndim == 2 and data.shape[1] == 3
     assert len(time) == len(data), "Time and data must have the same length"
 
-    if attrs is None:
+    if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
     out = xr.DataArray(
         data,
         coords=[time[:], ["x", "y", "z"]],
         dims=["time", "comp"],
         attrs=attrs,
```

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/ttns2datetime64.py` & `pyrfu-2.4.4/pyrfu/pyrf/ttns2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/unix2datetime64.py` & `pyrfu-2.4.4/pyrfu/pyrf/unix2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/vht.py` & `pyrfu-2.4.4/pyrfu/pyrf/vht.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/wave_fft.py` & `pyrfu-2.4.4/pyrfu/pyrf/wave_fft.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/wavelet.py` & `pyrfu-2.4.4/pyrfu/pyrf/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/wavepolarize_means.py` & `pyrfu-2.4.4/pyrfu/pyrf/wavepolarize_means.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/pyrf/waverage.py` & `pyrfu-2.4.4/pyrfu/pyrf/waverage.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/solo/db_init.py` & `pyrfu-2.4.4/pyrfu/solo/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/solo/read_lfr_density.py` & `pyrfu-2.4.4/pyrfu/solo/read_lfr_density.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu/solo/read_tnr.py` & `pyrfu-2.4.4/pyrfu/solo/read_tnr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.3/pyrfu.egg-info/PKG-INFO` & `pyrfu-2.4.4/pyrfu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -211,15 +211,14 @@
 - `matplotlib <https://matplotlib.org>`_ >=3.5.2
 - `numba <http://numba.pydata.org>`_ >=0.54.1
 - `numpy <https://www.numpy.org>`_ >=1.20.3
 - `pandas <https://pandas.pydata.org/>`_ >=1.3.4
 - `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
 - `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
 - `scipy <https://scipy.org>`_ >=1.7.3
-- `Sphinx <https://www.sphinx-doc.org/en/master/>`_ >=4.3.0
 - `tqdm <https://tqdm.github.io/>`_ >=4.62.3
 - `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
 
 
 Testing dependencies are:
 
 - `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
```

### Comparing `pyrfu-2.4.3/venv/bin/activate_this.py` & `pyrfu-2.4.4/venv/bin/activate_this.py`

 * *Files identical despite different names*

