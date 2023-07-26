# Comparing `tmp/nasa-scrub-2.6.5.tar.gz` & `tmp/nasa-scrub-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasa-scrub-2.6.5.tar", last modified: Mon May  8 23:50:48 2023, max compression
+gzip compressed data, was "nasa-scrub-2.7.tar", last modified: Wed Jul 26 22:06:46 2023, max compression
```

## Comparing `nasa-scrub-2.6.5.tar` & `nasa-scrub-2.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.459542 nasa-scrub-2.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/configuration-inputs.md
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/filtering.md
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/output.md
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/release-checklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/reviewing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.459542 nasa-scrub-2.6.5/nasa_scrub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/scrub_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/scrubme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/collaborator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/collaborator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/collaborator/do_collaborator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/scrub_gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/scrub_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/scrub_gui/do_scrub_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.467542 nasa-scrub-2.6.5/scrub/tools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/csv_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_codesonar_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_coverity_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_gbuild_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_gcc_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_javac_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_pylint_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_sonarqube_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21844 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/translate_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.467542 nasa-scrub-2.6.5/scrub/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/codeql.template
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/codesonar.template
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/coverity.template
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/gbuild.template
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/gcc.template
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/javac.template
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/pylint.template
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/sonarqube.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/scrub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/diff_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/do_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/scrub/utils/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/FilteringDefaults
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/create_file_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/do_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/filter_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/scrub_defaults.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/scrub_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.180109 nasa-scrub-2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-26 22:06:26.000000 nasa-scrub-2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 22:06:26.000000 nasa-scrub-2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 22:06:46.180109 nasa-scrub-2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-26 22:06:26.000000 nasa-scrub-2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.172109 nasa-scrub-2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/configuration-inputs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/filtering.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/release-checklist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/reviewing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-26 22:06:26.000000 nasa-scrub-2.7/docs/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/nasa_scrub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 22:06:46.000000 nasa-scrub-2.7/nasa_scrub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 22:06:26.000000 nasa-scrub-2.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/scrub_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/scrubme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/targets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/targets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/targets/collaborator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/targets/collaborator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/targets/collaborator/do_collaborator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/targets/scrub_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/targets/scrub_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/targets/scrub_gui/do_scrub_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.176109 nasa-scrub-2.7/scrub/tools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/csv_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_codesonar_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_coverity_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_gbuild_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_gcc_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_javac_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_pylint_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/get_sonarqube_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/parsers/translate_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.180109 nasa-scrub-2.7/scrub/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/codeql.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/codesonar.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/coverity.template
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/gbuild.template
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/gcc.template
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/javac.template
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/pylint.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/tools/templates/sonarqube.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.180109 nasa-scrub-2.7/scrub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/diff_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/do_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:46.180109 nasa-scrub-2.7/scrub/utils/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/filtering/FilteringDefaults
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/filtering/create_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/filtering/do_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/filtering/filter_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/scrub_defaults.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-26 22:06:26.000000 nasa-scrub-2.7/scrub/utils/scrub_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 22:06:46.180109 nasa-scrub-2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 22:06:26.000000 nasa-scrub-2.7/setup.py
```

### Comparing `nasa-scrub-2.6.5/LICENSE` & `nasa-scrub-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/PKG-INFO` & `nasa-scrub-2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-scrub
-Version: 2.6.5
+Version: 2.7
 Summary: SCRUB is an orchestration and aggregation tool for static code analysis tools.
 Home-page: https://github.com/nasa/scrub
 Author: Lyle Barner
 Author-email: lyle.barner@jpl.nasa.gov
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/nasa/scrub/issues
 Project-URL: Documentation, https://nasa.github.io/scrub
```

### Comparing `nasa-scrub-2.6.5/README.md` & `nasa-scrub-2.7/README.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/README.md` & `nasa-scrub-2.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/configuration-inputs.md` & `nasa-scrub-2.7/docs/configuration-inputs.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/configuration.md` & `nasa-scrub-2.7/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/contributing.md` & `nasa-scrub-2.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/faq.md` & `nasa-scrub-2.7/docs/faq.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/filtering.md` & `nasa-scrub-2.7/docs/filtering.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/installation.md` & `nasa-scrub-2.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/output.md` & `nasa-scrub-2.7/docs/output.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/release-checklist.md` & `nasa-scrub-2.7/docs/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/reviewing.md` & `nasa-scrub-2.7/docs/reviewing.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/troubleshooting.md` & `nasa-scrub-2.7/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/usage.md` & `nasa-scrub-2.7/docs/usage.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/docs/utilities.md` & `nasa-scrub-2.7/docs/utilities.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/nasa_scrub.egg-info/PKG-INFO` & `nasa-scrub-2.7/nasa_scrub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-scrub
-Version: 2.6.5
+Version: 2.7
 Summary: SCRUB is an orchestration and aggregation tool for static code analysis tools.
 Home-page: https://github.com/nasa/scrub
 Author: Lyle Barner
 Author-email: lyle.barner@jpl.nasa.gov
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/nasa/scrub/issues
 Project-URL: Documentation, https://nasa.github.io/scrub
