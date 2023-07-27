# Comparing `tmp/cosmosis-2.5.1.tar.gz` & `tmp/cosmosis-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-2.5.1.tar", last modified: Thu May 25 17:04:56 2023, max compression
+gzip compressed data, was "cosmosis-3.0.tar", last modified: Thu Jul 27 14:15:44 2023, max compression
```

## Comparing `cosmosis-2.5.1.tar` & `cosmosis-3.0.tar`

### file list

```diff
@@ -1,280 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.371160 cosmosis-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-25 17:04:55.000000 cosmosis-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-25 17:04:55.000000 cosmosis-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 17:04:56.371160 cosmosis-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 17:04:55.000000 cosmosis-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.331160 cosmosis-2.5.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-05-25 17:04:55.000000 cosmosis-2.5.1/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-05-25 17:04:55.000000 cosmosis-2.5.1/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-25 17:04:55.000000 cosmosis-2.5.1/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-05-25 17:04:55.000000 cosmosis-2.5.1/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-05-25 17:04:55.000000 cosmosis-2.5.1/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.335160 cosmosis-2.5.1/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.335160 cosmosis-2.5.1/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.339160 cosmosis-2.5.1/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.339160 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17838 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.343160 cosmosis-2.5.1/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.343160 cosmosis-2.5.1/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7217 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.347160 cosmosis-2.5.1/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16163 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48757 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.347160 cosmosis-2.5.1/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.347160 cosmosis-2.5.1/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    56629 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.347160 cosmosis-2.5.1/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7265 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6726 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4715 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.351160 cosmosis-2.5.1/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4790 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.355160 cosmosis-2.5.1/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.355160 cosmosis-2.5.1/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.355160 cosmosis-2.5.1/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.355160 cosmosis-2.5.1/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.355160 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.359160 cosmosis-2.5.1/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.359160 cosmosis-2.5.1/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4537 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.359160 cosmosis-2.5.1/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.359160 cosmosis-2.5.1/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.359160 cosmosis-2.5.1/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.363160 cosmosis-2.5.1/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11516 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.367160 cosmosis-2.5.1/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.371160 cosmosis-2.5.1/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_module4.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 17:04:55.000000 cosmosis-2.5.1/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:56.335160 cosmosis-2.5.1/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 17:04:56.000000 cosmosis-2.5.1/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-25 17:04:56.000000 cosmosis-2.5.1/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:04:56.000000 cosmosis-2.5.1/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 17:04:56.000000 cosmosis-2.5.1/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 17:04:56.000000 cosmosis-2.5.1/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 17:04:55.000000 cosmosis-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:04:56.371160 cosmosis-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-25 17:04:55.000000 cosmosis-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-27 14:15:42.000000 cosmosis-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-27 14:15:42.000000 cosmosis-3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 14:15:44.823149 cosmosis-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 14:15:42.000000 cosmosis-3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.799148 cosmosis-3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-27 14:15:42.000000 cosmosis-3.0/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5362 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.807148 cosmosis-3.0/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7452 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4683 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4578 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.811149 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.815148 cosmosis-3.0/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.819149 cosmosis-3.0/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11469 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/example_module4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.823149 cosmosis-3.0/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 14:15:42.000000 cosmosis-3.0/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:44.803148 cosmosis-3.0/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 14:15:44.000000 cosmosis-3.0/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 14:15:42.000000 cosmosis-3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:15:44.823149 cosmosis-3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-27 14:15:42.000000 cosmosis-3.0/setup.py
```

### Comparing `cosmosis-2.5.1/LICENSE` & `cosmosis-3.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2014-22 The CosmoSIS Team
+Copyright 2014-23 The CosmoSIS Team
 
 The CosmoSIS core is licensed as described below.  Some individual components within the software have their own licenses - see the notices in their directories.  Notably, Polychord and Multinest are licensed only for academic use.
 
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `cosmosis-2.5.1/MANIFEST.in` & `cosmosis-3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/bin/cosmosis-configure` & `cosmosis-3.0/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/bin/cosmosis-extract` & `cosmosis-3.0/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/bin/cosmosis-sample-fisher` & `cosmosis-3.0/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/__init__.py` & `cosmosis-3.0/cosmosis/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .main import run_cosmosis
 from .runtime import MPIPool, LikelihoodPipeline, FunctionModule, \
                      stdout_redirected, Inifile, CosmosisConfigurationError, \
-                     MPIPool, Module, FunctionModule, ClassModule
+                     MPIPool, Module, FunctionModule, ClassModule, logs
 from .samplers import Sampler
 from . import samplers
 from .version import __version__
 from .datablock import option_section, DataBlock
 from .gaussian_likelihood import GaussianLikelihood, \
                                  SingleValueGaussianLikelihood, \
                                  WindowedGaussianLikelihood
```

### Comparing `cosmosis-2.5.1/cosmosis/config/compilers.mk` & `cosmosis-3.0/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/configure.py` & `cosmosis-3.0/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/constants.py` & `cosmosis-3.0/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/Makefile` & `cosmosis-3.0/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.0/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/c_datablock.h` & `cosmosis-3.0/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/clamp.hh` & `cosmosis-3.0/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.0/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.0/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.0/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.0/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.0/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.0/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.0/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.0/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.0/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/datablock.cc` & `cosmosis-3.0/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/datablock.hh` & `cosmosis-3.0/cosmosis/datablock/datablock.hh`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,18 @@
 // use from C++, which is permitted to throw exceptions, and again
 // with an interface that is guaranteed never to throw exceptions.
 //
 // The C interface does not provide direct access to the memory
 // controlled by the DataBlock; it provides the user with a copy of
 // the data, copied to a memory location of the user's
 // specification. For any array obtained from the DataBlock, the C
-// user must deallocate the array when he is done with it. The
+// user must deallocate the array when done with it. The
 // deallocation does not need to be done for arrays that are on the
 // stack, into which DataBlock copies the data.
 //
-//  TODO: Add support for 2-dimensional arrays of the numeric types.
-//
 //----------------------------------------------------------------------
 
 #include <string>
 #include <map>
 #include <cctype>
 #include <ostream>
```

### Comparing `cosmosis-2.5.1/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.0/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.0/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/datablock_status.h` & `cosmosis-3.0/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/entry.cc` & `cosmosis-3.0/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/entry.hh` & `cosmosis-3.0/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/generate_sections.py` & `cosmosis-3.0/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/handler.c` & `cosmosis-3.0/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/ndarray.hh` & `cosmosis-3.0/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/section.cc` & `cosmosis-3.0/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/section.hh` & `cosmosis-3.0/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/section_names.h` & `cosmosis-3.0/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/datablock/section_names.txt` & `cosmosis-3.0/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/gaussian_likelihood.py` & `cosmosis-3.0/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/main.py` & `cosmosis-3.0/cosmosis/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,67 +7,64 @@
 import argparse
 import os
 import pdb
 import cProfile
 from .runtime.config import Inifile, CosmosisConfigurationError
 from .runtime.pipeline import LikelihoodPipeline
 from .runtime import mpi_pool
+from .runtime import logs
 from .runtime import process_pool
-from .runtime.utils import ParseExtraParameters, stdout_redirected, import_by_path
+from .runtime.utils import ParseExtraParameters, stdout_redirected, import_by_path, under_over_line, underline, overline
 from .samplers.sampler import Sampler, ParallelSampler, Hints
 from . import output as output_module
 from .runtime.handler import activate_segfault_handling
 from .version import __version__
 
 
 RUNTIME_INI_SECTION = "runtime"
 
 
-def demo_1_special (args):
-    if "demo1.ini" in args.inifile:
+def demo_1_special (inifile):
+    if "demo1.ini" in inifile:
         print("""
 Congratulations: you have just run cosmosis demo one!
 
 You can make plots of the outputs of this using this command:
     cosmosis-postprocess demos/demo1.ini -o outputs/demo1
 
 Then you can try out the other demos...
 ... and read the information about plotting their output and what they are doing online.
 Please get in touch with any problems, ideally by filing an Issue. Thanks!
 """)
 
 
-def demo_10_special (args):
-    if   "demo10.ini" in args.inifile   and   not os.getenv ("HALOFIT", ""):
+def demo_10_special(inifile):
+    if   "demo10.ini" in inifile   and   not os.getenv ("HALOFIT", ""):
         print()
         print("Welcome to demo10!")
         print()
         print("**PLEASE NOTE**:")
         print()
         print("There are two flavours of this demo, selected through an ")
         print("environment variable called `HALOFIT'; this variable is not ")
         print("currently set, so we are giving it the value `takahashi'.")
 
         os.environ ["HALOFIT"] = "takahashi"
 
 
 
-def demo_20a_special (args):
-    if  "demo20a.ini" in args.inifile:
+def demo_20a_special(inifile):
+    if  "demo20a.ini" in inifile:
         print ()
         print ("You have completed demo20a, now run demo20b and compare")
         print ("results with demo5!")
 
 
-def demo_20b_special (args):
-    if   "demo20b.ini" in args.inifile   and   not os.path.isfile ("./demo20a.txt"):
-        print ()
-        print ("********************************************************")
-        print ("*** YOU MUST RUN demo20a BEFORE YOU CAN RUN demo20b. ***")
-        print ("********************************************************")
+    if   "demo20b.ini" in inifile   and   not os.path.isfile ("./demo20a.txt"):
+        print(under_over_line("YOU MUST RUN demo20a BEFORE YOU CAN RUN demo20b.", chr='*'))
 
 def sampler_main_loop(sampler, output, pool, is_root):
     # Run the sampler until convergence
     # which really means "finished" here - 
     # a sampler can "converge" just by reaching the 
     # limit of the number of samples it is allowed.
     if is_root:
@@ -116,102 +113,190 @@
         if isinstance(priors_file, Inifile):
             prior_ini = priors_file
         else:
             prior_ini=Inifile(priors_file)
         prior_ini.write(comment_wrapper)
     output.comment("END_OF_PRIORS_INI")
 
-def setup_output(sampler_class, sampler_number, ini, pool, number_samplers, sample_method, resume):
+def setup_output(sampler_class, sampler_number, ini, pool, number_samplers, sample_method, resume, output):
+
+    output_original = output
 
     needs_output = sampler_class.needs_output and \
        (pool is None or pool.is_master() or sampler_class.parallel_output)
 
     if not needs_output:
         return None
 
+    if output_original is None:
+        #create the output files and methods.
+        try:
+            output_options = dict(ini.items('output'))
+        except configparser.NoSectionError:
+            raise ValueError("ERROR:\nFor the sampler (%s) you chose in the [runtime] section of the ini file I also need an [output] section describing how to save results\n\n"%sample_method)
+        #Additionally we tell the output here if
+        #we are parallel or not.
+        if (pool is not None) and (sampler_class.parallel_output):
+            output_options['rank'] = pool.rank
+            output_options['parallel'] = pool.size
+
+        #Give different output filenames to the different sampling steps
+        #Only change if this is not the last sampling step - the final
+        #one retains the name in the output file.
+        # Change, e.g. demo17.txt to demo17.fisher.txt
+        if ("filename" in output_options) and (sampler_number<number_samplers-1):
+            filename = output_options['filename']
+            filename, ext = os.path.splitext(filename)
+            filename += '.' + sampler_class.name
+            filename += ext
+            output_options['filename'] = filename
+
+        if ("filename" in output_options):
+            print("* Saving output -> {}".format(output_options['filename']))
+
+        #Generate the output from a factory
+        output = output_module.output_from_options(output_options, resume)
+    elif isinstance(output_original, output_module.OutputBase):
+        output = output_original
+    elif isinstance(output_original, str):
+        if output_original == "astropy":
+            output = output_module.AstropyOutput()
+        elif output_original == "none":
+            output = output_module.NullOutput()
+        elif output_original == "in_memory":
+            output = output_module.InMemoryOutput()
+        else:
+            raise ValueError(f"Unknown output option {output_original}")
+    else:
+        raise ValueError(f"Unknown output type {type(output_original)}")
+        
 
-    #create the output files and methods.
-    try:
-        output_options = dict(ini.items('output'))
-    except configparser.NoSectionError:
-        raise ValueError("ERROR:\nFor the sampler (%s) you chose in the [runtime] section of the ini file I also need an [output] section describing how to save results\n\n"%sample_method)
-    #Additionally we tell the output here if
-    #we are parallel or not.
-    if (pool is not None) and (sampler_class.parallel_output):
-        output_options['rank'] = pool.rank
-        output_options['parallel'] = pool.size
-
-    #Give different output filenames to the different sampling steps
-    #Only change if this is not the last sampling step - the final
-    #one retains the name in the output file.
-    # Change, e.g. demo17.txt to demo17.fisher.txt
-    if ("filename" in output_options) and (sampler_number<number_samplers-1):
-        filename = output_options['filename']
-        filename, ext = os.path.splitext(filename)
-        filename += '.' + sampler_class.name
-        filename += ext
-        output_options['filename'] = filename
-
-
-    #Generate the output from a factory
-    output = output_module.output_from_options(output_options, resume)
     output.metadata("sampler", sample_method)
 
-    if ("filename" in output_options):
-        print("* Saving output -> {}".format(output_options['filename']))
-
     return output
 
 
-def run_cosmosis(args, pool=None, ini=None, pipeline=None, values=None, priors=None):
+def run_cosmosis(ini, pool=None, pipeline=None, values=None, priors=None, override=None,
+                 profile_mem=0, profile_cpu="", variables=None, only=None, output=None):
+    """
+    Execute cosmosis.
+
+    Parameters
+    ----------
+    ini: str, cosmosis.Inifile, or None
+        The parameter file from which to build the cosmosis run. If set to a string the
+        file is read from disc. If set to None, the other parameters must contain
+        all the required CosmoSIS parameters.
+    
+    pool: None, cosmosis.MPIPool, or cosmosis.process_pool.Pool
+        A pool object to enable multi-process parallel execution. If left as the default
+        None then the code is run with a single process (though modules may still run
+        using OpenMP parallelism).
+    
+    pipeline: None or cosmosis.LikelihoodPipeline
+        If set, ignore the pipeline definition in the ini file and use this pipeline
+        instead.
+    
+    values: None or dict[str, str]->str
+        If set, ignore the numerical parameter values in the ini file and use these 
+        instead.
+    
+    priors: None or dict[str, str]->str
+        If set, ignore the prior values in the ini file and use these 
+        instead. 
+
+    override: None or dict[str, str]->str
+        If set, override parameter values in the ini file from the dictionary.
+    
+    profile_mem: int
+        If changed from the default zero value, print a memory profile every 
+        profile_mem seconds.
+
+    profile_cpu: str
+        If changed from the default empty string, print CPU profile information
+        and also save to the named file. If running in parallel, save to 
+        {profile_cpu}.{rank}.
+    
+    variables: None or dict[str, str]->str
+        If set, override variable values in the ini file from the dictionary.
+
+    only: None or str
+        If set, fix all the variable values except the one supplied.
+
+    output: None or cosmosis.Output
+        If set, use this output object to save the results. If not set, create
+        an output object from the ini file.
+    """
     no_subprocesses = os.environ.get("COSMOSIS_NO_SUBPROCESS", "") not in ["", "0"]
-    # In case we need to hand-hold a naive demo-10 user.
+
+    smp = isinstance(pool, process_pool.Pool)
 
     # Load configuration.
     is_root = (pool is None) or pool.is_master()
-    if ini is None:
-        ini = Inifile(args.inifile, override=args.params, print_include_messages=is_root)
+    ini_is_str = isinstance(ini, str)
+    ini_original = ini
+    output_original = output
+    ini = Inifile(ini, override=override, print_include_messages=is_root)
 
     pre_script = ini.get(RUNTIME_INI_SECTION, "pre_script", fallback="")
     post_script = ini.get(RUNTIME_INI_SECTION, "post_script", fallback="")
 
+    verbosity = ini.get(RUNTIME_INI_SECTION, "verbosity", fallback="")
+    
+    if not verbosity:
+        if ini.has_option("pipeline", "quiet"):
+            quiet = ini.getboolean("pipeline", "quiet", fallback=False)
+            verbosity = "quiet" if quiet else "standard"
+        else:
+            verbosity = ini.get(RUNTIME_INI_SECTION, "output", fallback="standard")
+    logs.set_verbosity(verbosity)
+
+    if ini.has_option("pipeline", "quiet") and is_root:
+        logs.warning("Deprecated: The [pipeline] quiet option is deprecated.  Set [runtime] verbosity instead.")
+
     if is_root and pre_script:
         if no_subprocesses:
             print("Warning: subprocesses not allowed on this system as")
             print("COSMOSIS_NO_SUBPROCESS variable was set.")
             print("Ignoring pre-script.")
         else:
             status = os.WEXITSTATUS(os.system(pre_script))
             if status:
                 raise RuntimeError("The pre-run script {} retuned non-zero status {}".format(
                     pre_script, status))
 
-    if is_root and args.mem:
+    if is_root and profile_mem:
         from cosmosis.runtime.memmon import MemoryMonitor
         # This launches a memory monitor that prints out (from a new thread)
-        # the memory usage every args.mem seconds
-        mem = MemoryMonitor.start_in_thread(interval=args.mem)
+        # the memory usage every profile_mem seconds
+        mem = MemoryMonitor.start_in_thread(interval=profile_mem)
 
-    if args.profile:
+    if profile_cpu:
         profile = cProfile.Profile()
         profile.enable()
 
     # Create pipeline.
     if pipeline is None:
         cleanup_pipeline = True
         pool_stdout = ini.getboolean(RUNTIME_INI_SECTION, "pool_stdout", fallback=False)
+        if is_root:
+            if ini_is_str:
+                print(underline(f"Setting up pipeline from parameter file {ini_original}"))
+            else:
+                print(underline(f"Setting up pipeline from pre-constructed configuration"))
+
         if is_root or pool_stdout:
-            pipeline = LikelihoodPipeline(ini, override=args.variables, values=values, only=args.only, priors=priors)
+            pipeline = LikelihoodPipeline(ini, override=variables, values=values, only=only, priors=priors)
         else:
-            # Suppress output on everything except the master process
             if pool_stdout:
-                pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only, priors=priors)
+                pipeline = LikelihoodPipeline(ini, override=variables, only=only, priors=priors)
             else:
+                # Suppress output on everything except the root process
                 with stdout_redirected():
-                    pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only, priors=priors)
+                    pipeline = LikelihoodPipeline(ini, override=variables, only=only, priors=priors)
 
         if pipeline.do_fast_slow:
             pipeline.setup_fast_subspaces()
     else:
         # We should not cleanup a pipeline which we didn't make
         cleanup_pipeline = False
 
@@ -281,24 +366,30 @@
             # Switch off the main cosmosis resume mechanism
             resume = False
 
         # Not all samplers can be resumed.
         if resume and not sampler_class.supports_resume:
             print("NOTE: You set resume=T in the [runtime] section but the sampler {} does not support resuming yet.  I will ignore this option.".format(sampler_name))
             resume=False
-
+        
 
         if is_root:
-            print("****************************")
+            print("****************************************************")
             print("* Running sampler {}/{}: {}".format(sampler_number+1,number_samplers, sampler_name))
+            if pool and smp:
+                print(f"* Using multiprocessing (SMP) with {pool.size} processes.")
+            elif pool:
+                print(f"* Using MPI with {pool.size} processes.")
+            else:
+                print("* Running in serial mode.")
 
-        output = setup_output(sampler_class, sampler_number, ini, pool, number_samplers, sample_method, resume)
+        output = setup_output(sampler_class, sampler_number, ini, pool, number_samplers, sample_method, resume, output_original)
 
         if is_root:
-            print("****************************")
+            print("****************************************************")
 
         #Initialize our sampler, with the class we got above.
         #It needs an extra pool argument if it is a ParallelSampler.
         #All the parallel samplers can also act serially too.
         if pool and sampler_class.is_parallel_sampler:
             sampler = sampler_class(ini, pipeline, output, pool)
         else:
@@ -315,39 +406,60 @@
             sampler_class.supports_resume and \
             (is_root or sampler_class.parallel_output):
            sampler.resume()
 
         if output:
             write_header_output(output, ini, values, pipeline)
 
+        sys.stdout.flush()
+        sys.stderr.flush()
+
 
         sampler_main_loop(sampler, output, pool, is_root)
         distribution_hints.update(sampler.distribution_hints)
 
