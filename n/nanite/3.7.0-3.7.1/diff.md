# Comparing `tmp/nanite-3.7.0.tar.gz` & `tmp/nanite-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanite-3.7.0.tar", last modified: Mon Jul 24 13:26:43 2023, max compression
+gzip compressed data, was "nanite-3.7.1.tar", last modified: Thu Jul 27 13:05:17 2023, max compression
```

## Comparing `nanite-3.7.0.tar` & `nanite-3.7.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.675730 nanite-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 13:26:27.000000 nanite-3.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 13:26:27.000000 nanite-3.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-24 13:26:27.000000 nanite-3.7.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 13:26:27.000000 nanite-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 13:26:27.000000 nanite-3.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 13:26:43.675730 nanite-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 13:26:27.000000 nanite-3.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/data/
--rw-r--r--   0 runner    (1001) docker     (123)   131520 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/data/force-save-example.jpk-force
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/fancy_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/nanite_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/nanite_preprocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/extensions/simple_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28646 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/fitting_geometry.png
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/fitting_geometry.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/img/nanite-fit-example.png
--rw-r--r--   0 runner    (1001) docker     (123)    86373 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/img/nanite-rate-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/nanite.bib
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_code_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_fitting_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_rating_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 13:26:27.000000 nanite-3.7.0/docs/sec_z_bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.647730 nanite-3.7.0/examples/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)   159955 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/data/zebrafish-head-section-gray-matter.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/fit_and_rate.png
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/fit_and_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/generate_example_images.py
--rw-r--r--   0 runner    (1001) docker     (123)   104455 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/model_spherical_indenter.png
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-24 13:26:27.000000 nanite-3.7.0/examples/model_spherical_indenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/cli/rating.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/indent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.655730 nanite-3.7.0/nanite/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_conical_indenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_hertz_paraboloidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_hertz_three_sided_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_sneddon_spherical.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/model_sneddon_spherical_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/model/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/poc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/qmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.655730 nanite-3.7.0/nanite/rate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/rater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/regressors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.659730 nanite-3.7.0/nanite/rate/ts_zef18/
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_bin_size.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/rate/ts_zef18/train_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-24 13:26:27.000000 nanite-3.7.0/nanite/smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.651730 nanite-3.7.0/nanite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 13:26:43.000000 nanite-3.7.0/nanite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-24 13:26:27.000000 nanite-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:26:43.675730 nanite-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-24 13:26:27.000000 nanite-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.663730 nanite-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:26:43.675730 nanite-3.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/cli-profile-1.7.8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/cli-profile-2.1.0.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    68411 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   158553 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   497346 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   407527 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
--rwxr-xr-x   0 runner    (1001) docker     (123)  1645418 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   953060 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   401583 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
--rw-r--r--   0 runner    (1001) docker     (123)   400957 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
--rwxr-xr-x   0 runner    (1001) docker     (123)   193751 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101264 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101240 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   103538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   101531 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)   311042 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6785 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
--rwxr-xr-x   0 runner    (1001) docker     (123)     6799 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   596184 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)   188079 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/model_external_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    93520 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/data/rate-export_1.7.8.h5
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_cli_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_emodulus_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_indent2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_parabol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_hertz_pyramid_three.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_sneddon_spherical_invert_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_model_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_open_jpk_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_poc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_qmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_rate_training_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-24 13:26:27.000000 nanite-3.7.0/tests/test_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.043677 nanite-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-27 13:05:01.000000 nanite-3.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-27 13:05:01.000000 nanite-3.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-27 13:05:01.000000 nanite-3.7.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 13:05:01.000000 nanite-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-27 13:05:01.000000 nanite-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-27 13:05:17.043677 nanite-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-27 13:05:01.000000 nanite-3.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.011677 nanite-3.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.011677 nanite-3.7.1/docs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   131520 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/data/force-save-example.jpk-force
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.011677 nanite-3.7.1/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/extensions/fancy_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/extensions/nanite_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/extensions/nanite_preprocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/extensions/simple_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28646 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/fitting_geometry.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/fitting_geometry.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.011677 nanite-3.7.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/img/nanite-fit-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86373 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/img/nanite-rate-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/nanite.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_code_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_fitting_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_rating_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 13:05:01.000000 nanite-3.7.1/docs/sec_z_bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.015677 nanite-3.7.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.015677 nanite-3.7.1/examples/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159955 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/data/zebrafish-head-section-gray-matter.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/fit_and_rate.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/fit_and_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/generate_example_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104455 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/model_spherical_indenter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-27 13:05:01.000000 nanite-3.7.1/examples/model_spherical_indenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.015677 nanite-3.7.1/nanite/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.015677 nanite-3.7.1/nanite/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/cli/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/cli/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/indent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.019677 nanite-3.7.1/nanite/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/model_conical_indenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/model_hertz_paraboloidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/model_hertz_three_sided_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/model_sneddon_spherical.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/model/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/qmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.019677 nanite-3.7.1/nanite/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/regressors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.023677 nanite-3.7.1/nanite/rate/ts_zef18/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_bin_apr_spikes_count.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_bin_cp_position.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_bin_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_size.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/rate/ts_zef18/train_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-27 13:05:01.000000 nanite-3.7.1/nanite/smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.015677 nanite-3.7.1/nanite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 13:05:16.000000 nanite-3.7.1/nanite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 13:05:01.000000 nanite-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:05:17.043677 nanite-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 13:05:01.000000 nanite-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.027677 nanite-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:17.043677 nanite-3.7.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/cli-profile-1.7.8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/cli-profile-2.1.0.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68411 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   158553 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   497346 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   407527 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1645418 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   953060 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   401583 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map
+-rw-r--r--   0 runner    (1001) docker     (123)   400957 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map
+-rwxr-xr-x   0 runner    (1001) docker     (123)   193751 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101264 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101240 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   103538 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101531 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)   311042 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6785 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6783 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6799 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   596184 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)   188079 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/fmt-jpk-fd_spot3-0192.jpk-force
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/model_external_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93520 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/data/rate-export_1.7.8.h5
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_cli_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_cli_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_cli_rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_fit_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_fit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_fit_emodulus_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_fit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_indent2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_hertz_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_hertz_parabol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_hertz_pyramid_three.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_sneddon_spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_sneddon_spherical_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_sneddon_spherical_invert_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_model_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_open_jpk_variation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_qmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_rate_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_rate_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_rate_training_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-27 13:05:01.000000 nanite-3.7.1/tests/test_smooth.py
```

### Comparing `nanite-3.7.0/.gitignore` & `nanite-3.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/CHANGELOG` & `nanite-3.7.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+3.7.1
+ - setup: wrong package setup
 3.7.0
  - feat: subtract linear slope from indentation curve (#22)
  - ref: return normalization reference type for details from POC and preproc
  - setup: bump scipy to 1.10.0 due to memory leak vulnerability
 3.6.0
  - tests: make tests less strict and some cleanup
  - setup: drop support for Python 3.8 and 3.9
```

### Comparing `nanite-3.7.0/LICENSE` & `nanite-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/PKG-INFO` & `nanite-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanite
-Version: 3.7.0
+Version: 3.7.1
 Summary: Loading, fitting, and rating AFM force-distance data
 Author: Paul Müller, Shada Abuhattum
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3
 Project-URL: source, https://github.com/AFM-Analysis/nanite
 Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
 Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
```

### Comparing `nanite-3.7.0/README.rst` & `nanite-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/conf.py` & `nanite-3.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/data/force-save-example.jpk-force` & `nanite-3.7.1/docs/data/force-save-example.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/extensions/fancy_include.py` & `nanite-3.7.1/docs/extensions/fancy_include.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/extensions/github_changelog.py` & `nanite-3.7.1/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/extensions/nanite_models.py` & `nanite-3.7.1/docs/extensions/nanite_models.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/extensions/nanite_preprocs.py` & `nanite-3.7.1/docs/extensions/nanite_preprocs.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/extensions/simple_argparse.py` & `nanite-3.7.1/docs/extensions/simple_argparse.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/fitting_geometry.png` & `nanite-3.7.1/docs/fitting_geometry.png`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/fitting_geometry.svg` & `nanite-3.7.1/docs/fitting_geometry.svg`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/img/nanite-fit-example.png` & `nanite-3.7.1/docs/img/nanite-fit-example.png`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/img/nanite-rate-example.png` & `nanite-3.7.1/docs/img/nanite-rate-example.png`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/index.rst` & `nanite-3.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/nanite.bib` & `nanite-3.7.1/docs/nanite.bib`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_cli.rst` & `nanite-3.7.1/docs/sec_cli.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_code_reference.rst` & `nanite-3.7.1/docs/sec_code_reference.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_develop.rst` & `nanite-3.7.1/docs/sec_develop.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_fitting_guide.rst` & `nanite-3.7.1/docs/sec_fitting_guide.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_getting_started.rst` & `nanite-3.7.1/docs/sec_getting_started.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/docs/sec_rating_workflow.rst` & `nanite-3.7.1/docs/sec_rating_workflow.rst`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/data/zebrafish-head-section-gray-matter.jpk-force` & `nanite-3.7.1/examples/data/zebrafish-head-section-gray-matter.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/fit_and_rate.png` & `nanite-3.7.1/examples/fit_and_rate.png`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/fit_and_rate.py` & `nanite-3.7.1/examples/fit_and_rate.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/generate_example_images.py` & `nanite-3.7.1/examples/generate_example_images.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/model_spherical_indenter.png` & `nanite-3.7.1/examples/model_spherical_indenter.png`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/examples/model_spherical_indenter.py` & `nanite-3.7.1/examples/model_spherical_indenter.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/cli/plotting.py` & `nanite-3.7.1/nanite/cli/plotting.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/cli/profile.py` & `nanite-3.7.1/nanite/cli/profile.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/cli/rating.py` & `nanite-3.7.1/nanite/cli/rating.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/fit.py` & `nanite-3.7.1/nanite/fit.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/group.py` & `nanite-3.7.1/nanite/group.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/indent.py` & `nanite-3.7.1/nanite/indent.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/__init__.py` & `nanite-3.7.1/nanite/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/core.py` & `nanite-3.7.1/nanite/model/core.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/logic.py` & `nanite-3.7.1/nanite/model/logic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/model_conical_indenter.py` & `nanite-3.7.1/nanite/model/model_conical_indenter.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/model_hertz_paraboloidal.py` & `nanite-3.7.1/nanite/model/model_hertz_paraboloidal.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/model_hertz_three_sided_pyramid.py` & `nanite-3.7.1/nanite/model/model_hertz_three_sided_pyramid.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/model_sneddon_spherical.pyx` & `nanite-3.7.1/nanite/model/model_sneddon_spherical.pyx`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/model_sneddon_spherical_approximation.py` & `nanite-3.7.1/nanite/model/model_sneddon_spherical_approximation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/model/residuals.py` & `nanite-3.7.1/nanite/model/residuals.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/poc.py` & `nanite-3.7.1/nanite/poc.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/preproc.py` & `nanite-3.7.1/nanite/preproc.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/qmap.py` & `nanite-3.7.1/nanite/qmap.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/features.py` & `nanite-3.7.1/nanite/rate/features.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/io.py` & `nanite-3.7.1/nanite/rate/io.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/rater.py` & `nanite-3.7.1/nanite/rate/rater.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/regressors.py` & `nanite-3.7.1/nanite/rate/regressors.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_flatness.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_size.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_size.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_apr_sum.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_bln_slope.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_bln_variation.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_cp_curvature.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_cp_magnitude.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_maxima_75perc.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_monotony.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_spike_area.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_sum.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_feat_con_idt_sum_75perc.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/rate/ts_zef18/train_response.txt` & `nanite-3.7.1/nanite/rate/ts_zef18/train_response.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/read.py` & `nanite-3.7.1/nanite/read.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite/smooth.py` & `nanite-3.7.1/nanite/smooth.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/nanite.egg-info/PKG-INFO` & `nanite-3.7.1/nanite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanite
-Version: 3.7.0
+Version: 3.7.1
 Summary: Loading, fitting, and rating AFM force-distance data
 Author: Paul Müller, Shada Abuhattum
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3
 Project-URL: source, https://github.com/AFM-Analysis/nanite
 Project-URL: tracker, https://github.com/AFM-Analysis/nanite/issues
 Project-URL: documentation, https://nanite.readthedocs.io/en/stable/
```

### Comparing `nanite-3.7.0/nanite.egg-info/SOURCES.txt` & `nanite-3.7.1/nanite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/pyproject.toml` & `nanite-3.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -55,13 +55,10 @@
 
 [project.urls]
 source = "https://github.com/AFM-Analysis/nanite"
 tracker = "https://github.com/AFM-Analysis/nanite/issues"
 documentation = "https://nanite.readthedocs.io/en/stable/"
 changelog = "https://nanite.readthedocs.io/en/stable/sec_changelog.html"
 
-[tool.setuptools.packages]
-find = {}
-
 [tool.setuptools_scm]
 write_to = "nanite/_version.py"
 version_scheme = "post-release"
```

### Comparing `nanite-3.7.0/tests/common.py` & `nanite-3.7.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/conftest.py` & `nanite-3.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv` & `nanite-3.7.1/tests/data/fmt-afm-workshop-fd_single_2021-10-22_14.16.csv`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-cl_calibration_force-save-2015-02-04.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_flipsign_2015.05.22-15.31.49.352.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map-data-reference-points.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map0d_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map1d_2016-11-07.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map2x2_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map_bad_2013-05-27_1.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map` & `nanite-3.7.1/tests/data/fmt-jpk-fd_map_bad_2013-05-27_2.jpk-force-map`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_1.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_2.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_3.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_4.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_2017-01-16_5.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_GWAT_2017-10-17.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead10_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead46_2017-04-20.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_bad_bead7_2017-04-27.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_tilted-baseline-drift-mitotic_2021-01-29.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_single_tilted-baseline-shift-adyp_2023-06-26.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/fmt-jpk-fd_spot3-0192.jpk-force` & `nanite-3.7.1/tests/data/fmt-jpk-fd_spot3-0192.jpk-force`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/model_external_basic.py` & `nanite-3.7.1/tests/data/model_external_basic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/data/rate-export_1.7.8.h5` & `nanite-3.7.1/tests/data/rate-export_1.7.8.h5`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_cli_plotting.py` & `nanite-3.7.1/tests/test_cli_plotting.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_cli_profile.py` & `nanite-3.7.1/tests/test_cli_profile.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_cli_rating.py` & `nanite-3.7.1/tests/test_cli_rating.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_fit_ancillary.py` & `nanite-3.7.1/tests/test_fit_ancillary.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_fit_base.py` & `nanite-3.7.1/tests/test_fit_base.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_fit_emodulus_search.py` & `nanite-3.7.1/tests/test_fit_emodulus_search.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_fit_hash.py` & `nanite-3.7.1/tests/test_fit_hash.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_fit_properties.py` & `nanite-3.7.1/tests/test_fit_properties.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_group.py` & `nanite-3.7.1/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_indent.py` & `nanite-3.7.1/tests/test_indent.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_indent2.py` & `nanite-3.7.1/tests/test_indent2.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model.py` & `nanite-3.7.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_core.py` & `nanite-3.7.1/tests/test_model_core.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_expr.py` & `nanite-3.7.1/tests/test_model_expr.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_hertz_cone.py` & `nanite-3.7.1/tests/test_model_hertz_cone.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_hertz_parabol.py` & `nanite-3.7.1/tests/test_model_hertz_parabol.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_hertz_pyramid_three.py` & `nanite-3.7.1/tests/test_model_hertz_pyramid_three.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_logic.py` & `nanite-3.7.1/tests/test_model_logic.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_sneddon_spherical.py` & `nanite-3.7.1/tests/test_model_sneddon_spherical.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_sneddon_spherical_approximation.py` & `nanite-3.7.1/tests/test_model_sneddon_spherical_approximation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_model_style.py` & `nanite-3.7.1/tests/test_model_style.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_open_jpk_variation.py` & `nanite-3.7.1/tests/test_open_jpk_variation.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_poc.py` & `nanite-3.7.1/tests/test_poc.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_preproc.py` & `nanite-3.7.1/tests/test_preproc.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_qmap.py` & `nanite-3.7.1/tests/test_qmap.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_rate_features.py` & `nanite-3.7.1/tests/test_rate_features.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_rate_io.py` & `nanite-3.7.1/tests/test_rate_io.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_rate_training_set.py` & `nanite-3.7.1/tests/test_rate_training_set.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_read.py` & `nanite-3.7.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `nanite-3.7.0/tests/test_smooth.py` & `nanite-3.7.1/tests/test_smooth.py`

 * *Files identical despite different names*