```

### Comparing `nasa-scrub-2.6.5/nasa_scrub.egg-info/SOURCES.txt` & `nasa-scrub-2.7/nasa_scrub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/scrub_cli.py` & `nasa-scrub-2.7/scrub/scrub_cli.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/scrubme.py` & `nasa-scrub-2.7/scrub/scrubme.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,19 +80,25 @@
 
     # Make sure the working directory exists
     if not scrub_conf_data.get('scrub_working_dir').exists():
         print('ERROR: Working directory ' + str(scrub_conf_data.get('scrub_working_dir')) + ' does not exist.')
         sys.exit(10)
 
     # Make a copy of the scrub.cfg file and add it to the log
-    shutil.copyfile(conf_file, str(scrub_conf_data.get('scrub_analysis_dir').joinpath('scrub.cfg')))
+    try:
+        shutil.copyfile(conf_file, str(scrub_conf_data.get('scrub_analysis_dir').joinpath('scrub.cfg')))
+    except PermissionError:
+        print("WARNING: Could not create copy of configuration file {}".format(scrub_conf_data.get('scrub_analysis_dir').joinpath('scrub.cfg')))
 
     # Create a VERSION file
-    with open(str(scrub_conf_data.get('scrub_analysis_dir').joinpath('VERSION')), 'w') as output_fh:
-        output_fh.write(__version__)
+    try:
+        with open(str(scrub_conf_data.get('scrub_analysis_dir').joinpath('VERSION')), 'w') as output_fh:
+            output_fh.write(__version__)
+    except PermissionError:
+        logging.warning('Could not create VERSION file {}'.format(str(scrub_conf_data.get('scrub_analysis_dir').joinpath('VERSION'))))
 
     try:
         # Get the templates
         available_analysis_templates = list(scrub_path.glob('tools/templates/*template'))
 
         # Append the custom templates if provided
         if scrub_conf_data.get('custom_templates'):
@@ -137,23 +143,18 @@
                 analysis_script = analysis_scripts_dir.joinpath(tool_name + '.sh')
                 tool_analysis_dir = scrub_conf_data.get('scrub_working_dir').joinpath(tool_name + '_analysis')
 
                 # Add derived values to configuration values
                 scrub_conf_data.update({'tool_analysis_dir': tool_analysis_dir})
 
                 # Create the analysis scripts directory
-                if not analysis_scripts_dir.exists():
-                    analysis_scripts_dir.mkdir()
-                    analysis_scripts_dir.chmod(0o755)
+                scrub_utilities.create_dir(analysis_scripts_dir, True)
 
                 # Create the tool analysis directory
-                if tool_analysis_dir.exists():
-                    shutil.rmtree(tool_analysis_dir)
-                tool_analysis_dir.mkdir()
-                tool_analysis_dir.chmod(0o755)
+                scrub_utilities.create_dir(tool_analysis_dir, True, True)
 
                 # Create the log file
                 analysis_log_file = scrub_conf_data.get('scrub_log_dir').joinpath(tool_name + '.log')
                 scrub_utilities.create_logger(analysis_log_file, console_logging)
 
                 # Print a status message
                 logging.info('')
@@ -232,43 +233,48 @@
             execution_time = time.time() - start_time
 
             # Update the execution status
             execution_status.append(['filtering', filtering_status, execution_time])
 
     finally:
         # Move the results back with the source code if necessary
