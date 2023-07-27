# Comparing `tmp/zod-0.3.2.tar.gz` & `tmp/zod-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.3.2.tar", max compression
+gzip compressed data, was "zod-0.3.3.tar", max compression
```

## Comparing `zod-0.3.2.tar` & `zod-0.3.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1073 2023-07-27 14:12:14.254627 zod-0.3.2/LICENSE
--rw-r--r--   0        0        0     4809 2023-07-27 14:12:14.254627 zod-0.3.2/README.md
--rw-r--r--   0        0        0     1783 2023-07-27 14:12:14.254627 zod-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      982 2023-07-27 14:12:14.254627 zod-0.3.2/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-07-27 14:12:14.254627 zod-0.3.2/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/lane.py
--rw-r--r--   0        0        0     4931 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-07-27 14:12:14.254627 zod-0.3.2/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    16544 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/download.py
--rw-r--r--   0        0        0     7431 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6032 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1351 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/main.py
--rw-r--r--   0        0        0      645 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/utils.py
--rw-r--r--   0        0        0     4366 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/verify.py
--rw-r--r--   0        0        0     4658 2023-07-27 14:12:14.254627 zod-0.3.2/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-07-27 14:12:14.254627 zod-0.3.2/zod/constants.py
--rw-r--r--   0        0        0      184 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-07-27 14:12:14.254627 zod-0.3.2/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12046 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-07-27 14:12:14.254627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0      437 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      355 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8399 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-07-27 14:12:14.258627 zod-0.3.2/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-07-27 14:12:14.258627 zod-0.3.2/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-07-27 14:12:14.258627 zod-0.3.2/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-07-27 14:12:14.258627 zod-0.3.2/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-07-27 14:12:14.258627 zod-0.3.2/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-07-27 14:12:14.258627 zod-0.3.2/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-07-27 14:12:14.258627 zod-0.3.2/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-07-27 14:12:14.258627 zod-0.3.2/zod/zod_drives.py
--rw-r--r--   0        0        0     1147 2023-07-27 14:12:14.258627 zod-0.3.2/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-07-27 14:12:14.258627 zod-0.3.2/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-27 14:36:28.753546 zod-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4809 2023-07-27 14:36:28.753546 zod-0.3.3/README.md
+-rw-r--r--   0        0        0     1783 2023-07-27 14:36:28.753546 zod-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-07-27 14:36:28.753546 zod-0.3.3/zod/__init__.py
+-rw-r--r--   0        0        0     4266 2023-07-27 14:36:28.753546 zod-0.3.3/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/lane.py
+-rw-r--r--   0        0        0     4931 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-07-27 14:36:28.753546 zod-0.3.3/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    16476 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/download.py
+-rw-r--r--   0        0        0     7431 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6032 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1351 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/main.py
+-rw-r--r--   0        0        0      645 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/utils.py
+-rw-r--r--   0        0        0     4366 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/verify.py
+-rw-r--r--   0        0        0     4658 2023-07-27 14:36:28.753546 zod-0.3.3/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-07-27 14:36:28.753546 zod-0.3.3/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-07-27 14:36:28.753546 zod-0.3.3/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-07-27 14:36:28.757546 zod-0.3.3/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12046 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0      437 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      355 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8399 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-07-27 14:36:28.757546 zod-0.3.3/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-07-27 14:36:28.757546 zod-0.3.3/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-07-27 14:36:28.757546 zod-0.3.3/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-07-27 14:36:28.757546 zod-0.3.3/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-07-27 14:36:28.757546 zod-0.3.3/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-07-27 14:36:28.757546 zod-0.3.3/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-07-27 14:36:28.757546 zod-0.3.3/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-07-27 14:36:28.757546 zod-0.3.3/zod/zod_drives.py
+-rw-r--r--   0        0        0     1147 2023-07-27 14:36:28.757546 zod-0.3.3/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-07-27 14:36:28.757546 zod-0.3.3/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.3.3/PKG-INFO
```

### Comparing `zod-0.3.2/LICENSE` & `zod-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/README.md` & `zod-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/pyproject.toml` & `zod-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.3.2"
+version = "0.3.3"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.3.2/zod/__init__.py` & `zod-0.3.3/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/_zod_dataset.py` & `zod-0.3.3/zod/_zod_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,23 @@
         """Get all frame ids (excluding blackisted ones)."""
         return self._train_ids.union(self._val_ids)
 
     def _load_infos(self) -> Tuple[Dict[str, Information], Set[str], Set[str]]:
         """Load frames for the given version."""
         trainval_path = osp.join(self._dataset_root, self.trainval_files[self._version])
         if not osp.exists(trainval_path):
-            msg = f"Could not find trainval file: {trainval_path}."
+            msg = f"Could not find trainval file: {trainval_path}.\n"
             if osp.exists(trainval_path.replace("-", "_")):
                 msg += (
                     "However, found old, incompatible trainval files. Please either downgrade zod "
                     "to < 0.2 or download new files with `zod download --no-images --no-lidar`"
                 )
