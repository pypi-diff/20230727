# Comparing `tmp/rapthor-1.0.tar.gz` & `tmp/rapthor-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapthor-1.0.tar", last modified: Thu Jun  8 19:32:57 2023, max compression
+gzip compressed data, was "rapthor-1.1.tar", last modified: Thu Jul 27 13:01:40 2023, max compression
```

## Comparing `rapthor-1.0.tar` & `rapthor-1.1.tar`

### file list

```diff
@@ -1,125 +1,209 @@
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.230547 rapthor-1.0/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    18026 2023-06-08 12:43:15.000000 rapthor-1.0/LICENSE
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2400 2023-06-08 19:32:57.230547 rapthor-1.0/PKG-INFO
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1885 2023-06-08 12:43:15.000000 rapthor-1.0/README.md
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.222546 rapthor-1.0/bin/
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     1101 2023-06-08 12:43:15.000000 rapthor-1.0/bin/concat_linc_files
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)    42709 2023-06-08 12:43:15.000000 rapthor-1.0/bin/plotrapthor
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     2529 2023-06-08 19:28:33.000000 rapthor-1.0/bin/rapthor
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.222546 rapthor-1.0/rapthor/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       23 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2336 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/_logging.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      293 2023-06-08 19:19:18.000000 rapthor-1.0/rapthor/_version.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.222546 rapthor-1.0/rapthor/lib/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     8460 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/cluster.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1587 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/context.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2197 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/cwl.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    10605 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/cwlrunner.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     9147 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/facet.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    69090 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/field.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     8861 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/image.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    21189 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/miscellaneous.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    23643 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/observation.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     9059 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/operation.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    33862 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/parset.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    35000 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/screen.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    24758 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/sector.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     6507 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/lib/strategy.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4394 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/modifystate.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.222546 rapthor-1.0/rapthor/operations/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/operations/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    18322 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/operations/calibrate.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    19520 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/operations/image.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4959 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/operations/mosaic.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     7761 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/operations/predict.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.218546 rapthor-1.0/rapthor/pipeline/
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.226547 rapthor-1.0/rapthor/pipeline/execution/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      577 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/execution/concat_ms.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      685 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/execution/fetch_data.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2269 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/execution/hba_nl.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3189 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/execution/run_rapthor.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      558 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/execution/tar_directory.cwl
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.226547 rapthor-1.0/rapthor/pipeline/parsets/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    33119 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/calibrate_pipeline.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    14524 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/image_pipeline.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    17073 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/image_sector_pipeline.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2890 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/mosaic_pipeline.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3305 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/mosaic_type_pipeline.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     7249 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/parsets/predict_pipeline.cwl
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.230547 rapthor-1.0/rapthor/pipeline/steps/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1103 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/adjust_h5parm_sources.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2194 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/blank_image.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1013 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/collect_h5parms.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2571 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/combine_h5parms.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3852 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3579 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_debug.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3975 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_joint.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3953 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_separate.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3861 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_separate_no_joint.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3593 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_scalarcomplexgain.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     5965 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_scalarphase.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2659 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/filter_skymodel.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2105 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/make_aterm_images.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1315 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/make_mosaic.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1528 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/make_mosaic_template.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1666 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/make_region_file.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      602 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/merge_array_directories.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      562 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/merge_array_files.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      739 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/plot_solutions.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3284 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/predict_model_data.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2063 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/predict_model_data_phase_only.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2667 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2412 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data_no_screens.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2366 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data_no_screens_phase_only.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2397 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/process_slow_gains.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1462 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/regrid_image.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1112 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/split_h5parms.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3660 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/subtract_sector_models.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      386 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/writable_dir.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4570 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_image_facets.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3443 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_image_no_dde.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     7384 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_image_screens.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4723 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_facets.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3791 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_no_dde.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     5260 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_screens.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1294 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/pipeline/steps/wsclean_restore.cwl
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4060 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/process.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.230547 rapthor-1.0/rapthor/scripts/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/__init__.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3409 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/adjust_h5parm_sources.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     4575 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/blank_image.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)    23267 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/combine_h5parms.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     4125 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/concat_ms.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)    21432 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/filter_skymodel.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     6006 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/make_aterm_images.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     2567 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/make_mosaic.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3936 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/make_mosaic_template.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3118 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/make_region_file.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)      102 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/mpi_runner.sh
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     4533 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/plot_rapthor_timing.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)    18242 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/process_slow_gains.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3261 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/regrid_image.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)     6162 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/split_h5parms.py
--rwxrwxr-x   0 marcel    (1000) marcel    (1000)    33453 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/scripts/subtract_sector_models.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.230547 rapthor-1.0/rapthor/skymodels/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1006 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3C196-pandey.skymodel
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      364 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c147-SH.skymodel
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      364 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c286-SH.skymodel
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      349 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c287-SH.skymodel
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      412 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c295-twocomp.skymodel.deprecated
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      349 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c380-SH.skymodel
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      365 2023-06-08 12:43:15.000000 rapthor-1.0/rapthor/skymodels/3c48-SH.skymodel
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.222546 rapthor-1.0/rapthor.egg-info/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2400 2023-06-08 19:32:57.000000 rapthor-1.0/rapthor.egg-info/PKG-INFO
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4012 2023-06-08 19:32:57.000000 rapthor-1.0/rapthor.egg-info/SOURCES.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-06-08 19:32:57.000000 rapthor-1.0/rapthor.egg-info/dependency_links.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      124 2023-06-08 19:32:57.000000 rapthor-1.0/rapthor.egg-info/requires.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        8 2023-06-08 19:32:57.000000 rapthor-1.0/rapthor.egg-info/top_level.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       38 2023-06-08 19:32:57.230547 rapthor-1.0/setup.cfg
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     2654 2023-06-08 19:19:18.000000 rapthor-1.0/setup.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-06-08 19:32:57.230547 rapthor-1.0/test/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      594 2023-06-08 12:43:15.000000 rapthor-1.0/test/test_context.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     3133 2023-06-08 12:43:15.000000 rapthor-1.0/test/test_facet.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4054 2023-06-08 12:43:15.000000 rapthor-1.0/test/test_field.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1483 2023-06-08 12:43:15.000000 rapthor-1.0/test/test_screen.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.224700 rapthor-1.1/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       59 2023-07-27 07:28:46.000000 rapthor-1.1/.dockerignore
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2303 2023-07-27 07:28:46.000000 rapthor-1.1/.gitignore
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2098 2023-07-27 07:28:46.000000 rapthor-1.1/.gitlab-ci.yml
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      821 2023-07-27 07:28:46.000000 rapthor-1.1/.readthedocs.yaml
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.192700 rapthor-1.1/Docker/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     6483 2023-07-27 07:28:46.000000 rapthor-1.1/Docker/Dockerfile
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     7006 2023-07-27 10:18:21.000000 rapthor-1.1/Docker/Dockerfile.cuda
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      771 2023-07-27 07:28:46.000000 rapthor-1.1/Docker/build.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    35099 2023-07-27 07:28:46.000000 rapthor-1.1/LICENSE
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    44012 2023-07-27 13:01:40.224700 rapthor-1.1/PKG-INFO
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2653 2023-07-27 07:28:46.000000 rapthor-1.1/README.md
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.192700 rapthor-1.1/bin/
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     1493 2023-07-27 10:41:52.000000 rapthor-1.1/bin/concat_linc_files
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    42709 2023-07-27 07:28:46.000000 rapthor-1.1/bin/plotrapthor
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     1924 2023-07-27 07:28:46.000000 rapthor-1.1/bin/rapthor
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.196699 rapthor-1.1/ci/
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      553 2023-07-27 07:28:46.000000 rapthor-1.1/ci/debug.sh
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      120 2023-07-27 07:28:46.000000 rapthor-1.1/ci/run.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5711 2023-07-27 07:28:46.000000 rapthor-1.1/ci/ubuntu_20_04-base
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      208 2023-07-27 07:28:46.000000 rapthor-1.1/ci/ubuntu_20_04-rapthor
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.188699 rapthor-1.1/debug/
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.196699 rapthor-1.1/debug/everybeam/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      449 2023-07-27 07:28:46.000000 rapthor-1.1/debug/everybeam/Dockerfile
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)       32 2023-07-27 07:28:46.000000 rapthor-1.1/debug/everybeam/build.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      286 2023-07-27 07:28:46.000000 rapthor-1.1/debug/everybeam/fails.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      394 2023-07-27 07:28:46.000000 rapthor-1.1/debug/everybeam/run.sh
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.196699 rapthor-1.1/debug/scan_ms/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      482 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/Dockerfile
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)       32 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/build.sh
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      103 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/entry.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      116 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/fails.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      345 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/run.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      116 2023-07-27 07:28:46.000000 rapthor-1.1/debug/scan_ms/succeeds.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.196699 rapthor-1.1/docs/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      638 2023-07-27 07:28:46.000000 rapthor-1.1/docs/Makefile
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      799 2023-07-27 07:28:46.000000 rapthor-1.1/docs/make.bat
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       27 2023-07-27 07:28:46.000000 rapthor-1.1/docs/requirements.txt
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.200699 rapthor-1.1/docs/source/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      218 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/acknowledgements.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      797 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/capabilities.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1590 2023-07-27 12:59:15.000000 rapthor-1.1/docs/source/changelog.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      191 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/cluster_module.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3110 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/code.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2488 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/conf.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      158 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/context_module.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      232 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/field_class.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      215 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/future.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      183 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/help.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      625 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/index.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2542 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/installation.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      189 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/miscellaneous_module.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      202 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/observation_class.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1006 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/operation_class.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     8359 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/operations.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    18659 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/parset.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      165 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/parset_module.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2119 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/preparation.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1142 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/products.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)   489811 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/rapthor_flow.png
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5550 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/running.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      158 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/sector_class.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      595 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/steps.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5517 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/strategy.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      651 2023-07-27 10:41:52.000000 rapthor-1.1/docs/source/structure.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2552 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/tips.rst
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       36 2023-07-27 07:28:46.000000 rapthor-1.1/docs/source/tutorials.rst
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.204700 rapthor-1.1/examples/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2544 2023-07-27 07:28:46.000000 rapthor-1.1/examples/custom_calibration_strategy.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4026 2023-07-27 07:28:46.000000 rapthor-1.1/examples/default_calibration_strategy.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      224 2023-07-27 07:28:46.000000 rapthor-1.1/examples/full_parset.sh
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      866 2023-07-27 07:28:46.000000 rapthor-1.1/examples/ini2json.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    10346 2023-07-27 10:41:52.000000 rapthor-1.1/examples/rapthor.parset
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2611 2023-07-27 07:28:46.000000 rapthor-1.1/pyproject.toml
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.204700 rapthor-1.1/rapthor/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       23 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2801 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/_logging.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      155 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor/_version.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.208700 rapthor-1.1/rapthor/lib/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     8460 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/cluster.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1587 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/context.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2197 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/cwl.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    10978 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/lib/cwlrunner.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     9147 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/facet.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    70118 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/lib/field.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     9146 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/fitsimage.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    25349 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/miscellaneous.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    23644 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/lib/observation.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     9051 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/lib/operation.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    35312 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/lib/parset.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    35000 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/screen.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    24981 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/lib/sector.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     6507 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/lib/strategy.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4411 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/modifystate.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.208700 rapthor-1.1/rapthor/operations/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/operations/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    18436 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/operations/calibrate.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    20548 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/operations/image.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4960 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/operations/mosaic.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     7876 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/operations/predict.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.188699 rapthor-1.1/rapthor/pipeline/
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.208700 rapthor-1.1/rapthor/pipeline/execution/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      577 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/concat_ms.cwl
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.188699 rapthor-1.1/rapthor/pipeline/execution/examples/
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.208700 rapthor-1.1/rapthor/pipeline/execution/examples/hba_nl/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      465 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/examples/hba_nl/L667526.config.json
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1066 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/examples/hba_nl/hba_nl.json
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      324 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/examples/hba_nl/hba_nl.sh
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      685 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/fetch_data.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2269 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/hba_nl.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3189 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/run_rapthor.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      558 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/tar_directory.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      846 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/execution/utils.js
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.212700 rapthor-1.1/rapthor/pipeline/parsets/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    33403 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/calibrate_pipeline.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    15257 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/image_pipeline.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    19028 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/image_sector_pipeline.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2890 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/mosaic_pipeline.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3305 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/mosaic_type_pipeline.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     7410 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/parsets/predict_pipeline.cwl
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.216700 rapthor-1.1/rapthor/pipeline/steps/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1103 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/adjust_h5parm_sources.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2194 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/blank_image.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2481 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/calculate_image_diagnostics.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1013 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/collect_h5parms.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2571 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/combine_h5parms.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1196 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/concat_ms_files_in_time.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4014 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3579 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_debug.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4137 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_joint.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4115 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_separate.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4023 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_separate_no_joint.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3755 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_scalarcomplexgain.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     6222 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_scalarphase.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3753 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/filter_skymodel.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2102 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/make_aterm_images.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1315 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/make_mosaic.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1528 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/make_mosaic_template.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1666 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/make_region_file.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      602 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/merge_array_directories.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      562 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/merge_array_files.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      739 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/plot_solutions.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3478 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/predict_model_data.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2296 2023-07-27 10:18:21.000000 rapthor-1.1/rapthor/pipeline/steps/predict_model_data_phase_only.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2667 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2412 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data_no_screens.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2366 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data_no_screens_phase_only.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     2397 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/process_slow_gains.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1462 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/regrid_image.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1112 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/split_h5parms.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3660 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/subtract_sector_models.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      386 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/writable_dir.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4608 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_image_facets.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3527 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_image_no_dde.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     7419 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_image_screens.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4761 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_facets.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3875 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_no_dde.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5298 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_screens.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1294 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/pipeline/steps/wsclean_restore.cwl
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4460 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/process.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.220700 rapthor-1.1/rapthor/scripts/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/__init__.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3409 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/adjust_h5parm_sources.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     4575 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/blank_image.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    11367 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/calculate_image_diagnostics.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    23267 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/combine_h5parms.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     7298 2023-07-27 10:41:52.000000 rapthor-1.1/rapthor/scripts/concat_ms.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    13813 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/filter_skymodel.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     6006 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/make_aterm_images.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     2567 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/make_mosaic.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3940 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/make_mosaic_template.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3118 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/make_region_file.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)      102 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/mpi_runner.sh
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    11069 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/plot_rapthor_timing.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    18242 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/process_slow_gains.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     3265 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/regrid_image.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)     6162 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/split_h5parms.py
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    33453 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/scripts/subtract_sector_models.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.220700 rapthor-1.1/rapthor/skymodels/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1006 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3C196-pandey.skymodel
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      364 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c147-SH.skymodel
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      364 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c286-SH.skymodel
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      349 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c287-SH.skymodel
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      412 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c295-twocomp.skymodel.deprecated
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      349 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c380-SH.skymodel
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      365 2023-07-27 07:28:46.000000 rapthor-1.1/rapthor/skymodels/3c48-SH.skymodel
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.204700 rapthor-1.1/rapthor.egg-info/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    44012 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor.egg-info/PKG-INFO
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5990 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      165 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor.egg-info/requires.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        8 2023-07-27 13:01:40.000000 rapthor-1.1/rapthor.egg-info/top_level.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      184 2023-07-27 07:28:46.000000 rapthor-1.1/requirements.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      100 2023-07-27 13:01:40.224700 rapthor-1.1/setup.cfg
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.220700 rapthor-1.1/test/
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.224700 rapthor-1.1/test/resources/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)   149824 2023-07-27 08:50:33.000000 rapthor-1.1/test/resources/calibration_skymodel.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      865 2023-07-27 08:50:33.000000 rapthor-1.1/test/resources/test.parset
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)   253045 2023-07-27 08:50:33.000000 rapthor-1.1/test/resources/test_apparent_sky.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)   250730 2023-07-27 08:50:33.000000 rapthor-1.1/test/resources/test_true_sky.txt
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2023-07-27 13:01:40.224700 rapthor-1.1/test/scripts/
+-rwxrwxr-x   0 marcel    (1000) marcel    (1000)    15967 2023-07-27 08:50:33.000000 rapthor-1.1/test/scripts/compare_workflow_results.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      600 2023-07-27 08:50:33.000000 rapthor-1.1/test/test_context.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3133 2023-07-27 08:50:33.000000 rapthor-1.1/test/test_facet.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     3977 2023-07-27 08:50:33.000000 rapthor-1.1/test/test_field.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4344 2023-07-27 10:17:47.000000 rapthor-1.1/test/test_parset.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1483 2023-07-27 08:50:33.000000 rapthor-1.1/test/test_screen.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      104 2023-07-27 07:28:46.000000 rapthor-1.1/tox.ini
```

### Comparing `rapthor-1.0/PKG-INFO` & `rapthor-1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-Metadata-Version: 2.1
-Name: rapthor
-Version: 1.0
-Summary: Rapthor: LOFAR DDE Pipeline
-Home-page: https://git.astron.nl/RD/rapthor
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Rapthor: LOFAR DDE Pipeline
-===========================
+# Rapthor: LOFAR DDE Pipeline
 
 Rapthor is an experimental pipeline for correcting direction-dependent effects in LOFAR data. It uses DPPP and WSClean to derive and apply the corrections in facets or as smooth 2-D screens. It uses [CWL](https://www.commonwl.org) for the pipeline language and [Toil](http://toil.ucsc-cgl.org) to run the pipelines.
 
 ## Documentation
 
 Extensive documentation can be found on [Read the Docs](https://rapthor.readthedocs.io/en/latest/).
 
 
-Installation
-------------
+## Installation
 
 To install rapthor, follow the instructions below.
 
 
 ### Dependencies
 
 Rapthor requires the following packages (beyond those installed automatically with rapthor):
@@ -38,29 +20,47 @@
 * [DP3](https://git.astron.nl/RD/DP3) (version v4.1 or later; building with [Dysco](https://github.com/aroffringa/dysco) and [EveryBeam](https://git.astron.nl/RD/EveryBeam) is required)
 * [LSMTool](https://git.astron.nl/RD/LSMTool) (version 1.4.2 or later)
 * [LoSoTo](https://github.com/revoltek/losoto) (version 2.0 or later)
 * [PyBDSF](https://github.com/lofar-astron/PyBDSF) (version 1.9.2 or later)
 
 ### Downloading and Installing
 
-Get the latest developer version by cloning the git repository:
+Installation can be done in a number of ways. In order of preference (read:
+ease of use):
 
-    git clone https://git.astron.nl/RD/rapthor.git
+1. Install the latest release from PyPI:
+
+    ```
+    pip install rapthor
+    ```
+
+2. Install directly from the Rapthor git repository. This option is useful if you want to use one or more features that have not yet been released:
 
-Then install with:
+    ```
+    pip install --upgrade pip
+    pip install git+https://git.astron.nl/RD/rapthor.git[@<branch|tag|hash>]
+    ```
+    If the optional `@<branch|tag|hash>` is omitted, `HEAD` of the `master` branch will used.
 
+3. Clone the git repository, and install from your working copy. This option is mostly used by developers who want to make local changes:
+
+    ```
+    pip install --upgrade pip
+    git clone https://git.astron.nl/RD/rapthor.git
     cd rapthor
+    git checkout [<branch|tag|hash>]  #optionally
     pip install .
+    ```
+
+#### Note
 
-Or, alternatively, in one go:
+When installing Rapthor from source (options 2 and 3), you will need `pip` version 23 or later. That is why you need to upgrade to the latest version of `pip` *before* you install from source.
 
-    pip install git+https://git.astron.nl/RD/rapthor.git
 
-Usage
------
+## Usage
 
 The `rapthor` executable can be used from the command line with
 a parset that defines the parameters of the run. E.g.:
 
     $ rapthor rapthor.parset
 
 The parset defines the input and working directories, various options, etc. For details,
```

### Comparing `rapthor-1.0/bin/concat_linc_files` & `rapthor-1.1/bin/concat_linc_files`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 import argparse
 import glob
 import os
 import sys
 from rapthor.scripts.concat_ms import concat_ms
 
 
-def main(input_path, output_file):
+def main(input_path, output_file, overwrite=False):
     """
     Concatenate MS files from Linc for input to Rapthor
 
     Parameters
     ----------
     input_path : str
         Full path to the directory with the Linc MS files
     output_file : str
         Filename of output file
+    overwrite : bool, optional
+        If True and output_file points to an existing file, the file is
+        overwritten
     """
     msfiles = []
     for pattern in ["*.ms", "*.MS"]:
         msfiles.extend(glob.glob(os.path.join(input_path, pattern)))
-    return concat_ms(msfiles, output_file)
+    return concat_ms(msfiles, output_file, overwrite=overwrite)
 
 
 if __name__ == "__main__":
     descriptiontext = "Concatenate Linc MS files.\n"
     parser = argparse.ArgumentParser(
         description=descriptiontext, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument(
         "input_path", help="Full path to the directory with the Linc MS files"
     )
     parser.add_argument("output_file", help="Output filename")
+    parser.add_argument('--overwrite', help='Overwrite existing output file', type=bool,
+                        default=False)
 
     args = parser.parse_args()
-    sys.exit(main(args.input_path, args.output_file))
+    try:
+        sys.exit(main(args.input_path, args.output_file, overwrite=args.overwrite))
+    except Exception as e:
+        print('Error: {}'.format(e))
```

### Comparing `rapthor-1.0/bin/plotrapthor` & `rapthor-1.1/bin/plotrapthor`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/bin/rapthor` & `rapthor-1.1/bin/rapthor`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 from rapthor._version import __version__ as version
 from rapthor import process, modifystate
-from rapthor.lib.parset import parset_read
 import logging
 import optparse
 import sys
 
 
 if __name__ == '__main__':
     parser = optparse.OptionParser(usage='%prog <parset>',
@@ -45,25 +44,12 @@
         logging_level = 'info'
 
     if options.r:
         # Run state modification tool
         modifystate.run(parset_file)
     else:
         try:
-            parset = parset_read(parset_file, use_log_file=False)
-        except KeyError as e:
-            log = logging.getLogger('rapthor:parset')
-            log.critical('The parset is missing the required parameter %s', e)
-            sys.exit(-1)
-        except Exception as e:
-            log = logging.getLogger('rapthor:parset')
-            log.critical('Failed to parse parset:\n%s', e)
-            sys.exit(-1)
-        try:
             # Run the processing
             process.run(parset_file, logging_level=logging_level)
         except Exception as e:
             log = logging.getLogger('rapthor')
-            if parset['cluster_specific']['debug_workflow']:
-                log.exception(str(e))
-            else:
-                log.critical(str(e))
+            log.critical(e)
```

### Comparing `rapthor-1.0/rapthor/_logging.py` & `rapthor-1.1/rapthor/_logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,32 @@
 
 def add_coloring_to_emit_ansi(fn):
     """
     Colorize the logging output
     """
     def new(*args):
         levelno = args[0].levelno
-        if(levelno >= 50):
+        if (levelno >= 50):
             color = '\x1b[31m'  # red
-        elif(levelno >= 40):
+        elif (levelno >= 40):
             color = '\x1b[31m'  # red
-        elif(levelno >= 30):
+        elif (levelno >= 30):
             color = '\x1b[33m'  # yellow
-        elif(levelno >= 20):
+        elif (levelno >= 20):
             color = '\x1b[32m'  # green
-        elif(levelno >= 10):
+        elif (levelno >= 10):
             color = '\x1b[35m'  # pink
         else:
             color = '\x1b[0m'   # normal
+        if isinstance(args[0].msg, Exception):
+            # For exceptions, add the class name (e.g., "KeyError") to the
+            # logged message. Also strip single quotes from the error message
+            # to avoid things like: "KeyError: 'missing_key'"
+            args[0].msg = "{0}: {1}".format(args[0].msg.__class__.__name__,
+                                            str(args[0].msg).strip("'"))
         args[0].msg = color + args[0].msg + '\x1b[0m'
         return fn(*args)
     return new
 
 
 def set_level(level):
     """
@@ -63,14 +69,15 @@
     """
     Define and add a file handler
     """
     fh = logging.FileHandler(log_file)
     fh.setLevel(logging.DEBUG)  # file always logs everything
     formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(name)s - %(message)s')
     fh.setFormatter(formatter)
+    fh.emit = add_coloring_to_emit_ansi(fh.emit)
     fh.addFilter(Whitelist())
     logging.root.addHandler(fh)
 
 
 # Define and add console handler (in color)
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)  # default log level
```

### Comparing `rapthor-1.0/rapthor/lib/cluster.py` & `rapthor-1.1/rapthor/lib/cluster.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/lib/context.py` & `rapthor-1.1/rapthor/lib/context.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/lib/cwl.py` & `rapthor-1.1/rapthor/lib/cwl.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/lib/cwlrunner.py` & `rapthor-1.1/rapthor/lib/cwlrunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,26 +152,28 @@
 
     def setup(self):
         """
         Prepare runner for running. Adds some additional preprations to base class.
         """
         super().setup()
         self.args.extend(['--batchSystem', self.operation.batch_system])
+        # Bypass the file store; it only has benefits when using object stores like S3
+        self.args.extend(['--bypass-file-store'])
         if self.operation.batch_system == 'slurm':
-            self.args.extend(['--bypass-file-store'])
             self.args.extend(['--disableCaching'])
             self.args.extend(['--defaultCores', str(self.operation.cpus_per_task)])
             self.args.extend(['--defaultMemory', self.operation.mem_per_node_gb])
 
             # When the slurm batch system is used, the use of --bypass-file-store
             # requires that --tmp-outdir-prefix points to a shared filesystem, so
             # here we set it to the output directory
             prefix = os.path.join(self.operation.pipeline_working_dir, self.command + '.')
             self.args.extend(['--tmp-outdir-prefix', prefix])
         self.args.extend(['--maxLocalJobs', str(self.operation.max_nodes)])
+        self.args.extend(['--maxJobs', str(self.operation.max_nodes)])
         self.args.extend(['--jobStore', self.operation.jobstore])
         if os.path.exists(self.operation.jobstore):
             self.args.extend(['--restart'])
         self.args.extend(['--writeLogs', self.operation.log_dir])
         self.args.extend(['--writeLogsFromAllJobs'])  # also keep logs of successful jobs
         self.args.extend(['--maxLogFileSize', '0'])  # disable truncation of log files
         if self.operation.scratch_dir is not None:
@@ -187,14 +189,18 @@
                 prefix = os.path.join(self.operation.scratch_dir, self.command + '.')
                 self.args.extend(['--tmp-outdir-prefix', prefix])
         if self.operation.coordination_dir is not None:
             self.args.extend(['--coordinationDir', self.operation.coordination_dir])
         self.args.extend(['--clean', 'never'])  # preserves the job store for future runs
         self.args.extend(['--servicePollingInterval', '10'])
         if self.operation.debug_workflow:
+            if self.operation.batch_system != 'single_machine':
+                raise ValueError(
+                    'The debug_workflow option can only be used when batch_system = "single_machine".'
+                )
             self.args.extend(['--cleanWorkDir', 'never'])
             self.args.extend(['--debugWorker'])  # NOTE: stdout/stderr are not redirected to the log
             self.args.extend(['--logDebug'])
         os.environ.update(self.toil_env_variables)
 
     def teardown(self):
         """
```

### Comparing `rapthor-1.0/rapthor/lib/facet.py` & `rapthor-1.1/rapthor/lib/facet.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/lib/field.py` & `rapthor-1.1/rapthor/lib/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Definition of the Field class
 """
 import os
-import sys
 import logging
 import numpy as np
 import lsmtool
 import lsmtool.skymodel
 from rapthor.lib import miscellaneous as misc
 from rapthor.lib.observation import Observation
 from rapthor.lib.sector import Sector
 from shapely.geometry import Point, Polygon, MultiPolygon
 from astropy.table import vstack
 import rtree.index
 import glob
+from astropy.coordinates import SkyCoord
+import astropy.units as u
 
 
 class Field(object):
     """
     The Field object stores parameters needed for processing of the field
 
     Parameters
@@ -58,14 +59,15 @@
         if self.dde_method == 'screens':
             self.use_screens = True
         else:
             self.use_screens = False
         self.screen_type = self.parset['imaging_specific']['screen_type']
         self.use_mpi = self.parset['imaging_specific']['use_mpi']
         self.parallelbaselines = self.parset['calibration_specific']['parallelbaselines']
+        self.sagecalpredict= self.parset['calibration_specific']['sagecalpredict']
         self.reweight = self.parset['imaging_specific']['reweight']
         self.do_multiscale_clean = self.parset['imaging_specific']['do_multiscale_clean']
         self.apply_diagonal_solutions = self.parset['imaging_specific']['apply_diagonal_solutions']
         self.solverlbfgs_dof = self.parset['calibration_specific']['solverlbfgs_dof']
         self.solverlbfgs_iter = self.parset['calibration_specific']['solverlbfgs_iter']
         self.solverlbfgs_minibatches = self.parset['calibration_specific']['solverlbfgs_minibatches']
 
@@ -188,15 +190,15 @@
         """
         Break observations into smaller time chunks if desired
 
         Chunking is done if:
 
         - the specified data_fraction < 1 (so part of an observation is to be processed)
         - nobs * nsectors < nnodes (so all nodes can be used efficiently. In particular,
-          the predict pipeline parallelizes over sectors and observations, so we need
+          the predict operation parallelizes over sectors and observations, so we need
           enough observations to allow all nodes to be occupied.)
 
         Parameters
         ----------
         data_fraction : float, optional
             Fraction of data to use during processing
         """
@@ -325,15 +327,15 @@
             Filename of input makesourcedb apparent-flux sky model file
         regroup : bool, optional
             If False, the calibration sky model is not regrouped to the target flux.
             Instead, the existing calibration groups are used
         find_sources : bool, optional
             If True, group the sky model by thresholding to find sources. This is not
             needed if the input sky model was filtered by PyBDSF in the imaging
-            pipeline
+            operation
         target_flux : float, optional
             Target flux in Jy for grouping
         target_number : int, optional
             Target number of patches for grouping
         index : index
             Iteration index
         """
@@ -347,40 +349,36 @@
         misc.create_directory(dst_dir)
         self.bright_source_skymodel_file = os.path.join(dst_dir, 'bright_source_skymodel.txt')
 
         # First check whether sky models already exist due to a previous run and attempt
         # to load them
         try:
             self.calibration_skymodel = lsmtool.load(str(self.calibration_skymodel_file))
-            self.num_patches = len(self.calibration_skymodel.getPatchNames())
-            calibrators_skymodel = lsmtool.load(str(self.calibrators_only_skymodel_file))
-            self.calibrator_patch_names = calibrators_skymodel.getPatchNames().tolist()
-            self.calibrator_fluxes = calibrators_skymodel.getColValues('I', aggregate='sum').tolist()
+            self.calibrators_only_skymodel = lsmtool.load(str(self.calibrators_only_skymodel_file))
             self.source_skymodel = lsmtool.load(str(self.source_skymodel_file))
 
             if self.peel_bright_sources:
                 # The bright-source model file may not exist if there are no bright sources,
-                # but also if a reset of the imaging pipeline was done. Unfortunately, there
+                # but also if a reset of the imaging operation was done. Unfortunately, there
                 # is no way to determine which of these two possibilities is the case. So, if
                 # it does not exist, we have to regenerate the sky models
                 if os.path.exists(self.bright_source_skymodel_file):
                     self.bright_source_skymodel = lsmtool.load(str(self.bright_source_skymodel_file))
                     all_skymodels_loaded = True
                 else:
                     all_skymodels_loaded = False
             else:
-                self.bright_source_skymodel = calibrators_skymodel
+                self.bright_source_skymodel = self.calibrators_only_skymodel
                 all_skymodels_loaded = True
         except IOError:
             all_skymodels_loaded = False
 
         if all_skymodels_loaded:
             # If all the required sky models were loaded from files, return; otherwise,
             # continue on to regenerate the sky models from scratch
-            self.log.info('Using {} calibration patches'.format(self.num_patches))
             return
 
         # If sky models do not already exist, make them
         self.log.info('Analyzing sky model...')
         if type(skymodel_true_sky) is not lsmtool.skymodel.SkyModel:
             skymodel_true_sky = lsmtool.load(str(skymodel_true_sky),
                                              beamMS=self.beam_ms_filename)
@@ -565,30 +563,27 @@
         source_names = bright_source_skymodel.getColValues('Name').tolist()
         bright_source_names = bright_source_skymodel_apparent_sky.getColValues('Name').tolist()
         matching_ind = []
         for i, sn in enumerate(bright_source_names):
             matching_ind.append(source_names.index(sn))
         bright_source_skymodel.select(np.array(matching_ind))
 
-        # Transfer patches to the bright-source model
+        # Transfer patches to the bright-source model. At this point, it is now the
+        # model of calibrator sources only, so copy and save it and write it out for
+        # later use
         if regroup:
             # Transfer from the apparent-flux sky model (regrouped above)
             self.transfer_patches(bright_source_skymodel_apparent_sky, bright_source_skymodel)
         else:
             # Transfer from the true-flux sky model
             patch_dict = skymodel_true_sky.getPatchPositions()
             self.transfer_patches(skymodel_true_sky, bright_source_skymodel,
                                   patch_dict=patch_dict)
-
-        # Save the bright-source (i.e., calibrator) flux densities (in Jy) for use
-        # in the calibration pipeline for weighting of the directions during screen
-        # fitting
         bright_source_skymodel.write(self.calibrators_only_skymodel_file, clobber=True)
-        self.calibrator_patch_names = bright_source_skymodel.getPatchNames().tolist()
-        self.calibrator_fluxes = bright_source_skymodel.getColValues('I', aggregate='sum').tolist()
+        self.calibrators_only_skymodel = bright_source_skymodel.copy()
 
         # Now remove any bright sources that lie outside the imaged area, as they
         # should not be peeled
         if len(self.imaging_sectors) > 0:
             for i, sector in enumerate(self.imaging_sectors):
                 sm = bright_source_skymodel.copy()
                 sm = sector.filter_skymodel(sm)
@@ -601,20 +596,14 @@
                         filtered_skymodel.concatenate(sm)
             bright_source_skymodel = filtered_skymodel
             if len(bright_source_skymodel) > 0:
                 bright_source_skymodel.setPatchPositions()
 
         # Write sky models to disk for use in calibration, etc.
         calibration_skymodel = skymodel_true_sky
-        self.num_patches = len(calibration_skymodel.getPatchNames())
-        if self.num_patches > 1:
-            infix = 'es'
-        else:
-            infix = ''
-        self.log.info('Using {0} calibration patch{1}'.format(self.num_patches, infix))
         calibration_skymodel.write(self.calibration_skymodel_file, clobber=True)
         self.calibration_skymodel = calibration_skymodel
         if len(bright_source_skymodel) > 0:
             bright_source_skymodel.write(self.bright_source_skymodel_file, clobber=True)
         self.bright_source_skymodel = bright_source_skymodel
 
     def update_skymodels(self, index, regroup, target_flux=None, target_number=None,
@@ -734,19 +723,28 @@
                 matching_radius_deg = 30.0 / 3600.0  # => 30 arcsec
                 skymodel_true_sky.concatenate(skymodel_true_sky_start, matchBy='position',
                                               radius=matching_radius_deg,
                                               keep='from1', inheritPatches=True)
                 skymodel_apparent_sky = None
 
             # Use concatenated sky models to make new calibration model (we set find_sources
-            # to False to preserve the source patches defined in the image pipeline by PyBDSF)
+            # to False to preserve the source patches defined in the image operation by PyBDSF)
             self.make_skymodels(skymodel_true_sky, skymodel_apparent_sky=skymodel_apparent_sky,
                                 regroup=regroup, find_sources=False, target_flux=target_flux,
                                 target_number=target_number, index=index)
 
+        # Save the number of calibrators and their names, positions, and flux
+        # densities (in Jy) for use in the calibration and imaging operations
+        self.calibrator_patch_names = self.calibrators_only_skymodel.getPatchNames().tolist()
+        self.calibrator_fluxes = self.calibrators_only_skymodel.getColValues('I', aggregate='sum').tolist()
+        self.calibrator_positions = self.calibrators_only_skymodel.getPatchPositions()
+        self.num_patches = len(self.calibrator_patch_names)
+        suffix = 'es' if self.num_patches > 1 else ''
+        self.log.info('Using {0} calibration patch{1}'.format(self.num_patches, suffix))
+
         # Adjust sector boundaries to avoid known sources and update their sky models.
         self.adjust_sector_boundaries()
         self.log.info('Making sector sky models (for predicting)...')
         for sector in self.imaging_sectors:
             sector.calibration_skymodel = self.calibration_skymodel.copy()
             sector.make_skymodel(index)
 
@@ -760,17 +758,21 @@
         # not imaged; they are only used in prediction and subtraction
         self.define_outlier_sectors(index)
 
         # Finally, make a list containing all sectors
         self.sectors = self.imaging_sectors + self.outlier_sectors + self.bright_source_sectors
         self.nsectors = len(self.sectors)
 
-        # Clean up to minimize memory usage
+    def remove_skymodels(self):
+        """
+        Remove sky models to minimize memory usage
+        """
         self.calibration_skymodel = None
         self.source_skymodel = None
+        self.calibrators_only_skymodel = None
         for sector in self.sectors:
             sector.calibration_skymodel = None
             sector.predict_skymodel = None
             sector.field.source_skymodel = None
 
     def transfer_patches(self, from_skymodel, to_skymodel, patch_dict=None):
         """
@@ -789,14 +791,18 @@
         -------
         to_skymodel : sky model
             Sky model with patches matching those of from_skymodel
         """
         names_from = from_skymodel.getColValues('Name').tolist()
         names_to = to_skymodel.getColValues('Name').tolist()
 
+        if 'Patch' not in to_skymodel.table.colnames:
+            self.log.debug('to_skymodel does not have Patch column, adding it')
+            to_skymodel.group('single')
+
         if set(names_from) == set(names_to):
             # Both sky models have the same sources, so use indexing
             ind_ss = np.argsort(names_from)
             ind_ts = np.argsort(names_to)
             to_skymodel.table['Patch'][ind_ts] = from_skymodel.table['Patch'][ind_ss]
             to_skymodel._updateGroups()
         elif set(names_to).issubset(set(names_from)):
@@ -809,14 +815,28 @@
             raise ValueError('Cannot transfer patches since from_skymodel does not contain '
                              'all the sources in to_skymodel')
 
         if patch_dict is not None:
             to_skymodel.setPatchPositions(patchDict=patch_dict)
         return to_skymodel
 
+    def get_calibration_radius(self):
+        """
+        Returns the radius in degrees that encloses all calibrators
+        """
+        phase_center_coord = SkyCoord(ra=self.ra*u.degree, dec=self.dec*u.degree)
+        cal_ra = []
+        cal_dec = []
+        for cal, coord in self.calibrator_positions.items():
+            cal_ra.append(coord[0])
+            cal_dec.append(coord[1])
+        cal_coord = SkyCoord(ra=cal_ra, dec=cal_dec)
+        separation = phase_center_coord.separation(cal_coord)
+        return max(separation).value
+
     def define_imaging_sectors(self):
         """
         Defines the imaging sectors
         """
         self.imaging_sectors = []
 
         # Determine whether we use a user-supplied list of sectors or a grid
@@ -904,15 +924,15 @@
                 self.log.info('Using 1 imaging sector')
             else:
                 self.log.info('Using {0} imaging sectors ({1} in RA, {2} in Dec)'.format(
                               len(self.imaging_sectors), nsectors_ra, nsectors_dec))
 
         # Compute bounding box for all imaging sectors and store as a
         # a semi-colon-separated list of [maxRA; minDec; minRA; maxDec] (we use semi-
-        # colons as otherwise the pipeline parset parser will split the list). Also
+        # colons as otherwise the workflow parset parser will split the list). Also
         # store the midpoint as [midRA; midDec]. These values are needed for the aterm
         # image generation, so we use the padded polygons to ensure that the final
         # bounding box encloses all of the images *with* padding included.
         # Note: this is just once, rather than each time the sector borders are
         # adjusted, so that the image sizes do not change with iteration (so
         # mask images from previous iterations may be used)
         all_sectors = MultiPolygon([sector.poly_padded for sector in self.imaging_sectors])
@@ -1214,21 +1234,21 @@
             return False, False
 
         # Get noise, dynamic range, and number of sources from previous and current
         # images of each sector
         converged = []
         diverged = []
         for sector in self.imaging_sectors:
-            rmspre = sector.diagnostics[-2]['median_rms']
-            rmspost = sector.diagnostics[-1]['median_rms']
-            self.log.info('Ratio of current median image noise to previous image '
+            rmspre = sector.diagnostics[-2]['median_rms_flat_noise']
+            rmspost = sector.diagnostics[-1]['median_rms_flat_noise']
+            self.log.info('Ratio of current median image noise (non-PB-corrected) to previous image '
                           'noise for {0} = {1:.2f}'.format(sector.name, rmspost/rmspre))
-            dynrpre = sector.diagnostics[-2]['dynamic_range_global']
-            dynrpost = sector.diagnostics[-1]['dynamic_range_global']
-            self.log.info('Ratio of current image dynamic range to previous image '
+            dynrpre = sector.diagnostics[-2]['dynamic_range_global_flat_noise']
+            dynrpost = sector.diagnostics[-1]['dynamic_range_global_flat_noise']
+            self.log.info('Ratio of current image dynamic range (non-PB-corrected) to previous image '
                           'dynamic range for {0} = {1:.2f}'.format(sector.name, dynrpost/dynrpre))
             nsrcpre = sector.diagnostics[-2]['nsources']
             nsrcpost = sector.diagnostics[-1]['nsources']
             self.log.info('Ratio of current number of sources to previous number '
                           'of sources for {0} = {1:.2f}'.format(sector.name, nsrcpost/nsrcpre))
             if (rmspost / rmspre < convergence_ratio or
                     dynrpost / dynrpre > 1 / convergence_ratio or
@@ -1276,15 +1296,15 @@
 
         # Update field and sector dicts with the parameters for this iteration
         self.__dict__.update(step_dict)
         for sector in self.imaging_sectors:
             sector.__dict__.update(step_dict)
 
         # Update the sky models. We adjust the target flux used for calibrator selection
-        # by the ratio of (LOFAR / true) fluxes determined in the image pipeline of the
+        # by the ratio of (LOFAR / true) fluxes determined in the image operation of the
         # previous selfcal cycle. This adjustment is only done if the fractional change
         # is significant (as measured by the standard deviation in the ratio)
         target_flux = step_dict['target_flux']
         if self.lofar_to_true_flux_ratio <= 0:
             self.lofar_to_true_flux_ratio = 1.0  # disable adjustment
         if self.lofar_to_true_flux_ratio <= 1:
             fractional_change = 1 / self.lofar_to_true_flux_ratio - 1
@@ -1296,14 +1316,15 @@
                           'from {0:.2f} Jy to {1:.2f} Jy to account for the offset found '
                           'in the global flux scale'.format(step_dict['target_flux'],
                                                             target_flux))
         self.update_skymodels(index, step_dict['regroup_model'],
                               target_flux=target_flux,
                               target_number=step_dict['max_directions'],
                               final=final)
+        self.remove_skymodels()  # clean up sky models to reduce memory usage
 
         # Check whether outliers and bright sources need to be peeled
         nr_outlier_sectors = len(self.outlier_sectors)
         nr_imaging_sectors = len(self.imaging_sectors)
         nr_bright_source_sectors = len(self.bright_source_sectors)
         if nr_bright_source_sectors == 0:
             self.peel_bright_sources = False
```

### Comparing `rapthor-1.0/rapthor/lib/image.py` & `rapthor-1.1/rapthor/lib/fitsimage.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,30 +45,30 @@
             for hist in self.header['HISTORY']:
                 if 'AIPS   CLEAN BMAJ' in hist:
                     # remove every letter from the string
                     bmaj, bmin, pa = re.sub(' +', ' ', re.sub('[A-Z ]*=', '', hist)).strip().split(' ')
                     self.header['BMAJ'] = float(bmaj)
                     self.header['BMIN'] = float(bmin)
                     self.header['BPA'] = float(pa)
-        self.beam = [self.header['BMAJ'], self.header['BMIN'], self.header['BPA']]
+        self.beam = [float(self.header['BMAJ']), float(self.header['BMIN']), float(self.header['BPA'])]
 
     def find_freq(self):
         """
         Find frequency value in most common places of a fits header
         """
         self.freq = None
         if not self.header.get('RESTFREQ') is None and not self.header.get('RESTFREQ') == 0:
-            self.freq = self.header.get('RESTFREQ')
+            self.freq = float(self.header.get('RESTFREQ'))
         elif not self.header.get('FREQ') is None and not self.header.get('FREQ') == 0:
-            self.freq = self.header.get('FREQ')
+            self.freq = float(self.header.get('FREQ'))
         else:
             for i in range(5):
                 type_s = self.header.get('CTYPE%i' % i)
                 if type_s is not None and type_s[0:4] == 'FREQ':
-                    self.freq = self.header.get('CRVAL%i' % i)
+                    self.freq = float(self.header.get('CRVAL%i' % i))
 
     def flatten(self):
         """ Flatten a fits file so that it becomes a 2D image. Return new header and data """
         f = pyfits.open(self.imagefile)
 
         naxis = f[0].header['NAXIS']
         if naxis < 2:
@@ -105,14 +105,18 @@
             for i in range(naxis, 0, -1):
                 if i <= 2:
                     dataslice.append(np.s_[:],)
                 else:
                     dataslice.append(0)
             self.img_hdr = header
             self.img_data = f[0].data[tuple(dataslice)]
+        self.min_value = float(np.nanmin(self.img_data))
+        self.max_value = float(np.nanmax(self.img_data))
+        self.mean_value = float(np.nanmean(self.img_data))
+        self.median_value = float(np.nanmedian(self.img_data))
 
     def write(self, filename=None):
         if filename is None:
             filename = self.imagefile
         pyfits.writeto(filename, self.img_data, self.img_hdr, overwrite=True)
 
     def get_beam(self):
@@ -164,15 +168,15 @@
             sampling = 1
         data = self.img_data[::sampling]  # sample array
         data = data[ np.isfinite(data) ]
         oldrms = 1.
         for i in range(niter):
             rms = np.nanstd(data)
             if np.abs(oldrms-rms)/rms < eps:
-                self.noise = rms
+                self.noise = float(rms)
                 logging.debug('%s: Noise: %.3f mJy/b' % (self.imagefile, self.noise*1e3))
                 return
 
             data = data[np.abs(data)<3*rms]
             oldrms = rms
         raise Exception('Noise estimation failed to converge.')
```

### Comparing `rapthor-1.0/rapthor/lib/miscellaneous.py` & `rapthor-1.1/rapthor/lib/miscellaneous.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,78 +13,92 @@
 from shapely.prepared import prep
 from astropy.io import fits as pyfits
 from PIL import Image, ImageDraw
 import multiprocessing
 from math import modf, floor, ceil
 from losoto.h5parm import h5parm
 import lsmtool
+import sys
+from scipy.interpolate import interp1d
+from rapthor.lib.observation import Observation
 
 
-def download_skymodel(ra, dec, skymodel_path, radius=5.0, overwrite=False, source='TGSS', targetname='Patch'):
+def download_skymodel(ra, dec, skymodel_path, radius=5.0, overwrite=False, source='TGSS',
+                      targetname='Patch'):
     """
     Download the skymodel for the target field
 
     Parameters
     ----------
     ra : float
         Right ascension of the skymodel centre.
     dec : float
         Declination of the skymodel centre.
     skymodel_path : str
         Full name (with path) to the skymodel.
-    radius : float
+    radius : float, optional
         Radius for the TGSS/GSM cone search in degrees.
-    source : str
+    source : str, optional
         Source where to obtain a skymodel from. Can be TGSS or GSM. Default is TGSS.
-    overwrite : bool
+    overwrite : bool, optional
         Overwrite the existing skymodel pointed to by skymodel_path.
-    target_name : str
+    target_name : str, optional
         Give the patch a certain name. Default is "Patch".
     """
-    SKY_SERVERS = {'TGSS': 'http://tgssadr.strw.leidenuniv.nl/cgi-bin/gsmv4.cgi?coord={ra:f},{dec:f}&radius={radius:f}&unit=deg&deconv=y',
-                   'GSM': 'https://lcs165.lofar.eu/cgi-bin/gsmv1.cgi?coord={ra:f},{dec:f}&radius={radius:f}&unit=deg&deconv=y'}
+    SKY_SERVERS = {'TGSS': 'http://tgssadr.strw.leidenuniv.nl/cgi-bin/gsmv4.cgi?'
+                           'coord={ra:f},{dec:f}&radius={radius:f}&unit=deg&deconv=y',
+                   'GSM': 'https://lcs165.lofar.eu/cgi-bin/gsmv1.cgi?'
+                          'coord={ra:f},{dec:f}&radius={radius:f}&unit=deg&deconv=y'}
     if source.upper() not in SKY_SERVERS.keys():
-        raise ValueError('Unsupported skymodel source specified! Please use TGSS or GSM.')
+        raise ValueError('Unsupported sky model source specified! Please use TGSS or GSM.')
 
     logger = logging.getLogger('rapthor:skymodel')
 
     file_exists = os.path.isfile(skymodel_path)
     if file_exists and not overwrite:
-        logger.warning('Skymodel "%s" exists and overwrite is set to False! Not downloading skymodel. If this is a restart this may be intentional.' % skymodel_path)
+        logger.warning('Sky model "{}" exists and overwrite is set to False! Not '
+                       'downloading sky model. If this is a restart this may be '
+                       'intentional.'.format(skymodel_path))
         return
 
-    if (not file_exists) and os.path.exists(skymodel_path):
-        logger.error('Path "%s" exists but is not a file!' % skymodel_path)
+    if not file_exists and os.path.exists(skymodel_path):
         raise ValueError('Path "%s" exists but is not a file!' % skymodel_path)
 
-    # Empty strings are False. Only attempt directory creation if there is a directory path involved.
-    if (not file_exists) and os.path.dirname(skymodel_path) and (not os.path.exists(os.path.dirname(skymodel_path))):
+    # Empty strings are False. Only attempt directory creation if there is a
+    # directory path involved.
+    if (not file_exists
+            and os.path.dirname(skymodel_path)
+            and not os.path.exists(os.path.dirname(skymodel_path))):
         os.makedirs(os.path.dirname(skymodel_path))
 
     if file_exists and overwrite:
-        logger.warning('Found existing skymodel "%s" and overwrite is True. Deleting existing skymodel!' % skymodel_path)
+        logger.warning('Found existing sky model "{}" and overwrite is True. Deleting '
+                       'existing sky model!'.format(skymodel_path))
         os.remove(skymodel_path)
 
     logger.info('Downloading skymodel for the target into ' + skymodel_path)
 
-    tries = 0
-    while tries < 5:
-        result = subprocess.run(['wget', '-O', skymodel_path, SKY_SERVERS[source].format(ra=ra, dec=dec, radius=radius)])
+    max_tries = 5
+    for tries in range(1, 1 + max_tries):
+        result = subprocess.run(['wget', '-O', skymodel_path,
+                                 SKY_SERVERS[source].format(ra=ra, dec=dec, radius=radius)])
         if result.returncode != 0:
-            logger.error('Attempt {t:d} download of skymodel failed. Attempting {t:d} more times.'.format(t=5-tries))
+            if tries == max_tries:
+                raise IOError('Download of sky model failed after {} '
+                              'attempts.'.format(max_tries))
+            else:
+                logger.error('Attempt #{0:d} to download sky model failed. Attempting '
+                             '{1:d} more times.'.format(tries, max_tries - tries))
+                time.sleep(5)
         else:
             break
-        time.sleep(5)
-        tries += 1
-        if tries == 5:
-            logger.critical('Download of skymodel failed after 5 attempts.')
 
     if not os.path.isfile(skymodel_path):
-        logger.critical('Skymodel "%s" does not exist after trying to download the skymodel.' % skymodel_path)
-        raise IOError('Skymodel "%s" does not exist after trying to download the skymodel.' % skymodel_path)
+        raise IOError('Sky model file "{}" does not exist after trying to download the '
+                      'sky model.'.format(skymodel_path))
 
     # Treat all sources as one group (direction)
     skymodel = lsmtool.load(skymodel_path)
     skymodel.group('single', root=targetname)
     skymodel.write(clobber=True)
 
 
@@ -164,31 +178,31 @@
     """
     Make a blank FITS image and save it to disk
 
     Parameters
     ----------
     image_name : str
         Filename of output image
-    reference_ra_deg : float, optional
+    reference_ra_deg : float
         RA for center of output mask image
-    reference_dec_deg : float, optional
+    reference_dec_deg : float
         Dec for center of output mask image
     imsize : int, optional
         Size of output image
     cellsize_deg : float, optional
         Size of a pixel in degrees
-    freqs : list
+    freqs : list, optional
         Frequencies to use to construct extra axes (for IDG a-term images)
-    times : list
+    times : list, optional
         Times to use to construct extra axes (for IDG a-term images)
-    antennas : list
+    antennas : list, optional
         Antennas to use to construct extra axes (for IDG a-term images)
-    aterm_type : str
+    aterm_type : str, optional
         One of 'tec' or 'gain'
-    fill_val : int
+    fill_val : int, optional
         Value with which to fill the data
     """
     if freqs is not None and times is not None and antennas is not None:
         nants = len(antennas)
         ntimes = len(times)
         nfreqs = len(freqs)
         if aterm_type == 'tec':
@@ -318,20 +332,20 @@
         Array with rasterized polygon
     """
     poly = Polygon(verts)
     prepared_polygon = prep(poly)
 
     # Mask everything outside of the polygon plus its border (outline) with zeros
     # (inside polygon plus border are ones)
-    mask = Image.new('L', (data.shape[0], data.shape[1]), 0)
+    mask = Image.new('L', (data.shape[1], data.shape[0]), 0)
     ImageDraw.Draw(mask).polygon(verts, outline=1, fill=1)
     data *= mask
 
     # Now check the border precisely
-    mask = Image.new('L', (data.shape[0], data.shape[1]), 0)
+    mask = Image.new('L', (data.shape[1], data.shape[0]), 0)
     ImageDraw.Draw(mask).polygon(verts, outline=1, fill=0)
     masked_ind = np.where(np.array(mask).transpose())
     points = [Point(xm, ym) for xm, ym in zip(masked_ind[0], masked_ind[1])]
     outside_points = [v for v in points if prepared_polygon.disjoint(v)]
     for outside_point in outside_points:
         data[int(outside_point.y), int(outside_point.x)] = 0
 
@@ -589,14 +603,111 @@
         try:
             soltab = solset.getSoltab(soltabname)
             soltab.delete()
         except Exception:
             print('Error: soltab "{}" could not be removed'.format(soltabname))
 
 
+def calc_theoretical_noise(mslist, w_factor=1.5):
+    """
+    Return the expected theoretical image noise for a dataset
+
+    Note: the calculations follow those of SKA Memo 113 (see
+    http://www.skatelescope.org/uploaded/59513_113_Memo_Nijboer.pdf) and
+    assume no tapering. International stations are not included.
+
+    Parameters
+    ----------
+    mslist : list of str
+        List of the filenames of the input MS files
+    w_factor : float, optional
+        Factor for increase of noise due to the weighting scheme used
+        in imaging (typically ranges from 1.3 - 2)
+
+    Returns
+    -------
+    noise, unflagged_fraction : tuple of floats
+        Estimate of the expected theoretical noise in Jy/beam and the
+        unflagged fraction of the input data
+    """
+    nobs = len(mslist)
+    if nobs == 0:
+        # If no MS files, just return zero for the noise as we cannot
+        # estimate it
+        return 0.0
+
+    # Find the total time and the average total bandwidth, average frequency,
+    # average unflagged fraction, and average number of core and remote stations
+    # (for the averages, assume each observation has equal weight)
+    total_time = 0
+    total_bandwidth = 0
+    ncore = 0
+    nremote = 0
+    mid_freq = 0
+    unflagged_fraction = 0
+    for ms in mslist:
+        obs = Observation(ms)
+        total_time += obs.numsamples * obs.timepersample  # sec
+        total_bandwidth += obs.numchannels * obs.channelwidth  # Hz
+        ncore += len([stat for stat in obs.stations if stat.startswith('CS')])
+        nremote += len([stat for stat in obs.stations if stat.startswith('RS')])
+        mid_freq += (obs.endfreq + obs.startfreq) / 2 / 1e6  # MHz
+        unflagged_fraction += find_unflagged_fraction(ms)
+    total_bandwidth /= nobs
+    ncore = int(np.round(ncore / nobs))
+    nremote = int(np.round(nremote / nobs))
+    mean_freq = mid_freq / nobs
+    unflagged_fraction /= nobs
+
+    # Define table of system equivalent flux densities and interpolate
+    # to get the values at the mean frequency of the input observations.
+    # Note: values were taken from Table 9 of SKA Memo 113
+    sefd_freq_MHz = np.array([15, 30, 45, 60, 75, 120, 150, 180, 210, 240])
+    sefd_core_kJy = np.array([483, 89, 48, 32, 51, 3.6, 2.8, 3.2, 3.7, 4.1])
+    sefd_remote_kJy = np.array([483, 89, 48, 32, 51, 1.8, 1.4, 1.6, 1.8, 2.0])
+    f_core = interp1d(sefd_freq_MHz, sefd_core_kJy)
+    f_remote = interp1d(sefd_freq_MHz, sefd_remote_kJy)
+    sefd_core = f_core(mean_freq) * 1e3  # Jy
+    sefd_remote = f_remote(mean_freq) * 1e3  # Jy
+
+    # Calculate the theoretical noise, adjusted for the unflagged fraction
+    core_term = ncore * (ncore - 1) / 2 / sefd_core**2
+    remote_term = nremote * (nremote - 1) / 2 / sefd_remote**2
+    mixed_term = ncore * nremote / (sefd_core * sefd_remote)
+    noise = w_factor / np.sqrt(2 * (2 * total_time * total_bandwidth) *
+                               (core_term + mixed_term + remote_term))  # Jy
+    noise /= np.sqrt(unflagged_fraction)
+
+    return (noise, unflagged_fraction)
+
+
+def find_unflagged_fraction(ms_file):
+    """
+    Finds the fraction of data that is unflagged
+
+    Parameters
+    ----------
+    ms_file : str
+        Filename of input MS
+
+    Returns
+    -------
+    unflagged_fraction : float
+        Fraction of unflagged data
+    """
+    # Call taql. Note that we do not use pt.taql(), as pt.taql() can cause
+    # hanging/locking issues on some systems
+    result = subprocess.run("taql 'CALC sum([select nfalse(FLAG) from {0}]) / "
+                            "sum([select nelements(FLAG) from {0}])'".format(ms_file),
+                            shell=True, capture_output=True, check=True)
+    unflagged_fraction = float(result.stdout)
+
+    return unflagged_fraction
+
+
 def get_flagged_solution_fraction(h5file, solsetname='sol000'):
     """
     Get flagged fraction for solutions in given H5parm
 
     Parameters
     ----------
     h5file : str
```

### Comparing `rapthor-1.0/rapthor/lib/observation.py` & `rapthor-1.1/rapthor/lib/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         root_filename = os.path.basename(self.ms_filename)
         ms_model_filename = '{0}{1}.{2}_modeldata'.format(root_filename, self.infix,
                                                           sector_name)
         self.parameters['ms_model_filename'] = ms_model_filename
 
         # The filename of the sector's data with all non-sector sources peeled off
         # and/or with the weights adjusted (i.e., the data used as input for the
-        # imaging pipeline)
+        # imaging operation)
         self.ms_subtracted_filename = '{0}{1}.{2}'.format(root_filename, self.infix,
                                                           sector_name)
         self.parameters['ms_subtracted_filename'] = self.ms_subtracted_filename
 
         # The filename of the field data (after subtraction of outlier sources)
         self.ms_field = '{0}{1}_field'.format(root_filename, self.infix)
```

### Comparing `rapthor-1.0/rapthor/lib/operation.py` & `rapthor-1.1/rapthor/lib/operation.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 env_parset = Environment(loader=FileSystemLoader(os.path.join(DIR, '..', 'pipeline', 'parsets')))
 
 
 class Operation(object):
     """
     Generic operation class
 
-    An operation is simply a CWL pipeline that performs a part of the
-    processing. It holds the pipeline settings, populates the pipeline input and
-    parset templates, and runs the pipeline. The field object is passed between
+    An operation is simply a CWL workflow that performs a part of the
+    processing. It holds the workflow settings, populates the workflow input and
+    parset templates, and runs the workflow. The field object is passed between
     operations, each of which updates it with variables needed by other, subsequent,
     operations.
 
     Parameters
     ----------
     field : Field object
         Field for this operation
@@ -50,42 +50,41 @@
         self.force_serial_jobs = False  # force jobs to run serially
         self.use_mpi = False
 
         # Extra Toil env variables and Toil version
         self.toil_env_variables = {}
         self.toil_major_version = int(toil_version.version.split('.')[0])
 
-        # rapthor working directory
+        # Rapthor working directory
         self.rapthor_working_dir = self.parset['dir_working']
 
-        # Pipeline working dir
+        # Workflow working dir
         self.pipeline_working_dir = os.path.join(self.rapthor_working_dir,
                                                  'pipelines', self.name)
         misc.create_directory(self.pipeline_working_dir)
 
         # CWL runner settings
         self.cwl_runner = self.parset['cluster_specific']['cwl_runner']
         self.debug_workflow = self.parset['cluster_specific']['debug_workflow']
 
         # Maximum number of nodes to use
         self.max_nodes = self.parset['cluster_specific']['max_nodes']
 
-        # Directory that holds the pipeline logs in a convenient place
+        # Directory that holds the workflow logs in a convenient place
         self.log_dir = os.path.join(self.rapthor_working_dir, 'logs', self.name)
         misc.create_directory(self.log_dir)
 
         # Paths for scripts, etc. in the rapthor install directory
         self.rapthor_root_dir = os.path.split(DIR)[0]
         self.rapthor_pipeline_dir = os.path.join(self.rapthor_root_dir, 'pipeline')
         self.rapthor_script_dir = os.path.join(self.rapthor_root_dir, 'scripts')
 
-        # Input template name and output parset and inputs filenames for
-        # the pipeline. If the pipeline uses a subworkflow, its template filename must be
-        # defined in the subclass by self.subpipeline_parset_template to the right
-        # path
+        # Input template name and output parset and inputs filenames for the CWL workflow.
+        # If the workflow uses a subworkflow, its template filename must be defined in the
+        # subclass by self.subpipeline_parset_template to the right path
         self.pipeline_parset_template = '{0}_pipeline.cwl'.format(self.rootname)
         self.subpipeline_parset_template = None
         self.pipeline_parset_file = os.path.join(self.pipeline_working_dir,
                                                  'pipeline_parset.cwl')
         self.subpipeline_parset_file = os.path.join(self.pipeline_working_dir,
                                                     'subpipeline_parset.cwl')
         self.pipeline_inputs_file = os.path.join(self.pipeline_working_dir,
@@ -138,53 +137,53 @@
         if self.parset['cluster_specific']['use_container']:
             self.container = self.parset['cluster_specific']['container_type']
         else:
             self.container = None
 
     def set_parset_parameters(self):
         """
-        Define parameters needed for the pipeline parset template
+        Define parameters needed for the CWL workflow template
 
         The dictionary keys must match the jinja template variables used in the
-        corresponding pipeline parset.
+        corresponding workflow parset.
 
         The entries are defined in the subclasses as needed
         """
         self.parset_parms = {}
 
     def set_input_parameters(self):
         """
-        Define parameters needed for the pipeline inputs
+        Define parameters needed for the CWL workflow inputs
 
         The dictionary keys must match the workflow inputs defined in the corresponding
-        pipeline parset.
+        workflow parset.
 
         The entries are defined in the subclasses as needed
         """
         self.input_parms = {}
 
     def setup(self):
         """
         Set up this operation
 
-        This involves filling the pipeline parset template and writing the inputs file
+        This involves filling the workflow template and writing the inputs file
         """
         # Fill the parset template and save to a file
         self.set_parset_parameters()
         self.pipeline_parset_template = env_parset.get_template(self.pipeline_parset_template)
         tmp = self.pipeline_parset_template.render(self.parset_parms)
         with open(self.pipeline_parset_file, 'w') as f:
             f.write(tmp)
         if self.subpipeline_parset_template is not None:
             self.subpipeline_parset_template = env_parset.get_template(self.subpipeline_parset_template)
             tmp = self.subpipeline_parset_template.render(self.parset_parms)
             with open(self.subpipeline_parset_file, 'w') as f:
                 f.write(tmp)
 
-        # Save the pipeline inputs to a file
+        # Save the workflow inputs to a file
         self.set_input_parameters()
         with open(self.pipeline_inputs_file, 'w') as f:
             f.write(json.dumps(self.input_parms, cls=NpEncoder, indent=4, sort_keys=True))
 
     def finalize(self):
         """
         Finalize this operation.
@@ -200,15 +199,15 @@
         """
         return os.path.isfile(self.done_file)
 
     def run(self):
         """
         Runs the operation
         """
-        # Set up pipeline and call CWL runner
+        # Set up CWL workflow and call CWL runner
         self.setup()
         self.log.info('<-- Operation {0} started'.format(self.name))
 
         # Run current operation only if it hasn't run already.
         success = self.is_done()
         if not success:
             with Timer(self.log):
```

### Comparing `rapthor-1.0/rapthor/lib/parset.py` & `rapthor-1.1/rapthor/lib/parset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Module that holds all parset-related functions
 """
-import sys
 import os
 import glob
 import logging
 import configparser
 from rapthor._logging import set_log_file
 from astropy.coordinates import Angle
 import multiprocessing
@@ -25,39 +24,64 @@
         Use a log file as well as outputing to the screen
 
     Returns
     -------
     parset_dict : dict
         Dict of parset parameters
     """
-    if not os.path.isfile(parset_file):
-        raise FileNotFoundError("Missing parset file ({}).".format(parset_file))
-
     log.info("Reading parset file: {}".format(parset_file))
     parset = configparser.RawConfigParser()
-    parset.read(parset_file)
+    try:
+        if not parset.read(parset_file):
+            raise FileNotFoundError("Missing parset file ({}).".format(parset_file))
+    except configparser.ParsingError as err:
+        raise ValueError('Parset file {0} could not be parsed correctly.\n{1}'.format(parset_file, err))
 
     # Handle global parameters
     parset_dict = get_global_options(parset)
 
     # Handle calibration parameters
     parset_dict['calibration_specific'].update(get_calibration_options(parset))
 
     # Handle imaging parameters
     parset_dict['imaging_specific'].update(get_imaging_options(parset))
 
     # Handle cluster-specific parameters
     if not skip_cluster:
         parset_dict['cluster_specific'].update(get_cluster_options(parset))
 
+    # Check for invalid sections
+    given_sections = list(parset._sections.keys())
+    allowed_sections = ['global', 'calibration', 'imaging', 'cluster']
+    for section in given_sections:
+        if section not in allowed_sections:
+            log.warning('Section "{}" was given in the parset but is not a valid '
+                        'section name'.format(section))
+
+    # Check for required parameters. For now, the only required parameters
+    # are in the global section
+    required_parameters = {'global': ['dir_working', 'input_ms'],
+                           'calibration_specific': [],
+                           'imaging_specific': []}
+    if not skip_cluster:
+        required_parameters.update({'cluster_specific': []})
+    for section, key_list in required_parameters.items():
+        if section == 'global':
+            test_dict = parset_dict
+        else:
+            test_dict = parset_dict[section]
+        for key in key_list:
+            if key not in test_dict:
+                raise KeyError('The parset is missing the required parameter "{0}" '
+                               'in the [{1}] section'.format(key, section))
+
     # Set up working directory. All output will be placed in this directory
-    if not os.path.isdir(parset_dict['dir_working']):
-        os.mkdir(parset_dict['dir_working'])
     try:
-        os.chdir(parset_dict['dir_working'])
+        if not os.path.isdir(parset_dict['dir_working']):
+            os.mkdir(parset_dict['dir_working'])
         for subdir in ['logs', 'pipelines', 'regions', 'skymodels', 'images',
                        'solutions', 'plots']:
             subdir_path = os.path.join(parset_dict['dir_working'], subdir)
             if not os.path.isdir(subdir_path):
                 os.mkdir(subdir_path)
     except Exception as e:
         raise RuntimeError("Cannot use the working dir {0}: {1}".format(parset_dict['dir_working'], e))
@@ -71,15 +95,17 @@
     ms_search_list = parset_dict['input_ms'].strip('[]').split(',')
     ms_search_list = [ms.strip() for ms in ms_search_list]
     ms_files = []
     for search_str in ms_search_list:
         ms_files += glob.glob(os.path.join(search_str))
     parset_dict['mss'] = sorted(ms_files)
     if len(parset_dict['mss']) == 0:
-        raise FileNotFoundError('No input MS files were found!')
+        raise FileNotFoundError('No input MS files were found (searched for files '
+                                'matching: {}).'.format(', '.join('"{0}"'.format(search_str)
+                                                                  for search_str in ms_search_list)))
     log.info("Working on {} input MS file(s)".format(len(parset_dict['mss'])))
 
     # Make sure the initial skymodel is present
     if 'input_skymodel' not in parset_dict:
         if parset_dict['download_initial_skymodel']:
             log.info('No input sky model file given and download requested. Will automatically download skymodel.')
             parset_dict.update({'input_skymodel': os.path.join(parset_dict['dir_working'], 'skymodels', 'initial_skymodel.txt')})
@@ -96,22 +122,14 @@
             parset_dict['download_initial_skymodel'] = False
         else:
             log.info('User-provided skymodel is present, but download_overwrite_skymodel is True. Overwriting user-supplied skymodel with downloaded one.')
             parset_dict['download_initial_skymodel'] = True
     elif not os.path.exists(parset_dict['input_skymodel']):
         raise FileNotFoundError('Input sky model file "{}" not found.'.format(parset_dict['input_skymodel']))
 
-    # Check for invalid sections
-    given_sections = list(parset._sections.keys())
-    allowed_sections = ['global', 'calibration', 'imaging', 'cluster']
-    for section in given_sections:
-        if section not in allowed_sections:
-            log.warning('Section "{}" was given in the parset but is not a valid '
-                        'section name'.format(section))
-
     return parset_dict
 
 
 def get_global_options(parset):
     """
     Handle the global options
 
@@ -124,15 +142,19 @@
     -------
     parset_dict : dict
         Dictionary with all global options
 
     """
     # TODO: Repalce all "if 'some_key' in parset_dict:" with "parset_dict.setdefault(...)"
 
-    parset_dict = parset._sections['global'].copy()
+    try:
+        parset_dict = parset._sections['global'].copy()
+    except KeyError:
+        raise KeyError('The parset is missing the required [global] section')
+
     parset_dict.update({'calibration_specific': {}, 'imaging_specific': {}, 'cluster_specific': {}})
 
     # Fraction of data to use (default = 0.2). If less than one, the input data are divided
     # by time into chunks (of no less than slow_timestep_separate_sec below) that sum to the requested
     # fraction, spaced out evenly over the full time range
     if 'selfcal_data_fraction' in parset_dict:
         parset_dict['selfcal_data_fraction'] = parset.getfloat('global', 'selfcal_data_fraction')
@@ -221,15 +243,15 @@
         flag_list.append('flag_freqrange')
     if 'flag_expr' not in parset_dict:
         parset_dict['flag_expr'] = ' and '.join(flag_list)
     else:
         for f in flag_list:
             if f not in parset_dict['flag_expr']:
                 raise ValueError('Flag selection "{}" was specified but does not '
-                          'appear in flag_expr'.format(f))
+                                 'appear in flag_expr'.format(f))
 
     # Check for invalid options
     given_options = parset.options('global')
     allowed_options = ['dir_working', 'input_ms', 'strategy',
                        'use_compression', 'flag_abstime', 'flag_baseline', 'flag_freqrange',
                        'flag_expr', 'download_initial_skymodel', 'download_initial_skymodel_radius', 'download_initial_skymodel_server', 'download_overwrite_skymodel',
                        'input_skymodel', 'apparent_skymodel',
@@ -353,14 +375,20 @@
 
     # Parallel predict over baselines
     if 'parallelbaselines' in parset_dict:
         parset_dict['parallelbaselines'] = parset.getboolean('calibration', 'parallelbaselines')
     else:
         parset_dict['parallelbaselines'] = False
 
+    # Use SAGECalpredict
+    if 'sagecalpredict' in parset_dict:
+        parset_dict['sagecalpredict'] = parset.getboolean('calibration', 'sagecalpredict')
+    else:
+        parset_dict['sagecalpredict'] = False
+
     # LBFGS solver parameters
     if 'solverlbfgs_dof' in parset_dict:
         parset_dict['solverlbfgs_dof'] = parset.getfloat('calibration', 'solverlbfgs_dof')
     else:
         parset_dict['solverlbfgs_dof'] = 200.0
     if 'solverlbfgs_iter' in parset_dict:
         parset_dict['solverlbfgs_iter'] = parset.getint('calibration', 'solverlbfgs_iter')
@@ -376,15 +404,15 @@
                        'slow_timestep_separate_sec', 'onebeamperpatch',
                        'slow_freqstep_hz', 'propagatesolutions', 'maxiter', 'stepsize',
                        'tolerance', 'llssolver', 'fast_smoothnessconstraint',
                        'fast_smoothnessreffrequency', 'fast_smoothnessrefdistance',
                        'slow_smoothnessconstraint_joint',
                        'slow_smoothnessconstraint_separate', 'parallelbaselines',
                        'solveralgorithm', 'solverlbfgs_dof', 'solverlbfgs_iter',
-                       'solverlbfgs_minibatches']
+                       'solverlbfgs_minibatches','sagecalpredict']
     for option in given_options:
         if option not in allowed_options:
             log.warning('Option "{}" was given in the [calibration] section of the '
                         'parset but is not a valid calibration option'.format(option))
 
     return parset_dict
 
@@ -479,16 +507,16 @@
         len_list.append(len(val_list))
     else:
         parset_dict['sector_width_dec_deg_list'] = []
 
     # Check that all the above options have the same number of entries
     if len(set(len_list)) > 1:
         raise ValueError('The options sector_center_ra_list, sector_center_dec_list, '
-                  'sector_width_ra_deg_list, and sector_width_dec_deg_list '
-                  'must all have the same number of entries')
+                         'sector_width_ra_deg_list, and sector_width_dec_deg_list '
+                         'must all have the same number of entries')
 
     # IDG (image domain gridder) mode to use in WSClean (default = cpu). The mode can
     # be cpu, gpu, or hybrid.
     if 'idg_mode' not in parset_dict:
         parset_dict['idg_mode'] = 'cpu'
     if parset_dict['idg_mode'] not in ['cpu', 'gpu', 'hybrid']:
         raise ValueError('The option idg_mode must be one of "cpu", "gpu", or "hybrid"')
@@ -687,15 +715,15 @@
     # Full path to a local disk on the nodes for I/O-intensive processing. The path
     # must be the same for all nodes
     if 'dir_local' not in parset_dict:
         parset_dict['dir_local'] = None
     else:
         parset_dict['dir_local'] = parset_dict['dir_local']
 
-    # Run the pipelines inside a container (default = False)? If True, the pipeline
+    # Run the workflows inside a container (default = False)? If True, the CWL workflow
     # for each operation (such as calibrate or image) will be run inside a container.
     # The type of container can also be specified (one of docker, udocker, or
     # singularity; default = docker)
     if 'use_container' in parset_dict:
         parset_dict['use_container'] = parset.getboolean('cluster', 'use_container')
     else:
         parset_dict['use_container'] = False
@@ -705,15 +733,15 @@
     # Define CWL runner
     if 'cwl_runner' not in parset_dict:
         parset_dict['cwl_runner'] = 'toil'
     cwl_runner = parset_dict['cwl_runner']
     supported_cwl_runners = ('cwltool', 'toil')
     if cwl_runner not in supported_cwl_runners:
         raise ValueError("CWL runner '%s' is not supported; select one of: %s",
-                     cwl_runner, ', '.join(supported_cwl_runners))
+                         cwl_runner, ', '.join(supported_cwl_runners))
 
     # Set Toil's coordination directory (only used when Toil is used as the CWL runner;
     # default = selected automatically by Toil). Note that this directory does not
     # need to be on a shared file system but must be located one that is 100%
     # POSIX-compatible (which many shared file systems are not)
     if 'dir_coordination' not in parset_dict:
         parset_dict['dir_coordination'] = None
```

### Comparing `rapthor-1.0/rapthor/lib/screen.py` & `rapthor-1.1/rapthor/lib/screen.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/lib/sector.py` & `rapthor-1.1/rapthor/lib/sector.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import copy
 
 
 class Sector(object):
     """
     The Sector object contains various parameters for a sector of the field. Sectors
-    are used only in image and predict pipelines
+    are used only in image and predict operations
 
     Parameters
     ----------
     name : str
         Name of sector
     ra : float
         RA in degrees of sector center
@@ -55,15 +55,15 @@
         self.I_image_file_apparent_sky = None  # set by the Image operation
         self.I_mask_file = None   # set by the Image operation
         self.image_skymodel_file_apparent_sky = None  # set by the Image operation
         self.image_skymodel_file_true_sky = None  # set by the Image operation
         self.is_outlier = False
         self.is_bright_source = False
         self.imsize = None  # set to None to force calculation in set_imaging_parameters()
-        self.wsclean_image_padding = 1.2  # the WSClean default value, used in the pipelines
+        self.wsclean_image_padding = 1.2  # the WSClean default value, used in the workflows
         self.diagnostics = []  # list to hold dicts of image diagnostics
 
         # Make copies of the observation objects, as each sector may have its own
         # observation-specific settings
         self.observations = []
         for obs in field.observations:
             obs.log = None  # deepcopy cannot copy the log object
@@ -81,15 +81,15 @@
         """
         for obs in self.observations:
             obs.set_prediction_parameters(self.name, self.patches,
                                           os.path.join(self.field.working_dir, 'scratch'))
 
     def set_imaging_parameters(self, do_multiscale=False, recalculate_imsize=False):
         """
-        Sets the parameters needed for the imaging pipeline
+        Sets the parameters needed for the imaging operation
 
         Parameters
         ----------
         do_multiscale : bool, optional
             If True, multiscale clean is done
         recalculate_imsize : bool, optional
             If True, the image size is recalculated based on the current sector region
@@ -130,54 +130,59 @@
         if recalculate_imsize or self.imsize is None:
             xmin, ymin, xmax, ymax = self.poly.bounds
             self.width_ra = (xmax - xmin) * self.field.wcs_pixel_scale  # deg
             self.width_dec = (ymax - ymin) * self.field.wcs_pixel_scale  # deg
             self.imsize = [int(self.width_ra / self.cellsize_deg),
                            int(self.width_dec / self.cellsize_deg)]
 
-            # IDG does not yet support rectangular images, so ensure image is square
-            self.imsize = [max(self.imsize), max(self.imsize)]
-
-            # IDG has problems with small images, so set minimum size to 500 pixels and adjust
-            # padded polygon
-            minsize = 500
-            if max(self.imsize) < minsize:
-                dec_width_pix = self.width_dec / abs(self.field.wcs.wcs.cdelt[1])
-                padding_pix = dec_width_pix * (self.wsclean_image_padding - 1.0)
-                padding_pix *= minsize / max(self.imsize)  # scale padding to new imsize
-                self.poly_padded = self.poly.buffer(padding_pix)
-                self.imsize = [minsize, minsize]
+            if self.use_screens:
+                # IDG does not yet support rectangular images, so ensure image
+                # is square
+                self.imsize = [max(self.imsize), max(self.imsize)]
+
+                # IDG has problems with small images, so set minimum size to 500 pixels
+                # and adjust padded polygon
+                minsize = 500
+                if max(self.imsize) < minsize:
+                    dec_width_pix = self.width_dec / abs(self.field.wcs.wcs.cdelt[1])
+                    padding_pix = dec_width_pix * (self.wsclean_image_padding - 1.0)
+                    padding_pix *= minsize / max(self.imsize)  # scale padding to new imsize
+                    self.poly_padded = self.poly.buffer(padding_pix)
+                    self.imsize = [minsize, minsize]
 
             # Lastly, make sure the image size is an even number (odd sizes cause the
             # peak to lie not necessarily in the img center)
             if self.imsize[0] % 2:
                 self.imsize[0] += 1
+            if self.imsize[1] % 2:
                 self.imsize[1] += 1
 
         self.wsclean_imsize = "'{0} {1}'".format(self.imsize[0], self.imsize[1])
         self.log.debug('Image size is {0} x {1} pixels'.format(
                        self.imsize[0], self.imsize[1]))
 
         # Set number of output channels to get ~ 4 MHz per channel equivalent at 120 MHz
         # (the maximum averaging allowed for typical dTEC values of -0.5 < dTEC < 0.5)
         min_freq = np.min([obs.startfreq for obs in self.observations])
         target_bandwidth = 4e6 * min_freq / 120e6
         max_nchannels = np.max([obs.numchannels for obs in self.observations])
-        min_nchannels = 4  # we want at least 4 channels -- see below
+        min_nchannels = 1
         tot_bandwidth = 0.0
         for obs in self.observations:
             # Find observation with largest bandwidth
             obs_bandwidth = obs.numchannels * obs.channelwidth
             if obs_bandwidth > tot_bandwidth:
                 tot_bandwidth = obs_bandwidth
         self.wsclean_nchannels = max(min_nchannels, min(max_nchannels, int(np.ceil(tot_bandwidth / target_bandwidth))))
 
-        # Set number of channels to use in spectral fitting. Since we always use
-        # -fit-spectral-pol = 3 in the WSClean calls, simply set this to 4 channels
-        self.wsclean_deconvolution_channels = 4
+        # Set number of channels to use in spectral fitting. We set this to the
+        # number of channels, up to a maximum of 4 (and the fit spectral order to
+        # one less)
+        self.wsclean_deconvolution_channels = min(4, self.wsclean_nchannels)
+        self.wsclean_spectral_poly_order = max(1, self.wsclean_deconvolution_channels-1)
 
         # Set number of iterations. We scale the number of iterations depending on the
         # integration time and the distance of the sector center to the phase center, to
         # account for the reduced sensitivity of the image, assuming a Gaussian primary
         # beam. Lastly, we also reduce them if bright sources are peeled
         total_time_hr = 0.0
         for obs in self.observations:
```

### Comparing `rapthor-1.0/rapthor/lib/strategy.py` & `rapthor-1.1/rapthor/lib/strategy.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/modifystate.py` & `rapthor-1.1/rapthor/modifystate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module that modifies the state of the pipelines
+Module that modifies the state of the pipeline
 """
 from rapthor.lib.parset import parset_read
 from rapthor.lib.strategy import set_strategy
 from rapthor.lib.field import Field
 import filecmp
 import logging
 import os
@@ -11,15 +11,15 @@
 import sys
 
 log = logging.getLogger('rapthor:state')
 
 
 def run(parset_file):
     """
-    Modifies the state of one or more pipelines
+    Modifies the state of one or more operations
 
     Parameters
     ----------
     parset_file : str
         Filename of parset containing processing parameters
     """
     # Set logging level to suppress unnecessary messages
@@ -34,39 +34,39 @@
     field = Field(parset, mininmal=True)
     field.outlier_sectors = [None]
     field.imaging_sectors = [None]
 
     # Get the processing strategy
     strategy_steps = set_strategy(field)
 
-    # Check each operation for started pipelines
+    # Check each operation for started pipelines (workflows)
     operation_list = ['calibrate', 'predict', 'image', 'mosaic']  # in order of execution
     while True:
         pipelines = []
         for index, step in enumerate(strategy_steps):
             for opname in operation_list:
                 operation = os.path.join(parset['dir_working'], 'pipelines', '{0}_{1}'.format(opname, index+1))
                 if os.path.exists(operation):
                     pipelines.append(os.path.basename(operation))
 
-        # List pipelines and query user
+        # List operations and query user
         print('\nCurrent strategy: {}'.format(field.parset['strategy']))
-        print('\nPipelines:')
+        print('\nOperations:')
         i = 0
         if len(pipelines) == 0:
             print('    None')
             print('No reset can be done.')
             sys.exit(0)
         else:
             for p in pipelines:
                 i += 1
                 print('    {0}) {1}'.format(i, p))
         try:
             while(True):
-                p_number_raw = input('Enter number of pipeline to reset or "q" to quit: ')
+                p_number_raw = input('Enter number of operation to reset or "q" to quit: ')
                 try:
                     if p_number_raw.lower() == "q":
                         sys.exit(0)
                     elif int(p_number_raw) > 0 and int(p_number_raw) <= i:
                         break
                     else:
                         print("Please enter a number between 1 and {}".format(i))
@@ -75,39 +75,39 @@
         except KeyboardInterrupt:
             sys.exit(0)
         pipeline = pipelines[int(p_number_raw)-1]
 
         # Ask for confirmation
         try:
             while(True):
-                answer = input('Reset all pipelines from {} onwards (y/n)? '.format(pipeline))
+                answer = input('Reset all operations from {} onwards (y/n)? '.format(pipeline))
                 if (answer.lower() == "n" or answer.lower() == "no" or
                     answer.lower() == "y" or answer.lower() == "yes"):
                     break
                 else:
                     print('Please enter "y" or "n"')
         except KeyboardInterrupt:
             sys.exit(0)
 
-        # Reset pipeline states as requested
+        # Reset operation states as requested
         if answer.lower() == "y" or answer.lower() == "yes":
             print('Reseting state...')
             for pipeline in pipelines[int(p_number_raw)-1:]:
-                # Remove the pipeline working directory to ensure files from previous
+                # Remove the operation working directory to ensure files from previous
                 # runs are not kept and used in subsequent ones (e.g., Toil does not
                 # seem to always overwrite existing files from previous runs). This
                 # also removes Toil's jobstore when present (where the state is tracked).
                 # Other associated files are removed as well
                 path = os.path.join(parset['dir_working'], 'pipelines', pipeline)
                 shutil.rmtree(path, ignore_errors=True)
 
             # Now remove any sub-directories in the other output directories, that
             # are _not_ present in the 'pipelines' directory.
             for dirname in ('skymodels', 'solutions', 'logs', 'plots', 'regions', 'images'):
                 dcmp = filecmp.dircmp(
-                    os.path.join(parset['dir_working'], 'pipelines'), 
+                    os.path.join(parset['dir_working'], 'pipelines'),
                     os.path.join(parset['dir_working'], dirname)
                 )
                 for path in (os.path.join(dcmp.right, item) for item in dcmp.right_only):
                     shutil.rmtree(path, ignore_errors=True)
 
             print('Reset complete.')
```

### Comparing `rapthor-1.0/rapthor/operations/calibrate.py` & `rapthor-1.1/rapthor/operations/calibrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Operation to calibrate the field
     """
     def __init__(self, field, index):
         super(Calibrate, self).__init__(field, name='calibrate', index=index)
 
     def set_parset_parameters(self):
         """
-        Define parameters needed for the pipeline parset template
+        Define parameters needed for the CWL workflow template
         """
         if self.batch_system == 'slurm':
             # For some reason, setting coresMax ResourceRequirement hints does
             # not work with SLURM
             max_cores = None
         else:
             max_cores = self.field.parset['cluster_specific']['max_cores']
@@ -44,20 +44,20 @@
                              'do_joint_solve': do_joint_solve,
                              'use_scalarphase': self.field.use_scalarphase,
                              'apply_diagonal_solutions': self.field.apply_diagonal_solutions,
                              'max_cores': max_cores}
 
     def set_input_parameters(self):
         """
-        Define the pipeline inputs
+        Define the CWL workflow inputs
         """
         # First set the calibration parameters for each observation
         self.field.set_obs_parameters()
 
-        # Next, get the various parameters needed by the pipeline
+        # Next, get the various parameters needed by the workflow
         #
         # Get the filenames of the input files for each time chunk
         timechunk_filename = self.field.get_obs_parameters('timechunk_filename')
 
         # Get the start times and number of times for the time chunks (fast and slow
         # calibration)
         starttime = self.field.get_obs_parameters('starttime')
@@ -132,14 +132,15 @@
         propagatesolutions = self.field.propagatesolutions
         solveralgorithm = self.field.solveralgorithm
         onebeamperpatch = self.field.onebeamperpatch
         stepsize = self.field.stepsize
         tolerance = self.field.tolerance
         uvlambdamin = self.field.solve_min_uv_lambda
         parallelbaselines = self.field.parallelbaselines
+        sagecalpredict = self.field.sagecalpredict
         solverlbfgs_dof = self.field.solverlbfgs_dof
         solverlbfgs_iter = self.field.solverlbfgs_iter
         solverlbfgs_minibatches = self.field.solverlbfgs_minibatches
 
         # Get the size of the imaging area (for use in making the a-term images)
         sector_bounds_deg = '{}'.format(self.field.sector_bounds_deg)
         sector_bounds_mid_deg = '{}'.format(self.field.sector_bounds_mid_deg)
@@ -201,14 +202,15 @@
                             'propagatesolutions': propagatesolutions,
                             'solveralgorithm': solveralgorithm,
                             'onebeamperpatch': onebeamperpatch,
                             'stepsize': stepsize,
                             'tolerance': tolerance,
                             'uvlambdamin': uvlambdamin,
                             'parallelbaselines': parallelbaselines,
+                            'sagecalpredict': sagecalpredict,
                             'sector_bounds_deg': sector_bounds_deg,
                             'sector_bounds_mid_deg': sector_bounds_mid_deg,
                             'split_outh5parm': split_outh5parm,
                             'output_aterms_root': self.output_aterms_root,
                             'screen_type': screen_type,
                             'combined_h5parms': self.combined_h5parms,
                             'fast_antennaconstraint': fast_antennaconstraint,
```

### Comparing `rapthor-1.0/rapthor/operations/image.py` & `rapthor-1.1/rapthor/operations/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         super(Image, self).__init__(field, name='image', index=index)
 
         # For imaging we use a subworkflow, so we set the template filename for that here
         self.subpipeline_parset_template = '{0}_sector_pipeline.cwl'.format(self.rootname)
 
     def set_parset_parameters(self):
         """
-        Define parameters needed for the pipeline parset template
+        Define parameters needed for the CWL workflow template
         """
         if self.batch_system == 'slurm':
             # For some reason, setting coresMax ResourceRequirement hints does
             # not work with SLURM
             max_cores = None
         else:
             max_cores = self.field.parset['cluster_specific']['max_cores']
@@ -44,19 +44,20 @@
                              'peel_bright_sources': self.field.peel_bright_sources,
                              'max_cores': max_cores,
                              'use_mpi': self.field.use_mpi,
                              'toil_version': self.toil_major_version}
 
     def set_input_parameters(self):
         """
-        Define the pipeline inputs
+        Define the CWL workflow inputs
         """
         nsectors = len(self.field.imaging_sectors)
         obs_filename = []
         prepare_filename = []
+        concat_filename = []
         previous_mask_filename = []
         mask_filename = []
         starttime = []
         ntimes = []
         image_freqstep = []
         image_timestep = []
         dir_local = []
@@ -80,14 +81,15 @@
                 sector_obs_filename = [obs.ms_imaging_filename for obs in sector.observations]
             else:
                 sector_obs_filename = sector.get_obs_parameters('ms_filename')
             obs_filename.append(sector_obs_filename)
 
             # Set output MS filenames for step that prepares the data for WSClean
             prepare_filename.append(sector.get_obs_parameters('ms_prep_filename'))
+            concat_filename.append(image_root[-1] + '_concat.ms')
 
             # Set other parameters
             if sector.I_mask_file is not None:
                 # Use the existing mask
                 previous_mask_filename.append(sector.I_mask_file)
             else:
                 # Use a dummy mask
@@ -107,26 +109,28 @@
                 dir_local.append(self.pipeline_working_dir)
             else:
                 dir_local.append(self.scratch_dir)
             central_patch_name.append(sector.central_patch)
 
         self.input_parms = {'obs_filename': [CWLDir(name).to_json() for name in obs_filename],
                             'prepare_filename': prepare_filename,
+                            'concat_filename': concat_filename,
                             'previous_mask_filename': [None if name is None else CWLFile(name).to_json() for name in previous_mask_filename],
                             'mask_filename': mask_filename,
                             'starttime': starttime,
                             'ntimes': ntimes,
                             'image_freqstep': image_freqstep,
                             'image_timestep': image_timestep,
                             'phasecenter': phasecenter,
                             'image_name': image_root,
                             'dir_local': dir_local,
                             'do_slowgain_solve': [self.field.do_slowgain_solve] * nsectors,
                             'channels_out': [sector.wsclean_nchannels for sector in self.field.imaging_sectors],
                             'deconvolution_channels': [sector.wsclean_deconvolution_channels for sector in self.field.imaging_sectors],
+                            'fit_spectral_pol': [sector.wsclean_spectral_poly_order for sector in self.field.imaging_sectors],
                             'ra': [sector.ra for sector in self.field.imaging_sectors],
                             'dec': [sector.dec for sector in self.field.imaging_sectors],
                             'wsclean_imsize': [sector.imsize for sector in self.field.imaging_sectors],
                             'vertices_file': [CWLFile(sector.vertices_file).to_json() for sector in self.field.imaging_sectors],
                             'region_file': [None if sector.region_file is None else CWLFile(sector.region_file).to_json() for sector in self.field.imaging_sectors],
                             'wsclean_niter': [sector.wsclean_niter for sector in self.field.imaging_sectors],
                             'wsclean_nmiter': [sector.wsclean_nmiter for sector in self.field.imaging_sectors],
@@ -144,15 +148,15 @@
                             'dd_psf_grid': [sector.dd_psf_grid for sector in self.field.imaging_sectors],
                             'max_threads': self.field.parset['cluster_specific']['max_threads'],
                             'deconvolution_threads': self.field.parset['cluster_specific']['deconvolution_threads']}
 
         if self.field.peel_bright_sources:
             self.input_parms.update({'bright_skymodel_pb': CWLFile(self.field.bright_source_skymodel_file).to_json()})
         if self.field.use_mpi:
-            # Set number of nodes to allocate to each imaging subpipeline. We subtract
+            # Set number of nodes to allocate to each imaging subworkflow. We subtract
             # one node because Toil must use one node for its job, which in turn calls
             # salloc to reserve the nodes for the MPI job
             self.use_mpi = True
             nnodes = self.parset['cluster_specific']['max_nodes']
             nsubpipes = min(nsectors, nnodes)
             nnodes_per_subpipeline = max(1, int(nnodes / nsubpipes) - 1)
             self.input_parms.update({'mpi_nnodes': [nnodes_per_subpipeline] * nsectors})
@@ -168,23 +172,24 @@
                 # For faceting, we need inputs for making the ds9 facet region files
                 self.input_parms.update({'skymodel': CWLFile(self.field.calibration_skymodel_file).to_json()})
                 ra_mid = []
                 dec_mid = []
                 width_ra = []
                 width_dec = []
                 facet_region_file = []
+                min_width = 2 * self.field.get_calibration_radius() * 1.2
                 for sector in self.field.imaging_sectors:
                     # Note: WSClean requires that all sources in the h5parm must have
                     # corresponding regions in the facets region file. We ensure this
-                    # requirement is met by making the region file very large so that
-                    # it covers the full field (10x10 deg)
+                    # requirement is met by extending the regions to cover the larger of
+                    # the calibration region and the sector region, plus a 20% padding
                     ra_mid.append(self.field.ra)
                     dec_mid.append(self.field.dec)
-                    width_ra.append(10.0)
-                    width_dec.append(10.0)
+                    width_ra.append(max(min_width, sector.width_ra*1.2))
+                    width_dec.append(max(min_width, sector.width_dec*1.2))
                     facet_region_file.append('{}_facets_ds9.reg'.format(sector.name))
                 self.input_parms.update({'ra_mid': ra_mid})
                 self.input_parms.update({'dec_mid': dec_mid})
                 self.input_parms.update({'width_ra': width_ra})
                 self.input_parms.update({'width_dec': width_dec})
                 self.input_parms.update({'facet_region_file': facet_region_file})
                 if self.field.do_slowgain_solve:
@@ -213,27 +218,14 @@
         for sector in self.field.imaging_sectors:
             image_root = os.path.join(self.pipeline_working_dir, sector.name)
             sector.I_image_file_true_sky = image_root + '-MFS-image-pb.fits'
             sector.I_image_file_apparent_sky = image_root + '-MFS-image.fits'
             sector.I_model_file_true_sky = image_root + '-MFS-model.fits'
             sector.I_residual_file_apparent_sky = image_root + '-MFS-residual.fits'
 
-            # Check to see if a clean mask image was made (only made when at least one
-            # island is found in the Stokes I image). The filename is defined
-            # in the rapthor/scripts/filter_skymodel.py file
-            #
-            # Note: for now, the clean mask is not used as it has not been found to
-            # be necessary (WSClean automasking is used on its own)
-            use_clean_mask = False
-            mask_filename = sector.I_image_file_apparent_sky + '.mask'
-            if use_clean_mask and os.path.exists(mask_filename):
-                sector.I_mask_file = mask_filename
-            else:
-                sector.I_mask_file = None
-
             # The sky models, both true sky and apparent sky (the filenames are defined
             # in the rapthor/scripts/filter_skymodel.py file)
             sector.image_skymodel_file_true_sky = image_root + '.true_sky.txt'
             sector.image_skymodel_file_apparent_sky = image_root + '.apparent_sky.txt'
             dst_dir = os.path.join(self.parset['dir_working'], 'skymodels', 'image_{}'.format(self.index))
             misc.create_directory(dst_dir)
             for src_filename in [sector.image_skymodel_file_true_sky, sector.image_skymodel_file_apparent_sky]:
@@ -256,65 +248,79 @@
             # Read in the image diagnostics and log a summary of them
             diagnostics_file = image_root + '.image_diagnostics.json'
             with open(diagnostics_file, 'r') as f:
                 diagnostics_dict = json.load(f)
             sector.diagnostics.append(diagnostics_dict)
             try:
                 theoretical_rms = '{0:.1f} uJy/beam'.format(diagnostics_dict['theoretical_rms']*1e6)
-                min_rms = '{0:.1f} uJy/beam'.format(diagnostics_dict['min_rms']*1e6)
-                median_rms = '{0:.1f} uJy/beam'.format(diagnostics_dict['median_rms']*1e6)
-                dynr = '{0:.2g}'.format(diagnostics_dict['dynamic_range_global'])
+                min_rms_true_sky = '{0:.1f} uJy/beam'.format(diagnostics_dict['min_rms_true_sky']*1e6)
+                median_rms_true_sky = '{0:.1f} uJy/beam'.format(diagnostics_dict['median_rms_true_sky']*1e6)
+                dynr_true_sky = '{0:.2g}'.format(diagnostics_dict['dynamic_range_global_true_sky'])
+                min_rms_flat_noise = '{0:.1f} uJy/beam'.format(diagnostics_dict['min_rms_flat_noise']*1e6)
+                median_rms_flat_noise = '{0:.1f} uJy/beam'.format(diagnostics_dict['median_rms_flat_noise']*1e6)
+                dynr_flat_noise = '{0:.2g}'.format(diagnostics_dict['dynamic_range_global_flat_noise'])
                 nsources = '{0}'.format(diagnostics_dict['nsources'])
                 freq = '{0:.1f} MHz'.format(diagnostics_dict['freq']/1e6)
                 beam = '{0:.1f}" x {1:.1f}", PA = {2:.1f} deg'.format(diagnostics_dict['beam_fwhm'][0]*3600,
                                                                       diagnostics_dict['beam_fwhm'][1]*3600,
                                                                       diagnostics_dict['beam_fwhm'][2])
                 unflagged_data_fraction = '{0:.2f}'.format(diagnostics_dict['unflagged_data_fraction'])
                 self.log.info('Diagnostics for {}:'.format(sector.name))
-                self.log.info('    Min RMS noise = {0} (theoretical = {1})'.format(min_rms, theoretical_rms))
-                self.log.info('    Median RMS noise = {}'.format(median_rms))
-                self.log.info('    Dynamic range = {}'.format(dynr))
+                self.log.info('    Min RMS noise = {0} (non-PB-corrected), '
+                              '{1} (PB-corrected), {2} (theoretical)'.format(min_rms_flat_noise, min_rms_true_sky,
+                                                                             theoretical_rms))
+                self.log.info('    Median RMS noise = {0} (non-PB-corrected), '
+                              '{1} (PB-corrected)'.format(median_rms_flat_noise, median_rms_true_sky))
+                self.log.info('    Dynamic range = {0} (non-PB-corrected), '
+                              '{1} (PB-corrected)'.format(dynr_flat_noise, dynr_true_sky))
                 self.log.info('    Number of sources found by PyBDSF = {}'.format(nsources))
                 self.log.info('    Reference frequency = {}'.format(freq))
                 self.log.info('    Beam = {}'.format(beam))
                 self.log.info('    Fraction of unflagged data = {}'.format(unflagged_data_fraction))
-                if 'meanClippedRatio' in diagnostics_dict:
-                    # If 'meanClippedRatio' is present, assume all of the LSMTool-generated
-                    # comparison diagnostics are available (these are only generated if there
-                    # is a sufficient number of appropriate sources in the image to make the
-                    # comparison)
-                    #
-                    # Note: the reported error is not allowed to fall below
-                    # 10% for the flux ratio and 0.5" for the astrometry, as these
-                    # are the realistic minimum uncertainties in these values
-                    ratio = '{0:.1f}'.format(diagnostics_dict['meanClippedRatio'])
-                    self.field.lofar_to_true_flux_ratio = diagnostics_dict['meanClippedRatio']
-                    stdratio = '{0:.1f}'.format(max(0.1, diagnostics_dict['stdClippedRatio']))
-                    self.field.lofar_to_true_flux_std = max(0.1, diagnostics_dict['stdClippedRatio'])
+
+                # Log the estimates of the global flux ratio and astrometry offsets.
+                # If the required keys are not present, then there were not enough
+                # sources for a reliable estimate to be made so report 'N/A' (not
+                # available)
+                #
+                # Note: the reported error is not allowed to fall below 10% for
+                # the flux ratio and 0.5" for the astrometry, as these are the
+                # realistic minimum uncertainties in these values
+                if 'meanClippedRatio_pybdsf' in diagnostics_dict and 'stdClippedRatio_pybdsf' in diagnostics_dict:
+                    ratio = '{0:.1f}'.format(diagnostics_dict['meanClippedRatio_pybdsf'])
+                    self.field.lofar_to_true_flux_ratio = diagnostics_dict['meanClippedRatio_pybdsf']
+                    stdratio = '{0:.1f}'.format(max(0.1, diagnostics_dict['stdClippedRatio_pybdsf']))
+                    self.field.lofar_to_true_flux_std = max(0.1, diagnostics_dict['stdClippedRatio_pybdsf'])
                     self.log.info('    LOFAR/TGSS flux ratio = {0} +/- {1}'.format(ratio, stdratio))
+                else:
+                    self.field.lofar_to_true_flux_ratio = 1.0
+                    self.field.lofar_to_true_flux_std = 0.0
+                    self.log.info('    LOFAR/TGSS flux ratio = N/A')
+                if 'meanClippedRAOffsetDeg' in diagnostics_dict and 'stdClippedRAOffsetDeg' in diagnostics_dict:
                     raoff = '{0:.1f}"'.format(diagnostics_dict['meanClippedRAOffsetDeg']*3600)
                     stdraoff = '{0:.1f}"'.format(max(0.5, diagnostics_dict['stdClippedRAOffsetDeg']*3600))
                     self.log.info('    LOFAR-TGSS RA offset = {0} +/- {1}'.format(raoff, stdraoff))
+                else:
+                    self.log.info('    LOFAR-TGSS RA offset = N/A')
+                if 'meanClippedDecOffsetDeg' in diagnostics_dict and 'stdClippedDecOffsetDeg' in diagnostics_dict:
                     decoff = '{0:.1f}"'.format(diagnostics_dict['meanClippedDecOffsetDeg']*3600)
                     stddecoff = '{0:.1f}"'.format(max(0.5, diagnostics_dict['stdClippedDecOffsetDeg']*3600))
                     self.log.info('    LOFAR-TGSS Dec offset = {0} +/- {1}'.format(decoff, stddecoff))
                 else:
-                    self.field.lofar_to_true_flux_ratio = 1.0
-                    self.field.lofar_to_true_flux_std = 0.0
-                    self.log.info('    LOFAR/TGSS flux ratio = N/A')
-                    self.log.info('    LOFAR-TGSS RA offset = N/A')
                     self.log.info('    LOFAR-TGSS Dec offset = N/A')
             except KeyError:
-                self.log.warn('One or more of the expected image diagnostics unavailable '
+                self.log.warn('One or more of the expected image diagnostics is unavailable '
                               'for {}. Logging of diagnostics skipped.'.format(sector.name))
-                req_keys = ['theoretical_rms', 'min_rms', 'median_rms', 'dynamic_range_global',
+                req_keys = ['theoretical_rms', 'min_rms_flat_noise', 'median_rms_flat_noise',
+                            'dynamic_range_global_flat_noise', 'min_rms_true_sky',
+                            'median_rms_true_sky', 'dynamic_range_global_true_sky',
                             'nsources', 'freq', 'beam_fwhm', 'unflagged_data_fraction',
-                            'meanClippedRatio', 'stdClippedRatio', 'meanClippedRAOffsetDeg',
-                            'stdClippedRAOffsetDeg', 'meanClippedDecOffsetDeg',
-                            'stdClippedDecOffsetDeg']
+                            'meanClippedRatio_pybdsf', 'stdClippedRatio_pybdsf',
+                            'meanClippedRAOffsetDeg', 'stdClippedRAOffsetDeg',
+                            'meanClippedDecOffsetDeg', 'stdClippedDecOffsetDeg']
                 missing_keys = []
                 for key in req_keys:
                     if key not in diagnostics_dict:
                         missing_keys.append(key)
                 self.log.debug('Keys missing from the diagnostics dict: {}.'.format(', '.join(missing_keys)))
 
         # Finally call finalize() in the parent class
```

### Comparing `rapthor-1.0/rapthor/operations/mosaic.py` & `rapthor-1.1/rapthor/operations/mosaic.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.subpipeline_parset_template = '{0}_type_pipeline.cwl'.format(self.rootname)
 
         # Determine whether processing is needed
         self.skip_processing = len(self.field.imaging_sectors) < 2
 
     def set_parset_parameters(self):
         """
-        Define parameters needed for the pipeline parset template
+        Define parameters needed for the CWL workflow template
         """
         if self.batch_system == 'slurm':
             # For some reason, setting coresMax ResourceRequirement hints does
             # not work with SLURM
             max_cores = None
         else:
             max_cores = self.field.parset['cluster_specific']['max_cores']
@@ -39,15 +39,15 @@
                              'pipeline_working_dir': self.pipeline_working_dir,
                              'max_cores': max_cores,
                              'skip_processing': self.skip_processing,
                              'do_slowgain_solve': self.field.do_slowgain_solve}
 
     def set_input_parameters(self):
         """
-        Define the pipeline inputs
+        Define the CWL workflow inputs
         """
         # Define various input and output filenames
         sector_image_filename = []
         sector_vertices_filename = []
         regridded_image_filename = []
         template_image_filename = []
         self.image_names = ['I_image_file_true_sky', 'I_image_file_apparent_sky',
```

### Comparing `rapthor-1.0/rapthor/operations/predict.py` & `rapthor-1.1/rapthor/operations/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,29 @@
     Operation to predict model data
     """
     def __init__(self, field, index):
         super(Predict, self).__init__(field, name='predict', index=index)
 
     def set_parset_parameters(self):
         """
-        Define parameters needed for the pipeline parset template
+        Define parameters needed for the CWL workflow template
         """
         if self.batch_system == 'slurm':
             # For some reason, setting coresMax ResourceRequirement hints does
             # not work with SLURM
             max_cores = None
         else:
             max_cores = self.field.parset['cluster_specific']['max_cores']
         self.parset_parms = {'rapthor_pipeline_dir': self.rapthor_pipeline_dir,
                              'max_cores': max_cores,
                              'do_slowgain_solve': self.field.do_slowgain_solve}
 
     def set_input_parameters(self):
         """
-        Define the pipeline inputs
+        Define the CWL workflow inputs
         """
         # Make list of sectors for which prediction needs to be done. Any imaging
         # sectors should come first, followed by bright-source, then outlier sectors
         # (as required by the rapthor/scripts/subtract_sector_models.py script)
         sectors = []
         if len(self.field.imaging_sectors) > 1 or self.field.reweight:
             # If we have more than one imaging sector or reweighting is desired,
@@ -85,27 +85,29 @@
         peel_outliers = self.field.peel_outliers
         nr_bright = len(self.field.bright_source_sectors)
         peel_bright = self.field.peel_bright_sources
         reweight = self.field.reweight
         min_uv_lambda = self.field.parset['imaging_specific']['min_uv_lambda']
         max_uv_lambda = self.field.parset['imaging_specific']['max_uv_lambda']
         onebeamperpatch = self.field.onebeamperpatch
+        sagecalpredict = self.field.sagecalpredict
 
         self.input_parms = {'sector_filename': CWLDir(sector_filename).to_json(),
                             'sector_starttime': sector_starttime,
                             'sector_ntimes': sector_ntimes,
                             'sector_model_filename': sector_model_filename,
                             'sector_skymodel': CWLFile(sector_skymodel).to_json(),
                             'sector_patches': sector_patches,
                             'h5parm': CWLFile(self.field.h5parm_filename).to_json(),
                             'obs_solint_sec': obs_solint_sec,
                             'obs_solint_hz': obs_solint_hz,
                             'min_uv_lambda': min_uv_lambda,
                             'max_uv_lambda': max_uv_lambda,
                             'onebeamperpatch': onebeamperpatch,
+                            'sagecalpredict' : sagecalpredict,
                             'obs_filename': CWLDir(obs_filename).to_json(),
                             'obs_starttime': obs_starttime,
                             'obs_infix': obs_infix,
                             'nr_outliers': nr_outliers,
                             'peel_outliers': peel_outliers,
                             'nr_bright': nr_bright,
                             'peel_bright': peel_bright,
```

### Comparing `rapthor-1.0/rapthor/pipeline/execution/concat_ms.cwl` & `rapthor-1.1/rapthor/pipeline/execution/concat_ms.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/execution/fetch_data.cwl` & `rapthor-1.1/rapthor/pipeline/execution/fetch_data.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/execution/hba_nl.cwl` & `rapthor-1.1/rapthor/pipeline/execution/hba_nl.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/execution/run_rapthor.cwl` & `rapthor-1.1/rapthor/pipeline/execution/run_rapthor.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/execution/tar_directory.cwl` & `rapthor-1.1/rapthor/pipeline/execution/tar_directory.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/calibrate_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/calibrate_pipeline.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor calibration pipeline
+label: Rapthor calibration workflow
 doc: |
   This workflow performs direction-dependent calibration. In general,
   calibration is done in three steps: (1) a fast phase-only calibration (with
   core stations constrianed to have the same solutions) to correct for
   ionospheric effects, (2) a joint slow amplitude calibration (with all stations
   constrained to have the same solutions) to correct for beam errors, and (3) a
   further unconstrained slow gain calibration to correct for station-to-station
   differences. Steps (2) and (3) are skipped if the calibration is phase-only.
   This calibration scheme works for both HBA and LBA data. The final products of
-  this pipeline are solution tables (h5parm files), plots, and a-term screens (FITS
+  this workflow are solution tables (h5parm files), plots, and a-term screens (FITS
   files).
 
 requirements:
   ScatterFeatureRequirement: {}
   StepInputExpressionRequirement: {}
 
 {% if max_cores is not none %}
@@ -168,14 +168,19 @@
     type: boolean
 
   - id: parallelbaselines
     doc: |
       Flag that enables parallelization of model computation over baselines.
     type: boolean
 
+  - id: sagecalpredict
+    doc: |
+      Flag that enables model computation using SAGECal.
+    type: boolean
+
   - id: stepsize
     label: Solver step size
     doc: |
       The solver step size used between iterations (length = 1).
     type: float
 
   - id: tolerance
@@ -500,14 +505,16 @@
         source: solverlbfgs_iter
       - id: solverlbfgs_minibatches
         source: solverlbfgs_minibatches
       - id: onebeamperpatch
         source: onebeamperpatch
       - id: parallelbaselines
         source: parallelbaselines
+      - id: sagecalpredict
+        source: sagecalpredict
       - id: stepsize
         source: stepsize
       - id: tolerance
         source: tolerance
       - id: uvlambdamin
         source: uvlambdamin
       - id: smoothnessconstraint
@@ -610,14 +617,16 @@
         source: solverlbfgs_iter
       - id: solverlbfgs_minibatches
         source: solverlbfgs_minibatches
       - id: onebeamperpatch
         source: onebeamperpatch
       - id: parallelbaselines
         source: parallelbaselines
+      - id: sagecalpredict
+        source: sagecalpredict
       - id: stepsize
         source: stepsize
       - id: tolerance
         source: tolerance
       - id: uvlambdamin
         source: uvlambdamin
       - id: smoothnessconstraint
@@ -753,14 +762,16 @@
         source: solverlbfgs_iter
       - id: solverlbfgs_minibatches
         source: solverlbfgs_minibatches
       - id: onebeamperpatch
         source: onebeamperpatch
       - id: parallelbaselines
         source: parallelbaselines
+      - id: sagecalpredict
+        source: sagecalpredict
       - id: stepsize
         source: stepsize
       - id: tolerance
         source: tolerance
       - id: uvlambdamin
         source: uvlambdamin
       - id: smoothnessconstraint
```

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/image_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/image_pipeline.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor imaging pipeline
+label: Rapthor imaging workflow
 doc: |
   This workflow performs imaging with direction-dependent corrections. The
   imaging data are generated (and averaged if possible) and WSClean is
   used to perform the imaging. Masking and sky model filtering is then done
   using PyBDSF.
 
 requirements:
@@ -22,23 +22,31 @@
     type:
       type: array
       items:
         type: array
         items: Directory
 
   - id: prepare_filename
-    label: Filename of imaging MS
+    label: Filename of preparatory MS
     doc: |
-      The filenames of output MS files used for imaging (length = n_obs * n_sectors).
+      The filenames of the preparatory MS files used as input to concatenation
+      (length = n_obs * n_sectors).
     type:
       type: array
       items:
         type: array
         items: string
 
+  - id: concat_filename
+    label: Filename of imaging MS
+    doc: |
+      The filename of the MS file resulting from concatenation of the preparatory
+      files and used for imaging (length = n_sectors).
+    type: string[]
+
   - id: starttime
     label: Start time of each obs
     doc: |
       The start time (in casacore MVTime) for each observation (length = n_obs *
       n_sectors).
     type:
       type: array
@@ -263,14 +271,20 @@
 
   - id: deconvolution_channels
     label: Number of deconvolution channels
     doc: |
       The number of WSClean deconvolution channels (length = n_sectors).
     type: int[]
 
+  - id: fit_spectral_pol
+    label: Spectral poly order
+    doc: |
+      The order of WSClean spectral polynomial (length = n_sectors).
+    type: int[]
+
   - id: wsclean_niter
     label: Number of iterations
     doc: |
       The number of WSClean iterations (length = n_sectors).
     type: int[]
 
   - id: wsclean_nmiter
@@ -368,22 +382,22 @@
       type: array
       items:
         type: array
         items: int
 
 
 outputs:
-  - id: filtered_skymodels
+  - id: filtered_skymodel_true_sky
     outputSource:
-      - image_sector/filtered_skymodels
-    type:
-      type: array
-      items:
-        type: array
-        items: File
+      - image_sector/filtered_skymodel_true_sky
+    type: File[]
+  - id: filtered_skymodel_apparent_sky
+    outputSource:
+      - image_sector/filtered_skymodel_apparent_sky
+    type: File[]
   - id: sector_diagnostics
     outputSource:
       - image_sector/sector_diagnostics
     type: File[]
   - id: sector_images
     outputSource:
       - image_sector/sector_images
@@ -402,22 +416,24 @@
 {% endif %}
 
 
 steps:
   - id: image_sector
     label: Image a sector
     doc: |
-      This step is a subpipeline that performs the processing (imaging, etc) for
+      This step is a subworkflow that performs the processing (imaging, etc) for
       each sector.
     run: {{ pipeline_working_dir }}/subpipeline_parset.cwl
     in:
       - id: obs_filename
         source: obs_filename
       - id: prepare_filename
         source: prepare_filename
+      - id: concat_filename
+        source: concat_filename
       - id: starttime
         source: starttime
       - id: ntimes
         source: ntimes
       - id: image_freqstep
         source: image_freqstep
       - id: image_timestep
@@ -482,14 +498,16 @@
 # end use_facets / not use_facets
 {% endif %}
 # end use_screens / not use_screens
       - id: channels_out
         source: channels_out
       - id: deconvolution_channels
         source: deconvolution_channels
+      - id: fit_spectral_pol
+        source: fit_spectral_pol
       - id: wsclean_niter
         source: wsclean_niter
       - id: wsclean_nmiter
         source: wsclean_nmiter
       - id: robust
         source: robust
       - id: min_uv_lambda
@@ -522,48 +540,49 @@
 {% endif %}
 {% if peel_bright_sources %}
       - id: bright_skymodel_pb
         source: bright_skymodel_pb
 {% endif %}
 {% if use_screens %}
 # start use_screens
-    scatter: [obs_filename, prepare_filename, starttime, ntimes, image_freqstep,
-              image_timestep, previous_mask_filename, mask_filename,
+    scatter: [obs_filename, prepare_filename, concat_filename, starttime, ntimes,
+              image_freqstep, image_timestep, previous_mask_filename, mask_filename,
               phasecenter, ra, dec, image_name, cellsize_deg, wsclean_imsize,
               vertices_file, region_file,
 {% if use_mpi %}
               mpi_cpus_per_task, mpi_nnodes,
 {% endif %}
-              channels_out, deconvolution_channels, wsclean_niter,
-              wsclean_nmiter, robust, min_uv_lambda,
-              max_uv_lambda, do_multiscale, taper_arcsec, wsclean_mem,
-              auto_mask, idg_mode, threshisl, threshpix, dd_psf_grid]
+              channels_out, deconvolution_channels, fit_spectral_pol, wsclean_niter,
+              wsclean_nmiter, robust, min_uv_lambda, max_uv_lambda, do_multiscale,
+              taper_arcsec, wsclean_mem, auto_mask, idg_mode, threshisl, threshpix,
+              dd_psf_grid]
 {% else %}
 # start not use_screens
-    scatter: [obs_filename, prepare_filename, starttime, ntimes, image_freqstep,
-              image_timestep, previous_mask_filename, mask_filename,
+    scatter: [obs_filename, prepare_filename, concat_filename, starttime, ntimes,
+              image_freqstep, image_timestep, previous_mask_filename, mask_filename,
               phasecenter, ra, dec, image_name, cellsize_deg, wsclean_imsize,
               vertices_file, region_file,
 {% if use_mpi %}
               mpi_cpus_per_task, mpi_nnodes,
 {% endif %}
 {% if use_facets %}
               ra_mid, dec_mid, width_ra, width_dec, facet_region_file,
 {% else %}
               central_patch_name,
 {% endif %}
-              channels_out, deconvolution_channels, wsclean_niter,
-              wsclean_nmiter, robust, min_uv_lambda,
-              max_uv_lambda, do_multiscale, taper_arcsec, wsclean_mem,
-              auto_mask, idg_mode, threshisl, threshpix, dd_psf_grid]
+              channels_out, deconvolution_channels, fit_spectral_pol, wsclean_niter,
+              wsclean_nmiter, robust, min_uv_lambda, max_uv_lambda, do_multiscale,
+              taper_arcsec, wsclean_mem, auto_mask, idg_mode, threshisl, threshpix,
+              dd_psf_grid]
 {% endif %}
 # end use_screens / not use_screens
 
     scatterMethod: dotproduct
 
     out:
-      - id: filtered_skymodels
+      - id: filtered_skymodel_true_sky
+      - id: filtered_skymodel_apparent_sky
       - id: sector_images
       - id: sector_diagnostics
 {% if use_facets %}
       - id: region_file
 {% endif %}
```

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/image_sector_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/image_sector_pipeline.cwl`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor imaging subpipeline
+label: Rapthor imaging subworkflow
 doc: |
   This subworkflow performs imaging with direction-dependent corrections. The
   imaging data are generated (and averaged if possible) and WSClean is
   used to perform the imaging. Masking and sky model filtering is then done
   using PyBDSF.
 
 requirements:
@@ -23,19 +23,27 @@
     label: Filenames of input MS
     doc: |
       The filenames of input MS files for which imaging will be done (length =
       n_obs).
     type: Directory[]
 
   - id: prepare_filename
-    label: Filenames of imaging MS
+    label: Filenames of preparatory MSs
     doc: |
-      The filenames of output MS files used for imaging (length = n_obs).
+      The filenames of the preparatory MS files used as input to concatenation
+      (length = n_obs).
     type: string[]
 
+  - id: concat_filename
+    label: Filename of imaging MS
+    doc: |
+      The filename of the MS file resulting from concatenation of the preparatory
+      files and used for imaging (length = 1).
+    type: string
+
   - id: starttime
     label: Start times of each obs
     doc: |
       The start time (in casacore MVTime) for each observation (length = n_obs).
     type: string[]
 
   - id: ntimes
@@ -228,14 +236,20 @@
 
   - id: deconvolution_channels
     label: Number of deconvolution channels
     doc: |
       The number of WSClean deconvolution channels (length = 1).
     type: int
 
+  - id: fit_spectral_pol
+    label: Spectral poly order
+    doc: |
+      The order of WSClean spectral polynomial (length = 1).
+    type: int
+
   - id: wsclean_niter
     label: Number of iterations
     doc: |
       The number of WSClean iterations (length = 1).
     type: int
 
   - id: wsclean_nmiter
@@ -329,21 +343,25 @@
     doc: |
       The number of direction-dependent PSFs which should be fit horizontally and
       vertically in the image (length = 2).
     type: int[]
 
 
 outputs:
-  - id: filtered_skymodels
+  - id: filtered_skymodel_true_sky
     outputSource:
-      - filter/skymodels
-    type: File[]
+      - filter/filtered_skymodel_true_sky
+    type: File
+  - id: filtered_skymodel_apparent_sky
+    outputSource:
+      - filter/filtered_skymodel_apparent_sky
+    type: File
   - id: sector_diagnostics
     outputSource:
-      - filter/diagnostics
+      - find_diagnostics/diagnostics
     type: File
   - id: sector_images
     outputSource:
 {% if peel_bright_sources %}
       - restore_nonpb/restored_image
       - restore_pb/restored_image
 {% else %}
@@ -418,14 +436,27 @@
         source: central_patch_name
     scatter: [msin, msout, starttime, ntimes, freqstep, timestep]
 {% endif %}
     scatterMethod: dotproduct
     out:
       - id: msimg
 
+  - id: concat_in_time
+    label: Concatenate MS file in time
+    doc: |
+      This step concatenates the imaging MS files in time.
+    run: {{ rapthor_pipeline_dir }}/steps/concat_ms_files_in_time.cwl
+    in:
+      - id: mslist
+        source: prepare_imaging_data/msimg
+      - id: msout
+        source: concat_filename
+    out:
+      - id: msconcat
+
   - id: premask
     label: Make an image mask
     doc: |
       This step makes a FITS mask for the imaging.
     run: {{ rapthor_pipeline_dir }}/steps/blank_image.cwl
     in:
       - id: imagefile
@@ -515,15 +546,15 @@
     hints:
       ResourceRequirement:
         coresMin: {{ max_cores }}
         coresMax: {{ max_cores }}
 {% endif %}
     in:
       - id: msin
-        source: prepare_imaging_data/msimg
+        source: concat_in_time/msconcat
       - id: name
         source: image_name
       - id: mask
         source: premask/maskimg
 {% if use_mpi %}
       - id: ntasks
         source: mpi_cpus_per_task
@@ -564,14 +595,16 @@
         source: do_multiscale
       - id: cellsize_deg
         source: cellsize_deg
       - id: channels_out
         source: channels_out
       - id: deconvolution_channels
         source: deconvolution_channels
+      - id: fit_spectral_pol
+        source: fit_spectral_pol
       - id: taper_arcsec
         source: taper_arcsec
       - id: wsclean_mem
         source: wsclean_mem
       - id: auto_mask
         source: auto_mask
       - id: idg_mode
@@ -643,36 +676,69 @@
       - id: restored_image
 {% endif %}
 # end peel_bright_sources
 
   - id: filter
     label: Filter sources
     doc: |
-      This step uses PyBDSF to filter artifacts from the sky model and make
-      a clean mask for the next iteration, as well as derive various image
-      diagnostics.
+      This step uses PyBDSF to filter artifacts from the sky model.
     run: {{ rapthor_pipeline_dir }}/steps/filter_skymodel.cwl
     in:
 {% if peel_bright_sources %}
-      - id: input_image
+      - id: true_sky_image
+        source: restore_pb/restored_image
+      - id: flat_noise_image
         source: restore_nonpb/restored_image
-      - id: input_bright_skymodel_pb
+      - id: bright_true_sky_skymodel
         source: bright_skymodel_pb
 {% else %}
-      - id: input_image
+      - id: true_sky_image
+        source: image/image_pb_name
+      - id: flat_noise_image
         source: image/image_nonpb_name
 {% endif %}
-      - id: input_skymodel_pb
+      - id: true_sky_skymodel
         source: image/skymodel_pb
       - id: output_root
         source: image_name
       - id: vertices_file
         source: vertices_file
       - id: threshisl
         source: threshisl
       - id: threshpix
         source: threshpix
       - id: beamMS
-        source: prepare_imaging_data/msimg
+        source: obs_filename
+    out:
+      - id: filtered_skymodel_true_sky
+      - id: filtered_skymodel_apparent_sky
+      - id: diagnostics
+      - id: flat_noise_rms_image
+      - id: true_sky_rms_image
+      - id: source_catalog
+
+  - id: find_diagnostics
+    label: Find image diagnostics
+    doc: |
+      This step derives various image diagnostics.
+    run: {{ rapthor_pipeline_dir }}/steps/calculate_image_diagnostics.cwl
+    in:
+      - id: flat_noise_image
+        source: image/image_nonpb_name
+      - id: flat_noise_rms_image
+        source: filter/flat_noise_rms_image
+      - id: true_sky_image
+        source: image/image_pb_name
+      - id: true_sky_rms_image
+        source: filter/true_sky_rms_image
+      - id: input_catalog
+        source: filter/source_catalog
+      - id: input_skymodel
+        source: filter/filtered_skymodel_true_sky
+      - id: output_root
+        source: image_name
+      - id: obs_ms
+        source: obs_filename
+      - id: diagnostics_file
+        source: filter/diagnostics
     out:
-      - id: skymodels
       - id: diagnostics
```

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/mosaic_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/mosaic_pipeline.cwl`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor mosaicking pipeline
+label: Rapthor mosaicking workflow
 doc: |
-  This workflow performs the mosaicking of images made with the imaging pipeline.
+  This workflow performs the mosaicking of images made with the imaging workflow.
   If only a single image was made, processing is (mostly) skipped.
 
 {% if not skip_processing %}
 # start not skip_processing
 
 requirements:
   MultipleInputFeatureRequirement: {}
@@ -76,15 +76,15 @@
       - mosaic_by_type/mosaic_image
     type: File[]
 
 steps:
   - id: mosaic_by_type
     label: Mosiac an image type
     doc: |
-      This step is a subpipeline that performs the processing for each image
+      This step is a subworkflow that performs the processing for each image
       type.
     run: {{ pipeline_working_dir }}/subpipeline_parset.cwl
     in:
     - id: sector_image_filename
       source: sector_image_filename
     - id: sector_vertices_filename
       source: sector_vertices_filename
```

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/mosaic_type_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/mosaic_type_pipeline.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor mosaicking subpipeline
+label: Rapthor mosaicking subworkflow
 doc: |
   This subworkflow performs the mosaicking of a single type of image made with the
-  imaging pipeline. If only a single image was made, processing is (mostly) skipped.
+  imaging workflow. If only a single image was made, processing is (mostly) skipped.
 
 requirements:
   ScatterFeatureRequirement: {}
   StepInputExpressionRequirement: {}
 
 {% if max_cores is not none %}
 hints:
```

### Comparing `rapthor-1.0/rapthor/pipeline/parsets/predict_pipeline.cwl` & `rapthor-1.1/rapthor/pipeline/parsets/predict_pipeline.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cwlVersion: v1.2
 class: Workflow
-label: Rapthor prediction pipeline
+label: Rapthor prediction workflow
 doc: |
   This workflow performs direction-dependent prediction of sector sky models and
   subracts the resulting model data from the input data, reweighting if desired.
   The resulting data are suitable for imaging.
 
 requirements:
   ScatterFeatureRequirement: {}
@@ -47,29 +47,34 @@
 
   - id: onebeamperpatch
     doc: |
       Flag that determines whether to apply the beam once per patch or per each
       source (length = 1).
     type: boolean
 
+  - id: sagecalpredict
+    doc: |
+      Flag that enables prediction using SAGECAl.
+    type: boolean
+
   - id: sector_patches
     label: Names of sector calibration patches
     doc: |
       A list of lists giving the names of the calibration patches for each sector
       (length = n_obs * n_sectors).
     type:
       type: array
       items:
         type: array
         items: string
 
   - id: h5parm
     label: Filename of solution table
     doc: |
-      The filename of the h5parm solution table from the calibration pipeline (length
+      The filename of the h5parm solution table from the calibration workflow (length
       = 1).
     type: File
 
   - id: sector_skymodel
     label: Filename of sky model
     doc: |
       The filename of the input sky model text file of each sector (length = n_obs
@@ -196,14 +201,16 @@
         source: sector_model_filename
       - id: starttime
         source: sector_starttime
       - id: ntimes
         source: sector_ntimes
       - id: onebeamperpatch
         source: onebeamperpatch
+      - id: sagecalpredict
+        source: sagecalpredict
       - id: h5parm
         source: h5parm
       - id: sourcedb
         source: sector_skymodel
       - id: directions
         source: sector_patches
       - id: numthreads
@@ -215,15 +222,15 @@
 
   - id: subtract_sector_models
     label: Subtract the model uv data
     doc: |
       This step subtracts the model uv data generated in the previous step from the
       input MS files. For each sector, all sources that lie outside of the sector are
       subtracted (or peeled), generating data suitable for use as input to the imaging
-      pipeline. Reweighting by the residuals can also be done, by generating data in
+      workflow. Reweighting by the residuals can also be done, by generating data in
       which all sources have been subtracted.
     run: {{ rapthor_pipeline_dir }}/steps/subtract_sector_models.cwl
 {% if max_cores is not none %}
     hints:
       ResourceRequirement:
         coresMin: {{ max_cores }}
         coresMax: {{ max_cores }}
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/adjust_h5parm_sources.cwl` & `rapthor-1.1/rapthor/pipeline/steps/adjust_h5parm_sources.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/blank_image.cwl` & `rapthor-1.1/rapthor/pipeline/steps/blank_image.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/collect_h5parms.cwl` & `rapthor-1.1/rapthor/pipeline/steps/collect_h5parms.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/combine_h5parms.cwl` & `rapthor-1.1/rapthor/pipeline/steps/combine_h5parms.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,20 @@
       separate: False
   - id: parallelbaselines
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
   - id: stepsize
     type: float
     inputBinding:
       prefix: solve.stepsize=
       separate: False
   - id: tolerance
     type: float
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_debug.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_debug.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_joint.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_joint.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,20 @@
       separate: False
   - id: parallelbaselines 
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
   - id: stepsize
     type: float
     inputBinding:
       prefix: solve.stepsize=
       separate: False
   - id: tolerance
     type: float
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_separate.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_separate.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,20 @@
       separate: False
   - id: parallelbaselines
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
   - id: stepsize
     type: float
     inputBinding:
       prefix: solve.stepsize=
       separate: False
   - id: tolerance
     type: float
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_complexgain_separate_no_joint.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_complexgain_separate_no_joint.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,20 @@
       separate: False
   - id: parallelbaselines
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
   - id: stepsize
     type: float
     inputBinding:
       prefix: solve.stepsize=
       separate: False
   - id: tolerance
     type: float
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_scalarcomplexgain.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_scalarcomplexgain.cwl`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,20 @@
       separate: False
   - id: parallelbaselines
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
   - id: stepsize
     type: float
     inputBinding:
       prefix: solve.stepsize=
       separate: False
   - id: tolerance
     type: float
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/ddecal_solve_scalarphase.cwl` & `rapthor-1.1/rapthor/pipeline/steps/ddecal_solve_scalarphase.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
       Flag that enables parallel prediction over baselines.
     type: boolean
     inputBinding:
       prefix: solve.parallelbaselines=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
 
+  - id: sagecalpredict
+    label: predict using SAGECal
+    doc: |
+      Flag that enables prediction using SAGECal.
+    type: boolean
+    inputBinding:
+      prefix: solve.sagecalpredict=
+      valueFrom: "$(self ? 'True': 'False')"
+      separate: False
+
   - id: stepsize
     label: Solver step size
     doc: |
       The solver step size used between iterations.
     type: float
     inputBinding:
       prefix: solve.stepsize=
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/filter_skymodel.cwl` & `rapthor-1.1/rapthor/pipeline/steps/filter_skymodel.cwl`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 cwlVersion: v1.2
 class: CommandLineTool
 baseCommand: [filter_skymodel.py]
 label: Filter a sky model
 doc: |
-  This tool uses PyBDSF to filter artifacts from the sky model and make
-  a clean mask for the next iteration.
+  This tool uses PyBDSF to filter artifacts from the sky model and
+  to attenuate the source flux densities to make an apparent-sky
+  sky model.
 
 requirements:
   - class: InlineJavascriptRequirement
   - class: InitialWorkDirRequirement
     listing:
-      - entry: $(inputs.input_image)
+      - entry: $(inputs.flat_noise_image)
+        writable: true
+      - entry: $(inputs.true_sky_image)
         writable: true
-
 
 inputs:
-  - id: input_image
-    label: Input image
+  - id: flat_noise_image
+    label: Detection image
     doc: |
-      The filename of the input FITS image.
+      The filename of the input FITS image used for source detection.
     type: File
     inputBinding:
       position: 1
-  - id: input_skymodel_pb
+  - id: true_sky_image
+    label: Input image
+    doc: |
+      The filename of the input primary-beam-corrected FITS image.
+    type: File
+    inputBinding:
+      position: 2
+  - id: true_sky_skymodel
     label: PB-corrected model
     doc: |
       The filename of the input primary-beam-corrected sky model.
     type: File
     inputBinding:
-      position: 2
+      position: 3
   - id: output_root
     label: Output root name
     doc: |
       The root of the filenames of the output filtered sky models.
     type: string
     inputBinding:
-      position: 3
+      position: 4
   - id: vertices_file
     label: Filename of vertices file
     doc: |
       The filename of the file containing sector vertices.
     type: File
     inputBinding:
-      position: 4
-  - id: input_bright_skymodel_pb
+      position: 5
+  - id: beamMS
+    label: Filenames of MS files for beam
+    doc: |
+      The filenames of the MS files to use for beam calculations. These MS files
+      should have the original phase center of the observation.
+    type: Directory[]
+    inputBinding:
+      position: 6
+      itemSeparator: ","
+  - id: bright_true_sky_skymodel
     label: Bright-source PB-corrected model
     doc: |
       The filename of the input bright-source primary-beam-corrected sky model. Should
       not be given if peeling of bright sources was not done.
     type: File?
     inputBinding:
-      prefix: --input_bright_skymodel_pb=
+      prefix: --bright_true_sky_skymodel=
       separate: false
   - id: threshisl
     label: Island threshold
     doc: |
       The PyBDSF island threshold.
     type: float
     inputBinding:
@@ -64,37 +82,56 @@
     label: Pixel threshold
     doc: |
       The PyBDSF pixel threshold.
     type: float
     inputBinding:
       prefix: --threshpix=
       separate: false
-  - id: beamMS
-    label: Filename of MS file for beam
-    doc: |
-      The filenames of the MS files to use for beam calculations.
-    type: Directory[]
-    inputBinding:
-      prefix: --beamMS=
-      itemSeparator: ","
-      separate: false
 
 outputs:
-  - id: skymodels
-    label: Processed sky models, mask files, and images
+  - id: filtered_skymodel_true_sky
+    label: Processed true-sky sky model
     doc: |
-      The filenames of the filtered sky models, the generated mask files, and images.
-    type: File[]
+      The filename of the filtered true-sky sky model.
+    type: File
+    outputBinding:
+      glob: '$(inputs.output_root).true_sky.txt'
+  - id: filtered_skymodel_apparent_sky
+    label: Processed apparent-sky sky model
+    doc: |
+      The filename of the filtered apparent-sky sky model.
+    type: File
     outputBinding:
-      glob: ['$(inputs.output_root)-MFS-*.fits', '$(inputs.output_root)-MFS-*.mask', '$(inputs.output_root).*_sky.txt']
+      glob: '$(inputs.output_root).apparent_sky.txt'
   - id: diagnostics
     label: Image diagnostics
     doc: |
-      The image diagnostics, including RMS noise, dynamic range, frequency, and beam.
+      The image diagnostics, including number of sources.
     type: File
     outputBinding:
       glob: '$(inputs.output_root).image_diagnostics.json'
+  - id: flat_noise_rms_image
+    label: Flat-noise RMS image
+    doc: |
+      The flat-niose RMS image generated by PyBDSF.
+    type: File
+    outputBinding:
+      glob: '$(inputs.output_root).flat_noise_rms.fits'
+  - id: true_sky_rms_image
+    label: True-sky RMS image
+    doc: |
+      The true-sky RMS image generated by PyBDSF.
+    type: File
+    outputBinding:
+      glob: '$(inputs.output_root).true_sky_rms.fits'
+  - id: source_catalog
+    label: Source FITS catalog
+    doc: |
+      The source catalog generated by PyBDSF.
+    type: File
+    outputBinding:
+      glob: '$(inputs.output_root).source_catalog.fits'
 
 
 hints:
   - class: DockerRequirement
     dockerPull: 'astronrd/rapthor'
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/make_aterm_images.cwl` & `rapthor-1.1/rapthor/pipeline/steps/make_aterm_images.cwl`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     inputBinding:
       prefix: --bounds_mid_deg=
       separate: false
   - id: ncpu
     label: Number of CPUs
     doc: |
       The number of CPUs / cores to use.
-    type: string
+    type: int
     inputBinding:
       prefix: --ncpu=
       separate: false
 
 outputs:
   - id: output_images
     type: File[]
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/make_mosaic.cwl` & `rapthor-1.1/rapthor/pipeline/steps/make_mosaic.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/make_mosaic_template.cwl` & `rapthor-1.1/rapthor/pipeline/steps/make_mosaic_template.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/make_region_file.cwl` & `rapthor-1.1/rapthor/pipeline/steps/make_region_file.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/merge_array_directories.cwl` & `rapthor-1.1/rapthor/pipeline/steps/merge_array_directories.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/merge_array_files.cwl` & `rapthor-1.1/rapthor/pipeline/steps/merge_array_files.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/plot_solutions.cwl` & `rapthor-1.1/rapthor/pipeline/steps/plot_solutions.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/predict_model_data.cwl` & `rapthor-1.1/rapthor/pipeline/steps/predict_model_data.cwl`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
   InlineJavascriptRequirement: {}
 
 arguments:
   - msin.datacolumn=DATA
   - msout.overwrite=True
   - msout.writefullresflag=False
   - steps=[predict]
-  - predict.type=h5parmpredict  # needed to do multi-direction predict
   - predict.operation=replace
   - predict.applycal.correction=phase000
   - predict.applycal.steps=[slowamp,totalphase]
   - predict.applycal.slowamp.correction=amplitude000
   - predict.applycal.totalphase.correction=phase000
   - predict.usebeammodel=True
   - predict.beammode=array_factor
@@ -71,14 +70,24 @@
       Flag that sets beam correction per patch or per source.
     type: boolean
     inputBinding:
       prefix: predict.onebeamperpatch=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
 
+  - id: sagecalpredict
+    label: Use SAGECal predict
+    doc: |
+      Flag that enables prediction using SAGECal.
+    type: boolean
+    inputBinding:
+      prefix: predict.type=
+      valueFrom: "$(self ? 'sagecalpredict': 'h5parmpredict')"
+      separate: False
+
   - id: h5parm
     label: Solution table
     doc: |
       The solution table to use to corrupt the model visibilities.
     type: File
     inputBinding:
       prefix: predict.applycal.parmdb=
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/predict_model_data_phase_only.cwl` & `rapthor-1.1/rapthor/pipeline/steps/predict_model_data_phase_only.cwl`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
   InlineJavascriptRequirement: {}
 
 arguments:
   - msin.datacolumn=DATA
   - msout.overwrite=True
   - msout.writefullresflag=False
   - steps=[predict]
-  - predict.type=h5parmpredict
   - predict.operation=replace
   - predict.applycal.correction=phase000
   - predict.applycal.steps=[fastphase]
   - predict.applycal.fastphase.correction=phase000
   - predict.usebeammodel=True
   - predict.beammode=array_factor
   - msout.storagemanager=Dysco
@@ -49,14 +48,23 @@
       separate: False
   - id: onebeamperpatch
     type: boolean
     inputBinding:
       prefix: predict.onebeamperpatch=
       valueFrom: "$(self ? 'True': 'False')"
       separate: False
+  - id: sagecalpredict
+    label: Use SAGECal predict
+    doc: |
+      Flag that enables prediction using SAGECal.
+    type: boolean
+    inputBinding:
+      prefix: predict.type=
+      valueFrom: "$(self ? 'sagecalpredict': 'h5parmpredict')"
+      separate: False
   - id: h5parm
     type: File
     inputBinding:
       prefix: predict.applycal.parmdb=
       separate: False
   - id: sourcedb
     type: File
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data.cwl` & `rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data_no_screens.cwl` & `rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data_no_screens.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/prepare_imaging_data_no_screens_phase_only.cwl` & `rapthor-1.1/rapthor/pipeline/steps/prepare_imaging_data_no_screens_phase_only.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/process_slow_gains.cwl` & `rapthor-1.1/rapthor/pipeline/steps/process_slow_gains.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/regrid_image.cwl` & `rapthor-1.1/rapthor/pipeline/steps/regrid_image.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/split_h5parms.cwl` & `rapthor-1.1/rapthor/pipeline/steps/split_h5parms.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/pipeline/steps/subtract_sector_models.cwl` & `rapthor-1.1/rapthor/pipeline/steps/subtract_sector_models.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 class: CommandLineTool
 baseCommand: [subtract_sector_models.py]
 label: Subtracts sector model data
 doc: |
   This tool subtracts sector model uv data from the input MS files. For each
   sector, all sources that lie outside of the sector are subtracted (or
   peeled), generating data suitable for use as input to the imaging
-  pipeline. Reweighting by the residuals can also be done, by generating
+  workflow. Reweighting by the residuals can also be done, by generating
   data in which all sources have been subtracted.
 
 requirements:
   - class: InlineJavascriptRequirement
 
 arguments:
   - '--weights_colname=WEIGHT_SPECTRUM'
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_image_facets.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_image_facets.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     prefix: -parallel-deconvolution
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
     prefix: -local-rms-method
   - valueFrom: '120'
@@ -44,15 +42,15 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    type: Directory[]
+    type: Directory
     inputBinding:
       position: 5
   - id: name
     type: string
     inputBinding:
       prefix: -name
   - id: mask
@@ -102,14 +100,18 @@
     type: int
     inputBinding:
       prefix: -channels-out
   - id: deconvolution_channels
     type: int
     inputBinding:
       prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     type: float
     inputBinding:
       prefix: -taper-gaussian
   - id: wsclean_mem
     type: float
     inputBinding:
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_image_no_dde.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_image_no_dde.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,14 @@
     prefix: -temp-dir
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '4'
-    prefix: -deconvolution-channels
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
     prefix: -local-rms-method
   - valueFrom: 'briggs'
@@ -42,15 +38,15 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    type: Directory[]
+    type: Directory
     inputBinding:
       position: 3
   - id: name
     type: string
     inputBinding:
       prefix: -name
   - id: mask
@@ -89,14 +85,22 @@
     type: float
     inputBinding:
       prefix: -scale
   - id: channels_out
     type: int
     inputBinding:
       prefix: -channels-out
+  - id: deconvolution_channels
+    type: int
+    inputBinding:
+      prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     type: float
     inputBinding:
       prefix: -taper-gaussian
   - id: wsclean_mem
     type: float
     inputBinding:
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_image_screens.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_image_screens.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
     prefix: -temp-dir
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '2048'
     prefix: -parallel-deconvolution
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
@@ -58,18 +56,18 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    label: Filenames of input MS
+    label: Filename of input MS
     doc: |
-      The filenames of input MS files for which imaging will be done.
-    type: Directory[]
+      The filename of input MS file for which imaging will be done.
+    type: Directory
     inputBinding:
       position: 3
   - id: name
     label: Filename of output image
     doc: |
       The root filename of the output image.
     type: string
@@ -158,14 +156,18 @@
   - id: deconvolution_channels
     label: Number of deconvolution channels
     doc: |
       The number of deconvolution channels.
     type: int
     inputBinding:
       prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     label: Taper value
     doc: |
       The taper value in arcsec.
     type: float
     inputBinding:
       prefix: -taper-gaussian
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_facets.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_facets.cwl`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
     prefix: -parallel-deconvolution
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
     prefix: -local-rms-method
   - valueFrom: '120'
@@ -49,15 +47,15 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    type: Directory[]
+    type: Directory
     inputBinding:
       position: 5
   - id: name
     type: string
     inputBinding:
       prefix: -name
   - id: mask
@@ -107,14 +105,18 @@
     type: int
     inputBinding:
       prefix: -channels-out
   - id: deconvolution_channels
     type: int
     inputBinding:
       prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     type: float
     inputBinding:
       prefix: -taper-gaussian
   - id: wsclean_mem
     type: float
     inputBinding:
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_no_dde.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_no_dde.cwl`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,14 @@
     prefix: -temp-dir
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '4'
-    prefix: -deconvolution-channels
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
     prefix: -local-rms-method
   - valueFrom: 'briggs'
@@ -47,15 +43,15 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    type: Directory[]
+    type: Directory
     inputBinding:
       position: 3
   - id: name
     type: string
     inputBinding:
       prefix: -name
   - id: mask
@@ -94,14 +90,22 @@
     type: float
     inputBinding:
       prefix: -scale
   - id: channels_out
     type: int
     inputBinding:
       prefix: -channels-out
+  - id: deconvolution_channels
+    type: int
+    inputBinding:
+      prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     type: float
     inputBinding:
       prefix: -taper-gaussian
   - id: wsclean_mem
     type: float
     inputBinding:
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_mpi_image_screens.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_mpi_image_screens.cwl`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,14 @@
     prefix: -temp-dir
   - valueFrom: 'I'
     prefix: -pol
   - valueFrom: '0.85'
     prefix: -mgain
   - valueFrom: '0.8'
     prefix: -multiscale-scale-bias
-  - valueFrom: '3'
-    prefix: -fit-spectral-pol
   - valueFrom: '2048'
     prefix: -parallel-deconvolution
   - valueFrom: '1.0'
     prefix: -auto-threshold
   - valueFrom: '50'
     prefix: -local-rms-window
   - valueFrom: 'rms-with-min'
@@ -67,15 +65,15 @@
     # correctly if it's given together with 'briggs'. We force the parts to be adjacent
     # using the position arg here and below
     prefix: -weight
     position: 1
 
 inputs:
   - id: msin
-    type: Directory[]
+    type: Directory
     inputBinding:
       position: 3
   - id: name
     type: string
     inputBinding:
       prefix: -name
   - id: mask
@@ -128,14 +126,18 @@
     type: int
     inputBinding:
       prefix: -channels-out
   - id: deconvolution_channels
     type: int
     inputBinding:
       prefix: -deconvolution-channels
+  - id: fit_spectral_pol
+    type: int
+    inputBinding:
+      prefix: -fit-spectral-pol
   - id: taper_arcsec
     type: float
     inputBinding:
       prefix: -taper-gaussian
   - id: wsclean_mem
     type: float
     inputBinding:
```

### Comparing `rapthor-1.0/rapthor/pipeline/steps/wsclean_restore.cwl` & `rapthor-1.1/rapthor/pipeline/steps/wsclean_restore.cwl`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/process.py` & `rapthor-1.1/rapthor/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,17 +66,24 @@
             # Mosaic the sectors, for now just Stokes I
             # TODO: run mosaic ops for IQUV+residuals
             op = Mosaic(field, index+1)
             op.run()
 
         # Check for selfcal convergence/divergence
         if field.do_check:
+            log.info("Checking selfcal convergence...")
             has_converged, has_diverged = field.check_selfcal_progress()
-            if has_converged or has_diverged:
-                # Stop the cycle
+            if not has_converged and not has_diverged:
+                # Continue selfcal
+                log.info("Improvement in image noise, dynamic range, and/or number of "
+                         "sources exceeds that set by the convergence ratio of "
+                         "{0}.".format(field.convergence_ratio))
+                log.info("Continuing selfcal...")
+            else:
+                # Stop selfcal
                 if has_converged:
                     log.info("Selfcal has converged (improvement in image noise, dynamic "
                              "range, and number of sources does not exceed that set by the "
                              "convergence ratio of {0})".format(field.convergence_ratio))
                 if has_diverged:
                     log.warning("Selfcal has diverged (ratio of current image noise "
                                 "to previous value is > {})".format(field.divergence_ratio))
```

### Comparing `rapthor-1.0/rapthor/scripts/adjust_h5parm_sources.py` & `rapthor-1.1/rapthor/scripts/adjust_h5parm_sources.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/blank_image.py` & `rapthor-1.1/rapthor/scripts/blank_image.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/combine_h5parms.py` & `rapthor-1.1/rapthor/scripts/combine_h5parms.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/make_aterm_images.py` & `rapthor-1.1/rapthor/scripts/make_aterm_images.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/make_mosaic.py` & `rapthor-1.1/rapthor/scripts/make_mosaic.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/make_mosaic_template.py` & `rapthor-1.1/rapthor/scripts/make_mosaic_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Script to make a template image for mosaicking
 """
 import argparse
 from argparse import RawTextHelpFormatter
-from rapthor.lib.image import FITSImage
+from rapthor.lib.fitsimage import FITSImage
 from rapthor.lib import miscellaneous as misc
 from astropy.io import fits as pyfits
 from astropy.wcs import WCS as pywcs
 import numpy as np
 
 
 def main(input_image_list, vertices_file_list, output_image, skip=False, padding=1.1):
```

### Comparing `rapthor-1.0/rapthor/scripts/make_region_file.py` & `rapthor-1.1/rapthor/scripts/make_region_file.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/process_slow_gains.py` & `rapthor-1.1/rapthor/scripts/process_slow_gains.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/regrid_image.py` & `rapthor-1.1/rapthor/scripts/regrid_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """
 Script to regrid a FITS image
 """
 import argparse
 from argparse import RawTextHelpFormatter
 from rapthor.lib import miscellaneous as misc
-from rapthor.lib.image import FITSImage
+from rapthor.lib.fitsimage import FITSImage
 from reproject import reproject_interp
 from astropy.io import fits as pyfits
 from astropy.wcs import WCS as pywcs
 import numpy as np
 import os
 import shutil
```

### Comparing `rapthor-1.0/rapthor/scripts/split_h5parms.py` & `rapthor-1.1/rapthor/scripts/split_h5parms.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/scripts/subtract_sector_models.py` & `rapthor-1.1/rapthor/scripts/subtract_sector_models.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/rapthor/skymodels/3C196-pandey.skymodel` & `rapthor-1.1/rapthor/skymodels/3C196-pandey.skymodel`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/setup.py` & `rapthor-1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,92 @@
-from setuptools import setup, Command
-import os
-import rapthor._version
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools>=45",
+    "setuptools_scm[toml]>=6.2",
+    "wheel",
+]
+
+[project]
+name = "rapthor"
+authors = [
+    {name = "David Rafferty", email = "drafferty@hs.uni-hamburg.de"},
+    {name = "Marcel Loose", email = "loose@astron.nl"},
+    {name = "Andre Offringa", email = "offringa@astron.nl"},
+    {name = "Arend G. Dijkstra", email = "adijkstra@astron.nl"},
+    {name = "Tammo Jan Dijkema", email = "dijkema@astron.nl"},
+    {name = "Mark de Wever", email = "mark.dewever@stcorp.nl"},
+    {name = "Frits Sweijen", email = "sweijen@astron.nl"},
+    {name = "Sarod Yatawatta", email = "yatawatta@astron.nl"},
+]
+description = "Rapthor: LOFAR DDE Pipeline"
+readme = "README.md"
+requires-python = ">=3.7"
+license = {file = "LICENSE"}
+classifiers=[
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Natural Language :: English",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: Astronomy",
+]
+dependencies = [
+    "astropy",
+    "bdsf",
+    "importlib-metadata; python_version<'3.8'",
+    "jinja2",
+    "losoto",
+    "lsmtool",
+    "numpy",
+    "python-casacore",
+    "python-dateutil",
+    "reproject",
+    "Rtree",
+    "scipy",
+    "shapely",
+    "toil[cwl]>=5.10",
+]
+dynamic = ["version"]
+
+[tool.setuptools]
+# package-data is specified below in section [tool.setuptools.package-data]
+include-package-data = false
+packages = [
+    "rapthor",
+    "rapthor.lib",
+    "rapthor.operations",
+]
+script-files = [
+    "bin/concat_linc_files",
+    "bin/plotrapthor",
+    "bin/rapthor",
+    "rapthor/scripts/adjust_h5parm_sources.py",
+    "rapthor/scripts/blank_image.py",
+    "rapthor/scripts/calculate_image_diagnostics.py",
+    "rapthor/scripts/combine_h5parms.py",
+    "rapthor/scripts/concat_ms.py",
+    "rapthor/scripts/filter_skymodel.py",
+    "rapthor/scripts/make_aterm_images.py",
+    "rapthor/scripts/make_mosaic.py",
+    "rapthor/scripts/make_mosaic_template.py",
+    "rapthor/scripts/make_region_file.py",
+    "rapthor/scripts/mpi_runner.sh",
+    "rapthor/scripts/process_slow_gains.py",
+    "rapthor/scripts/regrid_image.py",
+    "rapthor/scripts/split_h5parms.py",
+    "rapthor/scripts/subtract_sector_models.py",
+]
+
+[tool.setuptools.package-data]
+rapthor = [
+    "pipeline/**",
+    "scripts/*",
+    "skymodels/*"
+]
 
-description = 'Rapthor: LOFAR DDE Pipeline'
-long_description = description
-if os.path.exists('README.md'):
-    with open('README.md') as f:
-        long_description = f.read()
+# [tool.setuptools.dynamic]
+# version = {attr = "rapthor._version.__version__"}
 
-
-class PyTest(Command):
-    user_options = []
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        import sys
-        import subprocess
-        errno = subprocess.call([sys.executable, 'runtests.py'])
-        raise SystemExit(errno)
-
-
-setup(
-    name='rapthor',
-    version=rapthor._version.__version__,
-    url='https://git.astron.nl/RD/rapthor',
-    description=description,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    platforms='any',
-    classifiers=['Programming Language :: Python :: 3',
-                 'Development Status :: 4 - Beta',
-                 'Natural Language :: English',
-                 'Intended Audience :: Science/Research',
-                 'Operating System :: POSIX :: Linux',
-                 'Topic :: Scientific/Engineering :: Astronomy'],
-    # toil[cwl]!=5.6 because of https://github.com/DataBiosphere/toil/issues/4101
-    # toil[cwl]!=5.8 because of https://gitter.im/bd2k-genomics-toil/Lobby?at=63d7f912ec2bfc62867d36e6
-    install_requires=['numpy', 'scipy', 'astropy', 'jinja2', 'shapely',
-                      'toil[cwl]!=5.6,!=5.8', 'reproject', 'python-dateutil',
-                      'Rtree', 'lsmtool', 'losoto', 'bdsf',
-                      'python-casacore'],
-    python_requires=">=3.7",
-    scripts=['bin/rapthor',
-             'bin/plotrapthor',
-             'bin/concat_linc_files',
-             'rapthor/scripts/adjust_h5parm_sources.py',
-             'rapthor/scripts/blank_image.py',
-             'rapthor/scripts/combine_h5parms.py',
-             'rapthor/scripts/concat_ms.py',
-             'rapthor/scripts/filter_skymodel.py',
-             'rapthor/scripts/make_aterm_images.py',
-             'rapthor/scripts/make_region_file.py',
-             'rapthor/scripts/make_mosaic.py',
-             'rapthor/scripts/make_mosaic_template.py',
-             'rapthor/scripts/process_slow_gains.py',
-             'rapthor/scripts/regrid_image.py',
-             'rapthor/scripts/subtract_sector_models.py',
-             'rapthor/scripts/split_h5parms.py',
-             'rapthor/scripts/mpi_runner.sh'],
-    packages=['rapthor', 'rapthor.operations', 'rapthor.lib'],
-    package_data={'rapthor': ['pipeline/*/*.cwl',
-                              'scripts/*',
-                              'skymodels/*']},
-    cmdclass={'test': PyTest})
+[tool.setuptools_scm]
+write_to = "rapthor/_version.py"
```

### Comparing `rapthor-1.0/test/test_facet.py` & `rapthor-1.1/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `rapthor-1.0/test/test_field.py` & `rapthor-1.1/test/test_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             self.downloadms(testmsname)
         else:
             print('ms file found')
 
         self.par = parset_read('resources/test.parset')
         self.field = Field(self.par)
         self.field.scan_observations()
-        self.field.make_skymodels('resources/test_true_sky.txt', skymodel_apparent_sky='resources/test_apparent_sky.txt', target_flux=0.1)
+        self.field.update_skymodels(1, True, target_flux=0.2)
         self.field.set_obs_parameters()
         self.field.define_imaging_sectors()
         self.field.define_outlier_sectors(1)
 
     @classmethod
     def tearDownClass(self):
         os.system('rm -r images/ logs/ pipelines/ regions/ scratch/ skymodels/ solutions/')
```

### Comparing `rapthor-1.0/test/test_screen.py` & `rapthor-1.1/test/test_screen.py`

 * *Files identical despite different names*