+        # get total number of evaluations on all MPI processes
+        if pool is None:
+            run_count_total = pipeline.run_count
+            run_count_ok_total = pipeline.run_count_ok
+        else:
+            run_count_total = pool.comm.allreduce(pipeline.run_count)
+            run_count_ok_total = pool.comm.allreduce(pipeline.run_count_ok)
+        
+        if is_root and sampler_name != 'test':
+            logs.overview(f"Total posterior evaluations = {run_count_total} across all processes")
+            logs.overview(f"Successful posterior evaluations = {run_count_ok_total} across all processes")
+            if output:
+                output.final("evaluations", run_count_total)
+                output.final("successes", run_count_total)
+                output.final("complete", "1")
+
+
         if output:
             output.close()
 
     if cleanup_pipeline:
         pipeline.cleanup()
 
-    if args.profile:
+    if profile_cpu:
         profile.disable()
-        if (pool is not None) and (not args.smp):
-            profile_name = args.profile + f'.{pool.rank}'
+        if (pool is not None) and (not smp):
+            profile_name = profile_cpu + f'.{pool.rank}'
         else:
-            profile_name = args.profile
+            profile_name = profile_cpu
         profile.dump_stats(profile_name)
         profile.print_stats("cumtime")
 
-    if is_root and args.mem:
+    if is_root and profile_mem:
         mem.stop()
 
-    # Extra-special actions we take to mollycoddle a brand-new user!
-    demo_1_special (args)
-    demo_20a_special (args)
+    # Extra-special actions we take to help new users playing with the demos
+    demo_1_special(str(ini))
+    demo_10_special(str(ini))
+    demo_20a_special (str(ini))
 
     # User can specify in the runtime section a post-run script to launch.
     # In general this may be less useful than the pre-run script, because
     # often chains time-out instead of actually completing.
     # But we still offer it
     if post_script and is_root:
         # This decodes the exist status
@@ -355,17 +467,23 @@
             print("Warning: subprocesses not allowed on this system as")
             print("COSMOSIS_NO_SUBPROCESS variable was set.")
             print("Ignoring post-script.")
         else:
             status = os.WEXITSTATUS(os.system(post_script))
             if status:
                 sys.stdout.write("WARNING: The post-run script {} failed with error {}".format(
-                    post_script, error))
+                    post_script, status))
 
-    return 0
+    if isinstance(output_original, str):
+        if output_original == "astropy":
+            return 0, output.table
+        else:
+            return 0, output
+    else:
+        return 0
 
 
 def make_graph(inifile, dotfile, params=None, variables=None):
     """
     Make a graphviz "dot" format file, describing the pipeline
     and how data is passed from section to section.
 
@@ -412,42 +530,35 @@
     try:
         args = parser.parse_args(sys.argv[1:])
 
         if args.graph:
             make_graph(args.inifile, args.graph, args.params, args.variables)
             return 0
 
-        demo_10_special (args)
-        demo_20b_special (args)
-
         if args.segfaults:
             activate_segfault_handling()
 
         # initialize parallel workers
         if args.mpi:
             with mpi_pool.MPIPool() as pool:
-                return run_cosmosis(args,pool)
+                return run_cosmosis(ini=args.inifile, pool=pool, override=args.params, profile_mem=args.mem, profile_cpu=args.profile, variables=args.variables, only=args.only)
         elif args.smp:
             with process_pool.Pool(args.smp) as pool:
-                return run_cosmosis(args,pool)
+                return run_cosmosis(ini=args.inifile, pool=pool, override=args.params, profile_mem=args.mem, profile_cpu=args.profile, variables=args.variables, only=args.only)
         else:
             try:
-                return run_cosmosis(args)
+                return run_cosmosis(ini=args.inifile, pool=None, override=args.params, profile_mem=args.mem, profile_cpu=args.profile, variables=args.variables, only=args.only)
             except Exception as error:
                 if args.pdb:
                     print("There was an exception - starting python debugger because you ran with --pdb")
                     print(error)
                     pdb.post_mortem()
                 else:
                     raise
     except CosmosisConfigurationError as e:
         print(e)
         return 1
 
-    # Extra-special actions we take to mollycoddle a brand-new user!
-    demo_1_special (args)
-    demo_20a_special (args)
-
 
 if __name__=="__main__":
     status = main()
     sys.exit(status)
```

### Comparing `cosmosis-2.5.1/cosmosis/output/cosmomc_output.py` & `cosmosis-3.0/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/output/fits_output.py` & `cosmosis-3.0/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/output/in_memory_output.py` & `cosmosis-3.0/cosmosis/output/in_memory_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,7 +34,9 @@
         if resume:
             raise ValueError("Cannot resume from in-memory output")
         return cls()
 
     @classmethod
     def load_from_options(cls, options):
         raise ValueError("No output was saved from this run")
+
+
```

### Comparing `cosmosis-2.5.1/cosmosis/output/null_output.py` & `cosmosis-3.0/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/output/output_base.py` & `cosmosis-3.0/cosmosis/output/output_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import abc
-import logging
 import numpy as np
 import fcntl
-import datetime
-import os
 
 output_registry = {}
-LOG_LEVEL_NOISY = 15
 
 class OutputMetaclass(abc.ABCMeta):
     def __init__(cls, name, b, d):
         abc.ABCMeta.__init__(cls, name, b, d)
         if name == "OutputBase":
             return
         if not name.endswith("Output"):
@@ -43,27 +39,14 @@
     def __init__(self):
         super(OutputBase,self).__init__()
         self._columns = []
         self.closed=False
         self.begun_sampling = False
         self.resumed = False
 
-    def log_debug(self, message, *args, **kwargs):
-        logging.debug(message, *args, **kwargs)
-    def log_noisy(self, message, *args, **kwargs):
-        logging.log(LOG_LEVEL_NOISY, message, *args, **kwargs)
-    def log_info(self, message, *args, **kwargs):
-        logging.info(message, *args, **kwargs)
-    def log_warning(self, message, *args, **kwargs):
-        logging.warning(message, *args, **kwargs)
-    def log_error(self, message, *args, **kwargs):
-        logging.error(message, *args, **kwargs)
-    def log_critical(self, message, *args, **kwargs):
-        logging.critical(message, *args, **kwargs)
-
     @property
     def columns(self):
         return self._columns
 
     @columns.setter
     def columns(self, columns):
         self._columns = columns
@@ -95,15 +78,15 @@
         return [c[0] for c in self._columns]
 
     def comment(self, comment):
         """
         Save a comment.  Ordering will be preserved
         if you save multiple ones.
         """
-        self._write_comment(comment)
+        self._write_comment(comment.strip('\n'))
 
     def parameters(self, *param_groups):
         """ 
         Tell the outputter to save a vector of parameters.
 
         You can pass in either arrays/lists, which will
         be concatenated together, or mix in some scalars
```

### Comparing `cosmosis-2.5.1/cosmosis/output/text_output.py` & `cosmosis-3.0/cosmosis/output/text_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 
         self._filename = filename + self.FILE_EXTENSION
 
         dirname, _ = os.path.split(self._filename)
         mkdir(dirname)
 
         if resume and utils.file_exists_and_is_empty(self._filename):
-            print("You set resume=T but the file {} is empty so I will start afresh".format(self._filename))
+            print("* You set resume=T but the file {} is empty so I will start afresh".format(self._filename))
             self._file = open(self._filename, "w")
             self.resumed = False
         elif resume and os.path.exists(self._filename):
-            print("Note: You set resume=T so I will resume from file {}".format(self._filename))
+            print("* Note: You set resume=T so I will resume from file {}".format(self._filename))
             self._file = open(self._filename, "r+")
             # Jump to the end of the file
             self._file.seek(0,2)
             self.resumed = True
         else:
             if resume:
-                print("Note: You set resume=T but the file {} does not exist so I will start a new one".format(self._filename))
+                print("* Note: You set resume=T but the file {} does not exist so I will start a new one".format(self._filename))
             self._file = open(self._filename, "w")
             self.resumed = False
         if lock:
             try:
                 self.lock_file(self._file)
             except IOError:
                 error_msg = """
```

### Comparing `cosmosis-2.5.1/cosmosis/output/utils.py` & `cosmosis-3.0/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/plotting/chain_plots.py` & `cosmosis-3.0/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/plotting/grid_plots.py` & `cosmosis-3.0/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/plotting/plotter.py` & `cosmosis-3.0/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/__init__.py` & `cosmosis-3.0/cosmosis/postprocessing/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .inputs import read_input
+from .main import run_cosmosis_postprocess
 from .postprocess import (
     postprocessor_for_sampler,
     MetropolisHastingsProcessor,
     EmceeProcessor,
     ZeusProcessor,
     KombineProcessor,
     PymcProcessor,
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.0/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,16 @@
     #and then override to supply their own plot content
     def plot(self):
         pylab.figure(self.figure.number)
 
     #Need not be over-ridden
     def save(self):
         pylab.figure(self.figure.number)
-        if not self.quiet: print("Saving ", self.outfile)
+        if not self.quiet:
+            print("Saving ", self.outfile)
         pylab.savefig(self.outfile)
 
     #Need not be overridden. Called by the main function
     @classmethod
     def make(cls, dirname, outdir, prefix, suffix):
         p = cls(dirname, outdir, prefix, suffix)
         p.plot()
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/density.py` & `cosmosis-3.0/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/elements.py` & `cosmosis-3.0/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/inputs.py` & `cosmosis-3.0/cosmosis/postprocessing/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,48 @@
 def read_input(filename, force_text=False, weighted=False):
     """
     Read cosmosis output data, either by:
      - specifying a cosmosis .txt output file
      - specifying a cosmosis .ini input file that includes the output file specification
      - specifying a directory containing cosmosis test sampler output
      - specifying a non-cosmosis output file containing samples or weighted samples
