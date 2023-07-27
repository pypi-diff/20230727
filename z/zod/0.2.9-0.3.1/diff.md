# Comparing `tmp/zod-0.2.9.tar.gz` & `tmp/zod-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.9.tar", max compression
+gzip compressed data, was "zod-0.3.1.tar", max compression
```

## Comparing `zod-0.2.9.tar` & `zod-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0     1073 2023-06-21 12:50:03.778136 zod-0.2.9/LICENSE
--rw-r--r--   0        0        0     4809 2023-06-21 12:50:03.778136 zod-0.2.9/README.md
--rw-r--r--   0        0        0     1783 2023-06-21 12:50:03.778136 zod-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      982 2023-06-21 12:50:03.778136 zod-0.2.9/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-21 12:50:03.778136 zod-0.2.9/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/lane.py
--rw-r--r--   0        0        0     4931 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    15086 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6032 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/utils.py
--rw-r--r--   0        0        0     4658 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-06-21 12:50:03.778136 zod-0.2.9/zod/constants.py
--rw-r--r--   0        0        0      184 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12046 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0      437 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      355 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8399 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_drives.py
--rw-r--r--   0        0        0     1147 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-27 14:08:21.135618 zod-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4809 2023-07-27 14:08:21.135618 zod-0.3.1/README.md
+-rw-r--r--   0        0        0     1783 2023-07-27 14:08:21.139618 zod-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-07-27 14:08:21.139618 zod-0.3.1/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-07-27 14:08:21.139618 zod-0.3.1/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/lane.py
+-rw-r--r--   0        0        0     4931 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-07-27 14:08:21.139618 zod-0.3.1/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    16544 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/download.py
+-rw-r--r--   0        0        0     7431 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6032 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1351 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/main.py
+-rw-r--r--   0        0        0      645 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/utils.py
+-rw-r--r--   0        0        0     4362 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/verify.py
+-rw-r--r--   0        0        0     4658 2023-07-27 14:08:21.139618 zod-0.3.1/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-07-27 14:08:21.139618 zod-0.3.1/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-07-27 14:08:21.139618 zod-0.3.1/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12046 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0      437 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      355 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8399 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-07-27 14:08:21.139618 zod-0.3.1/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-07-27 14:08:21.143618 zod-0.3.1/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-07-27 14:08:21.143618 zod-0.3.1/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-07-27 14:08:21.143618 zod-0.3.1/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-07-27 14:08:21.143618 zod-0.3.1/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-07-27 14:08:21.143618 zod-0.3.1/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-07-27 14:08:21.143618 zod-0.3.1/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-07-27 14:08:21.143618 zod-0.3.1/zod/zod_drives.py
+-rw-r--r--   0        0        0     1147 2023-07-27 14:08:21.143618 zod-0.3.1/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-07-27 14:08:21.143618 zod-0.3.1/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.3.1/PKG-INFO
```

### Comparing `zod-0.2.9/LICENSE` & `zod-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/README.md` & `zod-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/pyproject.toml` & `zod-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.9"
+version = "0.3.1"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.9/zod/__init__.py` & `zod-0.3.1/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/_zod_dataset.py` & `zod-0.3.1/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/anno/lane.py` & `zod-0.3.1/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/anno/object.py` & `zod-0.3.1/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/anno/parser.py` & `zod-0.3.1/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/anno/tsr/class_map.py` & `zod-0.3.1/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/anno/tsr/traffic_sign.py` & `zod-0.3.1/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/cli/download_zod.py` & `zod-0.3.1/zod/cli/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 import os.path as osp
 import subprocess
 import tarfile
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from enum import Enum
 
+import requests
 from tqdm import tqdm
 
-from zod.cli.utils import SubDataset
+from zod.cli.utils import SubDataset, Version
 
 try:
     import click.exceptions
     import dropbox
     import dropbox.exceptions
     import dropbox.files
     import dropbox.sharing
@@ -23,36 +23,32 @@
 except ImportError:
     print('zod is installed without the CLI dependencies: pip install "zod[cli]"')
     exit(1)
 
 
 APP_KEY = "kcvokw7c7votepo"
 REFRESH_TOKEN = "z2h_5rjphJEAAAAAAAAAAUWtQlltCYlMbZ2WqMgtymELhiSuKIksxAYeArubKnZV"
-CHUNK_SIZE = 1024 * 1024  # 1 MB
-TIMEOUT = 60 * 60  # 1 hour
+CHUNK_SIZE = 8 * 1024 * 1024  # 8 MB
+TIMEOUT = 8 * 60 * 60  # 8 hours
 
 app = typer.Typer(help="Zenseact Open Dataset Downloader", no_args_is_help=True)
 
 
