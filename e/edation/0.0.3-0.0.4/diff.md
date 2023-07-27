# Comparing `tmp/edation-0.0.3.tar.gz` & `tmp/edation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edation-0.0.3.tar", max compression
+gzip compressed data, was "edation-0.0.4.tar", max compression
```

## Comparing `edation-0.0.3.tar` & `edation-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.3/README.md
--rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.3/edation/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/__init__.py
--rw-r--r--   0        0        0     4929 2023-07-27 12:48:18.706113 edation-0.0.3/edation/adapter/identity.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/repo/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-27 12:48:17.736113 edation-0.0.3/edation/adapter/repo/file_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/repo/odb_dataset.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/repo/odb_tests.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/repo/odb_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/stats/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/adapter/visual/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/application/__init__.py
--rw-r--r--   0        0        0     2004 2023-07-27 12:50:52.326113 edation-0.0.3/edation/application/ports/driven/identity.py
--rw-r--r--   0        0        0     2504 2023-07-27 12:50:52.326113 edation-0.0.3/edation/application/ports/driven/repo.py
--rw-r--r--   0        0        0     1707 2023-07-27 12:50:52.326113 edation-0.0.3/edation/application/ports/driven/stats.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/application/ports/driven/visual.py
--rw-r--r--   0        0        0     2897 2023-07-27 12:48:16.846113 edation-0.0.3/edation/application/ports/driver/base.py
--rw-r--r--   0        0        0     3572 2023-07-27 12:51:36.096113 edation-0.0.3/edation/application/ports/driver/data.py
--rw-r--r--   0        0        0     1835 2023-07-27 12:48:14.866114 edation-0.0.3/edation/application/visual/base.py
--rw-r--r--   0        0        0     3672 2023-07-27 12:51:36.096113 edation-0.0.3/edation/container.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/domain/__init__.py
--rw-r--r--   0        0        0     9426 2023-07-27 12:51:36.106114 edation-0.0.3/edation/domain/base.py
--rw-r--r--   0        0        0     4321 2023-07-27 12:50:52.326113 edation-0.0.3/edation/domain/data.py
--rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.3/edation/edation.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/service/__init__.py
--rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.3/edation/service/io.py
--rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.3/edation/setup.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/__init__.py
--rw-r--r--   0        0        0     9270 2023-07-27 12:48:12.896113 edation-0.0.3/edation/stats/base.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/centrality/__init__.py
--rw-r--r--   0        0        0     6903 2023-07-27 12:48:10.016113 edation-0.0.3/edation/stats/centrality/ttest.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/correlation/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-27 12:48:08.966113 edation-0.0.3/edation/stats/correlation/pearson.py
--rw-r--r--   0        0        0     5808 2023-07-27 12:48:07.986113 edation-0.0.3/edation/stats/correlation/spearman.py
--rw-r--r--   0        0        0     3657 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/descriptive.py
--rw-r--r--   0        0        0    29599 2023-07-27 12:48:11.946113 edation-0.0.3/edation/stats/distribution.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/goodness_of_fit/__init__.py
--rw-r--r--   0        0        0     6728 2023-07-27 12:48:07.056113 edation-0.0.3/edation/stats/goodness_of_fit/chisquare.py
--rw-r--r--   0        0        0     8435 2023-07-27 12:48:06.046113 edation-0.0.3/edation/stats/goodness_of_fit/ksone.py
--rw-r--r--   0        0        0     7403 2023-07-27 12:48:04.936113 edation-0.0.3/edation/stats/goodness_of_fit/kstwo.py
--rw-r--r--   0        0        0     5862 2023-07-27 12:48:03.846113 edation-0.0.3/edation/stats/goodness_of_fit/shapiro.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/stats/independence/__init__.py
--rw-r--r--   0        0        0     9210 2023-07-27 12:48:02.586113 edation-0.0.3/edation/stats/independence/chisquare.py
--rw-r--r--   0        0        0     2212 2023-07-27 12:48:10.986113 edation-0.0.3/edation/stats/profile.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.3/edation/visual/__init__.py
--rw-r--r--   0        0        0     9944 2023-07-27 12:50:52.326113 edation-0.0.3/edation/visual/association.py
--rw-r--r--   0        0        0     4881 2023-07-27 12:50:52.326113 edation-0.0.3/edation/visual/base.py
--rw-r--r--   0        0        0    12011 2023-07-27 12:48:00.436113 edation-0.0.3/edation/visual/config.py
--rw-r--r--   0        0        0    12053 2023-07-27 12:50:52.326113 edation-0.0.3/edation/visual/distribution.py
--rw-r--r--   0        0        0     2281 2023-07-27 12:50:51.866114 edation-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3575 2023-07-27 13:01:42.745266 edation-0.0.3/setup.py
--rw-r--r--   0        0        0     3493 2023-07-27 13:01:42.745742 edation-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.4/README.md
+-rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.4/edation/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/__init__.py
+-rw-r--r--   0        0        0     4929 2023-07-27 12:48:18.706113 edation-0.0.4/edation/adapter/identity.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/__init__.py
+-rw-r--r--   0        0        0     2480 2023-07-27 12:48:17.736113 edation-0.0.4/edation/adapter/repo/file_visual.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_dataset.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_tests.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/repo/odb_visual.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/stats/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/adapter/visual/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/__init__.py
+-rw-r--r--   0        0        0     2004 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/identity.py
+-rw-r--r--   0        0        0     2504 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/repo.py
+-rw-r--r--   0        0        0     1707 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/stats.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/application/ports/driven/visual.py
+-rw-r--r--   0        0        0     2897 2023-07-27 12:48:16.846113 edation-0.0.4/edation/application/ports/driver/base.py
+-rw-r--r--   0        0        0     3572 2023-07-27 12:51:36.096113 edation-0.0.4/edation/application/ports/driver/data.py
+-rw-r--r--   0        0        0     1835 2023-07-27 12:48:14.866114 edation-0.0.4/edation/application/visual/base.py
+-rw-r--r--   0        0        0     3672 2023-07-27 12:51:36.096113 edation-0.0.4/edation/container.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/domain/__init__.py
+-rw-r--r--   0        0        0     9426 2023-07-27 12:51:36.106114 edation-0.0.4/edation/domain/base.py
+-rw-r--r--   0        0        0     4321 2023-07-27 12:50:52.326113 edation-0.0.4/edation/domain/data.py
+-rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.4/edation/edation.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/service/__init__.py
+-rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.4/edation/service/io.py
+-rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.4/edation/setup.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/__init__.py
+-rw-r--r--   0        0        0     9276 2023-07-27 17:05:13.106114 edation-0.0.4/edation/stats/base.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/centrality/__init__.py
+-rw-r--r--   0        0        0     7237 2023-07-27 17:03:51.146113 edation-0.0.4/edation/stats/centrality/ttest.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/correlation/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-27 12:48:08.966113 edation-0.0.4/edation/stats/correlation/pearson.py
+-rw-r--r--   0        0        0     5808 2023-07-27 12:48:07.986113 edation-0.0.4/edation/stats/correlation/spearman.py
+-rw-r--r--   0        0        0     3657 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/descriptive.py
+-rw-r--r--   0        0        0    29599 2023-07-27 12:48:11.946113 edation-0.0.4/edation/stats/distribution.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/goodness_of_fit/__init__.py
+-rw-r--r--   0        0        0     6728 2023-07-27 12:48:07.056113 edation-0.0.4/edation/stats/goodness_of_fit/chisquare.py
+-rw-r--r--   0        0        0     8435 2023-07-27 12:48:06.046113 edation-0.0.4/edation/stats/goodness_of_fit/ksone.py
+-rw-r--r--   0        0        0     7403 2023-07-27 12:48:04.936113 edation-0.0.4/edation/stats/goodness_of_fit/kstwo.py
+-rw-r--r--   0        0        0     5862 2023-07-27 12:48:03.846113 edation-0.0.4/edation/stats/goodness_of_fit/shapiro.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/stats/independence/__init__.py
+-rw-r--r--   0        0        0     9210 2023-07-27 12:48:02.586113 edation-0.0.4/edation/stats/independence/chisquare.py
+-rw-r--r--   0        0        0     2212 2023-07-27 12:48:10.986113 edation-0.0.4/edation/stats/profile.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/__init__.py
+-rw-r--r--   0        0        0     9944 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/association.py
+-rw-r--r--   0        0        0     4881 2023-07-27 12:50:52.326113 edation-0.0.4/edation/visual/base.py
+-rw-r--r--   0        0        0    12712 2023-07-27 15:26:02.746113 edation-0.0.4/edation/visual/config.py
+-rw-r--r--   0        0        0    12022 2023-07-27 14:26:55.666113 edation-0.0.4/edation/visual/distribution.py
+-rw-r--r--   0        0        0     2281 2023-07-27 18:04:17.406113 edation-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3575 2023-07-27 18:04:44.268134 edation-0.0.4/setup.py
+-rw-r--r--   0        0        0     3493 2023-07-27 18:04:44.268624 edation-0.0.4/PKG-INFO
```

### Comparing `edation-0.0.3/README.md` & `edation-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/__init__.py` & `edation-0.0.4/edation/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/__init__.py` & `edation-0.0.4/edation/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/identity.py` & `edation-0.0.4/edation/adapter/identity.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/repo/__init__.py` & `edation-0.0.4/edation/adapter/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/repo/file_visual.py` & `edation-0.0.4/edation/adapter/repo/file_visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/repo/odb_dataset.py` & `edation-0.0.4/edation/adapter/repo/odb_dataset.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/repo/odb_tests.py` & `edation-0.0.4/edation/adapter/repo/odb_tests.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/repo/odb_visual.py` & `edation-0.0.4/edation/adapter/repo/odb_visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/stats/__init__.py` & `edation-0.0.4/edation/adapter/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/adapter/visual/__init__.py` & `edation-0.0.4/edation/adapter/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/__init__.py` & `edation-0.0.4/edation/application/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driven/identity.py` & `edation-0.0.4/edation/application/ports/driven/identity.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driven/repo.py` & `edation-0.0.4/edation/application/ports/driven/repo.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driven/stats.py` & `edation-0.0.4/edation/application/ports/driven/stats.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driven/visual.py` & `edation-0.0.4/edation/application/ports/driven/visual.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driver/base.py` & `edation-0.0.4/edation/application/ports/driver/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/ports/driver/data.py` & `edation-0.0.4/edation/application/ports/driver/data.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/application/visual/base.py` & `edation-0.0.4/edation/application/visual/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/container.py` & `edation-0.0.4/edation/container.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/domain/__init__.py` & `edation-0.0.4/edation/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/domain/base.py` & `edation-0.0.4/edation/domain/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/domain/data.py` & `edation-0.0.4/edation/domain/data.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/edation.py` & `edation-0.0.4/edation/edation.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/service/__init__.py` & `edation-0.0.4/edation/service/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/service/io.py` & `edation-0.0.4/edation/service/io.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/setup.py` & `edation-0.0.4/edation/setup.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/__init__.py` & `edation-0.0.4/edation/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/base.py` & `edation-0.0.4/edation/stats/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 # Filename   : /edation/stats/base.py                                                              #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Monday June 5th 2023 12:13:09 am                                                    #
-# Modified   : Thursday July 27th 2023 08:48:12 am                                                 #
+# Modified   : Thursday July 27th 2023 01:05:12 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from abc import ABC, abstractmethod
 import logging
 from dataclasses import dataclass, fields
 from typing import Union
 
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
+from scipy import stats
 
 from edation.service.io import IOService
 from edation import IMMUTABLE_TYPES, SEQUENCE_TYPES
 from edation.visual.config import Canvas
 
 # ------------------------------------------------------------------------------------------------ #
 sns.set_style(Canvas.style)
