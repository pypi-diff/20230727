# Comparing `tmp/rad-0.16.0.tar.gz` & `tmp/rad-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.16.0.tar", last modified: Tue Jun 27 14:59:48 2023, max compression
+gzip compressed data, was "rad-0.17.0.tar", last modified: Thu Jul 27 20:01:18 2023, max compression
```

## Comparing `rad-0.16.0.tar` & `rad-0.17.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 14:59:35.000000 rad-0.16.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 14:59:35.000000 rad-0.16.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 14:59:35.000000 rad-0.16.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-27 14:59:35.000000 rad-0.16.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-27 14:59:35.000000 rad-0.16.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 14:59:35.000000 rad-0.16.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-06-27 14:59:35.000000 rad-0.16.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-27 14:59:35.000000 rad-0.16.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 14:59:35.000000 rad-0.16.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-27 14:59:35.000000 rad-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-27 14:59:48.357072 rad-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-27 14:59:35.000000 rad-0.16.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-27 14:59:35.000000 rad-0.16.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.337072 rad-0.16.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 14:59:35.000000 rad-0.16.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-27 14:59:35.000000 rad-0.16.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 14:59:35.000000 rad-0.16.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 14:59:35.000000 rad-0.16.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-27 14:59:35.000000 rad-0.16.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 14:59:35.000000 rad-0.16.0/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 14:59:35.000000 rad-0.16.0/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 14:59:35.000000 rad-0.16.0/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-27 14:59:35.000000 rad-0.16.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-27 14:59:35.000000 rad-0.16.0/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-06-27 14:59:35.000000 rad-0.16.0/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:59:48.361072 rad-0.16.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/src/rad/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.349072 rad-0.16.0/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.349072 rad-0.16.0/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.353072 rad-0.16.0/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/variance-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 14:59:35.000000 rad-0.16.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-27 14:59:35.000000 rad-0.16.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.949386 rad-0.17.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 20:01:09.000000 rad-0.17.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 20:01:09.000000 rad-0.17.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 20:01:09.000000 rad-0.17.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-27 20:01:09.000000 rad-0.17.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-27 20:01:09.000000 rad-0.17.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-27 20:01:09.000000 rad-0.17.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-27 20:01:09.000000 rad-0.17.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-27 20:01:09.000000 rad-0.17.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 20:01:09.000000 rad-0.17.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-27 20:01:09.000000 rad-0.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-27 20:01:18.945386 rad-0.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 20:01:09.000000 rad-0.17.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-27 20:01:09.000000 rad-0.17.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 20:01:09.000000 rad-0.17.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-07-27 20:01:09.000000 rad-0.17.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-27 20:01:09.000000 rad-0.17.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 20:01:09.000000 rad-0.17.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-27 20:01:09.000000 rad-0.17.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 20:01:09.000000 rad-0.17.0/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 20:01:09.000000 rad-0.17.0/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 20:01:09.000000 rad-0.17.0/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 20:01:09.000000 rad-0.17.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-07-27 20:01:09.000000 rad-0.17.0/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-07-27 20:01:09.000000 rad-0.17.0/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:01:18.949386 rad-0.17.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.941386 rad-0.17.0/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/variance-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 20:01:09.000000 rad-0.17.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 20:01:09.000000 rad-0.17.0/tox.ini
```

### Comparing `rad-0.16.0/.github/pull_request_template.md` & `rad-0.17.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/.github/workflows/changelog.yml` & `rad-0.17.0/.github/workflows/changelog.yml`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 jobs:
   changelog:
     name: Confirm changelog entry
     runs-on: ubuntu-latest
     steps:
     - name: Check change log entry
-      uses: pllim/action-check_astropy_changelog@main
+      uses: scientific-python/action-check-changelogfile@6087eddce1d684b0132be651a4dad97699513113  # 0.2
       env:
         CHANGELOG_FILENAME: CHANGES.rst
         CHECK_MILESTONE: false
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `rad-0.16.0/.github/workflows/ci.yml` & `rad-0.17.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/.github/workflows/publish-to-pypi.yml` & `rad-0.17.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/.github/workflows/release.yml` & `rad-0.17.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/.gitignore` & `rad-0.17.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/.pre-commit-config.yaml` & `rad-0.17.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -30,32 +30,32 @@
   hooks:
     - id: codespell
       args: ["--write-changes"]
       additional_dependencies:
         - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: 'v3.7.0'