+            else:
+                cls_name = f"{self.__class__.__name__}-{self._version}"
+                msg += f"Make sure you have downloaded {cls_name} to {self._dataset_root}"
             raise FileNotFoundError(msg)
         with open(trainval_path, "r") as f:
             all_ids = json.load(f)
 
         func = partial(_create_frame, dataset_root=self._dataset_root)
         if self._mp and self._version == FULL:
             infos = process_map(
```

### Comparing `zod-0.3.2/zod/anno/lane.py` & `zod-0.3.3/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/anno/object.py` & `zod-0.3.3/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/anno/parser.py` & `zod-0.3.3/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/anno/tsr/class_map.py` & `zod-0.3.3/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/anno/tsr/traffic_sign.py` & `zod-0.3.3/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/download.py` & `zod-0.3.3/zod/cli/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,34 +204,32 @@
     data_name = file_name.split(".")[0]
     download_path = osp.join(info.dl_dir, f"{file_name}_{info.content_hash[:8]}")
     if _already_downloaded(download_path, info.size):
         if not info.extract_already_downloaded:
             tqdm.write(f"{data_name} already exists. Skipping download and extraction.")
             should_extract = False
         else:
-            tqdm.write(f"File {data_name} already exists. Skipping download.")
+            tqdm.write(f"{data_name} already exists. Skipping download.")
     elif info.dry_run:
-        typer.echo(f"Would download {info.file_path} to {download_path}")
+        msg = "download" if not should_extract else "download and extract"
+        typer.echo(f"Would {msg} {info.file_path} to {download_path}")
+        return
     else:
         try:
             _download(download_path, dbx, info)
         except Exception as e:
             print(f"Error downloading {data_name}: {e}. Please retry")
             return
 
     if should_extract:
-        if info.dry_run:
-            typer.echo(f"Would extract {data_name} to {info.extract_dir}")
+        try:
+            _extract(download_path, info.extract_dir)
+        except Exception as e:
+            print(f"Error extracting {data_name}: {e}. Please retry")
             return
-        else:
-            try:
-                _extract(download_path, info.extract_dir)
-            except Exception as e:
-                print(f"Error extracting {data_name}: {e}. Please retry")
-                return
 
     if info.rm and not info.dry_run:
         os.remove(download_path)
 
 
 def _filter_entry(entry: dropbox.files.Metadata, settings: FilterSettings) -> bool:
     """Filter the entry based on the flags."""
@@ -388,15 +386,15 @@
     dry_run: bool = typer.Option(False, help="Print what would be downloaded", rich_help_panel=GEN),
     extract: bool = typer.Option(True, help="Unpack the archives", rich_help_panel=GEN),
     extract_already_downloaded: bool = typer.Option(
         False, help="Extract already downloaded archives", rich_help_panel=GEN
     ),
     parallel: bool = typer.Option(True, help="Download files in parallel", rich_help_panel=GEN),
     max_workers: int = typer.Option(
-        8, help="Max number of workers for parallel downloads", rich_help_panel=GEN
+        None, help="Max number of workers for parallel downloads", rich_help_panel=GEN
     ),
     no_confirm: bool = typer.Option(
         False,
         "-y",
         "--no-confirm/--confirm",
         help="Don't ask for confirmation",
         is_flag=True,
```

### Comparing `zod-0.3.2/zod/cli/extract_tsr_patches.py` & `zod-0.3.3/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/generate_coco_json.py` & `zod-0.3.3/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/main.py` & `zod-0.3.3/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/utils.py` & `zod-0.3.3/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/verify.py` & `zod-0.3.3/zod/cli/verify.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/cli/visualize_lidar.py` & `zod-0.3.3/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/constants.py` & `zod-0.3.3/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/box.py` & `zod-0.3.3/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/calibration.py` & `zod-0.3.3/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/ego_motion.py` & `zod-0.3.3/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/frame.py` & `zod-0.3.3/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/geometry.py` & `zod-0.3.3/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/info.py` & `zod-0.3.3/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/metadata.py` & `zod-0.3.3/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/sensor.py` & `zod-0.3.3/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/sequence.py` & `zod-0.3.3/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/data_classes/vehicle_data.py` & `zod-0.3.3/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_experimental/eval.py` & `zod-0.3.3/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_experimental/matching.py` & `zod-0.3.3/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_experimental/utils.py` & `zod-0.3.3/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.3.3/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.3.3/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/utils/compensation.py` & `zod-0.3.3/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/utils/geometry.py` & `zod-0.3.3/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/utils/polygon_transformations.py` & `zod-0.3.3/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/utils/utils.py` & `zod-0.3.3/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/utils/visualization.py` & `zod-0.3.3/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/bev_utils.py` & `zod-0.3.3/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/colorlabeler.py` & `zod-0.3.3/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/lidar_3d.py` & `zod-0.3.3/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/lidar_bev.py` & `zod-0.3.3/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/lidar_on_image.py` & `zod-0.3.3/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/object_visualization.py` & `zod-0.3.3/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/oxts_on_image.py` & `zod-0.3.3/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/oxts_visualization.py` & `zod-0.3.3/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/visualization/polygon_utils.py` & `zod-0.3.3/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/zod_drives.py` & `zod-0.3.3/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/zod_frames.py` & `zod-0.3.3/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/zod/zod_sequences.py` & `zod-0.3.3/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.3.2/PKG-INFO` & `zod-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.3.2
+Version: 0.3.3
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

