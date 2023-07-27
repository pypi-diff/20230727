# Comparing `tmp/edation-0.0.4.tar.gz` & `tmp/edation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edation-0.0.4.tar", max compression
+gzip compressed data, was "edation-0.0.5.tar", max compression
```

## Comparing `edation-0.0.4.tar` & `edation-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.4/README.md
--rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.4/edation/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/__init__.py
--rw-r--r--   0        0        0     4929 2023-07-27 12:48:18.706113 edation-0.0.4/edation/adapter/identity.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-27 12:48:17.736113 edation-0.0.4/edation/adapter/repo/file_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_dataset.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_tests.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/stats/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/visual/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/__init__.py
--rw-r--r--   0        0        0     2004 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/identity.py
--rw-r--r--   0        0        0     2504 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/repo.py
--rw-r--r--   0        0        0     1707 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/stats.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/visual.py
--rw-r--r--   0        0        0     2897 2023-07-27 12:48:16.846113 edation-0.0.4/edation/application/ports/driver/base.py
--rw-r--r--   0        0        0     3572 2023-07-27 12:51:36.096113 edation-0.0.4/edation/application/ports/driver/data.py
--rw-r--r--   0        0        0     1835 2023-07-27 12:48:14.866114 edation-0.0.4/edation/application/visual/base.py
--rw-r--r--   0        0        0     3672 2023-07-27 12:51:36.096113 edation-0.0.4/edation/container.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/domain/__init__.py
--rw-r--r--   0        0        0     9426 2023-07-27 12:51:36.106114 edation-0.0.4/edation/domain/base.py
--rw-r--r--   0        0        0     4321 2023-07-27 12:50:52.326113 edation-0.0.4/edation/domain/data.py
--rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.4/edation/edation.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/service/__init__.py
--rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.4/edation/service/io.py
--rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.4/edation/setup.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/__init__.py
--rw-r--r--   0        0        0     9276 2023-07-27 17:05:13.106114 edation-0.0.4/edation/stats/base.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/centrality/__init__.py
--rw-r--r--   0        0        0     7237 2023-07-27 17:03:51.146113 edation-0.0.4/edation/stats/centrality/ttest.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/correlation/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-27 12:48:08.966113 edation-0.0.4/edation/stats/correlation/pearson.py
--rw-r--r--   0        0        0     5808 2023-07-27 12:48:07.986113 edation-0.0.4/edation/stats/correlation/spearman.py
--rw-r--r--   0        0        0     3657 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/descriptive.py
--rw-r--r--   0        0        0    29599 2023-07-27 12:48:11.946113 edation-0.0.4/edation/stats/distribution.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/goodness_of_fit/__init__.py
--rw-r--r--   0        0        0     6728 2023-07-27 12:48:07.056113 edation-0.0.4/edation/stats/goodness_of_fit/chisquare.py
--rw-r--r--   0        0        0     8435 2023-07-27 12:48:06.046113 edation-0.0.4/edation/stats/goodness_of_fit/ksone.py
--rw-r--r--   0        0        0     7403 2023-07-27 12:48:04.936113 edation-0.0.4/edation/stats/goodness_of_fit/kstwo.py
--rw-r--r--   0        0        0     5862 2023-07-27 12:48:03.846113 edation-0.0.4/edation/stats/goodness_of_fit/shapiro.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/independence/__init__.py
--rw-r--r--   0        0        0     9210 2023-07-27 12:48:02.586113 edation-0.0.4/edation/stats/independence/chisquare.py
--rw-r--r--   0        0        0     2212 2023-07-27 12:48:10.986113 edation-0.0.4/edation/stats/profile.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/__init__.py
--rw-r--r--   0        0        0     9944 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/association.py
--rw-r--r--   0        0        0     4881 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/base.py
--rw-r--r--   0        0        0    12712 2023-07-27 15:26:02.746113 edation-0.0.4/edation/visual/config.py
--rw-r--r--   0        0        0    12022 2023-07-27 14:26:55.666113 edation-0.0.4/edation/visual/distribution.py
--rw-r--r--   0        0        0     2281 2023-07-27 18:04:17.406113 edation-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3575 2023-07-27 18:04:44.268134 edation-0.0.4/setup.py
--rw-r--r--   0        0        0     3493 2023-07-27 18:04:44.268624 edation-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.5/README.md
+-rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.5/edation/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/__init__.py
+-rw-r--r--   0        0        0     4929 2023-07-27 12:48:18.706113 edation-0.0.5/edation/adapter/identity.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/__init__.py
+-rw-r--r--   0        0        0     2480 2023-07-27 12:48:17.736113 edation-0.0.5/edation/adapter/repo/file_visual.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_dataset.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_tests.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_visual.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/stats/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/visual/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/__init__.py
+-rw-r--r--   0        0        0     2004 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/identity.py
+-rw-r--r--   0        0        0     2504 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/repo.py
+-rw-r--r--   0        0        0     1707 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/stats.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/visual.py
+-rw-r--r--   0        0        0     2897 2023-07-27 12:48:16.846113 edation-0.0.5/edation/application/ports/driver/base.py
+-rw-r--r--   0        0        0     3572 2023-07-27 12:51:36.096113 edation-0.0.5/edation/application/ports/driver/data.py
+-rw-r--r--   0        0        0     1835 2023-07-27 12:48:14.866114 edation-0.0.5/edation/application/visual/base.py
+-rw-r--r--   0        0        0     3672 2023-07-27 12:51:36.096113 edation-0.0.5/edation/container.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/domain/__init__.py
+-rw-r--r--   0        0        0     9426 2023-07-27 12:51:36.106114 edation-0.0.5/edation/domain/base.py
+-rw-r--r--   0        0        0     4321 2023-07-27 12:50:52.326113 edation-0.0.5/edation/domain/data.py
+-rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.5/edation/edation.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/service/__init__.py
+-rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.5/edation/service/io.py
+-rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.5/edation/setup.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/__init__.py
+-rw-r--r--   0        0        0     9276 2023-07-27 17:05:13.106114 edation-0.0.5/edation/stats/base.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/centrality/__init__.py
+-rw-r--r--   0        0        0     7237 2023-07-27 17:03:51.146113 edation-0.0.5/edation/stats/centrality/ttest.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/correlation/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-27 12:48:08.966113 edation-0.0.5/edation/stats/correlation/pearson.py
+-rw-r--r--   0        0        0     5808 2023-07-27 12:48:07.986113 edation-0.0.5/edation/stats/correlation/spearman.py
+-rw-r--r--   0        0        0     3657 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/descriptive.py
+-rw-r--r--   0        0        0    29599 2023-07-27 12:48:11.946113 edation-0.0.5/edation/stats/distribution.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/goodness_of_fit/__init__.py
+-rw-r--r--   0        0        0     6728 2023-07-27 12:48:07.056113 edation-0.0.5/edation/stats/goodness_of_fit/chisquare.py
+-rw-r--r--   0        0        0     8435 2023-07-27 12:48:06.046113 edation-0.0.5/edation/stats/goodness_of_fit/ksone.py
+-rw-r--r--   0        0        0     7403 2023-07-27 12:48:04.936113 edation-0.0.5/edation/stats/goodness_of_fit/kstwo.py
+-rw-r--r--   0        0        0     5862 2023-07-27 12:48:03.846113 edation-0.0.5/edation/stats/goodness_of_fit/shapiro.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/independence/__init__.py
+-rw-r--r--   0        0        0     9210 2023-07-27 12:48:02.586113 edation-0.0.5/edation/stats/independence/chisquare.py
+-rw-r--r--   0        0        0     2212 2023-07-27 12:48:10.986113 edation-0.0.5/edation/stats/profile.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/visual/__init__.py
+-rw-r--r--   0        0        0     9944 2023-07-27 12:50:52.326113 edation-0.0.5/edation/visual/association.py
+-rw-r--r--   0        0        0     4883 2023-07-27 18:21:38.446113 edation-0.0.5/edation/visual/base.py
+-rw-r--r--   0        0        0    12712 2023-07-27 15:26:02.746113 edation-0.0.5/edation/visual/config.py
+-rw-r--r--   0        0        0    12022 2023-07-27 14:26:55.666113 edation-0.0.5/edation/visual/distribution.py
+-rw-r--r--   0        0        0     2281 2023-07-27 18:22:07.636114 edation-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3575 2023-07-27 18:22:46.615177 edation-0.0.5/setup.py
+-rw-r--r--   0        0        0     3493 2023-07-27 18:22:46.615676 edation-0.0.5/PKG-INFO
```

### Comparing `edation-0.0.4/README.md` & `edation-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/__init__.py` & `edation-0.0.5/edation/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/__init__.py` & `edation-0.0.5/edation/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/identity.py` & `edation-0.0.5/edation/adapter/identity.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/repo/__init__.py` & `edation-0.0.5/edation/adapter/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/repo/file_visual.py` & `edation-0.0.5/edation/adapter/repo/file_visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/repo/odb_dataset.py` & `edation-0.0.5/edation/adapter/repo/odb_dataset.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/repo/odb_tests.py` & `edation-0.0.5/edation/adapter/repo/odb_tests.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/repo/odb_visual.py` & `edation-0.0.5/edation/adapter/repo/odb_visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/stats/__init__.py` & `edation-0.0.5/edation/adapter/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/adapter/visual/__init__.py` & `edation-0.0.5/edation/adapter/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/__init__.py` & `edation-0.0.5/edation/application/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driven/identity.py` & `edation-0.0.5/edation/application/ports/driven/identity.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driven/repo.py` & `edation-0.0.5/edation/application/ports/driven/repo.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driven/stats.py` & `edation-0.0.5/edation/application/ports/driven/stats.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driven/visual.py` & `edation-0.0.5/edation/application/ports/driven/visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driver/base.py` & `edation-0.0.5/edation/application/ports/driver/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/ports/driver/data.py` & `edation-0.0.5/edation/application/ports/driver/data.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/application/visual/base.py` & `edation-0.0.5/edation/application/visual/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/container.py` & `edation-0.0.5/edation/container.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/domain/__init__.py` & `edation-0.0.5/edation/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/domain/base.py` & `edation-0.0.5/edation/domain/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/domain/data.py` & `edation-0.0.5/edation/domain/data.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/edation.py` & `edation-0.0.5/edation/edation.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/service/__init__.py` & `edation-0.0.5/edation/service/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/service/io.py` & `edation-0.0.5/edation/service/io.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/setup.py` & `edation-0.0.5/edation/setup.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/__init__.py` & `edation-0.0.5/edation/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/base.py` & `edation-0.0.5/edation/stats/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/centrality/__init__.py` & `edation-0.0.5/edation/stats/centrality/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/centrality/ttest.py` & `edation-0.0.5/edation/stats/centrality/ttest.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/correlation/__init__.py` & `edation-0.0.5/edation/stats/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/correlation/pearson.py` & `edation-0.0.5/edation/stats/correlation/pearson.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/correlation/spearman.py` & `edation-0.0.5/edation/stats/correlation/spearman.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/descriptive.py` & `edation-0.0.5/edation/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/distribution.py` & `edation-0.0.5/edation/stats/distribution.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/goodness_of_fit/__init__.py` & `edation-0.0.5/edation/stats/goodness_of_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/goodness_of_fit/chisquare.py` & `edation-0.0.5/edation/stats/goodness_of_fit/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/goodness_of_fit/ksone.py` & `edation-0.0.5/edation/stats/goodness_of_fit/ksone.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/goodness_of_fit/kstwo.py` & `edation-0.0.5/edation/stats/goodness_of_fit/kstwo.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/goodness_of_fit/shapiro.py` & `edation-0.0.5/edation/stats/goodness_of_fit/shapiro.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/independence/__init__.py` & `edation-0.0.5/edation/stats/independence/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/independence/chisquare.py` & `edation-0.0.5/edation/stats/independence/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/stats/profile.py` & `edation-0.0.5/edation/stats/profile.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/visual/__init__.py` & `edation-0.0.5/edation/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/visual/association.py` & `edation-0.0.5/edation/visual/association.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/visual/base.py` & `edation-0.0.5/edation/visual/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Filename   : /edation/visual/base.py                                                             #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Sunday May 28th 2023 06:23:03 pm                                                    #
-# Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
+# Modified   : Thursday July 27th 2023 02:21:38 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import List
@@ -30,15 +30,15 @@
 # ------------------------------------------------------------------------------------------------ #
 class Visual(ABC):
     """Abstract base class for plot classes."""
 
     __default_palette = "blues_r"
 
     def __init__(self) -> None:
-        self.get_set_styling()
+        # self.get_set_styling()
         self._logger = logging.getLogger(f"{self.__class__.__name__}")
 
     @abstractmethod
     def __call__(self, *args, **kwargs) -> plt.Axes:
         """Presents the visualization."""
 
     def _wrap_ticklabels(
```

### Comparing `edation-0.0.4/edation/visual/config.py` & `edation-0.0.5/edation/visual/config.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/edation/visual/distribution.py` & `edation-0.0.5/edation/visual/distribution.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.4/pyproject.toml` & `edation-0.0.5/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edation"
-version = "0.0.4"
+version = "0.0.5"
 description = "Exploratory Data Analysis Framework"
 authors = [
     "John James <john.james.ai.studio@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `edation-0.0.4/setup.py` & `edation-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'edation.visual']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'edation',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Exploratory Data Analysis Framework',
     'long_description': "# EDAtion - An Exploratory Data Analysis Framework\n\n[![PyPI](https://img.shields.io/pypi/v/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - License](https://img.shields.io/pypi/l/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n\n---\n\n**Documentation**: [https://john-james-ai.github.io/edation](https://john-james-ai.github.io/edation)\n\n**Source Code**: [https://github.com/john-james-ai/edation](https://github.com/john-james-ai/edation)\n\n**PyPI**: [https://pypi.org/project/edation/](https://pypi.org/project/edation/)\n\n---\n\nExploratory Data Analysis Framework\n\n## Installation\n\n```sh\npip install edation\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/john-james-ai/edation/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/john-james-ai/edation/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/john-james-ai/edation/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n",
     'author': 'John James',
     'author_email': 'john.james.ai.studio@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://john-james-ai.github.io/edation',
```

### Comparing `edation-0.0.4/PKG-INFO` & `edation-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edation
-Version: 0.0.4
+Version: 0.0.5
 Summary: Exploratory Data Analysis Framework
 Home-page: https://john-james-ai.github.io/edation
 License: MIT
 Author: John James
 Author-email: john.james.ai.studio@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