-        if scrub_conf_data.get('scrub_working_dir') != scrub_conf_data.get('scrub_analysis_dir'):
-            # Move every item in the directory
-            for item in scrub_conf_data.get('scrub_working_dir').iterdir():
-                # Remove the destination directory, if it exists
-                if scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem).exists():
-                    shutil.rmtree(scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem))
+        try:
+            if scrub_conf_data.get('scrub_working_dir') != scrub_conf_data.get('scrub_analysis_dir'):
+                # Move every item in the directory
+                for item in scrub_conf_data.get('scrub_working_dir').iterdir():
+                    # Remove the destination directory, if it exists
+                    if scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem).exists():
+                        shutil.rmtree(scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem))
+
+                    # Move the contents
+                    shutil.move(item, scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem))
+
+                # Remove the working directory
+                shutil.rmtree(scrub_conf_data.get('scrub_working_dir'))
+
+        except PermissionError:
+            print("\tWARNING: Could not move results from {} to {}".format(scrub_conf_data.get('scrub_working_dir'), scrub_conf_data.get('scrub_analysis_dir')))
+            print("\t\tResults will remain at {}".format(scrub_conf_data.get('scrub_working_dir')))
+
+        # Create a visible directory of results, if it doesn't already exist
+        viewable_results_dir = scrub_conf_data.get('source_dir').joinpath('scrub_results')
+        scrub_utilities.create_dir(viewable_results_dir, False)
 
-                # Move the contents
-                shutil.move(item, scrub_conf_data.get('scrub_analysis_dir').joinpath(item.stem))
+        # Create symbolic links for the output files
+        file_extensions = ['*.scrub', '*.sarif']
+        for extension in file_extensions:
+            for scrub_file in scrub_conf_data.get('scrub_analysis_dir').glob(extension):
+                symlink_path = viewable_results_dir.joinpath(scrub_file.name)
+                try:
+                    if not symlink_path.exists():
+                        os.symlink(os.path.relpath(str(scrub_file), str(viewable_results_dir)), symlink_path)
 
-            # Remove the working directory
-            shutil.rmtree(scrub_conf_data.get('scrub_working_dir'))
+                except PermissionError:
+                    logging.warning('Could not create symbolic link {}'.format(viewable_results_dir.joinpath(scrub_file.name)))
 
-        # Create a visible directory of results
-        viewable_results_dir = scrub_conf_data.get('source_dir').joinpath('scrub_results')
-        if viewable_results_dir.exists():
-            shutil.rmtree(viewable_results_dir)
-        viewable_results_dir.mkdir()
-        viewable_results_dir.chmod(0o755)
-
-        # Copy SCRUB format output files
-        for scrub_file in scrub_conf_data.get('scrub_analysis_dir').glob('*.scrub'):
-            os.symlink(os.path.relpath(str(scrub_file), str(viewable_results_dir)),
-                       viewable_results_dir.joinpath(scrub_file.name))
-
-        # Copy the SARIF format output files
-        for sarif_file in scrub_conf_data.get('sarif_results_dir').glob('*.sarif'):
-            os.symlink(os.path.relpath(str(sarif_file), str(viewable_results_dir)),
-                       viewable_results_dir.joinpath(sarif_file.name))
 
         # Print a status message
         tool_failure_count = 0
         total_execution_time = 0
         print('\nTool Execution Status:\n')
         for status in execution_status:
             # Track the execution time
```

### Comparing `nasa-scrub-2.6.5/scrub/targets/collaborator/do_collaborator.py` & `nasa-scrub-2.7/scrub/targets/collaborator/do_collaborator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import os
 import logging
 import pwd
 import traceback
 import shutil
 import subprocess
+import pathlib
 from scrub.utils import scrub_utilities
 from scrub.utils.filtering import create_file_list
 
 
 def login(bin_dir, login_flags):
     """This function logs in users to Collaborator.
 
@@ -112,15 +113,15 @@
                           "'": "&apos;",
                           "<": "&lt;",
                           ">": "&gt;",
                           "&": "&amp;"}
     defect_list = []
 
     # Import the defects from the file of interest
-    with open(scrub_file, 'r') as fh:
+    with open(scrub_file, 'r', encoding='UTF-8') as fh:
         results = fh.read()
 
     # Split the results into defects
     defects = results.split('\n\n')
 
     # Extract defect info
     for raw_defect in defects:
@@ -476,22 +477,18 @@
             if (collaborator_exit_code > 0) and (tool_conf_data.get('collaborator_review_id') > 0):
                 subcommand = ('admin review delete ' + str(tool_conf_data.get('collaborator_review_id')))
                 execute_ccollab(str(tool_conf_data.get('collaborator_ccollab_location')), subcommand)
 
             # Close the loggers
             logging.getLogger().handlers = []
 
-            # Update the permissions of the log file if it exists
-            if tool_conf_data.get('collaborator_log_file').exists():
-                tool_conf_data.get('collaborator_log_file').chmod(0o644)
-
-                # Move the log file to line up with the review id, if it exists
-                if tool_conf_data.get('collaborator_review_id') > 0:
-                    shutil.move(tool_conf_data.get('collaborator_log_file'),
-                                tool_conf_data.get('scrub_log_dir').joinpath('collaborator_' + str(tool_conf_data.get('collaborator_review_id')) + '.log'))
+            # Move the log file to line up with the review id, if it exists
+            if tool_conf_data.get('collaborator_log_file').exists() and tool_conf_data.get('collaborator_review_id') > 0:
+                shutil.move(tool_conf_data.get('collaborator_log_file'),
+                            tool_conf_data.get('scrub_log_dir').joinpath('collaborator_' + str(tool_conf_data.get('collaborator_review_id')) + '.log'))
 
     # Return the exit code
     return collaborator_exit_code
 
 
 def initialize_analysis(tool_conf_data):
     """The purpose of this function is to prepare the tool to perform analysis.