-
+     - passing in an astropy table of the chain
 
     Params:
         filename: string, paths to any of the options described above
         force_text: bool, default=False - regardless of the file ending assume it is text columns
         weighted: bool, default=False - if a non-cosmosis file is passed, assume that its samples have weights
     Returns:
         sampler - string with the name of the sampler in
         ini - a dictionary of information containing the output and metadata, suitable for instantiating a postprocessor.
     """
-    if filename.endswith("txt") or force_text:
+    if "astropy" in str(type(filename)):
+        from astropy.table import Table
+        if not isinstance(filename, Table):
+            raise ValueError("If you pass in an astropy table it must be an astropy table")
+        metadata = filename.meta
+        sampler = metadata.get("sampler")
+        # in this case the table already contains all the information we need
+        ini = filename
+
+    elif filename.endswith("txt") or force_text:
         output_info = TextColumnOutput.load_from_options({"filename":filename})
         metadata=output_info[2][0]
         sampler = metadata.get("sampler")
         if sampler is None:
             print("This is not a cosmosis output file.")
             print("So I will assume it is a generic MCMC file")
             if weighted:
                 sampler = "weighted_metropolis"
             else:
                 sampler = "metropolis"
             ini = output_info
         else:
             ini = {"sampler":sampler, sampler:metadata, "data":output_info, "output":dict(format="text", filename=filename)}
+
     elif filename.endswith("fits"):
         output_info = FitsOutput.load_from_options({"filename":filename})
         metadata=output_info[2][0]
         sampler = metadata.get("sampler")
         if sampler is None:
             print("This is not a cosmosis output file.")
             print("So I will assume it is a generic MCMC file")
@@ -58,8 +68,9 @@
         ini.set("runtime", "sampler", sampler)
         ini.set("test", "save_dir", filename)
     else:
         #Determine the sampler and get the class
         #designed to postprocess the output of that sampler
         ini = Inifile(filename)
         sampler = ini.get("runtime", "sampler")
+
     return sampler, ini
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/latex.ini` & `cosmosis-3.0/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.0/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/plots.py` & `cosmosis-3.0/cosmosis/postprocessing/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -611,40 +611,49 @@
         xcut0 = xcut.min()
         xcut1 = xcut.max() + 1
         ycut0 = ycut.min()
         ycut1 = ycut.max() + 1
         return xout[xcut0:xcut1], yout[ycut0:ycut1], like[xcut0:xcut1, ycut0:ycut1]
 
     def make_corner_plot(self, figure=None):
-        from matplotlib.ticker import AutoMinorLocator, AutoLocator, ScalarFormatter
-        from matplotlib.axis import Ticker
-
         pairs = list(self.parameter_pairs())
 
         # parameters, in the order we will use
         params = list(dict.fromkeys([p[0] for p in pairs]))
         nparam = len(params)
         fig, filename = self.figure("corner")
 
-        # enlarge for this extra big figure
-        size = min(4 * nparam, 24)
-        fig.set_size_inches(size, size)
+        # If we are making a corner plot with two different chains
+        # then there may be different parameters in the two of them.
+        # In that case just inherit the parameters from the first one.
+        if fig.get_axes():
+            params = fig._cosmosis_params
+            nparam = len(params)
+            axes = fig._cosmosis_axes
+            new = False
+        else:
+            # enlarge for this extra big figure
+            size = min(4 * nparam, 24)
+            fig.set_size_inches(size, size)
+            axes = fig.subplots(nparam, nparam, squeeze=False)
+            fig._cosmosis_params = params[:]
+            fig._cosmosis_axes = axes
+            new = True
 
-        axes = fig.subplots(nparam, nparam, squeeze=False)
         for i in range(nparam):
             for j in range(nparam):
                 ax = axes[i, j]
 
                 # Switch on minor ticks and have them point inwards like sensible people
                 ax.tick_params(direction='in', which='both', bottom=True, left=True)
                 ax.tick_params(which='minor', length=5, bottom=True, left=True)
                 ax.minorticks_on()
 
                 # Remove upper right above diagonal
-                if j > i:
+                if j > i and new:
                     fig.delaxes(ax)
                     continue
 
                 p1 = params[j]
                 p2 = params[i]
                 if i == j:
                     # Left column only has a y-label, and others also have no y tick labels
@@ -659,27 +668,28 @@
                         ax.set_xlabel(self.latex(p2))
                     else:
                         ax.xaxis.set_ticklabels([])
 
                     if nparam > 10:
                         ax.xaxis.set_ticklabels([])
 
+                    if p1 not in self.cache:
+                        continue
+
                     # Use the same 1D information as in the 1D plots
                     x, like = self.cache[p1]
 
                     # Plot and set the limits explicitly.
                     # Trying to use the sharex / sharey feature here is painful
                     # because we want to remove the diagonal, and that seems to make
                     # the tick stuff really fiddly.
                     ax.plot(x, like / like.max(), color=self.line_color())
                     ax.set_xlim(x.min(), x.max())
                     ax.set_ylim(0, 1.1)
 
-                    # ax.tick_params(axis='both', which='minor', bottom=True, left=True)
-
                 else:
                     # We might have done the swap thing, in which case
                     # check both directions.
                     # If the user has done some funny things with the --only or --either
                     # parameters then things might get funny here, so allow missing panels.
                     try:
                         x, y, like, levels = self.cache[p1, p2]
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.0/cosmosis/postprocessing/postprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,24 +298,30 @@
 	sampler="dynesty"
 
 	def weight_col(self):
 		if hasattr(self, "_weight_col"):
 			return self._weight_col
 		w = self.get_col("log_weight")
 		w = np.exp(w - w.max())
-		self._weight_col = w / w.sum()
+		# w = w[w>0]
+		self._good_index = w > 0
+		self._weight_col = (w / w.sum())[self._good_index]
 		return self._weight_col
 
 	def reduced_col(self, name, stacked=True):
 		col = self.get_col(name)
-		return col
+		self.weight_col()
+		x = col[self._good_index]
+		return x
 
 class NautilusProcess(DynestyProcessor):
 	sampler = "nautilus"
 
+		
+
 
 class PMCPostProcessor(WeightedMetropolisProcessor):
 	sampler="pmc"
 	elements = [
 		plots.WeightedMetropolisPlots,
 		statistics.WeightedMetropolisStatistics,
 		#statistics.WeightedMetropolisHastingsCovariance,
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.0/cosmosis/postprocessing/postprocess_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from . import elements
 from . import plots
 from . import statistics
 import numpy as np
 from cosmosis import output as output_module
-from ..runtime.config import Inifile
-import imp
+from ..runtime import Inifile
+from ..runtime.utils import import_by_path
 import os
 postprocessor_registry = {}
 
 from io import StringIO
 
 
 class PostProcessMetaclass(abc.ABCMeta):
@@ -79,19 +79,20 @@
         self.data = new_data
 
 
 
     def derive_extra_columns(self):
         if not self.derive_file: return
         name = os.path.splitext(os.path.split(self.derive_file)[1])[0]
-        module = imp.load_source(name, self.derive_file)
+        module = import_by_path(name, self.derive_file)
         functions = [getattr(module,f) for f in dir(module) if f.startswith('derive_')]
         print("Deriving new columns from these functions in {}:".format(self.derive_file))
         for f in functions:
             self.derive_extra_column(f)
+
     def load_tuple(self, inputs):
         self.colnames, self.data, self.metadata, self.comments, self.final_metadata = inputs
         self.name = "Data"
         for chain in self.metadata:
             for key,val in list(chain.items()):
                 self.sampler_options[key] = val
 
@@ -122,22 +123,38 @@
         self.data = [np.array(inputs.rows)]
         self.metadata = [{k:v[0] for k, v in inputs.meta.items()}]
         self.final_metadata = [{k:v[0] for k, v in inputs.final_meta.items()}]
         self.comments = [inputs.comments[:]]
         for chain in self.metadata:
             for key,val in list(chain.items()):
                 self.sampler_options[key] = val
-
-
+    
+    def load_astropy(self, inputs):
+        self.name = inputs.meta.get("chain_name", "chain")
+        self.colnames = inputs.colnames
+        # convert astropy table to numpy array
+        self.data = [np.array([inputs[c] for c in self.colnames]).T]
+        self.metadata = [inputs.meta]
+        self.final_metadata = [{
+            k[6:]: v
+            for k, v in meta.items()
+            if k.startswith("final:")
+        } for meta in self.metadata]
+        self.comments = [meta["comments"] for meta in self.metadata]
+        for meta in self.metadata:
+            for key, val in meta.items():
+                self.sampler_options[key] = val
 
     def sampler_option(self, key, default=None):
         return self.sampler_options.get(key, default)
 
     def load_chain(self, ini):
-        if isinstance(ini, tuple):
+        if "astropy" in str(type(ini)):
+            self.load_astropy(ini)
+        elif isinstance(ini, tuple):
             self.load_tuple(ini)
         elif isinstance(ini, dict):
             self.load_dict(ini)
         elif isinstance(ini, output_module.InMemoryOutput):
             self.load_in_memory_storage(ini)
         else:
             self.load_ini(ini)
@@ -215,17 +232,19 @@
                     print(traceback.format_exc())
         return files
 
     def finalize(self):
         print("Finalizing:")
         for e in self.steps:
             e.finalize()
+    
+    def save(self):
         for f in list(self.outputs.values()):
             print("Output: ", f.filename)
-            f.finalize()
+            f.save()
 
     def apply_tweaks(self, tweaks):
         if tweaks.filename==plots.Tweaks.filename:
             print(tweaks.filename)
             print("Please fill in the 'filename' attribute of your tweaks")
             print("Put the base name (without the directory, prefix, or suffix)")
             print("of the filename you want to tweak.")
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/reruns.py` & `cosmosis-3.0/cosmosis/postprocessing/reruns.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 			params_ini.add_section('test')
 		except:
 			pass
 
 		likes = params_ini.get('pipeline', 'likelihoods', fallback='')
 		params_ini.set('pipeline', 'values', values_file.name)
 		params_ini.set('pipeline', 'priors', priors_file.name)
-		params_ini.set('pipeline', 'quiet', 'F')
 		params_ini.set('pipeline', 'timing', 'T')
 		params_ini.set('pipeline', 'debug', 'T')
 		params_ini.set('runtime', 'sampler', 'test')
 		params_ini.set('test', 'save_dir', self.rerun_dirname)
 
 
 		params_ini.write(params_file)
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/statistics.py` & `cosmosis-3.0/cosmosis/postprocessing/statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,36 +4,48 @@
 try: 
     from getdist import MCSamples
 except: 
     MCSamples = None
 # getdist not implemented for polychord and grid sampler yet
 import numpy as np
 import scipy as sp
+from io import StringIO
 from .utils import std_weight, mean_weight, median_weight, percentile_weight, find_asymmetric_errorbars
-from .outputs import PostprocessText
+from .outputs import PostprocessText, PostprocessTable, MiniTable
+
+
 
 class Statistics(PostProcessorElement):
     def __init__(self, *args, **kwargs):
         super(Statistics, self).__init__(*args, **kwargs)
 
     def run(self):
         print("I do not know how to generate statistics for this kind of data")
         return []
  
     def filename(self, base):
         filename = super(Statistics, self).filename("txt", base)
         return filename
 
+    def get_table_output(self, base, cols):
+        filename = self.filename(base)
+        f = self.get_output(base)
+        if f is None:
+            t = MiniTable(cols)
+            self.set_output(base, PostprocessTable(base, filename, t))
+        else:
+            t = f.value
+        return t
 
     def get_text_output(self, base, header="", section_name=""):
         filename = self.filename(base)
-        f = self.get_output(filename)
+        f = self.get_output(base)
         if f is None:
-            f = open(filename, 'w')
-            self.set_output(filename, PostprocessText(base,filename,f))
+            f = StringIO()
+            self.set_output(base, PostprocessText(base,filename,f))
             new_file = True
             if header:
                 f.write(header+'\n')
         else:
             f=f.value
             new_file = False
         if section_name:
@@ -41,91 +53,41 @@
         return f, filename, new_file
 
 class ConstrainingStatistics(Statistics):
 
     def report_file(self):
         #Get the filenames to make
         return [
-            self.report_file_mean(),
-            self.report_file_median(),
-            self.report_file_mode(),
-            self.report_file_l95(),
-            self.report_file_u95(),
-            self.report_file_l68(),
-            self.report_file_u68(),
-            self.report_file_err("lerr68", self.lerr68),
-            self.report_file_err("uerr68", self.uerr68),
-            self.report_file_err("lerr95", self.lerr95),
-            self.report_file_err("uerr95", self.uerr95),
-            self.report_file_err("peak1d", self.peak1d),
+            self.report_centroid("means", self.mu),
+            self.report_centroid("medians", self.median),
+            self.report_centroid("modes", self.peak1d),
+            self.report_limit("l95", self.l95),
+            self.report_limit("u95", self.u95),
+            self.report_limit("l68", self.l68),
+            self.report_limit("u68", self.u68),
+            self.report_limit("lerr68", self.lerr68),
+            self.report_limit("uerr68", self.uerr68),
+            self.report_limit("lerr95", self.lerr95),
+            self.report_limit("uerr95", self.uerr95),
+            self.report_limit("peak1d", self.peak1d),
         ]
-    def report_file_mean(self):        
-        #Generate the means file
-        header = "#parameter mean std_dev"
-        marge_file, marge_filename, new_file = self.get_text_output("means", header, self.source.name)
-        for P in zip(self.source.colnames, self.mu, self.sigma):
-            marge_file.write("%s   %e   %e\n" % P)
-        return marge_filename
-
-    def report_file_median(self):
-        #Generate the medians file
-        header = "#parameter mean std_dev"
-        median_file, median_filename, new_file = self.get_text_output("medians", header, self.source.name)
-        for P in zip(self.source.colnames, self.median, self.sigma):
-            median_file.write("%s   %e   %e\n" % P)
-        return median_filename
-
-    def report_file_mode(self):
-        #Generate the mode file
-        header = "#parameter value"
-        best_file, best_filename, new_file = self.get_text_output("best_fit", header, self.source.name)
-        for P in zip(self.source.colnames, self.source.get_row(self.best_fit_index)):
-            best_file.write("%s        %g\n"%P)
-        return best_filename
-
-    def report_file_l95(self):
-        #Generate the medians file
-        header = "#parameter low95"
-        limit_file, limit_filename, new_file = self.get_text_output("low95", header, self.source.name)
-        for P in zip(self.source.colnames, self.l95):
-            limit_file.write("%s     %g\n" % P)
-        return limit_filename
-
-    def report_file_u95(self):
-        #Generate the medians file
-        header = "#parameter upper95"
-        limit_file, limit_filename, new_file = self.get_text_output("upper95", header, self.source.name)
-        for P in zip(self.source.colnames, self.u95):
-            limit_file.write("%s     %g\n" % P)
-        return limit_filename
-
-    def report_file_l68(self):
-        #Generate the medians file
-        header = "#parameter low68"
-        limit_file, limit_filename, new_file = self.get_text_output("low68", header, self.source.name)
-        for P in zip(self.source.colnames, self.l68):
-            limit_file.write("%s     %g\n" % P)
-        return limit_filename
-
-    def report_file_u68(self):
-        #Generate the medians file
-        header = "#parameter upper68"
-        limit_file, limit_filename, new_file = self.get_text_output("upper68", header, self.source.name)
-        for P in zip(self.source.colnames, self.u68):
-            limit_file.write("%s     %g\n" % P)
-        return limit_filename
-
-    def report_file_err(self, name, data):
-        #Generate the medians file
-        header = "#parameter {}".format(name)
-        limit_file, limit_filename, new_file = self.get_text_output(name, header, self.source.name)
-        for P in zip(self.source.colnames, data):
-            limit_file.write("%s     %g\n" % P)
-        return limit_filename
 
+    def report_centroid(self, kind, col):
+        cols = ["parameter", kind, "sigma", "data_set"]
+        table = self.get_table_output(kind, cols)
+        for (col, x, sigma) in zip(self.source.colnames, col, self.sigma):
+            table.append([col, x, sigma, self.source.label])
+        return table
+
+    def report_limit(self, kind, col):
+        cols = ["parameter", kind, "data_set"]
+        table = self.get_table_output(kind, cols)
+        for (col, x) in zip(self.source.colnames, col):
+            table.append([col, x, self.source.label])
+        return table
 
     @staticmethod
     def find_median(x, P):
         C = [0] + P.cumsum()
         return np.interp(C[-1]/2.0,C,x)
 
     @staticmethod
@@ -138,14 +100,15 @@
         self.report_screen_asym()
         self.report_screen_asym95()
         self.report_screen_median()
         self.report_screen_mode()
         self.report_screen_limits()
         #Print the same summary stats that go into the
         #files but to the screen instead, in a pretty format        
+
     def report_screen_mean(self):
         #Means
         print()
         print("Marginalized mean, std-dev:")
         for P in zip(self.source.colnames, self.mu, self.sigma):
             print('    %s = %g ± %g ' % P)
         print()
@@ -170,14 +133,15 @@
 
     def report_screen_median(self):
         #Medians
         print("Marginalized median, std-dev:")
         for P in zip(self.source.colnames, self.median, self.sigma):
             print('    %s = %g ± %g' % P)
         print()
+
     def report_screen_mode(self):
         #Mode
         print("Best likelihood:")
         for name, val in zip(self.source.colnames, self.source.get_row(self.best_fit_index)):
             print('    %s = %g' % (name, val))
         print()
 
@@ -187,14 +151,15 @@
         for name, val in zip(self.source.colnames, self.l95):
             print('    %s > %g' % (name, val))
         print()
         print("95% upper limits:")
         for name, val in zip(self.source.colnames, self.u95):
             print('    %s < %g' % (name, val))
         print()
+
         #Mode
         print("68% lower limits:")
         for name, val in zip(self.source.colnames, self.l68):
             print('    %s > %g' % (name, val))
         print()
         print("68% upper limits:")
         for name, val in zip(self.source.colnames, self.u68):
@@ -368,15 +333,16 @@
 
         col_names = [p for p in self.source.colnames if p.lower() not in ["like","post", "importance", "weight", "prior"]]
 
         if len(col_names)<2:
             return []
 
         if self.source.options.get("getdist",False):
-            covmat = self.source.gdc.cov()
+            # Have to manually skip the first bit here
+            covmat = self.source.gdc.cov()[:len(col_names),:len(col_names)]
         else:
 
             if hasattr(self, 'weight_col'):
                 w = self.weight_col()
             else:
                 w = None
 
@@ -386,29 +352,29 @@
         #For the proposal we just want the first 
         #nvaried rows/cols - we don't want to include
         #extra parameters like sigma8
         n = self.source.metadata[0]['n_varied']
         proposal = covmat[:n,:n]
 
         #Save the covariance matrix
-        f, filename, new_file = self.get_text_output("covmat")
-        if new_file:
-            f.write('#'+'    '.join(col_names)+'\n')
-            np.savetxt(f, covmat)
+        t1 = self.get_table_output("covmat", col_names)
+        if len(t1) == 0:
+            for row in covmat:
+                t1.append(row)
         else:
             print("NOT saving more than one covariance matrix - just using first ini file")
 
         #Save the proposal matrix
-        f, proposal_filename, new_file = self.get_text_output("proposal")
-        if new_file:
-            f.write('#'+'    '.join(col_names[:n])+'\n')
-            np.savetxt(f, proposal)
+        t2 = self.get_table_output("proposal", col_names[:n])
+        if len(t2) == 0:
+            for row in proposal:
+                t2.append(row)
         else:
             print("NOT saving more than one proposal matrix - just using first ini file")
-        return [filename, proposal_filename]
+        return [t1, t2]
 
 class MetropolisHastingsCovariance(ChainCovariance, Statistics, MCMCPostProcessorElement):
     pass
 
 class WeightedMetropolisHastingsCovariance(ChainCovariance, Statistics, MCMCPostProcessorElement):
     pass
 
@@ -455,16 +421,14 @@
         #Get the filenames to make
         return [
             self.report_file_mean(),
             self.report_file_median(),
             self.report_file_mode(),
             self.report_file_l95(),
             self.report_file_u95(),
-#            self.report_file_l68(),
-#            self.report_file_u68(),
             ]
 
     def compute_stats(self):
         #1D stats
         self.mu = np.zeros(self.ncol)
         self.median = np.zeros(self.ncol)
         self.sigma = np.zeros(self.ncol)
@@ -553,30 +517,32 @@
     def run(self):
         if len(self.source.data)<2:
             print()
             print("(One chain found. Run multiple chains if you want the Gelman-Rubin test)")
             print()
             return []
         names = [c for c in self.source.colnames if  c not in ['weight', 'like', 'post']]
-        header = "#parameter   R-1\n"
-        f, filename, is_new = self.get_text_output("gelman", header)
+        cols = ["parameter", "R-1", "data_set"]
+        t = self.get_table_output("gelman", cols)
+
         print()
         print("Gelman-Rubin tests")
         print("------------------")
         print("(Variance of means / Mean of variances.  Smaller is better, a few percent is usually good convergence)")
         print()
         for name in names:
             R1 = self.gelman_rubin(name)
-            f.write("{}   {}\n".format(name,R1))
+            t.append([name, R1, self.source.label])
+
             if R1>0.1:
                 print("{}    {}  -- POORLY CONVERGED PARAMETER AT 10% LEVEL".format(name,R1))
             else:
                 print("{}    {}".format(name,R1))
         print()
-        return [filename]
+        return [t]
 
 
 
 
 class DunkleyTest(MetropolisHastingsStatistics):
     """
     Run the Dunley et al (2005) power spectrum test
@@ -593,37 +559,39 @@
         n = self.source.metadata[0]['n_varied']
         jstar = []
         #Just sample over the sample parameters,
         #not the likelihood or the derived parameters
         params = self.source.colnames[:n]
         print("Dunkely et al (2005) power spectrum test.")
         print("For converged chains j* > %.1f:" %self.jstar_convergence_limit)
+
+        cols = ["parameter", "jstar", "data_set"]
+        t = self.get_table_output("dunkley", cols)
+
+
         for param in params:
             cols = self.reduced_col(param, stacked=False)
             for c,col in enumerate(cols):
                 js = self.compute_jstar(col)
                 jstar.append(js)
                 m = "Chain %d:  %-35s j* = %-.1f" % (c+1, param, js)
                 if js>20:
                     print("    %-50s" % m)
                 else:
                     print("    %-50s NOT CONVERGED!" % m)
+                
+                t.append([param, js, self.source.label])
         print()
         if not np.min(jstar)>self.jstar_convergence_limit:
             print("The Dunkley et al (2005) power spectrum test shows that this chain has NOT CONVERGED.")
             print("It is quite a conservative test, so no need to panic.")
         else:
             print("The power spectra for this chain suggests good convergence.")
         print()
-        header = '#'+'    '.join(params)
-        f, filename, new_file = self.get_text_output("dunkley", header, self.source.name)
-        f.write("\n")
-        f.write('    '.join(str(js) for js in jstar))
-        f.write("\n")
-        return [filename]
+        return [t]
 
 
     @staticmethod
     def compute_jstar(x):
         import scipy.optimize
 
         #Get the power spectrum of the chain
@@ -677,15 +645,15 @@
             rangedict[str(vlpar)] = np.array(vlpar.limits)
         try: 
             loglikes = self.source.reduced_col("post")
         except: 
             loglikes = self.source.reduced_col("like")
 
         if MCSamples:
-            gdc = MCSamples(samples = datapts,weights=weight,loglikes=loglikes, names=self.source.colnames,name_tag = self.source.name,ranges=rangedict)# ranges from value file
+            gdc = MCSamples(samples = datapts,weights=weight,loglikes=loglikes, names=self.source.colnames,name_tag = self.source.label,ranges=rangedict)# ranges from value file
         else:
             raise ImportError('GetDist is not installed')
         self.source.gdc = gdc
         return gdc
         
     def compute_basic_stats_col(self, col):
         data = self.reduced_col(col)
@@ -708,34 +676,34 @@
         # Use parent statistics, except add evidence information,
         # which is just read from the file
         files = super(MultinestStatistics,self).run()
         logz = self.source.final_metadata[0]["log_z"]
         try:
             logz_sigma = self.source.final_metadata[0]["log_z_error"]
         except KeyError:
-            logz_sigma = "(error not computed)"
+            logz_sigma = np.nan
         #First print to screen
         print("Bayesian evidence:")
         print(f"    log(Z) = {logz:.2f} ± {logz_sigma}")
         print()
 
 
         weight = self.weight_col()
         w = weight/weight.max()
         n_eff = w.sum()
 
         print("Effective number samples = ", n_eff)
         print()
         #Now save to file
-        header = '#logz    logz_sigma'
-        f, filename, new_file  = self.get_text_output("evidence", header, self.source.name)
-        f.write(f'{logz}    {logz_sigma}\n')
+        cols=["logz", "logz_sigma", "data_set"]
+        t = self.get_table_output("evidence", cols)
+        t.append([logz, logz_sigma, self.source.label])
 
         #Include evidence in list of created files
-        files.append(filename)
+        files.append(t)
         return files
 
 
 class PolychordStatistics(MultinestStatistics):
     pass
 
 #The class hierarchy is getting too complex for this - revise it
@@ -856,71 +824,69 @@
 
 class PolychordCovariance(MultinestCovariance):
     pass
 
 
 class CovarianceMatrix1D(Statistics):
     def run(self):
-        params = self.source.colnames
         Sigma = np.linalg.inv(self.source.data[0]).diagonal()**0.5
         Mu = [float(self.source.metadata[0]['mu_{0}'.format(i)]) for i in range(Sigma.size)]        
-        header = '#'+'    '.join(params)
-        f, filename, new_file = self.get_text_output("means", header, self.source.name)
+        cols = ['param', 'mean', 'std-dev', 'data_set']
+        t = self.get_table_output("means", cols)
 
-        for P in zip(self.source.colnames, Mu, Sigma):
-            f.write("%s   %e   %e\n" % P)
+        for p, mu, sigma in zip(self.source.colnames, Mu, Sigma):
+            t.append([p, mu, sigma, self.source.label])
 
         print()
         print("Marginalized mean, std-dev:")
         for P in zip(self.source.colnames, Mu, Sigma):
             print('    %s = %g ± %g' % P)
         print()
 
-        return [filename]
+        return [t]
 
 class CovarianceMatrixEllipseAreas(Statistics):
     def run(self):
         params = self.source.colnames
-        header = '#param1  param2  area figure_of_merit'
-        f, filename, new_file = self.get_text_output("ellipse_areas", header, self.source.name)
+        cols = ["param1", "param2", "area", "figure_of_merit", "data_set"]
+        t = self.get_table_output("ellipse_areas", cols)
 
         covmat_estimate = np.linalg.inv(self.source.data[0])
         for i,p1 in enumerate(params[:]):
             for j,p2 in enumerate(params[:]):
                 if j>=i: continue
                 #Get the 2x2 sub-matrix
                 C = covmat_estimate[:,[i,j]][[i,j],:]
                 area = 6.17 * np.pi * np.sqrt(np.linalg.det(C))
                 fom = 1.0/area
-                f.write("{0}  {1}  {2}  {3}\n".format(p1, p2, area, fom))
+                t.append([p1, p2, area, fom, self.source.label])
 
-        return [filename]
+        return [t]
 
 
 class FisherFigureOfMerit(Statistics):
     def run(self):
-        params = self.source.colnames
-        header = '#figure_of_merit\n#Definition: det(F)**(-0.5/n)'
-        f, filename, new_file = self.get_text_output("fisher_fom", header, self.source.name)
+        cols = ["figure_of_merit_reduced", "data_set"]
+        t = self.get_table_output("fisher_fom", cols)
         F = self.source.data[0]
         n = self.source.metadata[0]['n_varied']
         fom = (np.linalg.det(F))**(-0.5 / n)
-        f.write("{}\n".format(fom))
-        return [filename]
+        t.append([fom, self.source.label])
+        return [t]
 
 
 class Citations(Statistics):
     #This isn't really a statistic but it uses all the same
     #mechanisms
     def run(self):
         print() 
         message = "#You should cite these papers in any publication based on this pipeline."
         print(message)
         citations = set()
-        f, filename, new_file = self.get_text_output("citations", message, self.source.name)
+        f, filename, new_file = self.get_text_output("citations", message, self.source.label)
         for comment_set in self.source.comments:
             for comment in comment_set:
                 comment = comment.strip()
                 if comment.startswith("CITE"):
                     citation =comment[4:].strip()
                     citations.add(citation)
         for citation in citations:
```

### Comparing `cosmosis-2.5.1/cosmosis/postprocessing/utils.py` & `cosmosis-3.0/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/analytics.py` & `cosmosis-3.0/cosmosis/runtime/analytics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #coding: utf-8
-from cosmosis import output as output_module
-
+from ..runtime import logs
 import numpy as np
-import sys
-import os
+
 
 
 class Analytics(object):
     def __init__(self, params, pool=None):
         self.params = params
         self.pool = pool
 
@@ -44,15 +42,15 @@
             local_variance = self.m2 / float(self.total_steps-1)
             if self.pool:
                 return np.array(self.pool.gather(local_variance)).T
             else:
                 return local_variance
         return None
 