+  rev: 'v3.9.0'
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.272'
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: 'v0.0.280'
   hooks:
     - id: ruff
       args: ["--fix"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/bandit
   rev: 1.7.5
   hooks:
     - id: bandit
```

### Comparing `rad-0.16.0/CHANGES.rst` & `rad-0.17.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+0.18.0 (unreleased)
+-------------------
+
+-
+
+0.17.0 (2023-07-27)
+-------------------
+
+- Fix invalid uri fragment in rad_schema. [#286]
+
+- Update the steps listed in ``cal_step`` to reflect the currently implemented steps.
+  The new additions are ``outlier_detection``, ``refpix``, ``sky_match``, and ``tweak_reg``. [#282]
+
+- Update the steps listed in ``cal_step`` with the ``resample`` step. [#295]
+
+- Fix the URIs for ``inverselinearity`` and add consistency checks for names/uris. [#296]
+
 0.16.0 (2023-06-26)
 -------------------
 
 - Fix minor discrepancies found when looking over the schemas. [#267]
 
 - Bugfix for ``inverse_linearity-1.0.0``'s ``reftype`` so that it is CRDS
   compatible. [#272]
```

### Comparing `rad-0.16.0/CODE_OF_CONDUCT.md` & `rad-0.17.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/LICENSE` & `rad-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/Makefile` & `rad-0.17.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/_static/custom.css` & `rad-0.17.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/_static/stsci_logo.png` & `rad-0.17.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/conf.py` & `rad-0.17.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/index.rst` & `rad-0.17.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/make.bat` & `rad-0.17.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/docs/schemas.rst` & `rad-0.17.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/pyproject.toml` & `rad-0.17.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/scripts/insert_next_release.py` & `rad-0.17.0/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/scripts/set_release_date.py` & `rad-0.17.0/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/integration.py` & `rad-0.17.0/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.17.0/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -142,16 +142,16 @@
   description: |-
     Flat field information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/gain-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/gain-1.0.0
   title: Gain reference schema
   description: |-
     Gain reference schema
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/inverse_linearity-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverse_linearity-1.0.0
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/inverselinearity-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverselinearity-1.0.0
   title: Inverse linearity correction reference schema
   description: |-
     Inverse linearity correction reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/ipc-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ipc-1.0.0
   title: IPC kernel reference schema
   description: |-
```

### Comparing `rad-0.16.0/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         additionalProperties:
           $ref: "#"
       dependencies:
         type: object
         additionalProperties:
           anyOf:
             - $ref: "#"
-            - $ref: "http://json-schema.org/draft-04/schema#definitions/stringArray"
+            - $ref: "http://json-schema.org/draft-04/schema#/definitions/stringArray"
       allOf:
         $ref: "#/definitions/schemaArray"
       anyOf:
         $ref: "#/definitions/schemaArray"
       oneOf:
         $ref: "#/definitions/schemaArray"
       not:
```

### Comparing `rad-0.16.0/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverse_linearity-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverselinearity-1.0.0
 
 title: Inverse linearity correction reference schema
 
-datamodel_name: InverseLinearityRefModel
+datamodel_name: InverselinearityRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
```

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/variance-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/variance-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.17.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.16.0/src/rad.egg-info/SOURCES.txt` & `rad-0.17.0/src/rad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
 src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
 src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
 src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
 src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
 src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
 src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
-src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
+src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
 src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
 src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
 src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
 src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
```

### Comparing `rad-0.16.0/tests/test_integration.py` & `rad-0.17.0/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,7 +25,17 @@
 
 @pytest.mark.parametrize("schema_path", (importlib_resources.files(resources) / "schemas").glob("**/*.yaml"))
 def test_schema_integration(schema_path):
     content = schema_path.read_bytes()
     schema = yaml.safe_load(content)
     asdf_content = asdf.get_config().resource_manager[schema["id"]]
     assert asdf_content == content
+
+
+@pytest.mark.parametrize("schema_path", (importlib_resources.files(resources) / "schemas").glob("**/*.yaml"))
+def test_schema_filename(schema_path):
+    """
+    Check the filename pattern aligns with the schema ID.
+    """
+    schema = yaml.safe_load(schema_path.read_bytes())
+    id_suffix = str(schema_path.with_suffix("")).split(str(importlib_resources.files(resources)))[-1]
+    assert schema["id"].endswith(id_suffix)
```

### Comparing `rad-0.16.0/tests/test_manifest.py` & `rad-0.17.0/tests/test_manifest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """
 Test that the manifest file is correctly structured and refers
 to schemas that exist.
 """
 import asdf
+import pytest
+
+from .conftest import MANIFEST
 
 
 def test_manifest_valid(manifest):
     schema = asdf.schema.load_schema("asdf://asdf-format.org/core/schemas/extension_manifest-1.0.0")
 
     asdf.schema.validate(manifest, schema=schema)
 
     assert "title" in manifest
     assert "description" in manifest
 
-    for tag in manifest["tags"]:
-        # Check that the schema exists:
-        assert tag["schema_uri"] in asdf.get_config().resource_manager
-        # These are not required by the manifest schema but we're holding ourselves
-        # to a higher standard:
-        assert "title" in tag
-        assert "description" in tag
-        assert tag["tag_uri"].startswith("asdf://stsci.edu/datamodels/roman/tags/")
+
+@pytest.mark.parametrize("entry", MANIFEST["tags"])
+def test_manifest_entries(entry):
+    # Check that the schema exists:
+    assert entry["schema_uri"] in asdf.get_config().resource_manager
+    # These are not required by the manifest schema but we're holding ourselves
+    # to a higher standard:
+    assert "title" in entry
+    assert "description" in entry
+
+    # Check the URIs
+    assert entry["tag_uri"].startswith("asdf://stsci.edu/datamodels/roman/tags/")
+    uri_suffix = entry["tag_uri"].split("asdf://stsci.edu/datamodels/roman/tags/")[-1]
+    assert entry["schema_uri"].endswith(uri_suffix)
+    assert entry["schema_uri"].startswith("asdf://stsci.edu/datamodels/roman/schemas/")
```

### Comparing `rad-0.16.0/tests/test_schemas.py` & `rad-0.17.0/tests/test_schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 
 
 @pytest.fixture(scope="session", params=REF_FILE_SCHEMA_URIS)
 def ref_file_schema(request):
     return yaml.safe_load(asdf.get_config().resource_manager[request.param])
 
 
+@pytest.fixture(scope="session", params=[entry for entry in MANIFEST["tags"] if "/reference_files/" in entry["schema_uri"]])
+def ref_file_uris(request):
+    return request.param["tag_uri"], request.param["schema_uri"]
+
+
 @pytest.fixture(scope="session")
 def valid_tag_uris(manifest):
     uris = {t["tag_uri"] for t in manifest["tags"]}
     uris.update(
         [
             "tag:stsci.edu:asdf/time/time-1.1.0",
             "tag:stsci.edu:asdf/core/ndarray-1.0.0",
@@ -135,14 +140,31 @@
     def callback(node):
         if isinstance(node, Mapping) and "tag" in node:
             assert node["tag"] in valid_tag_uris
 
     asdf.treeutil.walk(schema, callback)
 
 
+def _model_name_from_schema_uri(schema_uri):
+    schema_name = schema_uri.split("/")[-1].split("-")[0]
+    class_name = "".join([p.capitalize() for p in schema_name.split("_")])
+    if schema_uri.startswith("asdf://stsci.edu/datamodels/roman/schemas/reference_files/"):
+        class_name += "Ref"
+
+    if class_name.startswith("Wfi") and "Ref" not in class_name:
+        class_name = class_name.split("Wfi")[-1]
+
+    return f"{class_name}Model"
+
+
+def test_datamodel_name(schema):
+    if "datamodel_name" in schema:
+        assert _model_name_from_schema_uri(schema["id"]) == schema["datamodel_name"]
+
+
 # Confirm that the optical_element filter in wfi_img_photom.yml matches WFI_OPTICAL_ELEMENTS
 def test_matched_optical_element_entries():
     phot_table_keys = list(
         asdf.schema.load_schema("asdf://stsci.edu/datamodels/roman/schemas/reference_files/wfi_img_photom-1.0.0")["properties"][
             "phot_table"
         ]["patternProperties"]
     )
@@ -174,7 +196,21 @@
 
 def test_reftype(ref_file_schema):
     """
     Check that the reftype is valid for CRDS
     """
     reftype = _get_reftype(ref_file_schema)
     assert is_crds_name(f"roman_wfi_{reftype.lower()}_0000.asdf")
+
+
+def test_reftype_tag(ref_file_uris):
+    """
+    Check that the URIs match the reftype for a valid CRDS check
+    """
+    tag_uri = ref_file_uris[0]
+    schema_uri = ref_file_uris[1]
+
+    schema = yaml.safe_load(asdf.get_config().resource_manager[schema_uri])
+    reftype = _get_reftype(schema).lower()
+
+    assert asdf.util.uri_match(f"asdf://stsci.edu/datamodels/roman/tags/reference_files/*{reftype}-*", tag_uri)
+    assert asdf.util.uri_match(f"asdf://stsci.edu/datamodels/roman/schemas/reference_files/*{reftype}-*", schema_uri)
```

### Comparing `rad-0.16.0/tox.ini` & `rad-0.17.0/tox.ini`

 * *Files identical despite different names*