@@ -516,14 +513,17 @@
     if tool_conf_data.get('collaborator_username') == '':
         tool_conf_data.update({'collaborator_username': current_user})
 
     # Create the working directory if it doesn't already exist
     if not collaborator_upload_dir.exists():
         collaborator_upload_dir.mkdir()
 
+    # Resolve the COLLABORATOR_FILTERS variable
+    tool_conf_data.update({'collaborator_filters': pathlib.Path(tool_conf_data.get('collaborator_filters'))})
+
     # Determine if Collaborator can be run
     if not (tool_conf_data.get('collaborator_server')):
         # Update the analysis flag if necessary
         if tool_conf_data.get('collaborator_export'):
             tool_conf_data.update({'collaborator_export': False})
 
             # Print a status message
```

### Comparing `nasa-scrub-2.6.5/scrub/targets/scrub_gui/do_scrub_gui.py` & `nasa-scrub-2.7/scrub/targets/scrub_gui/do_scrub_gui.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/csv_parser.py` & `nasa-scrub-2.7/scrub/tools/parsers/csv_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     output_dir = input_dir.joinpath('csv_output')
     timestamp = datetime.datetime.utcnow()
 
     # Make the output directory if it doesn't already exist
     if output_dir.exists():
         shutil.rmtree(str(output_dir))
     output_dir.mkdir()
-    output_dir.chmod(0o755)
 
     # Get a list of all the scrub files in the directory
     input_files = input_dir.glob('*.scrub')
 
     # Create the output file path
     output_file = output_dir.joinpath(timestamp.strftime("%m-%d-%Y") + '.csv')
```

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_codesonar_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_codesonar_warnings.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,13 +119,10 @@
                 output_fh.write('%s%03d <%s> :%s:%d: %s\n\t%s\n\t%s\n\n' %
                                 (id_prefix, warning_count, warning_level, warning_file, warning_line,
                                  warning_class, warning_summary, warning_link))
 
                 # Increase the warning_count
                 warning_count = warning_count + 1
 
-    # Update the permissions of the output file
-    output_file.chmod(0o644)
-
 
 if __name__ == '__main__':
     parse_warnings(pathlib.Path(sys.argv[1]), pathlib.Path(sys.argv[2]), sys.argv[3])
```

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_coverity_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_coverity_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_gbuild_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_gbuild_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_gcc_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_gcc_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_javac_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_javac_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_pylint_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_pylint_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/get_sonarqube_warnings.py` & `nasa-scrub-2.7/scrub/tools/parsers/get_sonarqube_warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,19 @@
         # Read in the input data
         with open(raw_findings_file, 'r') as input_fh:
             input_data = json.loads(input_fh.read())
 
         # Iterate through every finding in the input file
         if 'issues' in input_data.keys():
             findings = input_data['issues']
-        else:
+        elif 'hotspots' in input_data.keys():
             findings = input_data['hotspots']
+        else:
+            break
+
         for finding in findings:
             # Check to see if the warning should be suppressed
             if 'resolution' in finding.keys():
                 suppression = True
             else:
                 suppression = False
```

### Comparing `nasa-scrub-2.6.5/scrub/tools/parsers/translate_results.py` & `nasa-scrub-2.7/scrub/tools/parsers/translate_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,14 @@
             if not warning['suppress']:
                 # Create the SCRUB formatted warning
                 scrub_warning = format_scrub_warning(warning)
 
                 # Write the warning to the output file
                 output_fh.write(scrub_warning)
 