-class Version(str, Enum):
-    FULL = "full"
-    MINI = "mini"
-
-
 @dataclass
 class DownloadExtractInfo:
     """Information about a file to extract."""
 
     url: str
     file_path: str
     extract_dir: str
     dl_dir: str
     rm: bool
     dry_run: bool
     size: int
+    content_hash: str
     extract: bool
     extract_already_downloaded: bool
 
 
 @dataclass
 class FilterSettings:
     """Filter settings."""
@@ -80,14 +76,15 @@
     url: str
     output_dir: str
     rm: bool
     dry_run: bool
     extract: bool
     extract_already_downloaded: bool
     parallel: bool
+    max_workers: int = 8
 
     def __str__(self):
         return "\n".join([f"    {key}: {value}" for key, value in self.__dict__.items()])
 
 
 class ResumableDropbox(dropbox.Dropbox):
     """A patched dropbox client that allows to resume downloads."""
@@ -108,27 +105,24 @@
             del self._headers["Range"]
         return res
 
 
 def _print_final_msg(pbar: tqdm, basename: str):
     """Print a final message for each downloaded file, with stats and nice padding."""
     msg = "Downloaded " + basename + " " * (45 - len(basename))
-
-    # Print various download stats
     total_time = pbar.format_dict["elapsed"]
     size_in_mb = pbar.n / 1024 / 1024
-    speed = size_in_mb / total_time
+    speed_in_mb = size_in_mb / total_time
     for name, val, unit in [
         ("time", total_time, "s"),
         ("size", size_in_mb, "MB"),
-        ("speed", speed, "MB/s"),
+        ("speed", speed_in_mb, "MB/s"),
     ]:
         val = f"{val:.2f}{unit}"
         msg += f"{name}: {val}" + " " * (14 - len(val))
-
     tqdm.write(msg)
 
 
 def _download(download_path: str, dbx: ResumableDropbox, info: DownloadExtractInfo):
     current_size = 0
     if osp.exists(download_path):
         current_size = osp.getsize(download_path)
@@ -142,28 +136,31 @@
         initial=current_size,
     )
     if pbar.n > info.size:
         tqdm.write(
             f"Error! File {download_path} already exists and is larger than expected. "
             "Please delete and try again."
         )
+    if pbar.n > 0:
+        # this means we are retrying or resuming a previously interrupted download
+        tqdm.write(f"Resuming download of {download_path} from {current_size} bytes.")
     # Retry download if partial file exists (e.g. due to network error)
     while pbar.n < info.size:
-        if pbar.n > 0:
-            # this means we are retrying or resuming a previously interrupted download
-            tqdm.write(f"Resuming download of {download_path} from {current_size} bytes.")
-        _, response = dbx.sharing_get_shared_link_file(
-            url=info.url, path=info.file_path, start=pbar.n
-        )
-        with open(download_path, "ab") as f:
-            with contextlib.closing(response):
-                for chunk in response.iter_content(chunk_size=CHUNK_SIZE):
-                    if chunk:  # filter out keep-alive new chunks
-                        size = f.write(chunk)
-                        pbar.update(size)
+        try:
+            _, response = dbx.sharing_get_shared_link_file(
+                url=info.url, path=info.file_path, start=pbar.n
+            )
+            with open(download_path, "ab") as f:
+                with contextlib.closing(response):
+                    for chunk in response.iter_content(chunk_size=CHUNK_SIZE):
+                        if chunk:  # filter out keep-alive new chunks
+                            size = f.write(chunk)
+                            pbar.update(size)
+        except requests.exceptions.ChunkedEncodingError:
+            continue  # This can happen when dropbox unexpectly closes the connection
     # Final checks and printouts
     assert osp.getsize(download_path) == info.size
     _print_final_msg(pbar, basename)
 
 
 def _extract(tar_path: str, output_dir: str):
     """Extract a tar file to a directory."""
@@ -186,43 +183,63 @@
             # pbar.total = len(tar.getmembers())
             for member in tar.getmembers():
                 tar.extract(member=member, path=output_dir)
                 pbar.update(1)
     tqdm.write(f"Extracted {pbar.n} files from {osp.basename(tar_path)}.")
 
 
+def _already_downloaded(download_path: str, target_size: int):
+    """Check if the file is already downloaded."""
+    old_format_path = download_path.rsplit("_", 1)[0]  # /path/to/file_abc123 -> /path/to/file
+    if osp.exists(download_path) and osp.getsize(download_path) == target_size:
+        return True
+    elif osp.exists(old_format_path) and osp.getsize(old_format_path) == target_size:
+        return True
+    return False
+
+
 def _download_and_extract(dbx: ResumableDropbox, info: DownloadExtractInfo):
     """Download a file from a Dropbox share link to a local path."""
     should_extract = info.extract