@@ -124,35 +125,37 @@
         s = ""
         width = 32
         for k, v in self.__dict__.items():
             if type(v) in IMMUTABLE_TYPES:
                 s += f"\t{k.rjust(width,' ')} | {v}\n"
         return s
 
-    def _fill_curve(self, ax: plt.Axes, upper: float, lower: float = None) -> plt.Axes:
+    def _fill_reject_region(
+        self,
+        ax: plt.Axes,
+        lower: float,
+        upper: float,
+        lower_critical: float,
+        upper_critical: float,
+        dof: int,
+    ) -> plt.Axes:
         """Fills the area under the curve at the value of the hypothesis test statistic."""
 
+        # Fill lower tail
+        xlower = np.arange(lower, lower_critical, 0.001)
+        ax.fill_between(x=xlower, y1=0, y2=stats.t.pdf(xlower, dof), color=Canvas.colors.orange)
+
+        # Fill Upper Tail
+        xupper = np.arange(upper_critical, upper, 0.001)
+        ax.fill_between(x=xupper, y1=0, y2=stats.t.pdf(xupper, dof), color=Canvas.colors.orange)
+
+        # Plot the statistic
         line = ax.lines[0]
         xdata = line.get_xydata()[:, 0]
         ydata = line.get_xydata()[:, 1]