-    # Change the permissions of the output file
-    output_file.chmod(0o644)
-
 
 def verify_sarif(sarif_data):
     """This function checks the SARIF data for known errors.
 
     Inputs:
         - sarif_data: A list of dictionaries containing analysis results [list of dict]
 
@@ -494,17 +491,14 @@
         result_item = {}
 
     # Create the output file
     with open(output_file, 'w') as output_fh:
         # output_fh.write('{}'.format(json.dumps(sarif_output, indent=4)))
         json.dump(sarif_output, output_fh, indent=4)
 
-    # Change the permissions of the output file
-    output_file.chmod(0o644)
-
 
 def perform_translation(input_file, output_file, source_root, output_format):
     """This function takes in an analysis results file in legacy format (.scrub), then parses and converts the contents
        of each analysis result into the SARIF format.
 
     Inputs:
         - scrub_filename: The name of the .sarif file to parse and convert. [string]
```

### Comparing `nasa-scrub-2.6.5/scrub/tools/templates/codeql.template` & `nasa-scrub-2.7/scrub/tools/templates/codeql.template`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/templates/codesonar.template` & `nasa-scrub-2.7/scrub/tools/templates/codesonar.template`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/templates/coverity.template` & `nasa-scrub-2.7/scrub/tools/templates/coverity.template`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/tools/templates/sonarqube.template` & `nasa-scrub-2.7/scrub/tools/templates/sonarqube.template`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,15 @@
     # Check to see if the file is empty
     if [ ! -s "$RESULTS_FILE" ]; then
         exit 1
     fi
     # Check the contents, verify file is not empty, and make sure the max page hasn't been reached
     if grep -q "Can return only the first 10000 results" $RESULTS_FILE; then
         echo "WARNING: Not all results have been retrieved."
+        rm -f $RESULTS_FILE
         MORE_RESULTS=false
     elif [ $PAGE -gt 20 ]; then
         MORE_RESULTS=false
     elif grep -q "\"hotspots\":\[\]" $RESULTS_FILE; then
        rm -f $RESULTS_FILE
        MORE_RESULTS=false
     else
```

### Comparing `nasa-scrub-2.6.5/scrub/utils/diff_results.py` & `nasa-scrub-2.7/scrub/utils/diff_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
 import sys
-import glob
 import argparse
+import pathlib
 from scrub.tools.parsers import translate_results
 
 
 def parse_arguments():
     """This function handles argument parsing in preparation for diff utility."""
 
     # Create the parser
@@ -16,15 +17,16 @@
     parser.add_argument('--comparison-source', required=True)
     parser.add_argument('--comparison-scrub', required=True)
 
     # Parse the arguments
     args = vars(parser.parse_args(sys.argv[2:]))
 
     # Run analysis
-    diff(args['baseline_source'], args['baseline_scrub'], args['comparison_source'], args['comparison_scrub'])
+    diff(pathlib.Path(args['baseline_source']).resolve(), pathlib.Path(args['baseline_scrub']).resolve(),
+         pathlib.Path(args['comparison_source']).resolve(), pathlib.Path(args['comparison_scrub']).resolve())
 
 
 def get_lines(source_file, line):
     """This function gets the line number from the source code file of interest
 
     Inputs:
         - file: Absolute path to the source code file of interest [string]
@@ -77,16 +79,16 @@
     relative_warning = warning.copy()
 
     # Update the file path
     relative_warning['file'] = relative_warning['file'].relative_to(source_root)
 
     # Update the description
     for line in relative_warning['description']:
-        relative_warning['description'][relative_warning['description'].index(line)] = line.replace(source_root + '/',
-                                                                                                    '')
+        relative_warning['description'][relative_warning['description'].index(line)] = line.replace(str(source_root) +
+                                                                                                    '/', '')
 
     return relative_warning
 
 
 def find_exact_match(comparison_warning, baseline_warnings):
     """This functions checks to see if an exact match exists.
 
@@ -127,24 +129,24 @@
     Outputs:
         - probable_match: Is this a probable match with a baseline warning? [bool]
     """
 
     # Initialize variables
     probable_match = False
 
-    comparison_source_lines = get_lines(comparison_source_root + '/' + comparison_warning['file'],
+    comparison_source_lines = get_lines(comparison_source_root.joinpath(comparison_warning['file']),
                                         comparison_warning['line'])
 
     # Search through all of the baseline warnings and get the corresponding data
     for baseline_warning in baseline_warnings:
         # Check to see if the warning query and warning file match
         if ((baseline_warning['file'] == comparison_warning['file']) and
                 (baseline_warning['query'] == comparison_warning['query'])):
             # Get the baseline source file line
-            baseline_source_lines = get_lines(baseline_source_root + '/' + baseline_warning['file'],
+            baseline_source_lines = get_lines(baseline_source_root.joinpath(baseline_warning['file']),
                                               baseline_warning['line'])
 
             # Check to see if the source file lines match
             if baseline_source_lines == comparison_source_lines:
                 # Update the flag
                 probable_match = True
 
@@ -162,15 +164,15 @@
         --baseline_source: Absolute path to baseline source root directory [string]
         --baseline_scrub: Absolute path to the baseline SCRUB working directory [string]
         --comparison_source: Absolute path to comparison source root directory [string]
         --comparison_scrub: Absolute path to the comparison SCRUB working directory [string]
     """
 
     # Find all of the SCRUB files in comparison results