-    download_path = osp.join(info.dl_dir, osp.basename(info.file_path))
-    if osp.exists(download_path) and osp.getsize(download_path) == info.size:
+    file_name = osp.basename(info.file_path)
+    data_name = file_name.split(".")[0]
+    download_path = osp.join(info.dl_dir, f"{file_name}_{info.content_hash[:8]}")
+    if _already_downloaded(download_path, info.size):
         if not info.extract_already_downloaded:
-            tqdm.write(f"File {download_path} already exists. Skipping download and extraction.")
+            tqdm.write(f"{data_name} already exists. Skipping download and extraction.")
             should_extract = False
         else:
-            tqdm.write(f"File {download_path} already exists. Skipping download.")
+            tqdm.write(f"File {data_name} already exists. Skipping download.")
     elif info.dry_run:
         typer.echo(f"Would download {info.file_path} to {download_path}")
     else:
-        _download(download_path, dbx, info)
+        try:
+            _download(download_path, dbx, info)
+        except Exception as e:
+            print(f"Error downloading {data_name}: {e}. Please retry")
+            return
 
     if should_extract:
         if info.dry_run:
-            typer.echo(f"Would extract {download_path} to {info.extract_dir}")
+            typer.echo(f"Would extract {data_name} to {info.extract_dir}")
             return
         else:
-            _extract(download_path, info.extract_dir)
+            try:
+                _extract(download_path, info.extract_dir)
+            except Exception as e:
+                print(f"Error extracting {data_name}: {e}. Please retry")
+                return
 
     if info.rm and not info.dry_run:
         os.remove(download_path)
 
 
 def _filter_entry(entry: dropbox.files.Metadata, settings: FilterSettings) -> bool:
     """Filter the entry based on the flags."""
-    if settings.version == "mini":
+    if settings.version == Version.MINI:
         return "mini" in entry.name
     elif "mini" in entry.name:
         return False
 
     if not settings.annotations and "annotations" in entry.name:
         return False
     if "images" in entry.name:
@@ -248,23 +265,30 @@
             if tgt != -1 and distance > tgt:
                 return False
     return True
 
 
 def _download_dataset(dl_settings: DownloadSettings, filter_settings: FilterSettings, dirname: str):
     dbx = ResumableDropbox(app_key=APP_KEY, oauth2_refresh_token=REFRESH_TOKEN, timeout=TIMEOUT)