-    def gelman_rubin(self, quiet=True):
+    def gelman_rubin(self):
         # takes current traces and returns
         if self.pool is None or not self.pool.size > 1:
             raise RuntimeError("Gelman-Rubin statistic is only "
                                "valid for multiple chains.")
 
         if self.total_steps == 0:
             raise RuntimeError("Gelman-Rubin statistic not "
@@ -71,16 +69,14 @@
             # TODO: check for 0-values in W
             Rhat = np.sqrt(V/W)
         else:
             Rhat = None
 
         Rhat = self.pool.bcast(Rhat)
 
-        if not quiet and self.pool.is_master():
-            print()
-            print("Gelman-Rubin:")
+        if self.pool.is_master():
+            logs.important("Gelman-Rubin statistic:")
             for (p,R) in zip(self.params, Rhat):
-                print("    ", p, "   ", R)
-            print("Worst = ", Rhat.max())
-            print()
+                logs.important(f"    {p}   {R}")
+            logs.important(f"Worst = {Rhat.max()}")
 
         return Rhat
```

### Comparing `cosmosis-2.5.1/cosmosis/runtime/attribution.py` & `cosmosis-3.0/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/config.py` & `cosmosis-3.0/cosmosis/runtime/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,155 +3,83 @@
 
 u"""Definition of the :class:`Inifile` class."""
 
 
 import os
 import sys
 import collections
-import warnings
 import configparser
+import io
 
 class CosmosisConfigurationError(configparser.Error):
     u"""Something to throw when there is an error in a .ini file particular to Cosmosis.
 
     The (underlying) object simply carries a string providing information
     to the user.
 
     """
     pass
 
 class IncludingConfigParser(configparser.ConfigParser):
-    u"""Extension of built-in python :class:`ConfigParser` to \%include other files.
+    u"""Extension of built-in python :class:`ConfigParser` to %include other files.
 
     Use the line: %include filename.ini This is assumed to end a section,
     and the last section in the included file is assumed to end as well
 
     Note that the caller of the `read()` method may set a
     `no_expand_includes` attribute on this object, to cause any %include
     lines to *not* actually be actioned (they will be regarded as
     comments, but still delineate sections).
     """
 
     def __init__(self, defaults=None, print_include_messages=True):
         configparser.ConfigParser.__init__(self,
                                    defaults=defaults,
                                    dict_type=collections.OrderedDict,
-                                   strict=False)
+                                   strict=False,
+                                   inline_comment_prefixes=(';', '#'),
+                                   )
         self.print_include_messages = print_include_messages
 
     def _read(self, fp, fpname):
-        u"""Parse a sectioned setup file.
-
-        The sections in setup file contains a title line at the top,
-        indicated by a name in square brackets (`[]'), plus key/value
-        options lines, indicated by `name: value' format lines.
-        Continuations are represented by an embedded newline then
-        leading whitespace.  Blank lines, lines beginning with a '#',
-        and just about everything else are ignored.
+        """
+        This overrides the parent method to allow %include directives
+        to import additional files.
 
+        To do so we first read the file into a StringIO object, dealing
+        with the %include directives as we go, then pass that to the
+        parent method.
         """
-        cursect = None                        # None, or a dictionary
-        optname = None
-        lineno = 0
-        e = None                              # None, or an exception
-        while True:
-            line = fp.readline()
-            if not line:
-                break
-            lineno = lineno + 1
-            # comment or blank line?
-            if line.strip() == '' or line[0] in '#;':
-                continue
-            if line.split(None, 1)[0].lower() == 'rem' and line[0] in "rR":
-                # no leading whitespace
-                continue
-            # continuation line?
-            if line[0].isspace() and cursect is not None and optname:
-                value = line.strip()
-                if value:
-                    cursect[optname].append(value)
-            # a section header or option header?
+        s = io.StringIO()
+        for line in fp:
+            # check for include directives
+            if not getattr(self, 'no_expand_vars', False):
+                line = os.path.expandvars(line)
+
+            if line.lower().startswith('%include'):
+                _, filename = line.split()
+                filename = filename.strip('"').strip("'")
+
+                if self.print_include_messages:
+                    print(f"Reading included ini file: {filename}")
+                if not os.path.exists(filename):
+                    raise ValueError(f"Tried to include non-existent file {filename}")
+
+                # read the contents of the ini file into a new instance
+                # of this class, then we will write it out
+                sub_ini = self.__class__(filename)
+
+                # write the whole other file content to our StringIO
+                sub_ini.write(s)
             else:
-                #JAZ add environment variable expansion
-                if not getattr(self, 'no_expand_vars', False):
-                    line = os.path.expandvars(line)
-                # is it a section header?
-                mo = self.SECTCRE.match(line)
-                if mo:
-                    sectname = mo.group('header')
-                    if sectname in self._sections:
-                        cursect = self._sections[sectname]
-                    elif sectname == configparser.DEFAULTSECT:
-                        cursect = self._defaults
-                    else:
-                        cursect = self._dict()
-                        self._sections[sectname] = cursect
-                    # So sections can't start with a continuation line
-                    optname = None
-                # no section header in the file?
-                elif line.lower().startswith('%include'):
-                    if  not  getattr (self, 'no_expand_includes', False):
-                        include_statement, filename = line.split()
-                        filename = filename.strip('"').strip("'")
-                        if self.print_include_messages:
-                            sys.stdout.write("Reading included ini file: `"
-                                                               + filename + "'\n")
-                        if not os.path.exists(filename):
-                            # TODO: remove direct sys.stderr writes
-                            raise ValueError("Tried to include non-existent "
-                                          "ini file: `" + filename + "'\n")
-                        self.read(filename)
-                    cursect = None
-                elif cursect is None:
-                    raise configparser.MissingSectionHeaderError(fpname,
-                                                                 lineno,
-                                                                 line)
-                # an option line?
-                else:
-                    mo = self._optcre.match(line)
-                    if mo:
-                        optname, vi, optval = mo.group('option', 'vi', 'value')
-                        optname = self.optionxform(optname.rstrip())
-                        # This check is fine because the OPTCRE cannot
-                        # match if it would set optval to None
-                        if optval is not None:
-                            if vi in ('=', ':') and ';' in optval:
-                                # ';' is a comment delimiter only if it
-                                # follows a spacing character
-                                pos = optval.find(';')
-                                if pos != -1 and optval[pos-1].isspace():
-                                    optval = optval[:pos]
-                            optval = optval.strip()
-                            # allow empty values
-                            if optval == '""':
-                                optval = ''
-                            cursect[optname] = [optval]
-                        else:
-                            # valueless option handling
-                            cursect[optname] = optval
-                    else:
-                        # a non-fatal parsing error occurred.  set up the
-                        # exception but keep going. the exception will be
-                        # raised at the end of the file and will contain
-                        # a list of all bogus lines
-                        if not e:
-                            e = configparser.ParsingError(fpname)
-                        e.append(lineno, repr(line))
-        # if any parsing errors occurred, raise an exception
-        if e:
-            raise e
-
-        # join the multi-line values collected while reading
-        all_sections = [self._defaults]
-        all_sections.extend(list(self._sections.values()))
-        for options in all_sections:
-            for name, val in list(options.items()):
-                if isinstance(val, list):
-                    options[name] = '\n'.join(val)
+                s.write(line)
 
+        # rewind the stuff we have read
+        s.seek(0)
+        return super()._read(s, fpname)
 
 
 
 class Inifile(IncludingConfigParser):
 
     u"""A dictionary of `(section, name) -> value` pairs corresponding to entries in a .ini file.
 
@@ -167,15 +95,15 @@
 
     """
 
     def __init__(self, filename, defaults=None, override=None, print_include_messages=True):
         u"""Read in a configuration from `filename`.
 
         The `defaults` will be applied if a parameter is not specified in
-        the file (or \%included descendants), and the `override`s will be
+        the file (or %included descendants), and the `override`s will be
         imposed on the regardless of whether those parameters have
         assigned values or not.
 
         Where supplied, `defaults` and `override` should be dictionary
         mappings of `(section, name) -> value`.
 
         """
@@ -186,14 +114,22 @@
 
         # if we are pased a dict, convert it to an inifile
         if isinstance(filename, dict):
             for section, values in filename.items():
                 self.add_section(section)
                 for key, value in values.items():
                     self.set(section, key, str(value))
+        elif isinstance(filename, Inifile):
+            # This seems to be the only way to preserve the
+            # defaults.
+            # https://stackoverflow.com/questions/23416370/manually-building-a-deep-copy-of-a-configparser-in-python-2-7
+            s = io.StringIO()
+            filename.write(s)
+            s.seek(0)
+            self.read_file(s)
         # default read behaviour is to ignore unreadable files which
         # is probably not what we want here
         elif filename is not None:
             if isinstance(filename,str) and not os.path.exists(filename):
                 raise IOError("Unable to open configuration file `" + filename + "'")
             self.read(filename)
 
@@ -267,14 +203,22 @@
         try:
             return IncludingConfigParser.get(self, section, option, raw=raw, vars=vars, fallback=fallback)
         except (configparser.NoSectionError, configparser.NoOptionError) as e:
             if fallback is configparser._UNSET:
                 raise CosmosisConfigurationError("CosmoSIS looked for an option called '%s' in the '[%s]' section, but it was not in the ini file"%(option,section))
             else:
                 return fallback
+            
+    def __getitem__(self, key: tuple):
+        section, option = key
+        return self.get(section, option)
+
+    def __setitem__(self, key: tuple, value: str):
+        section, option = key
+        self.set(section, option, str(value))
 
     # these functions override the default parsers to allow for extra formats
     def getint(self, section, option, raw=False, vars=None, fallback=configparser._UNSET):
         u"""Get a value as an integer, or return `default` if the value is not found.
         
         If the `default` is not set and is needed, an error with a message
         to the user will be raised. (`None` is *not* acceptable as a
```

### Comparing `cosmosis-2.5.1/cosmosis/runtime/declare.py` & `cosmosis-3.0/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.0/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/memmon.py` & `cosmosis-3.0/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/module.py` & `cosmosis-3.0/cosmosis/runtime/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #coding: utf-8
-
-u"""Definition of :class:`Module`."""
-
-
 import os
-import ctypes
-import sys
-import numpy as np
 import abc
-from cosmosis.datablock import option_section, DataBlock, SectionOptions
+import sys
+import ctypes
+from ..datablock import option_section, DataBlock, SectionOptions
+from ..utils import underline
+
 
 MODULE_TYPE_EXECUTE_SIMPLE = "execute"
 MODULE_TYPE_EXECUTE_CONFIG = "execute_config"
 MODULE_TYPE_SETUP = "setup"
 MODULE_TYPE_CLEANUP = "cleanup"
 
 MODULE_LANG_PYTHON = "python"
@@ -181,33 +178,33 @@
             if (name not in accesses_by_last_module) and (name not in defaults):
                 msg = ("**** WARNING: Parameter '{}' in the [{}] section never used!\n"
                         .format(
                        name, section))
                 print(msg)
 
 
-    def setup_functions(self, config, quiet=True):
+    def setup_functions(self, config):
         u"""Call the /Module/ constructor.
 
         This method also pulls in the `execute_function` from the linked
         library.
 
         This function MUST be run after object initialization and before
         any other action takes place.
 
         """
         # We need to keep a reference to the full
         # config object for the access check report
+        from . import logs
         config_orig = config
         if not self.is_python:
             config = config._ptr
 
         if self.setup_function:
-            if not quiet:
-                print('-- Setting up module %s --' % (self.name))
+            logs.overview(underline(f'\nSetting up module {self.name}'))
             self.data = self.setup_function(config)
             self.access_check_report(config_orig)
         else:
             self.data = None
 
         if self.data is not None:
             module_type = MODULE_TYPE_EXECUTE_CONFIG
@@ -218,15 +215,15 @@
                                                      self.execute_function,
                                                      module_type,
                                                      set_types=self.is_dynamic)
         if self.execute_function is None:
             raise ValueError("Could not find a function 'execute' in module '"
                                  +  self.name + "'")
 
-    def setup(self, config, quiet=True):
+    def setup(self, config):
         u"""Call the /Module/ after copying config information constructor.
         
         This module is split from the main workhorse method  setup_functions
         so that Modules can be used more easily in external code.
         """
         if isinstance(config, dict):
             config = DataBlock.from_dict(config)
```

### Comparing `cosmosis-2.5.1/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.0/cosmosis/runtime/mpi_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 def _error_function(task):
     raise RuntimeError("Pool was sent tasks before being told what "
                        "function to apply.")
 
 
 class MPIPool(object):
-    def __init__(self, debug=False):
+    def __init__(self, debug=False, comm=None):
         try:
             from mpi4py import MPI
             self.MPI = MPI
         except ImportError:
             raise RuntimeError("MPI environment not found!")
-
-        self.comm = MPI.COMM_WORLD
+        if comm is None:
+            comm = self.MPI.COMM_WORLD
+        self.comm = comm
         self.rank = self.comm.Get_rank()
         self.size = self.comm.Get_size()
         self.debug = debug
 
         self.function = _error_function
         self.callback = None
```

### Comparing `cosmosis-2.5.1/cosmosis/runtime/parameter.py` & `cosmosis-3.0/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/pipeline.py` & `cosmosis-3.0/cosmosis/runtime/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 #coding: utf-8
 
 u"""Definition of :class:`Pipeline` and the specialization :class:`LikelihoodPipeline`."""
 
 
 import os
-import ctypes
 import sys
-import string
 import numpy as np
 import time
 import collections
 import warnings
-import configparser
 import traceback
-import signal
-from . import utils
 from . import config
 from . import parameter
 from . import prior
 from . import module
+from . import logs
 from ..datablock.cosmosis_py import block, section_names
 try:
     import faulthandler
     faulthandler.enable()
 except ImportError:
     pass
 
@@ -35,14 +31,20 @@
         self.block = None
         self.post = -np.inf
         self.like = -np.inf
 
     def set_like(self, L):
         self.like = L
         self.post = self.prior + self.like
+    
+    def log(self, i):
+        v = ", ".join(str(x) for x in self.vector)
+        logs.info(f"Posterior = {self.post} for parameter set #{i}: [{v}]")
+
+
 
 
 PIPELINE_INI_SECTION = "pipeline"
 NO_LIKELIHOOD_NAMES = "no_likelihood_names_sentinel"
 
 class MissingLikelihoodError(Exception):
 
@@ -352,16 +354,17 @@
         if isinstance(arg, config.Inifile):
             self.options = arg
         else:
             self.options = config.Inifile(arg)
 
         #This will be set later
         self.root_directory = self.options.get("runtime", "root", fallback=os.getcwd())
+        self.run_count = 0
+        self.run_count_ok = 0
 
-        self.quiet = self.options.getboolean(PIPELINE_INI_SECTION, "quiet", fallback=True)
         self.debug = self.options.getboolean(PIPELINE_INI_SECTION, "debug", fallback=False)
         self.timing = self.options.getboolean(PIPELINE_INI_SECTION, "timing", fallback=False)
         shortcut = self.options.get(PIPELINE_INI_SECTION, "shortcut", fallback="")
         if shortcut=="":
             shortcut=None
 
         self.do_fast_slow = self.options.getboolean(PIPELINE_INI_SECTION, "fast_slow", fallback=False)
@@ -437,26 +440,26 @@
             # we need to store an ID here to allow a hack to add new parameters
             # from the modules themselves.  Unfortunately cosmosis stores ints, whereas
             # python IDs are long.  So we split the ID into two parts here
 
             LikelihoodPipeline.pipeline_being_set_up.append(self)
             LikelihoodPipeline.module_being_set_up.append(module.name)
             try:
-                module.setup(config_block, quiet=self.quiet)
+                module.setup(config_block)
             finally:
                 # This should only go wrong if someone is doing something
                 # ridiculous, so I won't catch any error in it.
                 LikelihoodPipeline.pipeline_being_set_up.remove(self)
                 LikelihoodPipeline.module_being_set_up.remove(module.name)
 
             if self.timing:
                 timings.append(time.time())
 
-        if not self.quiet:
-            sys.stdout.write("Setup all pipeline modules\n")
+
+        logs.overview("Setup all pipeline modules\n")
 
         if self.timing:
             timings.append(time.time())
             sys.stdout.write("Module timing:\n")
             for name, t2, t1 in zip(self.modules, timings[1:], timings[:-1]):
                 sys.stdout.write("%s %f\n" % (name, t2-t1))
 
@@ -589,14 +592,15 @@
 
         Bear in mind the note on short-cuts in the class description
         above: if `shortcut_data` and `shortcut_module` are defined, then
         the pipeline will start at `shortcut_module` with `shortcut_data`
         as the initial parameter vector.
 
         """
+        self.run_count += 1
         modules = self.modules
         if self.timing:
             self.timings = None
 
         timings = []
         if self.shortcut_module:
             if self.shortcut_data is None:
@@ -606,63 +610,55 @@
                 existing_keys = set(data_package.keys())
                 for (sec, name) in self.shortcut_data.keys():
                     if (sec,name) not in existing_keys:
                         data_package[sec, name] = self.shortcut_data[sec,name]
         elif self.slow_subspace_cache:
             first_module = self.slow_subspace_cache.start_pipeline(data_package)
             if first_module != 0 and (self.debug or self.timing):
-                sys.stdout.write("COOL: Quickstarting pipeline from module {} (fast/slow)\n".format(first_module))
-                sys.stdout.flush()
+                logs.debug(f"Quickstarting pipeline from module {first_module} (fast/slow)")
         else:
             first_module = 0
 
         if self.timing:
             start_time = time.time()
 
         for module_number, module in enumerate(modules):
             if module_number<first_module:
                 continue
-            if self.debug:
-                sys.stdout.write("Running %.20s ...\n" % module)
-                sys.stdout.flush()
+            logs.noisy(f"Running module {module}")
             data_package.log_access("MODULE-START", module.name, "")
             if self.timing:
                 t1 = time.time()
 
             status = module.execute(data_package)
 
             if status is None:
                 raise ValueError(("A module you ran, '{}', did not return a proper status value.\n"+
                     "It should return an integer, 0 if everything worked.\n"+
                     "Sorry to be picky but this kind of thing is important.").format(module))
 
-            if self.debug:
-                sys.stdout.write("Done %.20s status = %d \n" % (module,status))
-                sys.stdout.flush()
+            logs.noisy("Done %.20s status = %d \n" % (module,status))
 
             if self.timing:
                 t2 = time.time()
                 timings.append(t2-t1)
                 sys.stdout.write("%s took: %.3f seconds\n"% (module,t2-t1))
 
             if status:
-                if self.debug:
+                if logs.is_enabled_for(logs.debug):
                     data_package.print_log()
-                    sys.stdout.flush()
-                    sys.stderr.write("Because you set debug=True I printed a log of "
-                                     "all access to data printed above.\n"
-                                     "Look for the word 'FAIL' \n")
-                    sys.stderr.write("Though the error message could also be somewhere above that.\n\n")
-                if not self.quiet:
-                    sys.stderr.write("Error running pipeline (%d)- "
-                                     "hopefully printed above here.\n"%status)
-                    sys.stderr.write("Aborting this run and returning "
-                                     "error status.\n")
-                    if not self.debug:
-                        sys.stderr.write("Setting debug=T in [pipeline] might help.\n")
+                    logs.noisy("Because you set debug verbosity I printed a log of "
+                                   "all access to data printed above. "
+                                   "Look for the word 'FAIL' \n"
+                                   "Though the error message could also be "
+                                   "somewhere above that.\n")
+
+                logs.warning("Error running pipeline ({status}). Returning zero likelihood. Error may be above.")
+                if not logs.is_enabled_for(logs.debug):
+                    logs.warning("Set log level to 'debug' for more info.")
                 return None
 
             # If we are using a fast/slow split (and we are not already running on a cached subset)
             # Then see if it wants to cache these results
             if self.slow_subspace_cache and first_module==0:
                 self.slow_subspace_cache.next_module_results(module_number, data_package)
 
@@ -672,16 +668,16 @@
                 self.shortcut_data = data_package.clone()
 
         if self.timing:
             end_time = time.time()
             sys.stdout.write("Total pipeline time: {:.3} seconds\n".format(end_time-start_time))
             self.timings = timings
 
-        if not self.quiet:
-            sys.stdout.write("Pipeline ran okay.\n")
+        logs.noisy("Pipeline ran okay.")
+        self.run_count_ok += 1
 
         data_package.log_access("MODULE-START", "Results", "")
         # return something
         self.has_run = True
         return True
 
     def clear_cache(self):
@@ -1193,42 +1189,40 @@
         priors = self.prior(p, all_params=all_params, total_only=False)
         r.prior = sum(pr[1] for pr in priors)
 
         if np.isnan(r.prior):
             r.prior = -np.inf
 
         if not np.isfinite(r.prior):
-            if not self.quiet:
-                print("Proposed outside bounds: prior -infinity")
+            logs.info("Proposed outside bounds: prior -infinity")
             return r
         try:
             like, r.extra, r.block = self.likelihood(p, return_data=True, all_params=all_params)
             r.set_like(like)
 
             if r.block is not None:
                 for name,pr in priors:
                     r.block["priors", name] = pr
 
         except Exception:
+            logs.error(f"Exception running likelihood at parameters: {p}."
+                            "You should fix this; for now, using zero likelihood.")
+            logs.error(traceback.format_exc())
             if self.debug:
-                sys.stderr.write("\n\nERROR: there was an exception running the likelihood:\n")
                 sys.stderr.write("\nBecause you have debug=T I will let this kill the chain.\n")
                 sys.stderr.write("The input parameters were:{}\n".format(repr(p)))
                 raise
 
-            sys.stderr.write("\n\nERROR: there was an exception running the likelihood:\n")
-            sys.stderr.write("The input parameters were:{}\n".format(repr(p)))
-            traceback.print_exc(file=sys.stderr)
-            sys.stderr.write("You should fix this but for now I will return NaN for the likelihood (because you have debug=F)\n\n")
-
         if np.isnan(r.post):
             r.post = -np.inf
 
         if np.isnan(r.like):
             r.like = -np.inf
+        
+        r.log(self.run_count)
 
         return r
 
 
 
 
     def posterior(self, p, return_data=False, all_params=False):
@@ -1269,50 +1263,43 @@
         likelihood_names = []
         for _,key in data.keys(section_names.likelihoods):
             if key.endswith("_like"):
                 name = key[:-5]
                 likelihood_names.append(name)
         self.likelihood_names = likelihood_names
 
-        if not self.quiet:
-            # Tell the user what we found.
-            print("Likelihoods not set in parameter file, so checking what is generated:")
-            for name in self.likelihood_names:
-                print("Found likelihood named {}".format(name))
-            if not self.likelihood_names:
-                print("No likelihoods found")
+        # Tell the user what we found.
+        print("Using likelihooods from first run:")
+        for name in self.likelihood_names:
+            print(f" - {name}")
+        if not self.likelihood_names:
+            print(" - (None found)")
 
     def _extract_likelihoods(self, data):
         "Extract the likelihoods from the block"
 
         section_name = section_names.likelihoods
 
         # loop through named likelihoods and sum their values
         likelihoods = []
         for likelihood_name in self.likelihood_names:
             try:
                 L = data.get_double(section_name,likelihood_name+"_like")
                 likelihoods.append(L)
-                if not self.quiet:
-                    print("    Likelihood {} = {}".format(likelihood_name, L))
+                logs.noisy(f"Likelihood {likelihood_name} = {L}")
             # Complain if not found
             except block.BlockError:
                 raise MissingLikelihoodError(likelihood_name, data)
 
         # Total likelihood
         like = sum(likelihoods)
 
-        # DM: Issue #181: Zuntz: replace NaN's with -inf's in posteriors and
-        #                 likelihoods.
         if np.isnan(like):
             like = -np.inf
 
-        if not self.quiet and self.likelihood_names:
-            sys.stdout.write("Likelihood total = {}\n".format(like))
-
         return like
 
         
     def likelihood(self, p, return_data=False, all_params=False):
         u"""Run the simulation pipeline, computing any log-likelihoods in the pipeline 
         given the given input parameter values, and return the sum of these.
```

### Comparing `cosmosis-2.5.1/cosmosis/runtime/prior.py` & `cosmosis-3.0/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/runtime/process_pool.py` & `cosmosis-3.0/cosmosis/runtime/process_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,16 @@
         self.rank = 0
         self.master_pid = os.getpid()
 
     def is_master(self):
         return self.master_pid == os.getpid()
 
     def map(self, function, args):
-        pool = multiprocessing.Pool(self.size)
-        results = pool.map(function, args)
-        pool.close()
+        with multiprocessing.Pool(self.size) as pool:
+            results = pool.map(function, args)
         return results
 
     def close(self):
         pass
 
     def bcast(self, data):
         return self.data
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/__init__.py` & `cosmosis-3.0/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.0/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.0/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.0/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-import itertools
 import numpy as np
-from cosmosis.output.text_output import TextColumnOutput
 from .. import ParallelSampler
-
+from ...runtime import logs
 
 def task(p):
     i,p = p
-    print("Running sample from prior: ", p)
     r = sampler.pipeline.run_results(p)
     #If requested, save the data to file
     if sampler.save_name:
         if r.block is None:
-            print("Failed to run parameters: {} so not saving".format(p))
+            logs.error("Failed to run parameters: {} so not saving".format(p))
         else:
             filename = "{}_{}".format(sampler.save_name, i)
             r.block.save_to_file(filename, clobber=True)
 
     return (r.prior, r.post, r.extra)
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.0/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ...runtime import logs
 from .. import ParallelSampler
 import numpy as np
 import sys
 
 
 def log_probability_function(p):
     return pipeline.likelihood(p)[0]
@@ -26,15 +27,16 @@
             self.min_ncall = self.read_ini("min_ncall",int, 2*self.nlive)
             self.min_eff = self.read_ini("min_eff",float, 10.0)
             default_queue_size = 1 if self.pool is None else self.pool.size
             self.queue_size = self.read_ini("queue_size", int, default_queue_size)
             self.parallel_prior = self.read_ini("parallel_prior", bool, True)
             self.max_call = self.read_ini("max_call", int, sys.maxsize)
             self.dlogz = self.read_ini("dlogz", float, 0.01)
-            self.print_progress = self.read_ini("print_progress", bool, True)
+            print_progress_default = logs.is_enabled_for(logs.logging.INFO)
+            self.print_progress = self.read_ini("print_progress", bool, print_progress_default)
 
             # if self.mode=='dynamic':
             #     raise ValueError("Dynesty mode 'dynamic' not yet implemented (sorry)")
 
             for sec,name in pipeline.extra_saves:
                 col = "{}--{}".format(sec,name)
                 print("WARNING: DYNESTY DOES NOT SUPPORT DERIVED PARAMS - NOT SAVING {}".format(col))
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.0/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ...runtime import logs
 from .. import ParallelSampler, sample_ellipsoid, sample_ball
 import numpy as np
 import sys
 
 
 def log_probability_function(p):
     r = emcee_pipeline.run_results(p)
@@ -24,14 +25,15 @@
             self.emcee_version = int(self.emcee.__version__[0])
 
 
             # Parameters of the emcee sampler
             self.nwalkers = self.read_ini("walkers", int, 2)
             self.samples = self.read_ini("samples", int, 1000)
             self.nsteps = self.read_ini("nsteps", int, 100)
+            self.a = self.read_ini("a", float, 2.0)
 
             assert self.nsteps>0, "You specified nsteps<=0 in the ini file - please set a positive integer"
             assert self.samples>0, "You specified samples<=0 in the ini file - please set a positive integer"
 
             random_start = self.read_ini("random_start", bool, False)
             start_file = self.read_ini("start_points", str, "")
             covmat_file = self.read_ini("covmat", str, "")
@@ -40,24 +42,24 @@
             #Starting positions and values for the chain
             self.num_samples = 0
             self.prob0 = None
             self.blob0 = None
 
             if start_file:
                 self.p0 = self.load_start(start_file)
-                self.output.log_info("Loaded starting position from %s", start_file)
+                print("Loaded starting position from %s", start_file)
             elif self.distribution_hints.has_cov():
                 center = self.start_estimate()
                 cov = self.distribution_hints.get_cov()
                 self.p0 = sample_ellipsoid(center, cov, size=self.nwalkers)
-                self.output.log_info("Generating starting positions from covmat from earlier in pipeline")
+                print("Generating starting positions from covmat from earlier in pipeline")
             elif covmat_file:
                 center = self.start_estimate()
                 cov = self.load_covmat(covmat_file)
-                self.output.log_info("Generating starting position from covmat in  %s", covmat_file)
+                print("Generating starting position from covmat in  %s", covmat_file)
                 iterations_limit = 100000
                 n=0
                 p0 = []
                 for i in range(iterations_limit):
                     p = sample_ellipsoid(center, cov)[0]
                     if np.isfinite(self.pipeline.prior(p)):
                         p0.append(p)
@@ -65,28 +67,33 @@
                         break
                 else:
                     raise ValueError("The covmat you used could not generate points inside the prior")
                 self.p0 = np.array(p0)
             elif random_start:
                 self.p0 = [self.pipeline.randomized_start()
                            for i in range(self.nwalkers)]
-                self.output.log_info("Generating random starting positions from within prior")
+                print("Generating random starting positions from within prior")
             else:
                 center_norm = self.pipeline.normalize_vector(self.start_estimate())
                 sigma_norm=np.repeat(1e-3, center_norm.size)
                 p0_norm = sample_ball(center_norm, sigma_norm, size=self.nwalkers)
                 p0_norm[p0_norm<=0] = 0.001
                 p0_norm[p0_norm>=1] = 0.999
                 self.p0 = [self.pipeline.denormalize_vector(p0_norm_i) for p0_norm_i in p0_norm]
-                self.output.log_info("Generating starting positions in small ball around starting point")
+                print("Generating starting positions in small ball around starting point")
+
+            if self.emcee_version < 3:
+                kw = {"a": self.a}
+            else:
+                kw = {"moves": [(emcee.moves.StretchMove(a=self.a), 1.0)]}
 
             #Finally we can create the sampler
             self.ensemble = self.emcee.EnsembleSampler(self.nwalkers, self.ndim,
                                                        log_probability_function,
-                                                       pool=self.pool)
+                                                       pool=self.pool, **kw)
 
     def resume(self):
         if self.output.resumed:
             data = np.genfromtxt(self.output._filename, invalid_raise=False)[:, :self.ndim]
             num_samples = len(data) // self.nwalkers
             self.p0 = data[-self.nwalkers:]
             self.num_samples += num_samples
@@ -152,14 +159,14 @@
         #Set the starting positions for the next chunk of samples
         #to the last ones for this chunk
         self.p0 = pos
         self.prob0 = prob
         self.blob0 = extra_info
         self.num_samples += self.nsteps
         acceptance_fraction = self.ensemble.acceptance_fraction.mean()
-        print("Done {} iterations of emcee. Acceptance fraction {:.3f}".format(
+        logs.overview("Done {} iterations of emcee. Acceptance fraction {:.3f}".format(
             self.num_samples, acceptance_fraction))
         sys.stdout.flush()
         self.output.final("mean_acceptance_fraction", acceptance_fraction)
 
     def is_converged(self):
         return self.num_samples >= self.samples
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.0/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.0/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from .. import ParallelSampler
 from . import fisher
 from ...datablock import BlockError
 import numpy as np
 import scipy.linalg
-from ...runtime import prior,utils
+from ...runtime import prior, utils, logs
 import sys
 
 def compute_fisher_vector(p, cov=False):
     # use normalized parameters - fisherPipeline is a global
     # variable because it has to be picklable)
     try:
         x = fisherPipeline.denormalize_vector(p)
     except ValueError:
-        print("Parameter vector outside limits: %r" % p)
+        logs.error("Parameter vector outside limits: %r" % p)
         return None
 
-    if not fisherPipeline.quiet:
-        print("Running: ",x)
-
     #Run the pipeline, generating a data block
     data = fisherPipeline.run_parameters(x)
 
     #If the pipeline failed, return "None"
     #This might happen if the parameters stray into
     #a bad region.
     if data is None:
@@ -84,22 +81,21 @@
     def compute_prior_matrix(self):
         #We include the priors as an additional matrix term
         #This is just added to the fisher matrix
         n = len(self.pipeline.varied_params)
         P = np.zeros((n,n))
         for i, param in enumerate(self.pipeline.varied_params):
             if isinstance(param.prior, prior.GaussianPrior) or isinstance(param.prior, prior.TruncatedGaussianPrior):
-                print("Applying additional prior sigma = {0} to {1}".format(param.prior.sigma, param))
-                print("This will be assumed to be centered at the parameter center regardless of what the ini file says")
-                print("The limits of the parameter will also not be respected.") 
-                print()
+                logs.important("Applying additional prior sigma = {0} to {1}".format(param.prior.sigma, param))
+                logs.important("This will be assumed to be centered at the parameter center regardless of what the ini file says")
+                logs.important("The limits of the parameter will also not be respected.") 
                 P[i,i] = 1./param.prior.sigma**2
             elif isinstance(param.prior, prior.ExponentialPrior) or isinstance(param.prior, prior.TruncatedExponentialPrior):
-                print("There is an exponential prior applied to parameter {0}".format(param))
-                print("This is *not* accounted for in the Fisher matrix")
+                logs.important("There is an exponential prior applied to parameter {0}".format(param))
+                logs.important("This is *not* accounted for in the Fisher matrix")
                 print()
             #uniform prior should have no effect on the fisher matrix.
             #at least up until the assumptions of the FM are violated anyway
         return P
 
 
 
@@ -127,34 +123,33 @@
             self.step_size, self.tolerance, self.maxiter, pool=self.pool)
 
         try:
             fisher_matrix = fisher_calc.compute_fisher_matrix()
         except fisher.FisherParameterError as error:
             param = str(self.pipeline.varied_params[error.parameter_index])
             if error.parameter_index==0:
-                message = """
+                raise ValueError(f"""
 There was an error running the pipeline for the Fisher Matrix for parameter:
-{}
+{param}
 Since this is the first parameter this might indicate a general error in the pipeline.
 You might want to check with the "test" sampler.
 
 It might also indicate that the parameter lower or upper limit is too close to its
 starting value so the points used to calculate the derivative are outside the range.
 If that is the case you should try calculating the Fisher Matrix at a different starting point.
-""".format(param)
+""")
             else:
-                message = """
+                raise ValueError(f"""
 There was an error running the pipeline for the Fisher Matrix for parameter:
-{}
+{param}
 
 This probably indicates that the parameter lower or upper limit is too close to its
 starting value, so the points used to calculate the derivative are outside the range.
 If that is the case you should try calculating the Fisher Matrix at a different starting point.
-""".format(param)
-            raise ValueError(message)
+""")
 
         fisher_matrix = self.pipeline.denormalize_matrix(fisher_matrix,inverse=True)
 
         P = self.compute_prior_matrix()
         fisher_matrix += P
 
         self.converged = True
@@ -162,11 +157,11 @@
         if self.converged:
             for row in fisher_matrix:
                 self.output.parameters(row)
         try:
             covariance_matrix = utils.symmetric_positive_definite_inverse(fisher_matrix)
             self.distribution_hints.set_cov(covariance_matrix)
         except ValueError:
-            sys.stderr.write("Generated covariance matrix was not positive definite - beware! ")
+            logs.error("Generated covariance matrix was not positive definite - beware! ")
 
     def is_converged(self):
         return self.converged
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.0/cosmosis/samplers/grid/grid_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,27 +47,25 @@
                 self.nstep = self.nsample
 
 
         #Also Generate the complete collection of parameter sets to run over.
         #This doesn't actually keep them all in memory, it is just the conceptual
         #outer product
         total_samples = self.nsample**len(self.pipeline.varied_params)
-        print()
         print("Total number of grid samples: ", total_samples)
 
         if total_samples>LARGE_JOB_SIZE:
             print("That is a very large number of samples.")
             if self.allow_large:
                 print("But you set allow_large=T so I will continue")
             else:
                 print("This is suspicously large so I am going to stop")
                 print("If you really want to do this set allow_large=T in the")
                 print("[grid] section of the ini file.")
                 raise ValueError("Suspicously large number of grid points %d ( = n_samp ^ n_dim = %d ^ %d); set allow_large=T in [grid] section to permit this."%(total_samples,self.nsample,len(self.pipeline.varied_params)))
-        print()
         
         # If our pipeline allows it we arrange it so that the
         # fast parameters change fastest in the sequence.
         # This is still not optimal for the multiprocessing case
         if self.pipeline.do_fast_slow:
             param_order = self.pipeline.slow_params + self.pipeline.fast_params
         else:
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.0/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 
 
 def task(p):
     #pipeline here refers to a global variable
     #created later.  This is the only way we know
     #to get MPI task sharing to work
@@ -40,21 +41,21 @@
 
         #Figure out which points to sample at in the current 
         #dimension
         d = self.dimension
         bounds = self.bounds[d]
         samples = np.linspace(bounds[0], bounds[1], self.nsteps)
 
-        self.output.log_noisy("Minimizing in %s"%self.pipeline.varied_params[d].name)
+        logs.overview("Minimizing in %s"%self.pipeline.varied_params[d].name)
 
         #Fill in the sample points for the current
         #dimension in the samples
         for (p,s) in zip(normed_points,samples):
             p[d] = s
-        # print 'normed points', normed_points
+
         #Denormalize the points to get the physical parameters
         points = [self.pipeline.denormalize_vector(p) for p in normed_points]
 
         #And send them off to the workers
         if self.pool:
             results = self.pool.map(task, points)
         else:
@@ -97,15 +98,15 @@
     
         #If we have been around all the parameters 
         #then update the best-fits
         if d==0:
             self.previous_maxlike = self.maxlike
             self.maxlike = results[best][0]
 
-        self.output.log_noisy("New best fit L = %lf at %s = %le"%(posteriors.max(), self.pipeline.varied_params[d].name,points[best][d]))
+        logs.overview(f"New best fit L = {posteriors.max()} at {self.pipeline.varied_params[d].name} = {points[best][d]}")
 
         #and go on to the next dimension
         self.dimension = (d+1)%self.ndim
 
         if self.is_converged() and self.output_ini:
             self.pipeline.create_ini(points[best], self.output_ini)
         self.iterations += 1
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/hints.py` & `cosmosis-3.0/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.0/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.0/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-from .. import ParallelSampler
+from .. import ParallelSampler, sample_ball
+from ...runtime import logs
 import numpy as np
 
 pipeline = None
 def log_probability_function(p):
     global pipeline
     r = pipeline.run_results(p)
     return r.post, (r.extra, r.prior)
 
 
 
-def sample_ball(p0, std, size=1):
-    """
-    Produce a ball of walkers around an initial parameter value.
-
-    :param p0: The initial parameter value.
-    :param std: The axis-aligned standard deviation.
-    :param size: The number of samples to produce.
-
-    Function liberated from emcee utils module.
-    http://dan.iel.fm/emcee/current/
-
-    """
-    assert(len(p0) == len(std))
-    return np.vstack([p0 + std * np.random.normal(size=len(p0))
-                      for i in range(size)])
-
 
 class KombineSampler(ParallelSampler):
     parallel_output = False
     sampler_outputs = [("prior", float), ("post", float)]
 
     def config(self):
         global pipeline
@@ -56,15 +41,15 @@
             self.num_samples = 0
             self.lnpost0 = None
             self.lnprop0 = None
             self.blob0 = None
 
             if start_file:
                 self.p0 = self.load_start(start_file)
-                self.output.log_info("Loaded starting position from %s", start_file)
+                print("Loaded starting position from %s", start_file)
             elif random_start:
                 self.p0 = [self.pipeline.randomized_start()
                            for i in range(self.nwalkers)]
             else:
                 center_norm = self.pipeline.normalize_vector(self.pipeline.start_vector())
                 sigma_norm=np.repeat(1e-3, center_norm.size)
                 p0_norm = sample_ball(center_norm, sigma_norm, size=self.nwalkers)
@@ -97,15 +82,15 @@
             results = self.ensemble.burnin(self.p0, update_interval=self.update_interval)
             try:
                 pos, post, prop, extra_info = results
             except ValueError:
                 pos, post, prop = results
                 extra_info = None
             if self.is_master():
-                print("Burn-in phase complete.")
+                logs.overview("Burn-in phase complete.")
             self.p0 = pos
             self.lnpost0 = post
             self.lnprop0 = prop
             self.blob0 = extra_info
             self.burned_in = True
             return
 
@@ -127,11 +112,11 @@
         # Set the starting positions for the next chunk of samples
         # to the last ones for this chunk
         self.p0 = pos
         self.lnpost0 = post
         self.prob0 = prop
         self.blob0 = extra_info
         self.num_samples += self.nsteps
-        self.output.log_info("Done %d iterations", self.num_samples)
+        print("Done %d iterations", self.num_samples)
 
     def is_converged(self):
         return self.num_samples >= self.samples
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.0/cosmosis/samplers/list/list_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 import numpy as np
 from cosmosis.output.text_output import TextColumnOutput
 from .. import ParallelSampler
-
+from ...runtime import logs
 
 def task(p):
     i,p = p
     results = list_sampler.pipeline.run_results(p, all_params=True)
     #If requested, save the data to file
     if list_sampler.save_name and results.block is not None:
         results.block.save_to_file(list_sampler.save_name+"_%d"%i, clobber=True)
@@ -60,25 +60,25 @@
         # each of the table parameters can be found
         replaced_params = []
         for i,column_name in enumerate(column_names):
             # ignore additional columns like e.g. "like", "weight"
             try:
                 section,name = column_name.split('--')
             except ValueError:
-                print("Not including column %s as not a cosmosis name" % column_name)
+                logs.important("Not including column %s as not a cosmosis name" % column_name)
                 continue
             section = section.lower()
             name = name.lower()
             # find the parameter in the pipeline parameter vector
             # may not be in there - warn about this
             try:
                 j = self.pipeline.parameters.index((section,name))
                 replaced_params.append((i,j))
             except ValueError:
-                print("Not including column %s as not in values file" % column_name)
+                logs.important("Not including column %s as not in values file" % column_name)
 
         #Create a collection of sample vectors at the start position.
         #This has to be a list, not an array, as it can contain integer parameters,
         #unlike most samplers
         v0 = self.pipeline.start_vector(all_params=True, as_array=False)
         sample_vectors = [v0[:] for i in range(len(samples))]
         #Fill in the varied parameters. We are not using the
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.0/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import Sampler
+from ...runtime import logs
 import numpy as np
 
 
 class MaxlikeSampler(Sampler):
     sampler_outputs = [("prior", float), ("like", float), ("post", float)]
 
     def config(self):
@@ -33,20 +34,19 @@
         import scipy.optimize
 
         def likefn(p_in):
             #Check the normalization
             if (not np.all(p_in>=0)) or (not np.all(p_in<=1)):
                 return np.inf
             p = self.pipeline.denormalize_vector(p_in)
+            r = self.pipeline.run_results(p)
             if self.max_posterior:
-                like, extra = self.pipeline.posterior(p)
-                self.output.log_debug("%s  post=%f"%('   '.join(str(x) for x in p),like))
+                return -r.post
             else:
-                like, extra = self.pipeline.likelihood(p)
-                self.output.log_debug("%s  like=%f"%('   '.join(str(x) for x in p),like))
+                return -r.like
             return -like
 
         # starting position in the normalized space.  This will be taken from
         # a previous sampler if available, or the values file if not.
         start_vector = self.pipeline.normalize_vector(self.start_estimate())
         bounds = [(0.0, 1.0) for p in self.pipeline.varied_params]
 
@@ -63,20 +63,19 @@
         opt = self.pipeline.denormalize_vector(opt_norm)
         
 
         #Some output - first log the parameters to the screen.
         #It's not really a warning - that's just a level name
         results = self.pipeline.run_results(opt)
         if self.max_posterior:
-
-            self.output.log_warning("Best fit (by posterior):\n%s"%'   '.join(str(x) for x in opt))
+            logs.overview("Best fit (by posterior):\n%s"%'   '.join(str(x) for x in opt))
         else:
-            self.output.log_warning("Best fit (by likelihood):\n%s"%'   '.join(str(x) for x in opt))
-        self.output.log_warning("Posterior: {}\n".format(results.post))
-        self.output.log_warning("Likelihood: {}\n".format(results.like))
+            logs.overview("Best fit (by likelihood):\n%s"%'   '.join(str(x) for x in opt))
+        logs.overview("Posterior: {}\n".format(results.post))
+        logs.overview("Likelihood: {}\n".format(results.like))
 
         #Next save them to the proper table file
         self.output.parameters(opt, results.extra, results.prior, results.like, results.post)
 
         #If requested, create a new ini file for the
         #best fit.
         if self.output_ini:
@@ -94,15 +93,15 @@
             else:
                 covmat = self.pipeline.denormalize_matrix(result.hess_inv)
         elif hasattr(result, 'hess'):
             covmat = self.pipeline.denormalize_matrix(np.linalg.inv(result.hess_inv))
 
         if covmat is None:
             if self.output_cov:
-               self.output.log_error("Sorry - the optimization method you chose does not return a covariance (or Hessian) matrix")
+               logs.error("Sorry - the optimization method you chose does not return a covariance (or Hessian) matrix")
         else:
             if self.output_cov:
                 np.savetxt(self.output_cov, covmat)
             self.distribution_hints.set_cov(covmat)
 
         self.converged = True
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.0/cosmosis/samplers/metropolis/metropolis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import numpy as np
+from ...runtime import logs
 from .proposal.standard import Proposal, FastSlowProposal
 from copy import copy
 
 
 class Bad(object):
     def __init__(self):
         self.post = -np.inf
 
 
 class MCMC(object):
-    def __init__(self, start, posterior, covariance, quiet=False,
+    def __init__(self, start, posterior, covariance,
         tuning_frequency=-1, tuning_grace=np.inf, tuning_end=np.inf, 
         scaling=2.4,
         exponential_probability=0.33333,
         use_cobaya=False,
         n_drag=0):
         """
         posterior should return a PipelineResults object
         """
         #Set up basic variables
         self.posterior = posterior
         self.p = np.array(start)
         self.ndim = len(self.p)
-        self.quiet=quiet
         #Run the pipeline for the first time, on the 
         #starting point
         self.Lp = self.posterior(self.p)
 
         #Proposal
         self.covariance = covariance
         cholesky = np.linalg.cholesky(covariance)
@@ -106,50 +106,44 @@
         return samples
 
     def _sample_metropolis(self):
         # proposal point and its likelihood
         q = self.proposal.propose(self.p)
         #assume two proposal subsets for now
         Lq = self.posterior(q)
-        if not self.quiet:
-            print("  ".join(str(x) for x in q))
         #acceptance test
         delta = Lq.post - self.Lp.post
         if  accept(Lq.post, self.Lp.post):
             #update if accepted
             self.Lp = Lq
             self.p = q
             self.accepted += 1
             self.accepted_since_tuning += 1
-            if not self.quiet:
-                print("[Accept delta={:.3g}]\n".format(delta))
-        elif not self.quiet:
-            print("[Reject delta={:.3g}]\n".format(delta))
+            logs.info(f"[Accept delta={delta:.3g}")
+        else:
+            logs.info(f"[Reject delta={delta:.3g}]")
 
         return self.Lp
 
 
     def _sample_dragging(self):
         # get params with same fast params but different slow ones
-        if not self.quiet:
-            print("starting drag")
-            print("Current post = ", self.Lp.post)
+        logs.noisy("Starting drag")
+        logs.noisy(f"Current post = {self.Lp.post}")
         start = self.p
         end = self.proposal.propose_slow(start)
 
 
         # posteriors and derived parameters etc.
         r_start = copy(self.Lp)
         r_end = self.posterior(end)
-        if not self.quiet:
-            print("slow proposal post = ", r_end.post)
+        logs.noisy(f"slow proposal post = {r_end.post}")
 
         if not np.isfinite(r_end.post):
-            if not self.quiet:
-                print("[Reject: nan/-inf posterior]\n")
+            logs.noisy("[Reject: nan/-inf posterior]\n")
             return self.Lp
 
 
         # coordinates of current start and end
         p1 = copy(start)
         p2 = copy(end)
 
@@ -160,16 +154,15 @@
         start_post = r1.post
         end_post = r2.post
 
         drag_accepts = 0
 
         for i in range(self.n_drag):
             delta_fast = self.proposal.propose_fast(p1) - p1
-            if not self.quiet:
-                print("delta fast", delta_fast)
+            logs.debug("delta fast", delta_fast)
             q1 = p1 + delta_fast
             q2 = p2 + delta_fast
 
             s1 = self.posterior(q1)
 
             if np.isfinite(s1.post):
                 s2 = self.posterior(q2)
@@ -186,42 +179,37 @@
 
             if accept_drag:
                 p1 = q1
                 p2 = q2
                 r1 = s1
                 r2 = s2
                 drag_accepts += 1
-                if not self.quiet:
-                    print("[Accept drag step delta={:.3g}]\n".format(Q1 - P1))
-            elif not self.quiet:
-                print("[Reject drag step delta={:.3g}]\n".format(Q1 - P1))
+                logs.debug("[Accept drag step delta={:.3g}]\n".format(Q1 - P1))
+            else:
+                logs.debug("[Reject drag step delta={:.3g}]\n".format(Q1 - P1))
 
             start_post += r1.post
             end_post += r2.post
 
-        if not self.quiet:
-            print("[Accepted {}/{} drag steps]".format(drag_accepts,self.n_drag))
+        logs.noisy("[Accepted {}/{} drag steps]".format(drag_accepts,self.n_drag))
 
         start_post /= self.n_drag
         end_post /= self.n_drag
         accept_overall = accept(end_post, start_post)
 
-        if not self.quiet:
-            print("Done drag")
+        logs.noisy("Done drag")
         if accept_overall:
             self.p = p2
             self.Lp = r_end
             self.accepted += 1
             self.accepted_since_tuning += 1
-            if not self.quiet:
-                print("[Accept delta={:.3g}]\n".format(end_post - start_post))
+            logs.noisy("[Accept delta={:.3g}]\n".format(end_post - start_post))
             return r2
         else:
-            if not self.quiet:
-                print("[Reject delta={:.3g}]\n".format(end_post - start_post))
+            logs.noisy("[Reject delta={:.3g}]\n".format(end_post - start_post))
             return self.Lp
 
 
 
     def should_tune_now(self):
         return (    
             self.tuning_frequency>0
@@ -234,21 +222,15 @@
     def update_covariance_estimate(self):
         n = self.iterations
         self.mean_estimate = np.mean(self.chain, axis=0)
         C = np.cov(np.transpose(self.chain))
         if is_positive_definite(C):
             self.covariance_estimate = C
         else:
-            print("Cov estimate not SPD.  If this keeps happening, be concerned.")
-            # chain_outfile = 'joe_dump_chain_{}.txt'.format(self.n_cov_fail)
-            # cov_outfile = 'joe_dump_cov_{}.txt'.format(self.n_cov_fail)
-            # self.n_cov_fail += 1
-            # np.savetxt(chain_outfile, self.chain)
-            # np.savetxt(cov_outfile, np.transpose(C))
-            # print("TEMPORARY (JOE - REMOVE LATER) - dumping to file")
+            logs.warning("Cov estimate not SPD.  If this keeps happening, be concerned.")
 
 
     def set_fast_slow(self, fast_indices, slow_indices, oversampling):
         if self.n_drag:
             oversampling = 1
             print("Overriding oversampling parameter -> 1 since using dragging")
         self.fast_indices = fast_indices
@@ -271,31 +253,31 @@
         self.tuning_frequency = self.original_tuning_frequency * oversampling
 
     def tune(self):
         self.update_covariance_estimate()
 
         f = (self.covariance_estimate.diagonal()**0.5-self.last_covariance_estimate.diagonal()**0.5)/self.last_covariance_estimate.diagonal()**0.5
         i = abs(f).argmax()
-        print("Largest parameter sigma fractional change = {:.1f}% for param {}".format(100*f[i], i))
+        logs.overview("Largest parameter sigma fractional change = {:.1f}% for param {}".format(100*f[i], i))
         self.last_covariance_estimate = self.covariance_estimate.copy()
 
-        print("Accepted since last tuning: {}%".format((100.*self.accepted_since_tuning)/self.iterations_since_tuning))
+        logs.overview("Accepted since last tuning: {}%".format((100.*self.accepted_since_tuning)/self.iterations_since_tuning))
         self.accepted_since_tuning = 0
         self.iterations_since_tuning = 0
 
 
         if self.use_cobaya:
-            print("Tuning cobaya proposal.")
+            logs.overview("Tuning cobaya proposal.")
             self.proposal.set_covariance(self.covariance_estimate)
         elif isinstance(self.proposal, FastSlowProposal):
-            print("Tuning fast/slow sampler proposal.")
+            logs.overview("Tuning fast/slow sampler proposal.")
             self.proposal = FastSlowProposal(self.covariance_estimate, 
                 self.fast_indices, self.slow_indices, self.oversampling,scaling=self.scaling, exponential_probability=self.exponential_probability)
         elif isinstance(self.proposal, Proposal):
-            print("Tuning standard sampler proposal.")
+            logs.overview("Tuning standard sampler proposal.")
             cholesky = np.linalg.cholesky(self.covariance_estimate)
             self.proposal = Proposal(cholesky, scaling=self.scaling, exponential_probability=self.exponential_probability)
         else:
             #unknown proposal type
             pass
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.0/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 from . import metropolis
 from cosmosis.runtime.analytics import Analytics
 import os
 
 #We need a global pipeline
 #object for MPI to work properly
@@ -68,25 +69,21 @@
         #start values from prior
         start = self.define_parameters(random_start, covmat_sample_start, covmat)
         print("MCMC starting point:")
         for param, x in zip(self.pipeline.varied_params, start):
             print("    ", param, x)
 
 
-        #Sampler object itself.
-        quiet = self.pipeline.quiet
-
         if use_cobaya:
             print("Using the Cobaya proposal")
 
         print(f"Will tune every {tuning_frequency} samples, from samples "
               f"{tuning_grace} to {self.tuning_end}.")
 
         self.sampler = metropolis.MCMC(start, posterior, covmat,
-            quiet=quiet, 
             tuning_frequency=tuning_frequency, # Will be multiplied by the oversampling
             tuning_grace=tuning_grace,         # within the sampler if needed
             tuning_end=self.tuning_end,
             exponential_probability=self.exponential_probability,
             use_cobaya=use_cobaya,
             n_drag = self.drag,
         )
@@ -152,17 +149,17 @@
         self.num_samples += self.n
         self.num_samples_post_tuning = self.num_samples - self.tuning_end
 
 
         overall_rate = (self.sampler.accepted * 1.0) / self.sampler.iterations
         recent_accepted = self.sampler.accepted - self.last_accept_count
         recent_rate = recent_accepted / self.n
-        print("Overall accepted {} / {} samples ({:.1%})" .format(
+        logs.overview("Overall accepted {} / {} samples ({:.1%})" .format(
             self.sampler.accepted, self.sampler.iterations, overall_rate))
-        print("Last {0} accepted {1} / {0} samples ({2:.1%})\n" .format(
+        logs.overview("Last {0} accepted {1} / {0} samples ({2:.1%})\n" .format(
             self.n, recent_accepted, recent_rate))
         self.last_accept_count = self.sampler.accepted
 
         # Regardless of save settings we never use tuning samples
         # for analytics
         if self.num_samples_post_tuning > 0:
             traces = np.array([r.vector for r in samples[-self.num_samples_post_tuning:]])
@@ -170,30 +167,30 @@
 
 
         if (self.num_samples_post_tuning > 0) or self.save_during_tuning:
             for i, result in enumerate(samples):
                 self.output.parameters(result.vector, result.extra, result.prior, result.post)
 
         if self.num_samples_post_tuning <= 0:
-            print("Tuning ends at {} samples\n".format(self.tuning_end))
+            logs.overview("Tuning ends at {} samples\n".format(self.tuning_end))
 
         self.write_resume_info([self.sampler, self.num_samples, self.num_samples_post_tuning])
 
     def is_converged(self):
          # user has pressed Ctrl-C
         if self.interrupted:
             return True
         if self.num_samples >= self.samples:
             print("Full number of samples generated; sampling complete")
             return True
         elif (self.num_samples > 0 and
               self.pool is not None and
               self.Rconverge is not None and
               self.num_samples_post_tuning > 0):
-            R = self.analytics.gelman_rubin(quiet=False)
+            R = self.analytics.gelman_rubin()
             R1 = abs(R - 1)
             return np.all(R1 <= self.Rconverge)
         else:
             return False
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.0/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.0/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.0/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 import ctypes as ct
 import os
 import sys
-import collections
 
 MINUIT_INI_SECTION = "minuit"
 
 loglike_type = ct.CFUNCTYPE(
     ct.c_double, #likelihood
     ct.POINTER(ct.c_double),  #parameter cube
 )
@@ -88,17 +88,14 @@
         def wrapped_likelihood(cube_p):
             vector = np.frombuffer(cube_type.from_address(ct.addressof(cube_p.contents)))
             try:
                 like, extra = self.pipeline.posterior(vector)
             except KeyboardInterrupt:
                 sys.exit(1)
             self.iterations += 1
-            if self.verbose:
-                print(self.iterations, like, "   ",  "    ".join(str(v) for v in vector))
-                sys.stdout.flush()
             return -like
 
         self.wrapped_likelihood = wrapped_likelihood
 
 
     def execute(self):
         #Run an iteration of minuit
@@ -106,49 +103,41 @@
 
 
         #update the current parameters
         self.param_vector = param_vector.copy()
         self.neval += status
 
         if status == 0:
-            print() 
-            print("SUCCESS: Minuit has converged!")
-            print()
+            logs.overview("SUCCESS: Minuit has converged!")
             self.save_results(param_vector, param_names, results)
             self.converged = True
             self.distribution_hints.set_peak(param_vector)
 
             if made_cov:
                 cov_matrix = cov_vector.reshape((self.ndim, self.ndim))
                 self.distribution_hints.set_cov(cov_matrix)
         elif self.neval > self.maxiter:
-            print()
-            print("MINUIT has failed to converge properly in the max number of iterations.  Sorry.")
-            print("Saving the best fitting parameters of the ones we tried, though beware: these are probably not the best-fit")
-            print()
+            logs.error("MINUIT has failed to converge properly in the max number of iterations.  Sorry.")
+            logs.error("Saving the best fitting parameters of the ones we tried, though beware: these are probably not the best-fit")
             self.save_results(param_vector, param_names, results)
             #we actually just use self.converged to indicate that the 
             #sampler should stop now
             self.converged = True
 
         else:
-            print()
-            print("Minuit did not converge this run; trying again")
-            print("until we run out of iterations.")
-            print()
+            logs.overview("Minuit did not converge this run; trying again")
+            logs.overview("until we run out of iterations.")
             
 
 
     def save_results(self, param_vector, param_names, results):
         section = None
 
         if self.pool is not None:
-            print()
-            print("Note that the # of function calls printed above is not the total count for all cores, just for one core.")
-            print()
+            logs.error("Note that the # of function calls printed above is not the total count for all cores, just for one core.")
 
         self.output.parameters(param_vector, results.extra, results.prior, results.post)
 
         if self.output_ini:
             self.pipeline.create_ini(param_vector, self.output_ini)
 
         for name, value in zip(param_names, param_vector):
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.0/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #coding: utf-8
 from .. import ParallelSampler
+from ...runtime import logs
 import ctypes as ct
 import os
 import cosmosis
 import numpy as np
 import sys
 
 loglike_type = ct.CFUNCTYPE(ct.c_double, 
@@ -122,37 +123,33 @@
         self.mode_ztolerance    = self.read_ini("mode_ztolerance", float, default=0.5)
 
         #Parameters with wrap-around edges - can help sampling
         #of parameters which are relatively flat in likelihood
         wrapped_params = self.read_ini("wrapped_params", str, default="")
         wrapped_params = wrapped_params.split()
         self.wrapping = [0 for i in range(self.ndim)]
-        if wrapped_params:
-            print("")
         for p in wrapped_params:
             try:
                 P = p.split('--')
             except ValueError:
                 raise ValueError("You included {} in wrapped_params mulitnest option but should be format: section--name".format(p))
             if P in self.pipeline.varied_params:
                 index = self.pipeline.varied_params.index(P)
                 self.wrapping[index] = 1
                 print("MULTINEST: Parameter {} ({}) will be wrapped around the edge of its prior".format(index,p))
             elif P in self.pipeline.parameters:
-                print("MULTINEST NOTE: You asked for wrapped sampling on {}. That parameter is not fixed in this pipeline, so this will have no effect.".format(p))
+                print("MULTINEST NOTE: You asked for wrapped sampling on {}. That parameter is not varied in this pipeline, so this will have no effect.".format(p))
             else:
                 raise ValueError("You asked for an unknown parameter, {} to be wrapped around in the multinest wrapped_params option.".format(p))
-        if wrapped_params:
-            print("")
 
 
 
         if self.output:
             def dumper(nsample, nlive, nparam, live, post, paramConstr, max_log_like, logz, ins_logz, log_z_err, context):
-                print("Saving %d samples" % nsample)
+                logs.overview("Saving %d samples" % nsample)
                 self.output_params(nsample, live, post, logz, ins_logz, log_z_err)
             self.wrapped_output_logger = dumper_type(dumper)
         else:
             def dumper(nsample, nlive, nparam, live, post, paramConstr, max_log_like, logz, ins_logz, log_z_err, context):
                 return
             self.wrapped_output_logger = dumper_type(dumper)
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.0/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.0/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,22 @@
                        ("post", float)]
 
     def config(self):
         global pipeline
         pipeline = self.pipeline
 
         if self.is_master():
-            self.n_live = self.read_ini("n_live", int, 1500)
+            self.n_live = self.read_ini("n_live", int, 2000)
             self.n_update = self.read_ini("n_update", int, self.n_live)
             self.enlarge_per_dim = self.read_ini("enlarge_per_dim", float, 1.1)
             self.n_points_min = self.read_ini("n_points_min", int,
                                               self.pipeline.nvaried + 50)
             self.split_threshold = self.read_ini("split_threshold", float,
                                                  100.0)
             self.n_networks = self.read_ini("n_networks", int, 4)
-            self.n_jobs = self.read_ini("n_jobs", int, 1)
             self.n_batch = self.read_ini("n_batch", int, 100)
             self.seed = self.read_ini("seed", int, -1)
             if self.seed < 0:
                 self.seed = None
             self.resume_ = self.read_ini("resume", bool, False)
             self.f_live = self.read_ini("f_live", float, 0.01)
             self.n_shell = self.read_ini("n_shell", int, self.n_batch)
@@ -76,15 +75,14 @@
             n_dim,
             n_live=self.n_live,
             n_update=self.n_update,
             enlarge_per_dim=self.enlarge_per_dim,
             n_points_min=self.n_points_min,
             split_threshold=self.split_threshold,
             n_networks=self.n_networks,
-            n_jobs=self.n_jobs,
             n_batch=self.n_batch,
             seed=self.seed,
             filepath=resume_filepath,
             resume=self.resume_,
             pool=self.pool,
             blobs_dtype=float
         )
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.0/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,19 @@
     if maxlike_sampler.pool:
         rank = maxlike_sampler.pool.rank
     else:
         rank = 0
     if (not np.all(p_in>=0)) or (not np.all(p_in<=1.0)):
         nfail += 1
         pstr = '   '.join(str(x) for x in p_in)
-        print("[Proc {}] Posterior = NaN for out-of-bounds: (normalized) point = {}".format(rank, pstr))
-        print("[Proc {}] fails= {}".format(rank, nfail))
         return np.inf
     neval +=1 
     p = maxlike_sampler.pipeline.denormalize_vector(p_in)
     post, extra = maxlike_sampler.pipeline.posterior(p)
     pstr = '   '.join(str(x) for x in p)
-    print("[Proc {} (evals={})] Posterior = {} for {} (derivative:{})".format(rank, neval, post, pstr,index))
     return -post
 
 
 
 def posterior_and_gradient(p_in):
     pstr = '   '.join(str(x) for x in p_in)
     print("Calculating gradient about (normalized) point {}".format(pstr))
@@ -81,17 +78,16 @@
 
         opt_norm = result.x
         opt = self.pipeline.denormalize_vector(opt_norm)
         
         results = self.pipeline.run_results(opt)
 
         #Some output - first log the parameters to the screen.
-        #It's not really a warning - that's just a level name
-        self.output.log_warning("Best fit:\n%s"%'   '.join(str(x) for x in opt))
-        self.output.log_warning("Best likelihood: %f\n", results.like)
+        print("Best fit:\n%s"%'   '.join(str(x) for x in opt))
+        print("Best likelihood: %f\n", results.like)
 
         #Next save them to the proper table file
         self.output.parameters(opt, results.extra, results.prior, results.like, results.post)
 
         #If requested, create a new ini file for the
         #best fit.
         if self.output_ini:
@@ -107,15 +103,15 @@
         if hasattr(result, 'hess_inv'):
             covmat = self.pipeline.denormalize_matrix(result.hess_inv)
         elif hasattr(result, 'hess'):
             covmat = self.pipeline.denormalize_matrix(np.linalg.inv(result.hess_inv))
 
         if covmat is None:
             if self.output_cov:
-               self.output.log_error("Sorry - the optimization method you chose does not return a covariance (or Hessian) matrix")
+               print("Sorry - the optimization method you chose does not return a covariance (or Hessian) matrix")
         else:
             if self.output_cov:
                 np.savetxt(self.output_cov, covmat)
             self.distribution_hints.set_cov(covmat)
 
         self.converged = True
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.0/cosmosis/samplers/pmc/pmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ...runtime import logs
 from numpy import pi, dot, exp, einsum
 import numpy as np
 
 
 class PopulationMonteCarlo(object):
 	"""
 	A Population Monte Carlo (PMC) sampler,
@@ -9,15 +10,15 @@
 	importance sampling
 	
 	This code follows the notation and methodolgy in
 	http://arxiv.org/pdf/0903.0837v1.pdf
 
 
 	"""
-	def __init__(self, posterior, n, start, sigma, pool=None, quiet=False, student=False, nu=2.0):
+	def __init__(self, posterior, n, start, sigma, pool=None, student=False, nu=2.0):
 		"""
 		posterior: the posterior function
 		n: number of components to use in the mixture
 		start: estimated mean of the distribution
 		sigma: estimated covariance matrix
 		pool (optional): an MPI or multiprocessing worker pool
 
@@ -26,15 +27,14 @@
 		mu = np.random.multivariate_normal(start, sigma, size=n)
 
 		if student:
 			self.components = [StudentsTComponent(1.0/n, m, sigma, nu) for m in mu]
 		else:
 			self.components = [GaussianComponent(1.0/n, m, sigma) for m in mu]
 		self.pool = pool
-		self.quiet=quiet #not currently used
 
 	def sample(self, n, update=True, do_kill=True):
 		"Draw a sample from the Gaussian mixture and update the mixture"
 		self.kill_count = n*1./len(self.components)/50.
 		self.kill = [False for c in self.components]
 		#draw sample from current mixture
 		component_index, x = self.draw(n)
@@ -62,15 +62,15 @@
 		#Components to draw from
 		N = np.arange(len(self.components))
 		C = np.random.choice(N, size=n, replace=True, p=A)
 		for i in N:
 			count = np.sum(C==i)
 			if count<self.kill_count:
 				self.kill[i] = True
-				print("Component %d less than kill count (%d < %d)" % (i, count, self.kill_count))
+				logs.debug(f"Component {i} less than kill count ({count} < {self.kill_count})")
 		x = np.array([self.components[c].sample() for c in C])
 		return C, x
 
 	def update_components(self, x, log_post, update, do_kill):
 		"Equations 13-16 of arxiv.org 0903.0837v1"
 
 		#x #n_sample*n_dim
@@ -85,15 +85,15 @@
 			return logw
 
 		w_norm = w/w.sum()  #n_sample
 
 		logw_norm = np.log(w_norm)
 		entropy =  -(w_norm*logw_norm).sum()
 		perplexity = np.exp(entropy) / len(x)
-		print("Perplexity = ", perplexity)
+		logs.debug(f"Perplexity = {perplexity}")
 
 
 		Aphi[np.isnan(Aphi)] = 0.0
 		w_norm[np.isnan(w_norm)] = 0.0
 		A = [m.alpha for m in self.components]
 		#rho_top = einsum('i,ij->ij', A, phi)  #n_component * n_sample
 		rho_bottom = Aphi.sum(0) #n_sample
@@ -101,20 +101,20 @@
 
 
 
 		for d,(m,rho_d) in enumerate(zip(self.components, rho)):
 			try:
 				m.update(w_norm, x, rho_d)
 			except np.linalg.LinAlgError as error:
-				print("Component not fitting the data very well", d, str(error))
+				logs.debug(f"Component not fitting the data very well {d} {error}")
 				self.kill[d] = True
 
 		if do_kill:
 			self.components = [c for c,kill in zip(self.components,self.kill) if not kill]
-		print("%d components remain" % len(self.components))
+		logs.debug("%d components remain" % len(self.components))
 		return logw
 
 
 
 class GaussianComponent(object):
 	"""
 	A single Gaussian component of the mixture model.
@@ -136,15 +136,15 @@
 	def update(self, w_norm, x, rho_d):
 		"Update the parameters according to the samples and rho values"
 		alpha = dot(w_norm, rho_d)  #scalar
 		if not alpha>0:
 			raise np.linalg.LinAlgError("alpha = %f"%alpha)
 		mu = einsum('i,ij,i->j',w_norm, x, rho_d) / alpha  #scalar
 		delta = x-mu  #n_sample * n_dim
-		print("Updating to mu = ", mu)
+		logs.debug(f"Updating to mu = {mu}")
 		sigma = einsum('i,ij,ik,i->jk',w_norm, delta, delta, rho_d) / alpha  #n_dim * n_dim
 		self.set(alpha, mu, sigma)
 
 	def phi(self, x):
 		"Evaluate the distribution"
 		d = (x-self.mu) #n_sample * n_dim
 		chi2 = einsum('ij,jk,ik->i',d,self.sigma_inv,d)
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.0/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler
+from ...runtime import logs
 from . import pmc
 import numpy as np
 
 #needs to be global for MPI to behave
 #I think this is still true, at least
 global pipeline
 
@@ -26,35 +27,30 @@
             default=1000)
         self.final_samples = self.read_ini("final_samples", int, 
             default=5000)
 
         #Student's t mode
         student = self.read_ini("student", bool, default=False)
         if student:
-            print()
             print("WARNING")
-            print()
             print("Student's t mode probably not working yet")
             print("Unless you are testing you should probably set")
             print("student=F")
-            print()
-            print()
             nu = self.read_ini("nu", float, default=2.0)
         else:
             nu = None
 
 
         #start values from prior
         start = self.pipeline.start_vector()
         covmat = self.load_covariance_matrix()
 
         #Sampler object itself.
-        quiet = self.pipeline.quiet
         self.sampler = pmc.PopulationMonteCarlo(posterior, self.n_components, 
-            start, covmat, quiet=quiet, student=student, nu=nu, pool=self.pool)
+            start, covmat, student=student, nu=nu, pool=self.pool)
 
         self.interrupted = False
         self.iterations = 0
         self.samples = 0
 
     def execute(self):
         if self.iterations==self.n_iterations:
@@ -75,24 +71,23 @@
         self.iterations += 1
         self.samples += n
 
         for (vector, post, extra, component, weight) in zip(*results):
             prior, extra = extra
             self.output.parameters(vector, extra, (component, prior, post, weight))
 
-        print("Done %d iterations, %d samples" % (self.iterations, self.samples))
+        logs.overview("Done %d iterations, %d samples" % (self.iterations, self.samples))
 
 
     def is_converged(self):
          # user has pressed Ctrl-C
         if self.interrupted:
-            print("Interrupted...")
             return True
         if self.iterations >= self.n_iterations+1:
-            print("Full number of samples generated; sampling complete")
+            logs.overview("Full number of samples generated; sampling complete")
             self.output.final("nsample", self.final_samples)
 
             return True
         return False
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.0/cosmosis/samplers/poco/poco_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             # Starting positions and values for the chain
             self.num_samples = 0
             self.prob0 = None
 
             self.p0 = np.array(
                 [self.pipeline.randomized_start() for i in range(self.nparticles)]
             )
-            self.output.log_info(
+            print(
                 "Generating random starting positions from within prior"
             )
 
             bounds = np.array([p.limits for p in self.pipeline.varied_params])
 
             # Finally we can create the sampler
             self.sampler = self.pocomc.Sampler(
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding: utf-8
 from .. import ParallelSampler
+from ...runtime import logs
 import ctypes as ct
 import os
-import cosmosis
 import numpy as np
 import sys
-from cosmosis.runtime.utils import mkdir
+from ...runtime.utils import mkdir
 import warnings
 
 prior_type = ct.CFUNCTYPE(None, 
     ct.POINTER(ct.c_double),  #hypercube
     ct.POINTER(ct.c_double),  #physical
     ct.c_int,   #ndim
 )
@@ -143,15 +143,15 @@
         self.equally_weighted_posteriors = self.read_ini("equally_weighted_posteriors", bool, True)       
         self.cluster_posteriors = self.read_ini("cluster_posteriors", bool, True)
 
         self.fast_fraction    = self.read_ini("fast_fraction", float, 0.5)
 
         if self.output:
             def dumper(ndead, nlive, npars, live, dead, logweights, log_z, log_z_err):
-                print("Saving %d samples" % ndead)
+                logs.overview("Saving %d samples" % ndead)
                 self.output_params(ndead, nlive, npars, live, dead, logweights, log_z, log_z_err)
             self.wrapped_output_logger = dumper_type(dumper)
         else:
             def dumper(ndead, nlive, npars, live, dead, logweights, log_z, log_z_err):
                 pass
             self.wrapped_output_logger = dumper_type(dumper)
 
@@ -168,16 +168,14 @@
             for i in range(ndim):
                 theta[i] = theta_vector[i]
 
         self.wrapped_prior = prior_type(prior)
 
         def likelihood(theta, ndim, phi, nderived):
             theta_vector = np.array([theta[i] for i in range(ndim)])
-            if not self.pipeline.quiet:
-                print(theta_vector)
 
             if np.any(~np.isfinite(theta_vector)):
                 return -np.inf
 
             try:
                 r = self.pipeline.run_results(theta_vector)
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.0/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.0/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 import os
-import itertools
 from cosmosis.runtime.analytics import Analytics
 import logging
 
 
 class PymcSampler(ParallelSampler):
     sampler_outputs = [("like", float)]
 
@@ -94,15 +94,15 @@
         likes = -0.5 * self.mcmc.trace('deviance')[:]
 
         for trace, like in zip(traces, likes):
             self.output.parameters(trace, like)
 
         self.analytics.add_traces(traces)
 
-        self.output.log_noisy("Done %d iterations" % self.num_samples)
+        logs.overview(f"Done {self.num_samples} iterations")
 
     def worker(self):
         while not self.is_converged():
             self.sample()
 
     def execute(self):
         self.sample()
@@ -111,15 +111,15 @@
         # user has pressed Ctrl-C
         if self.interrupted:
             return True
         if self.num_samples >= self.samples:
             return True
         elif self.num_samples > 0 and self.pool is not None and \
             self.Rconverge is not None:
-            R = self.analytics.gelman_rubin(quiet=self.pipeline.quiet)
+            R = self.analytics.gelman_rubin()
             R1 = abs(R - 1)
             return np.all(R1 <= self.Rconverge)
         else:
             return False
 
     def load_covariance_matrix(self):
         covmat_filename = self.read_ini("covmat",str,"").strip()
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/sampler.py` & `cosmosis-3.0/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/snake/snake.py` & `cosmosis-3.0/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.0/cosmosis/samplers/snake/snake_sampler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .. import ParallelSampler
+from ...runtime import logs
 import numpy as np
 from .snake import Snake
 
 def posterior(p_in):
     #Check the normalization
     if (not np.all(p_in>=0)) or (not np.all(p_in<=1)):
-        print(p_in)
         return -np.inf, ([np.nan for i in range(len(snake_pipeline.extra_saves))], -np.inf)
     p = snake_pipeline.denormalize_vector(p_in)
     results = snake_pipeline.run_results(p)
     return results.post, (results.extra, results.prior)
 
 
 class SnakeSampler(ParallelSampler):
@@ -32,15 +32,15 @@
     def execute(self):
         X, P, E = self.snake.iterate()
         for (x,post,(extra, prior)) in zip(X,P,E):
             try:
                 x = self.pipeline.denormalize_vector(x)
                 self.output.parameters(x, extra, prior, post)
             except ValueError:
-                print("The snake is trying to escape its bounds!")
+                logs.noisy("The snake is trying to escape its bounds!")
 
 
 
     def is_converged(self):
         if self.snake.converged():
             print("Snake has converged!")
             print("Best post = %f    Best surface point = %f" %(self.snake.best_like_ever, self.snake.best_fit_like))
```

### Comparing `cosmosis-2.5.1/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.0/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.0/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.0/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .. import ParallelSampler, sample_ellipsoid, sample_ball
+from ...runtime import logs
 import numpy as np
 import sys
 
 
 def log_probability_function(p):
     r = zeus_pipeline.run_results(p)
     return r.post, (r.prior, r.extra)
@@ -81,24 +82,24 @@
             self.num_samples = 0
             self.prob0 = None
             self.blob0 = None
 
             # Generate starting point
             if start_file:
                 self.p0 = self.load_start(start_file)
-                self.output.log_info("Loaded starting position from %s", start_file)
+                print("Loaded starting position from %s", start_file)
             elif self.distribution_hints.has_cov():
                 center = self.start_estimate()
                 cov = self.distribution_hints.get_cov()
                 self.p0 = sample_ellipsoid(center, cov, size=self.nwalkers)
-                self.output.log_info("Generating starting positions from covmat from earlier in pipeline")
+                print("Generating starting positions from covmat from earlier in pipeline")
             elif covmat_file:
                 center = self.start_estimate()
                 cov = self.load_covmat(covmat_file)
-                self.output.log_info("Generating starting position from covmat in  %s", covmat_file)
+                print("Generating starting position from covmat in  %s", covmat_file)
                 iterations_limit = 100000
                 n=0
                 p0 = []
                 for i in range(iterations_limit):
                     p = sample_ellipsoid(center, cov)[0]
                     if np.isfinite(self.pipeline.prior(p)):
                         p0.append(p)
@@ -106,23 +107,23 @@
                         break
                 else:
                     raise ValueError("The covmat you used could not generate points inside the prior")
                 self.p0 = np.array(p0)
             elif random_start:
                 self.p0 = [self.pipeline.randomized_start()
                            for i in range(self.nwalkers)]
-                self.output.log_info("Generating random starting positions from within prior")
+                print("Generating random starting positions from within prior")
             else:
                 center_norm = self.pipeline.normalize_vector(self.start_estimate())
                 sigma_norm=np.repeat(1e-3, center_norm.size)
                 p0_norm = sample_ball(center_norm, sigma_norm, size=self.nwalkers)
                 p0_norm[p0_norm<=0] = 0.001
                 p0_norm[p0_norm>=1] = 0.999
                 self.p0 = [self.pipeline.denormalize_vector(p0_norm_i) for p0_norm_i in p0_norm]
-                self.output.log_info("Generating starting positions in small ball around starting point")
+                print("Generating starting positions in small ball around starting point")
 
             #Finally we can create the sampler
             self.started = False
             self.sampler = self.zeus.EnsembleSampler(self.nwalkers, self.ndim,
                                                      log_probability_function,
                                                      tune=self.tune,
                                                      tolerance=self.tolerance,
```

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/Makefile` & `cosmosis-3.0/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.0/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.0/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.0/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.0/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.0/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.0/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.0/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_block.py` & `cosmosis-3.0/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_chaining.py` & `cosmosis-3.0/cosmosis/test/test_chaining.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,31 +21,29 @@
                 "p1=-3.0  0.0  3.0\n"
                 "p2=-3.0  0.0  3.0\n")
 
         params = {
             ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
             ('runtime', 'sampler'):  "maxlike fisher emcee",
             ("pipeline", "debug"): "T",
-            ("pipeline", "quiet"): "F",
             ("pipeline", "modules"): "test1",
             ("pipeline", "extra_output"): "parameters/p3",
             ("pipeline", "values"): values_file,
-            ("test1", "file"): "test_module.py",
+            ("test1", "file"): "example_module.py",
             ("output", "filename"): emcee_file,
             ("emcee", "walkers"): "8",
             ("emcee", "samples"): "100",
             ("maxlike", "tolerance"): "0.05",
             ("fisher", "step_size"): "0.01"
         }
 
 
-        args = parser.parse_args(["not_a_real_file"])
         ini = Inifile(None, override=params)
 
-        status = run_cosmosis(args, ini=ini)
+        status = run_cosmosis(ini)
 
         data = np.loadtxt(fisher_file)
         print(data.shape)
 
         data = np.loadtxt(maxlike_file)
         print(data.shape)
```

### Comparing `cosmosis-2.5.1/cosmosis/test/test_gaussian.py` & `cosmosis-3.0/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_lib.py` & `cosmosis-3.0/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_module2.py` & `cosmosis-3.0/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_modules.py` & `cosmosis-3.0/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_parameters.py` & `cosmosis-3.0/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_pipeline.py` & `cosmosis-3.0/cosmosis/test/test_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,17 @@
         "p1=-3.0  0.0  3.0\n"
         "p2=-3.0  0.0  3.0\n")
     values.flush()
 
     override = {
         ('runtime', 'root'): root,
         ("pipeline", "debug"): "F",
-        ("pipeline", "quiet"): "T",
         ("pipeline", "modules"): "test2",
         ("pipeline", "values"): values.name,
-        ("test2", "file"): "test_module2.py",
+        ("test2", "file"): "example_module2.py",
         ("emcee", "walkers"): "8",
         ("emcee", "samples"): "10"
     }
 
     ini = Inifile(None, override=override)
 
     # Make the pipeline itself
@@ -73,22 +72,22 @@
     assert p3.min() > -1.0
 
     return output
 
 def test_missing_setup():
     # check the register_new_parameter feature when no
     # setup is currently happening
-    module = Module("test2", root + "/test_module2.py")
+    module = Module("test2", root + "/example_module2.py")
     config = DataBlock()
     module.setup(config)
 
 def test_unused_param_warning(capsys):
     # check that an appropriate warning is generated
     # when a parameter is unused
-    module = Module("test", root + "/test_module.py")
+    module = Module("test", root + "/example_module.py")
     config = DataBlock()
     config['test', 'unused'] = "unused_parameter"
     module.setup(config)
     out, _ = capsys.readouterr()
     assert "**** WARNING: Parameter 'unused'" in out
 
 def test_vector_extra_outputs():
@@ -102,27 +101,25 @@
                 "p1=-3.0  0.0  3.0\n"
                 "p2=-3.0  0.0  3.0\n")
 
         params = {
             ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
             ('runtime', 'sampler'):  "emcee",
             ("pipeline", "debug"): "T",
-            ("pipeline", "quiet"): "F",
             ("pipeline", "modules"): "test1",
             ("pipeline", "extra_output"): "data_vector/test_theory#2",
             ("pipeline", "values"): values_file,
-            ("test1", "file"): "test_module.py",
+            ("test1", "file"): "example_module.py",
             ("output", "filename"): output_file,
             ("emcee", "walkers"): "8",
             ("emcee", "samples"): "10",
         }
 
-        args = parser.parse_args(["not_a_real_file"])
         ini = Inifile(None, override=params)
-        status = run_cosmosis(args, ini=ini)
+        status = run_cosmosis(ini)
 
         with open(output_file) as f:
             header = f.readline()
 
         assert "data_vector--test_theory_0" in header.lower()
         assert "data_vector--test_theory_1" in header.lower()
 
@@ -143,26 +140,24 @@
                 "p1=-3.0  0.0  3.0\n"
                 "p2=-3.0  0.0  3.0\n")
 
         params = {
             ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
             ('runtime', 'sampler'):  "emcee",
             ("pipeline", "debug"): "T",
-            ("pipeline", "quiet"): "F",
             ("pipeline", "modules"): "test1",
             ("pipeline", "values"): values_file,
-            ("test1", "file"): "test_module.py",
+            ("test1", "file"): "example_module.py",
             ("output", "filename"): output_file,
             ("emcee", "walkers"): "8",
             ("emcee", "samples"): "10",
         }
 
-        args = parser.parse_args(["not_a_real_file", "--profile", stats_file])
         ini = Inifile(None, override=params)
-        status = run_cosmosis(args, ini=ini)
+        status = run_cosmosis(ini, profile_cpu=stats_file)
 
         output = capsys.readouterr()
         assert "cumtime" in output.out
 
         stats = pstats.Stats(stats_file)
         stats.sort_stats("cumtime")
         stats.print_stats(10)
@@ -182,31 +177,29 @@
 
         params = {
             ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
             ('runtime', 'pre_script'): "this_executable_does_not_exist",
             ('runtime', 'post_script'): "this_executable_does_not_exist",
             ('runtime', 'sampler'):  "test",
             ("pipeline", "debug"): "F",
-            ("pipeline", "quiet"): "F",
             ("pipeline", "modules"): "test1",
             ("pipeline", "values"): values_file,
-            ("test1", "file"): "test_module.py",
+            ("test1", "file"): "example_module.py",
             ("output", "filename"): output_file,
         }
 
-        args = parser.parse_args(["not_a_real_file"])
         ini = Inifile(None, override=params)
 
         with pytest.raises(RuntimeError):
-            status = run_cosmosis(args, ini=ini)
+            status = run_cosmosis(ini)
 
         # shopuld work this time
         try:
             os.environ["COSMOSIS_NO_SUBPROCESS"] = "1"
-            status = run_cosmosis(args, ini=ini)
+            status = run_cosmosis(ini)
         finally:
             del os.environ["COSMOSIS_NO_SUBPROCESS"]
 
 def test_prior_override():
     with tempfile.TemporaryDirectory() as dirname:
         values_file = f"{dirname}/values.ini"
         output_file = f"{dirname}/output.txt"
@@ -217,31 +210,30 @@
                 "p2=-3.0  0.0  3.0\n")
 
         params = {
             ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
             ('runtime', 'sampler'):  "apriori",
             ('apriori', 'nsample'):  "1000",
             ("pipeline", "debug"): "F",
-            ("pipeline", "quiet"): "F",
             ("pipeline", "modules"): "test1",
             ("pipeline", "values"): values_file,
-            ("test1", "file"): "test_module.py",
+            ("test1", "file"): "example_module.py",
             ("output", "filename"): output_file,
         }
 
         args = parser.parse_args(["not_a_real_file"])
         ini = Inifile(None, override=params)
 
         priors_vals = {
             ('parameters', 'p1'): 'uniform -1.0    1.0'
         }
 
         priors = Inifile(None, override=priors_vals)
 
-        status = run_cosmosis(args, ini=ini, priors=priors)
+        status = run_cosmosis(ini, priors=priors)
         chain = np.loadtxt(output_file).T
         p1 = chain[0]
         p2 = chain[1]
         print(p1.min(), p1.max())
         assert p1.max() < 1.0
         assert p1.min() > -1.0
```

### Comparing `cosmosis-2.5.1/cosmosis/test/test_polychord.py` & `cosmosis-3.0/cosmosis/test/test_polychord.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,23 +26,22 @@
         "p2=-3.0  0.0  3.0\n"
         "p4=-3.0  0.0  3.0\n")
     values.flush()
 
     override = {
         ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
         ("pipeline", "debug"): "F",
-        ("pipeline", "quiet"): "T",
         ("pipeline", "modules"): "test1  test3 test4",
         ("pipeline", "extra_output"): "parameters/p3",
         ("pipeline", "values"): values.name,
         ("pipeline", "fast_slow"): str(fast_slow)[0],
         ("pipeline", "first_fast_module"): "test4",
-        ("test1", "file"): "test_module.py",
-        ("test3", "file"): "test_module3.py",
-        ("test4", "file"): "test_module4.py",
+        ("test1", "file"): "example_module.py",
+        ("test3", "file"): "example_module3.py",
+        ("test4", "file"): "example_module4.py",
     }
 
     for k,v in options.items():
         override[(sampler,k)] = str(v)
 
 
     ini = Inifile(None, override=override)
```

### Comparing `cosmosis-2.5.1/cosmosis/test/test_samplers.py` & `cosmosis-3.0/cosmosis/test/test_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from cosmosis.output.in_memory_output import InMemoryOutput
 from cosmosis.postprocessing import postprocessor_for_sampler
 import tempfile
 import os
 import sys
 import pytest
 import numpy as np
+from astropy.table import Table
 
 minuit_compiled = os.path.exists(cosmosis.samplers.minuit.minuit_sampler.libname)
 
 def run(name, check_prior, check_extra=True, can_postprocess=True, do_truth=False, no_extra=False, pp_extra=True, pp_2d=True, **options):
 
     sampler_class = Sampler.registry[name]
 
@@ -22,19 +23,18 @@
         "p1=-3.0  0.0  3.0\n"
         "p2=-3.0  0.0  3.0\n")
     values.flush()
 
     override = {
         ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
         ("pipeline", "debug"): "F",
-        ("pipeline", "quiet"): "T",
         ("pipeline", "modules"): "test1",
         ("pipeline", "extra_output"): "parameters/p3",
         ("pipeline", "values"): values.name,
-        ("test1", "file"): "test_module.py",
+        ("test1", "file"): "example_module.py",
     }
 
     for k,v in options.items():
         override[(name,k)] = str(v)
 
     if no_extra:
         del override[("pipeline", "extra_output")]
@@ -70,42 +70,49 @@
         pp_class = postprocessor_for_sampler(name)
         print(pp_class)
         with tempfile.TemporaryDirectory() as dirname:
             truth_file = values.name if do_truth else None
             pp = pp_class(output, "Chain", 0, outdir=dirname, prefix=name, truth=truth_file)
             pp_files = pp.run()
             pp.finalize()
+            pp.save()
             for p in pp_files:
                 print(p)
             postprocess_files = ['parameters--p1', 'parameters--p2']
             if pp_2d:
                 postprocess_files.append('2D_parameters--p2_parameters--p1')
             if check_extra and pp_extra and not no_extra:
                 postprocess_files.append('parameters--p3')
                 if pp_2d:
                     postprocess_files += ['2D_parameters--p3_parameters--p2', '2D_parameters--p3_parameters--p1']
             for p in postprocess_files:
                 filename = f"{dirname}{os.path.sep}{name}_{p}.png"
                 print("WANT ", filename)
                 assert filename in pp_files
                 assert os.path.exists(filename)
+            for p in os.listdir(dirname):
+                p = os.path.join(dirname, p)
+                if p.endswith(".txt"):
+                    Table.read(p, format='ascii.commented_header')
+                    print(f"Read file {p} as a table")
 
 
     return output
 
 
 def test_apriori():
     run('apriori', True, can_postprocess=False, nsample=100)
 
 def test_dynesty():
     # dynesty does not support extra params
     run('dynesty', False, check_extra=False, nlive=50, sample='unif')
 
 def test_emcee():
     run('emcee', True, walkers=8, samples=100)
+    run('emcee', True, walkers=8, samples=100, a=3.0)
 
 def test_truth():
     run('emcee', True, walkers=8, samples=100, do_truth=True)
 
 def test_fisher():
     run('fisher', False, check_extra=False)
```

### Comparing `cosmosis-2.5.1/cosmosis/test/test_text_output.py` & `cosmosis-3.0/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/test/test_utils.py` & `cosmosis-3.0/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.5.1/cosmosis/utils.py` & `cosmosis-3.0/cosmosis/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,34 +131,39 @@
     fd = getattr(file_or_fd, 'fileno', lambda: file_or_fd)()
     if not isinstance(fd, int):
         raise ValueError("Expected a file (`.fileno()`) or a file descriptor")
     return fd
 
 @contextmanager
 def stdout_redirected(to=os.devnull, stdout=None):
+    from .runtime import logs
     if stdout is None:
        stdout = sys.stdout
 
     stdout_fd = fileno(stdout)
     # copy stdout_fd before it is overwritten
     #NOTE: `copied` is inheritable on Windows when duplicating a standard stream
     with os.fdopen(os.dup(stdout_fd), 'wb') as copied: 
         stdout.flush()  # flush library buffers that dup2 knows nothing about
+        log_level = logs.get_level()
+        logs.set_level(51)
         try:
             os.dup2(fileno(to), stdout_fd)  # $ exec >&to
         except ValueError:  # filename
             with open(to, 'wb') as to_file:
                 os.dup2(to_file.fileno(), stdout_fd)  # $ exec > to
         try:
             yield stdout # allow code to be run with the redirected stdout
         finally:
             # restore stdout to its previous value
             #NOTE: dup2 makes stdout_fd inheritable unconditionally
             stdout.flush()
             os.dup2(copied.fileno(), stdout_fd)  # $ exec >&copied
+            logs.set_level(log_level)
+
 
 
 
 
 
 
 
@@ -335,26 +340,58 @@
     if p.returncode:
         return ""
     # There shouldn't be any newlines here, but in case there are in future
     # we replace them with spaces to avoid messing up output file formats
     return rev.decode('utf-8').strip().replace("\n", " ")
 
 
-def requires_python3(f):
-    @wraps(f)
-    def wrapper(*args, **kwargs):
-        if sys.version_info[0] < 3:
-            raise RuntimeError(
-                "You are using a CosmoSIS function ({}) "
-                " only available in python 3 and above".format(f))
-        return f(*args, **kwargs)
-    return wrapper
-
 
-@requires_python3
 def import_by_path(name, path):
     # https://stackoverflow.com/questions/67631/how-to-import-a-module-given-the-full-path
     import importlib.util
     spec = importlib.util.spec_from_file_location(name, path)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module
+
+
+def underline(s, char='-'):
+    """
+    Return a string with a line of the given character
+    underneath it.
+
+    Parameters
+    ----------
+    s : str
+        The string to underline
+    char : str, optional
+        The character to use for the line
+    """
+    return s + "\n" + char * len(s)
+
+def overline(s, char='-'):
+    """
+    Return a string with a line of the given character
+    over it.
+
+    Parameters
+    ----------
+    s : str
+        The string to overline
+    char : str, optional
+        The character to use for the line
+    """
+    return char * len(s) + "\n" + s
+
+def under_over_line(s, char='-'):
+    """
+    Return a string with a line of the given character
+    over and under it.
+
+    Parameters
+    ----------
+    s : str
+        The string to overline
+    char : str, optional
+        The character to use for the line
+    """
+    return underline(overline(s, char), char)
```

### Comparing `cosmosis-2.5.1/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.0/cosmosis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 bin/cosmosis
+bin/cosmosis-campaign
 bin/cosmosis-configure
 bin/cosmosis-extract
 bin/cosmosis-postprocess
 bin/cosmosis-sample-fisher
 cosmosis/Makefile
 cosmosis/__init__.py
+cosmosis/campaign.py
 cosmosis/configure.py
 cosmosis/constants.py
 cosmosis/gaussian_likelihood.py
 cosmosis/main.py
 cosmosis/names.py
 cosmosis/postprocess.py
 cosmosis/utils.py
@@ -55,14 +57,15 @@
 cosmosis/datablock/cosmosis_py/__init__.py
 cosmosis/datablock/cosmosis_py/block.py
 cosmosis/datablock/cosmosis_py/dbt_types.py
 cosmosis/datablock/cosmosis_py/errors.py
 cosmosis/datablock/cosmosis_py/lib.py
 cosmosis/datablock/cosmosis_py/section_names.py
 cosmosis/output/__init__.py
+cosmosis/output/astropy_output.py
 cosmosis/output/cosmomc_output.py
 cosmosis/output/fits_output.py
 cosmosis/output/in_memory_output.py
 cosmosis/output/null_output.py
 cosmosis/output/output_base.py
 cosmosis/output/text_output.py
 cosmosis/output/utils.py
@@ -76,27 +79,29 @@
 cosmosis/postprocessing/__init__.py
 cosmosis/postprocessing/cosmology_theory_plots.py
 cosmosis/postprocessing/density.py
 cosmosis/postprocessing/elements.py
 cosmosis/postprocessing/inputs.py
 cosmosis/postprocessing/latex.ini
 cosmosis/postprocessing/lazy_pylab.py
+cosmosis/postprocessing/main.py
 cosmosis/postprocessing/outputs.py
 cosmosis/postprocessing/plots.py
 cosmosis/postprocessing/postprocess.py
 cosmosis/postprocessing/postprocess_base.py
 cosmosis/postprocessing/reruns.py
 cosmosis/postprocessing/statistics.py
 cosmosis/postprocessing/utils.py
 cosmosis/runtime/__init__.py
 cosmosis/runtime/analytics.py
 cosmosis/runtime/attribution.py
 cosmosis/runtime/config.py
 cosmosis/runtime/declare.py
 cosmosis/runtime/handler.py
+cosmosis/runtime/logs.py
 cosmosis/runtime/memmon.py
 cosmosis/runtime/module.py
 cosmosis/runtime/mpi_pool.py
 cosmosis/runtime/parameter.py
 cosmosis/runtime/pipeline.py
 cosmosis/runtime/prior.py
 cosmosis/runtime/process_pool.py
@@ -199,22 +204,27 @@
 cosmosis/samplers/star/__init__.py
 cosmosis/samplers/star/star_sampler.py
 cosmosis/samplers/test/__init__.py
 cosmosis/samplers/test/test_sampler.py
 cosmosis/samplers/zeus/__init__.py
 cosmosis/samplers/zeus/zeus_sampler.py
 cosmosis/test/__init__.py
+cosmosis/test/campaign.yml
+cosmosis/test/example-priors.ini
+cosmosis/test/example-values.ini
+cosmosis/test/example.ini
+cosmosis/test/example_module.py
+cosmosis/test/example_module2.py
+cosmosis/test/example_module3.py
+cosmosis/test/example_module4.py
 cosmosis/test/test_block.py
+cosmosis/test/test_campaign.py
 cosmosis/test/test_chaining.py
 cosmosis/test/test_gaussian.py
 cosmosis/test/test_lib.py
-cosmosis/test/test_module.py
-cosmosis/test/test_module2.py
-cosmosis/test/test_module3.py
-cosmosis/test/test_module4.py
 cosmosis/test/test_modules.py
 cosmosis/test/test_parameters.py
 cosmosis/test/test_pipeline.py
 cosmosis/test/test_polychord.py
 cosmosis/test/test_samplers.py
 cosmosis/test/test_text_output.py
 cosmosis/test/test_utils.py
```

### Comparing `cosmosis-2.5.1/setup.py` & `cosmosis-3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import setuptools
-import distutils.command.build
-import distutils.command.clean
-import distutils.command.install
+import setuptools.command.install
+import setuptools.command.build_py
 import setuptools.command.develop
 import subprocess
 import os
 
 version = open('cosmosis/version.py').read().split('=')[1].strip().strip("'")
 
 
@@ -14,14 +13,15 @@
     "datablock/cosmosis_types.mod",
     "datablock/cosmosis_wrappers.mod",
     "datablock/cosmosis_modules.mod",
 ]
 
 scripts = [
     'bin/cosmosis',
+    'bin/cosmosis-campaign',
     'bin/cosmosis-configure',
     'bin/cosmosis-extract',
     'bin/cosmosis-sample-fisher',
     'bin/cosmosis-postprocess',
 ]
 
 c_headers = [
@@ -66,14 +66,19 @@
     "test/libtest/datablock_test.cc",
     "test/libtest/entry_test.cc",
     "test/libtest/ndarray_test.cc",
     "test/libtest/section_test.cc",
     "test/libtest/test_c_datablock_scalars.h",
     "test/libtest/test_c_datablock_scalars.template",
     "test/libtest/Makefile",
+    "test/campaign.yml",
+    "test/example-priors.ini",
+    "test/example-values.ini",
+    "test/example.ini",
+
 ]
 
 other_files = ["postprocessing/latex.ini"]
 
 compilers_config = ["config/compilers.mk", "config/subdirs.mk"]
 
 
@@ -120,25 +125,18 @@
 
     env['FC'] = env.get('FC', 'gfortran')
 
     subprocess.check_call(["make"], env=env, cwd="cosmosis")
 
 
 
-class build_cosmosis(setuptools.Command):
-    description = "Run the CosmoSIS build process"
-    user_options = []
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
+class build_py_cosmosis(setuptools.command.build_py.build_py):
     def run(self):
         make_cosmosis()
+        super().run()
 
 class clean_cosmosis(setuptools.Command):
     description = "Run the CosmoSIS clean process"
     user_options = []
 
     def initialize_options(self):
         pass
@@ -148,31 +146,27 @@
 
     def run(self):
         print("Running CosmoSIS main library clean command")
         cosmosis_src_dir = get_COSMOSIS_SRC_DIR()
         env = {"COSMOSIS_SRC_DIR": cosmosis_src_dir,}
         subprocess.check_call(["make", "clean"], env=env, cwd="cosmosis")
 
-        # Run the original clean command
-        self.run_command("clean_original")
-
-class install_cosmosis(distutils.command.install.install):
+class install_cosmosis(setuptools.command.install.install):
     description = "Run the CosmoSIS install process"
 
     def run(self):
         make_cosmosis()
         super().run()
 
 class develop_cosmosis(setuptools.command.develop.develop):
     description = "Install CosmoSIS in editable mode"
     def run(self):
         make_cosmosis()
         super().run()
 
-distutils.command.build.build.sub_commands.insert(0, ("build_cosmosis", None))
 
 requirements = [
     "pyyaml",
     "emcee",
     "numpy",
     "scipy",
     "matplotlib",
@@ -190,27 +184,25 @@
 
 ]
 
 all_package_files = (datablock_libs + sampler_libs
                             + c_headers + cc_headers + f90_mods 
                             + compilers_config + testing_files + other_files)
 
-
 setuptools.setup(name = 'cosmosis',
     description       = "The CosmoSIS parameter estimation library.",
     author            = "Joe Zuntz",
     author_email      = "joezuntz@googlemail.com",
     url               = "https://github.com/joezuntz/cosmosis",
     packages = setuptools.find_packages(),
     package_data = {"cosmosis" : all_package_files},
     scripts = scripts,
     install_requires = requirements,
     cmdclass={
-        "build_cosmosis": build_cosmosis,
+        "build_py": build_py_cosmosis,
         "install": install_cosmosis,
         "develop": develop_cosmosis,
         "clean": clean_cosmosis,
-        "clean_original": distutils.command.clean.clean,
     },
     version=version,
 )
```