-    comparison_scrub_files = glob.glob(comparison_scrub_root + '/*[!_diff].scrub')
+    comparison_scrub_files = list(comparison_scrub_root.glob('*[!_diff].scrub'))
 
     # Iterate through every SCRUB file and remove baseline results
     for comparison_scrub_file in comparison_scrub_files:
         # Print a status message
         print('Examining comparison results file: {}'.format(comparison_scrub_file))
 
         # Import the comparison SCRUB file data
@@ -223,11 +225,17 @@
 
         else:
             # Print a warning message
             print('    >> Baseline results file {} does not exist.'.format(baseline_scrub_file))
             print('    >> All results are new.')
 
         # Create the output file path
-        diff_output_file = comparison_scrub_root.joinpath(comparison_scrub_file.stem + '_diff.scrub')
+        diff_output_file = comparison_scrub_root.joinpath(comparison_scrub_file.stem + '.diff')
 
         # Write out the results
         translate_results.create_scrub_output_file(comparison_warnings_diff, diff_output_file)
+
+        # Create a symlink if possible
+        viewable_results_dir = comparison_source_root.joinpath('scrub_results')
+        if viewable_results_dir.exists():
+            os.symlink(os.path.relpath(str(diff_output_file), str(viewable_results_dir)),
+                       viewable_results_dir.joinpath(diff_output_file.name))
```

### Comparing `nasa-scrub-2.6.5/scrub/utils/do_clean.py` & `nasa-scrub-2.7/scrub/utils/do_clean.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/utils/filtering/create_file_list.py` & `nasa-scrub-2.7/scrub/utils/filtering/create_file_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
     # Initialize variables
     filtering_options = []
 
     # Read in the default filtering options
     with open(file_path, 'r') as input_fh:
         # Iterate through every line of the file
-        for line in input_fh.readlines():
-
+        for line in input_fh:
             # Check to make sure the line is formatted correctly
             if len(line.strip()) > 2 and line.startswith(('-', '+')):
                 # Append the filtering option
                 if line[1] == ' ':
                     filtering_options.append((line[0], line.strip()[2:]))
             elif not line.startswith('#'):
                 logging.warning('\tInvalid regex filtering line: {}'.format(line.strip()))