-    url, entries = _list_folder(dl_settings.url, dbx, dirname)
+    entries = _list_folder(dl_settings.url, dbx, dirname)
+    if not entries:
+        typer.echo(
+            "Warning! No files found. Check the url, but this could be a known dropbox error.\n"
+            "We are working on a fix, so please try again layer. Sorry for the inconvenience."
+        )
+        return
     dl_dir = osp.join(dl_settings.output_dir, "downloads", dirname)
     files_to_download = [
         DownloadExtractInfo(
-            url=url,
+            url=dl_settings.url,
             file_path=f"/{dirname}/" + entry.name,
             dl_dir=dl_dir,
             extract_dir=dl_settings.output_dir,
             size=entry.size,
+            content_hash=entry.content_hash,
             rm=dl_settings.rm,
             dry_run=dl_settings.dry_run,
             extract=dl_settings.extract,
             extract_already_downloaded=dl_settings.extract_already_downloaded,
         )
         for entry in entries
         if _filter_entry(entry, filter_settings)
@@ -273,22 +297,22 @@
         typer.echo("No files to download. Perhaps you specified too many filters?")
         return
 
     if not dl_settings.dry_run:
         os.makedirs(dl_settings.output_dir, exist_ok=True)
         os.makedirs(dl_dir, exist_ok=True)
     if dl_settings.parallel:
-        with ThreadPoolExecutor() as pool:
+        with ThreadPoolExecutor(max_workers=dl_settings.max_workers) as pool:
             pool.map(lambda info: _download_and_extract(dbx, info), files_to_download)
     else:
         for info in files_to_download:
             _download_and_extract(dbx, info)
 
 
-def _list_folder(url, dbx, path):
+def _list_folder(url, dbx: ResumableDropbox, path: str):
     shared_link = dropbox.files.SharedLink(url=url)
     try:
         res = dbx.files_list_folder(path=f"/{path}", shared_link=shared_link)
     except dropbox.exceptions.ApiError as err:
         raise click.exceptions.ClickException(
             f"Dropbox raised the following error:\n\t{err}\nThis could be due to:"
             '\n\ta) bad url. Please try it in a browser and specify with quotes (--url="<url>").'
@@ -296,15 +320,15 @@
             "\n\tc) other error (bad internet connection, dropbox outage, etc.)."
         )
 
     entries = res.entries
     while res.has_more:
         res = dbx.files_list_folder_continue(res.cursor)
         entries.extend(res.entries)
-    return url, entries
+    return entries
 
 
 def _print_summary(download_settings, filter_settings, subset):
     print("\nDownload settings:")
     print(download_settings)
     print("\nFilter settings:")
     if filter_settings.version == Version.MINI:
@@ -363,14 +387,17 @@
     rm: bool = typer.Option(False, help="Remove the downloaded archives", rich_help_panel=GEN),
     dry_run: bool = typer.Option(False, help="Print what would be downloaded", rich_help_panel=GEN),
     extract: bool = typer.Option(True, help="Unpack the archives", rich_help_panel=GEN),
     extract_already_downloaded: bool = typer.Option(
         False, help="Extract already downloaded archives", rich_help_panel=GEN
     ),
     parallel: bool = typer.Option(True, help="Download files in parallel", rich_help_panel=GEN),
+    max_workers: int = typer.Option(
+        8, help="Max number of workers for parallel downloads", rich_help_panel=GEN
+    ),
     no_confirm: bool = typer.Option(
         False,
         "-y",
         "--no-confirm/--confirm",
         help="Don't ask for confirmation",
         is_flag=True,
         flag_value=False,
@@ -397,14 +424,15 @@
         url=url,
         output_dir=output_dir,
         rm=rm,
         dry_run=dry_run,
         extract=extract,
         extract_already_downloaded=extract_already_downloaded,
         parallel=parallel,
+        max_workers=max_workers,
     )
     filter_settings = FilterSettings(
         version=version,
         annotations=annotations,
         images=images,
         blur=blur,
         dnat=dnat,
```

### Comparing `zod-0.2.9/zod/cli/extract_tsr_patches.py` & `zod-0.3.1/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/cli/generate_coco_json.py` & `zod-0.3.1/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/cli/main.py` & `zod-0.3.1/zod/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from pathlib import Path
-from typing import Tuple
-
 try:
     import typer
 except ImportError:
     print('Warning! zod is installed without the CLI dependencies:\npip install "zod[cli]"')
     exit(1)
 
-from zod.cli.download_zod import app as download_app
+from zod.cli.download import app as download_app
 from zod.cli.extract_tsr_patches import cli_dummy as tsr_dummy
 from zod.cli.generate_coco_json import convert_to_coco
+from zod.cli.verify import app as verify_app
 from zod.cli.visualize_lidar import app as visualize_lidar_app
 
 visualize_app = typer.Typer(help="Visualize ZOD.", no_args_is_help=True)
 visualize_app.add_typer(visualize_lidar_app, name="lidar")
 
 convert_app = typer.Typer(help="Convert ZOD to a different format.", no_args_is_help=True)
 convert_app.command("coco", no_args_is_help=True)(convert_to_coco)
@@ -27,13 +25,14 @@
     else:
         parent.add_typer(child, name=name)
 
 
 app = typer.Typer(help="Zenseact Open Dataset CLI.", no_args_is_help=True)
 
 add_child(app, download_app, "download")
+add_child(app, verify_app, "verify")
 add_child(app, visualize_app, "visualize")
 add_child(app, convert_app, "generate")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `zod-0.2.9/zod/cli/visualize_lidar.py` & `zod-0.3.1/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/constants.py` & `zod-0.3.1/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/box.py` & `zod-0.3.1/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/calibration.py` & `zod-0.3.1/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/ego_motion.py` & `zod-0.3.1/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/frame.py` & `zod-0.3.1/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/geometry.py` & `zod-0.3.1/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/info.py` & `zod-0.3.1/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/metadata.py` & `zod-0.3.1/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/sensor.py` & `zod-0.3.1/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/sequence.py` & `zod-0.3.1/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/data_classes/vehicle_data.py` & `zod-0.3.1/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_experimental/eval.py` & `zod-0.3.1/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_experimental/matching.py` & `zod-0.3.1/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_experimental/utils.py` & `zod-0.3.1/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.3.1/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.3.1/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/utils/compensation.py` & `zod-0.3.1/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/utils/geometry.py` & `zod-0.3.1/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/utils/polygon_transformations.py` & `zod-0.3.1/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/utils/utils.py` & `zod-0.3.1/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/utils/visualization.py` & `zod-0.3.1/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/bev_utils.py` & `zod-0.3.1/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/colorlabeler.py` & `zod-0.3.1/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/lidar_3d.py` & `zod-0.3.1/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/lidar_bev.py` & `zod-0.3.1/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/lidar_on_image.py` & `zod-0.3.1/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/object_visualization.py` & `zod-0.3.1/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/oxts_on_image.py` & `zod-0.3.1/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/oxts_visualization.py` & `zod-0.3.1/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/visualization/polygon_utils.py` & `zod-0.3.1/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/zod_drives.py` & `zod-0.3.1/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/zod_frames.py` & `zod-0.3.1/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/zod/zod_sequences.py` & `zod-0.3.1/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.9/PKG-INFO` & `zod-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.9
+Version: 0.3.1
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