-
-        # Fill lower tail
-        if lower is not None:
-            idx_lower = np.where(xdata > lower)[0][0]
-            fill_x = xdata[:idx_lower]
-            fill_y2 = ydata[:idx_lower]
-            ax.fill_between(x=fill_x, y1=0, y2=fill_y2, color=Canvas.colors.orange)
-
-        # Fill upper tail
-        idx_upper = np.where(xdata < upper)[0][-1]
-        fill_x = xdata[idx_upper:]
-        fill_y2 = ydata[idx_upper:]
-        ax.fill_between(x=fill_x, y1=0, y2=fill_y2, color=Canvas.colors.orange)
-
-        # Plot statistic
         try:
             idx = np.where(xdata > self.value)[0][0]
             x = xdata[idx]
             y = ydata[idx]
             ax = sns.regplot(
                 x=np.array([x]),
                 y=np.array([y]),
```

### Comparing `edation-0.0.3/edation/stats/centrality/__init__.py` & `edation-0.0.4/edation/stats/centrality/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/centrality/ttest.py` & `edation-0.0.4/edation/stats/centrality/ttest.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 # Filename   : /edation/stats/centrality/ttest.py                                                  #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday June 7th 2023 11:41:00 pm                                                 #
-# Modified   : Thursday July 27th 2023 08:48:09 am                                                 #
+# Modified   : Thursday July 27th 2023 01:03:50 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
+import logging
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from scipy import stats
 
 from edation.stats.profile import StatTestProfileTwo
@@ -47,29 +48,37 @@
     def plot(self, varname: str = None, ax: plt.Axes = None) -> plt.Axes:  # pragma: no cover
         canvas = Canvas()
         ax = ax or canvas.ax
         x = np.linspace(stats.t.ppf(0.001, self.dof), stats.t.ppf(0.999, self.dof), 500)
         y = stats.t.pdf(x, self.dof)
         ax = sns.lineplot(x=x, y=y, markers=False, dashes=False, sort=True, ax=ax)
 
+        self._logger = logging.getLogger(f"{self.__class__.__name__}")
+
         # Compute reject region
+        lower = x[0]
+        upper = x[-1]
         lower_alpha = self.alpha / 2
         upper_alpha = 1 - (self.alpha / 2)
-        lower = stats.t.ppf(lower_alpha, self.dof)
-        upper = stats.t.ppf(upper_alpha, self.dof)
+        lower_critical = stats.t.ppf(lower_alpha, self.dof)
+        upper_critical = stats.t.ppf(upper_alpha, self.dof)
+
+        self._logger.info(f"Lower={lower}")
+        self._logger.info(f"Upper={upper}")
 
         # Fill reject region at critical points
-        self._fill_curve(ax, lower, upper)
+        # self._fill_curve(ax, lower, upper)
+        self._fill_reject_region(ax, lower, upper, lower_critical, upper_critical, self.dof)
 
         ax.set_title(
             f"{self.result}",
             fontsize=canvas.fontsize_title,
         )
 
-        ax.set_xlabel(r"$X^2$")
+        # ax.set_xlabel(r"$X^2$")
         ax.set_ylabel("Probability Density")
         plt.tight_layout()
         return ax
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                          TEST                                                    #
```

### Comparing `edation-0.0.3/edation/stats/correlation/__init__.py` & `edation-0.0.4/edation/stats/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/correlation/pearson.py` & `edation-0.0.4/edation/stats/correlation/pearson.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/correlation/spearman.py` & `edation-0.0.4/edation/stats/correlation/spearman.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/descriptive.py` & `edation-0.0.4/edation/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/distribution.py` & `edation-0.0.4/edation/stats/distribution.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/goodness_of_fit/__init__.py` & `edation-0.0.4/edation/stats/goodness_of_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/goodness_of_fit/chisquare.py` & `edation-0.0.4/edation/stats/goodness_of_fit/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/goodness_of_fit/ksone.py` & `edation-0.0.4/edation/stats/goodness_of_fit/ksone.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/goodness_of_fit/kstwo.py` & `edation-0.0.4/edation/stats/goodness_of_fit/kstwo.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/goodness_of_fit/shapiro.py` & `edation-0.0.4/edation/stats/goodness_of_fit/shapiro.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/independence/__init__.py` & `edation-0.0.4/edation/stats/independence/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/independence/chisquare.py` & `edation-0.0.4/edation/stats/independence/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/stats/profile.py` & `edation-0.0.4/edation/stats/profile.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/visual/__init__.py` & `edation-0.0.4/edation/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/visual/association.py` & `edation-0.0.4/edation/visual/association.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/visual/base.py` & `edation-0.0.4/edation/visual/base.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.3/edation/visual/config.py` & `edation-0.0.4/edation/visual/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Filename   : /edation/visual/config.py                                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday May 24th 2023 04:11:27 pm                                                 #
-# Modified   : Thursday July 27th 2023 08:48:00 am                                                 #
+# Modified   : Thursday July 27th 2023 11:26:02 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass, field
@@ -70,14 +70,17 @@
     police_blue: str = "#2B4865"
     teal_blue: str = "#256D85"
     pale_robin_egg_blue: str = "#8FE3CF"
     russian_violet: str = "#231955"
     dark_cornflower_blue: str = "#1F4690"
     meat_brown: str = "#E8AA42"
     peach: str = "#FFE5B4"
+    dark_blue: str = "#002B5B"
+    blue: str = "#1F4690"
+    orange: str = "#E8AA42"
 
     def __post_init__(self) -> None:
         return
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                            Palettes                                              #
@@ -111,24 +114,40 @@
 class Canvas(PlotConfig):
     """Canvas class encapsulating the figure and axes objects."""
 
     style: str = "whitegrid"
     figsize: tuple = (12, 4)
     nrows: int = 1
     ncols: int = 1
+    saturation: float = 0.5
+    fontsize: int = 10
+    fontsize_title: int = 10
     fig: plt.figure = None
+    ax: plt.axes = None
     axs: List = field(default_factory=lambda: [plt.axes])
+    colors: Colors = Colors()
+
+    # def __post_init__(self) -> None:
+    #     width = int(self.figsize[0] / self.nrows)
+    #     height = int(self.figsize[1] / self.ncols)
+    #     figsize = []
+    #     figsize.append(width * self.ncols)
+    #     figsize.append(height * self.nrows)
+    #     self.fig, self.axs = plt.subplots(nrows=self.nrows, ncols=self.ncols, figsize=figsize)
 
     def __post_init__(self) -> None:
-        width = int(self.figsize[0] / self.nrows)
-        height = int(self.figsize[1] / self.ncols)
-        figsize = []
-        figsize.append(width * self.ncols)
-        figsize.append(height * self.nrows)
-        self.fig, self.axs = plt.subplots(nrows=self.nrows, ncols=self.ncols, figsize=figsize)
+        if self.nrows > 1 or self.ncols > 1:
+            figsize = []
+            figsize.append(self.figsize[0] * self.ncols)
+            figsize.append(self.figsize[1] * self.nrows)
+            self.fig, self.axs = plt.subplots(nrows=self.nrows, ncols=self.ncols, figsize=figsize)
+        else:
+            self.fig, self.ax = plt.subplots(
+                nrows=self.nrows, ncols=self.ncols, figsize=self.figsize
+            )
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                            STYLE                                                 #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class Styling(PlotConfig):
```

### Comparing `edation-0.0.3/edation/visual/distribution.py` & `edation-0.0.4/edation/visual/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Filename   : /edation/visual/distribution.py                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Sunday June 18th 2023 01:41:15 am                                                   #
-# Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
+# Modified   : Thursday July 27th 2023 10:26:55 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Visualizations Revealing the Distribution of Data"""
 import pandas as pd
 
@@ -37,14 +37,15 @@
 
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
+        kde: bool = True,
         ax: plt.Axes = None,
         title: str = None,
         style: str = "whitegrid",
         palette: str = "colorblind",
         *args,
         **kwargs,
     ) -> plt.Axes:
@@ -69,27 +70,24 @@
         style = self.get_set_styling(style=style, palette=palette)
 
         ax = sns.histplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
+            kde=kde,
             ax=ax,
             legend=True,
             pmax=style.saturation,
             *args,
             **kwargs,
         )
         if title:
             ax.set_title(title)
 
-        for container in ax.containers:
-            ax.bar_label(container)
-
-
 # ------------------------------------------------------------------------------------------------ #
 #                                       KDE PLOT                                                   #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class KDEPlot(Visual):  # pragma: no cover
     """Plot univariate or bivariate histograms to show distributions of datasets."""
```

### Comparing `edation-0.0.3/pyproject.toml` & `edation-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edation"
-version = "0.0.3"
+version = "0.0.4"
 description = "Exploratory Data Analysis Framework"
 authors = [
     "John James <john.james.ai.studio@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `edation-0.0.3/setup.py` & `edation-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'edation.visual']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'edation',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Exploratory Data Analysis Framework',
     'long_description': "# EDAtion - An Exploratory Data Analysis Framework\n\n[![PyPI](https://img.shields.io/pypi/v/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - License](https://img.shields.io/pypi/l/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n\n---\n\n**Documentation**: [https://john-james-ai.github.io/edation](https://john-james-ai.github.io/edation)\n\n**Source Code**: [https://github.com/john-james-ai/edation](https://github.com/john-james-ai/edation)\n\n**PyPI**: [https://pypi.org/project/edation/](https://pypi.org/project/edation/)\n\n---\n\nExploratory Data Analysis Framework\n\n## Installation\n\n```sh\npip install edation\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/john-james-ai/edation/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/john-james-ai/edation/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/john-james-ai/edation/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n",
     'author': 'John James',
     'author_email': 'john.james.ai.studio@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://john-james-ai.github.io/edation',
```

### Comparing `edation-0.0.3/PKG-INFO` & `edation-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edation
-Version: 0.0.3
+Version: 0.0.4
 Summary: Exploratory Data Analysis Framework
 Home-page: https://john-james-ai.github.io/edation
 License: MIT
 Author: John James
 Author-email: john.james.ai.studio@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