@@ -41,30 +40,42 @@
         - filtering_output_file: Absolute path to the output file containing a list of files to be included in analysis
                                  [string]
         - filtering_options_file: Absolute path to the filtering file to be used to create list of analysis files
                                   [string]
         - initial_filtering_list: Absolute path to the file containing an initial set of files [string]
     """
 
+    # Make sure the inputs are pathlib objects
+    source_root_dir = pathlib.Path(source_root_dir)
+    filtering_output_file = pathlib.Path(filtering_output_file)
+    filtering_options_file = pathlib.Path(filtering_options_file)
+    initial_filtering_list = pathlib.Path(initial_filtering_list)
+
     # Print a status message
     logging.info('')
     logging.info('\tCreating analysis filtering list...')
     logging.info('\t>> Executing command: create_file_list.create_file_list(%s, %s, %s, %s)', source_root_dir,
                  filtering_output_file, filtering_options_file, initial_filtering_list)
     logging.info('\t>> From directory: %s', pathlib.Path.cwd())
 
     # Initialize the variables
     raw_file_list = []
     default_filtering_options_file = pathlib.Path(__file__).parent.joinpath('FilteringDefaults').resolve()
 
     # Create the list of all available files, if necessary
-    if initial_filtering_list:
+    if initial_filtering_list.is_file():
         # Read in the list
         with open(initial_filtering_list, 'r') as input_fh:
-            raw_file_list = input_fh.readlines()
+            raw_input_data = input_fh.readlines()
+
+        # Strip whitespace from each element
+        raw_file_list = []
+        for index in range(len(raw_input_data)):
+            if raw_input_data[index] != '\n':
+                raw_file_list.append(raw_input_data[index].strip())
 
     else:
         for root, dir_names, file_names, in os.walk(source_root_dir, topdown=True):
             dir_names[:] = [d for d in dir_names if d not in ['.scrub', 'scrub_results']]
             for file_name in file_names:
                 raw_file_list.append(os.path.join(root, file_name))
 
@@ -85,22 +96,29 @@
 
         # Parse the filtering file
         filtering_options = parse_filtering_file(default_filtering_options_file)
 
     # Modify the list based on the include and exclude options
     filtered_file_list = raw_file_list.copy()
     for filtering_option in filtering_options:
-        for file_path in list(filter(re.compile(filtering_option[1]).search, raw_file_list)):
-            if filtering_option[0] == '-' and os.path.exists(file_path):
-                logging.debug('\tRemoving file from filtering list: %s', file_path)
-                filtered_file_list.remove(file_path)
-
-            elif filtering_option[0] == '+' and os.path.exists(file_path):
-                logging.debug('\tAdding file to filtering list: %s', file_path)
-                filtered_file_list.append(file_path)
+        try:
+            regex_option = re.compile(filtering_option[1]).search
+            for file_path in list(filter(regex_option, raw_file_list)):
+                # if filtering_option[0] == '-' and os.path.exists(file_path):
+                if filtering_option[0] == '-' and file_path in filtered_file_list:
+                    logging.debug('\tRemoving file from filtering list: %s', file_path)
+                    filtered_file_list.remove(file_path)
+
+                # elif filtering_option[0] == '+' and os.path.exists(file_path):
+                elif filtering_option[0] == '+':
+                    logging.debug('\tAdding file to filtering list: %s', file_path)
+                    filtered_file_list.append(file_path)
+        except:
+            logging.warning("\tUnable to process regex filter: {} {}".format(filtering_option[0], filtering_option[1]))
+            logging.warning("\t\tPlease ensure this is a valid regex format.")
 
     # Print the results to the output file
     filtered_file_list.sort()
     with open(filtering_output_file, 'w') as output_fh:
         for filtered_file in filtered_file_list:
             if pathlib.Path(filtered_file).anchor == '/':
                 relative_path = pathlib.Path(filtered_file).relative_to(source_root_dir)
```

### Comparing `nasa-scrub-2.6.5/scrub/utils/filtering/do_filtering.py` & `nasa-scrub-2.7/scrub/utils/filtering/do_filtering.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/utils/filtering/filter_results.py` & `nasa-scrub-2.7/scrub/utils/filtering/filter_results.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/utils/scrub_defaults.cfg` & `nasa-scrub-2.7/scrub/utils/scrub_defaults.cfg`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.5/scrub/utils/scrub_utilities.py` & `nasa-scrub-2.7/scrub/utils/scrub_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,45 @@
     def __exit__(self, exception, value, tb):
         self.busy = False
         time.sleep(self.delay)
         if exception is not None:
             return False
 
 
+def create_dir(directory, required, overwrite=False):
+    """This function handles creation of directories.
+
+    Inputs:
+        - directory: Absolute path to directory to be created [string]
+        - required: Is directory required for analysis? [bool]
+        - overwrite: Should existing directory be overwritten? [bool]
+
+    Outputs:
+        - None
+    """
+
+    try:
+        # Remove the directory if requested and it exists
+        if directory.exists():
+            if overwrite:
+                shutil.rmtree(directory)
+                directory.mkdir()
+
+        else:
+            # Create the directory and update permissions
+            directory.mkdir()
+
+    except PermissionError:
+        if required:
+            logging.error('Could not create directory {}. This directory is required for execution.'.format(directory))
+            raise
+        else:
+            logging.warning('Could not create directory {}'.format(directory))
+
+
 def get_pip_version():
     """This function gets the latest available version number from pip.
 
     Inputs:
         - None
 
     Outputs:
@@ -207,26 +238,46 @@
         - console_logging: Should debugging info be printed to the console?
             - Default value: logging.INFO
     """
 
     # Clear any existing loggers
     logging.getLogger().handlers = []
 
-    # Create the logger, if it doesn't already exist
-    logging.basicConfig(level=logging.DEBUG,
-                        format='%(asctime)s %(levelname)-8s %(message)s',
-                        filename=str(log_file),
-                        filemode='w')
-
-    # Start the console logger
-    console = logging.StreamHandler()
-    formatter = logging.Formatter('%(asctime)s %(levelname)-8s %(message)s')
-    console.setFormatter(formatter)
-    logging.getLogger('').addHandler(console)
-    console.setLevel(console_logging)
+    # Check permissions
+    try:
+        # Try to open the desired logging file to make sure permissions are correct
+        open(log_file, 'w').close()
+
+        # Create the logger, if it doesn't already exist
+        logging.basicConfig(level=logging.DEBUG,
+                            format='%(asctime)s %(levelname)-8s %(message)s',
+                            filename=str(log_file),
+                            filemode='w')
+
+        # Start the console logger
+        console = logging.StreamHandler()
+        formatter = logging.Formatter('%(asctime)s %(levelname)-8s %(message)s')
+        console.setFormatter(formatter)
+        logging.getLogger('').addHandler(console)
+        console.setLevel(console_logging)
+
+    except PermissionError:
+        print("\tWARNING: Could not create logging file {}".format(log_file))
+        print("\t\tLogging data will only print to console.")
+
+        # Create the console only logger
+        logging.basicConfig(level=logging.DEBUG,
+                            format='%(asctime)s %(levelname)-8s %(message)s')
+
+    # # Start the console logger
+    # console = logging.StreamHandler()
+    # formatter = logging.Formatter('%(asctime)s %(levelname)-8s %(message)s')
+    # console.setFormatter(formatter)
+    # logging.getLogger('').addHandler(console)
+    # console.setLevel(console_logging)
 
 
 def create_conf_file(output_path=None):
     """
     This function generates a blank configuration file at the desired output location.
 
     Inputs:
@@ -389,36 +440,27 @@
     """This function handles setting up the SCRUB analysis storage directory
 
     Inputs:
         - scrub_conf_data: Dictionary of values read from configuration file [dict]
     """
 
     # Create the .scrub analysis directory
-    if not scrub_conf_data.get('scrub_analysis_dir').exists():
-        scrub_conf_data.get('scrub_analysis_dir').mkdir()
-        scrub_conf_data.get('scrub_analysis_dir').chmod(0o755)
+    create_dir(scrub_conf_data.get('scrub_analysis_dir'), True)
 
     # Create the logging directory
-    if not scrub_conf_data.get('scrub_log_dir').exists():
-        scrub_conf_data.get('scrub_log_dir').mkdir()
-        scrub_conf_data.get('scrub_log_dir').chmod(0o755)
+    create_dir(scrub_conf_data.get('scrub_log_dir'), True)
 
     # Create the output directory
-    if not scrub_conf_data.get('raw_results_dir').exists():
-        scrub_conf_data.get('raw_results_dir').mkdir()
-        scrub_conf_data.get('raw_results_dir').chmod(0o755)
+    create_dir(scrub_conf_data.get('raw_results_dir'), True)
 
     # Create the SARIF results directory
-    if not scrub_conf_data.get('sarif_results_dir').exists():
-        scrub_conf_data.get('sarif_results_dir').mkdir()
-        scrub_conf_data.get('sarif_results_dir').chmod(0o755)
+    create_dir(scrub_conf_data.get('sarif_results_dir'), True)
 
     # Create the analysis directory if it doesn't exist
     if scrub_conf_data.get('scrub_working_dir') != scrub_conf_data.get('scrub_analysis_dir'):
         if scrub_conf_data.get('scrub_working_dir').exists():
             print('ERROR: SCRUB storage directory ' + str(scrub_conf_data.get('scrub_working_dir')) +
                   ' already exists. Aborting analysis.')
             sys.exit(10)
         else:
             # Create the scrub working dir
             scrub_conf_data.get('scrub_working_dir').mkdir()
-            scrub_conf_data.get('scrub_working_dir').chmod(0o755)
```

### Comparing `nasa-scrub-2.6.5/setup.cfg` & `nasa-scrub-2.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description_content_type = text/markdown
 name = nasa-scrub
 project_urls = 
 	Bug Tracker = https://github.com/nasa/scrub/issues
 	Documentation = https://nasa.github.io/scrub
 	Source = https://github.com/nasa/scrub
 url = https://github.com/nasa/scrub
-version = 2.6.5
+version = 2.7
 
 [options]
 include_package_data = True
 install_requires = 
 packages = find:
 setup_requires = 
 	setuptools
@@ -37,16 +37,16 @@
 	scrub = scrub.scrub_cli:main
 
 [options.packages.find]
 exclude = 
 	tests
 
 [bumpversion]
-new_version = 2.6.5
-current_version = 2.6.4
+new_version = 2.7
+current_version = 2.6.5
 commit = True
 tag = True
 
 [bumpversion:file:scrub/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

