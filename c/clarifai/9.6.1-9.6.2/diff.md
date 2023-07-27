# Comparing `tmp/clarifai-9.6.1.tar.gz` & `tmp/clarifai-9.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.6.1.tar", last modified: Thu Jul 27 18:52:25 2023, max compression
+gzip compressed data, was "clarifai-9.6.2.tar", last modified: Thu Jul 27 19:17:19 2023, max compression
```

## Comparing `clarifai-9.6.1.tar` & `clarifai-9.6.2.tar`

### file list

```diff
@@ -1,248 +1,284 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.902327 clarifai-9.6.1/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.6.1/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.6.1/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 18:52:25.902111 clarifai-9.6.1/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.6.1/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.761422 clarifai-9.6.1/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.815892 clarifai-9.6.1/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13909 2023-07-27 18:51:46.000000 clarifai-9.6.1/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.818157 clarifai-9.6.1/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.1/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.820807 clarifai-9.6.1/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/data_upload/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/data_upload/convert_csv.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.824169 clarifai-9.6.1/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.1/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.828184 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.736668 clarifai-9.6.1/clarifai/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.829128 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.830043 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.831323 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.832132 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.833173 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.833925 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.834755 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.835716 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.836720 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.837362 clarifai-9.6.1/clarifai/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.842655 clarifai-9.6.1/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.843798 clarifai-9.6.1/clarifai/models/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.845563 clarifai-9.6.1/clarifai/models/model_serving/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.847906 clarifai-9.6.1/clarifai/models/model_serving/cli/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/model_zip.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/repository.py
--rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/constants.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740612 clarifai-9.6.1/clarifai/models/model_serving/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.738995 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.739268 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.849671 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.739963 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740213 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.851678 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740805 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.741052 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.852825 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.854957 clarifai-9.6.1/clarifai/models/model_serving/model_config/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1731 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/deploy.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/serializer.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.857492 clarifai-9.6.1/clarifai/models/model_serving/models/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3701 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/model_types.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/models/output.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/pb_model.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.859676 clarifai-9.6.1/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.1/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.860740 clarifai-9.6.1/clarifai/runners/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.1/clarifai/runners/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.1/clarifai/runners/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.861798 clarifai-9.6.1/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.1/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.1/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.813597 clarifai-9.6.1/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     8294 2023-07-27 18:52:25.000000 clarifai-9.6.1/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)      255 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/entry_points.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       52 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.862722 clarifai-9.6.1/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.863577 clarifai-9.6.1/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13909 2023-07-27 18:51:46.000000 clarifai-9.6.1/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.864830 clarifai-9.6.1/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.1/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.866575 clarifai-9.6.1/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/data_upload/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/data_upload/convert_csv.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.869056 clarifai-9.6.1/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.871709 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.748250 clarifai-9.6.1/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.872200 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.873056 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.874012 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.874569 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.875471 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.876062 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.877112 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.877711 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.878661 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.879151 clarifai-9.6.1/clarifai_utils/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.883813 clarifai-9.6.1/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.884878 clarifai-9.6.1/clarifai_utils/models/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.886400 clarifai-9.6.1/clarifai_utils/models/model_serving/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.888466 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/model_zip.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/repository.py
--rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/constants.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.753763 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.751138 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.751391 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.889711 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.752157 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.752798 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.891281 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.754004 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.754449 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.892201 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.894195 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1731 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/deploy.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/serializer.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.896345 clarifai-9.6.1/clarifai_utils/models/model_serving/models/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3701 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/model_types.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/output.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/pb_model.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.898228 clarifai-9.6.1/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.1/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.899112 clarifai-9.6.1/clarifai_utils/runners/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.1/clarifai_utils/runners/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.1/clarifai_utils/runners/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.900117 clarifai-9.6.1/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.1/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.1/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-07-27 18:52:25.902386 clarifai-9.6.1/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)     1297 2023-07-27 18:52:03.000000 clarifai-9.6.1/setup.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.901738 clarifai-9.6.1/tests/
--rw-r--r--   0 zeiler     (503) staff       (20)     3184 2023-07-27 18:51:46.000000 clarifai-9.6.1/tests/test_auth.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4771 2023-07-07 03:39:45.000000 clarifai-9.6.1/tests/test_modules.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3716 2023-01-03 21:48:03.000000 clarifai-9.6.1/tests/test_stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.700517 clarifai-9.6.2/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.6.2/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.6.2/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 19:17:19.700307 clarifai-9.6.2/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.6.2/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.562806 clarifai-9.6.2/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.598110 clarifai-9.6.2/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13921 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.599955 clarifai-9.6.2/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.2/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.602855 clarifai-9.6.2/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.606160 clarifai-9.6.2/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.2/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.609688 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.2/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.543315 clarifai-9.6.2/clarifai/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.610514 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.611388 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.612726 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.613350 clarifai-9.6.2/clarifai/data_upload/examples/image_detection/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.614304 clarifai-9.6.2/clarifai/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_detection/voc/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.615046 clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.615987 clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/coco/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.617522 clarifai-9.6.2/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.618607 clarifai-9.6.2/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.619247 clarifai-9.6.2/clarifai/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.624835 clarifai-9.6.2/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.2/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.625941 clarifai-9.6.2/clarifai/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.627608 clarifai-9.6.2/clarifai/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.629863 clarifai-9.6.2/clarifai/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      196 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546919 clarifai-9.6.2/clarifai/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.544928 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.545026 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.631578 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.545399 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.545534 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.633184 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.545890 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546011 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.634803 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1847 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546255 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546352 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.635681 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546630 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.546722 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.637260 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1971 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.547015 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.547106 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.638726 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2119 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.640684 clarifai-9.6.2/clarifai/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2801 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     5683 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.643103 clarifai-9.6.2/clarifai/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7069 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3852 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.645288 clarifai-9.6.2/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.2/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.646495 clarifai-9.6.2/clarifai/runners/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.2/clarifai/runners/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.2/clarifai/runners/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.647475 clarifai-9.6.2/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.2/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.2/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.596905 clarifai-9.6.2/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 19:17:18.000000 clarifai-9.6.2/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     9812 2023-07-27 19:17:19.000000 clarifai-9.6.2/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-07-27 19:17:18.000000 clarifai-9.6.2/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)      255 2023-07-27 19:17:18.000000 clarifai-9.6.2/clarifai.egg-info/entry_points.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       52 2023-07-27 19:17:18.000000 clarifai-9.6.2/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-07-27 19:17:18.000000 clarifai-9.6.2/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.648213 clarifai-9.6.2/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.649242 clarifai-9.6.2/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13921 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.650874 clarifai-9.6.2/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.2/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.652636 clarifai-9.6.2/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.660889 clarifai-9.6.2/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.663678 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.550971 clarifai-9.6.2/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.664240 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.665106 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.666106 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.667083 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.668377 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/voc/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.669164 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.670026 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/coco/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.670618 clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.671543 clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.2/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.671915 clarifai-9.6.2/clarifai_utils/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.676674 clarifai-9.6.2/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.2/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.2/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.677668 clarifai-9.6.2/clarifai_utils/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.679204 clarifai-9.6.2/clarifai_utils/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.681475 clarifai-9.6.2/clarifai_utils/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      196 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.557293 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.553950 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.554260 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.682959 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.554677 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.554864 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.684437 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.555274 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.555390 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.686079 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1847 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.555951 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.556091 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.687158 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.556812 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.557024 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.688816 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1971 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.557495 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.557684 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.690414 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2119 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.692332 clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2801 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     5683 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.694659 clarifai-9.6.2/clarifai_utils/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7069 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3852 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1863 2023-07-27 19:16:32.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.2/clarifai_utils/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.696253 clarifai-9.6.2/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.2/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.2/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.697271 clarifai-9.6.2/clarifai_utils/runners/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.2/clarifai_utils/runners/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.2/clarifai_utils/runners/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.698219 clarifai-9.6.2/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.2/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.2/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-07-27 19:17:19.700585 clarifai-9.6.2/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)     1297 2023-07-27 19:16:32.000000 clarifai-9.6.2/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 19:17:19.699941 clarifai-9.6.2/tests/
+-rw-r--r--   0 zeiler     (503) staff       (20)     3184 2023-07-27 18:51:46.000000 clarifai-9.6.2/tests/test_auth.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4771 2023-07-07 03:39:45.000000 clarifai-9.6.2/tests/test_modules.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3716 2023-01-03 21:48:03.000000 clarifai-9.6.2/tests/test_stub.py
```

### Comparing `clarifai-9.6.1/LICENSE` & `clarifai-9.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/PKG-INFO` & `clarifai-9.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.6.1
+Version: 9.6.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.6.1/README.md` & `clarifai-9.6.2/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/auth/helper.py` & `clarifai-9.6.2/clarifai/auth/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         """
     # start with the env vars (potentially loaded from secrets.toml)
     # Don't validate yet as we'll layer on the query params next.
     auth = ClarifaiAuthHelper.from_env(validate=False)
 
     # Then add in the query params.
     try:
-      auth = auth.add_streamlit_query_params(query_params)
+      auth.add_streamlit_query_params(st.experimental_get_query_params())
     except Exception as e:
       st.error(e)
       st.stop()
       raise e
 
     # Then validate.
     try:
@@ -161,15 +161,15 @@
 
     """
 
     # Setup an empty one (not from env).
     auth = ClarifaiAuthHelper("", "", "", "", validate=False)
 
     # Then add in the query params.
-    auth = auth.add_streamlit_query_params(query_params)
+    auth.add_streamlit_query_params(query_params)
 
     # Then validate.
     auth.validate()
 
     return auth
 
   def add_streamlit_query_params(self, query_params: Any = "") -> "ClarifaiAuthHelper":
@@ -234,15 +234,15 @@
 
 Additionally, these optional params are supported:
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
-    token = os.environ("CLARIFAI_SESSION_TOKEN", "")
+    token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
 
   def get_user_app_id_proto(
       self,
```

### Comparing `clarifai-9.6.1/clarifai/client/abc.py` & `clarifai-9.6.2/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/client/stub.py` & `clarifai-9.6.2/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/convert_csv.py` & `clarifai-9.6.2/clarifai/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/base.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/features.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/image.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/text.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.2/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.2/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.2/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/dataset.py` & `clarifai-9.6.2/clarifai/data_upload/examples/image_detection/voc/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/dataset.py` & `clarifai-9.6.2/clarifai/data_upload/examples/image_segmentation/coco/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.2/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/examples.py` & `clarifai-9.6.2/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/data_upload/upload.py` & `clarifai-9.6.2/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.2/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/concepts.py` & `clarifai-9.6.2/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/datasets.py` & `clarifai-9.6.2/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/inputs.py` & `clarifai-9.6.2/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/installed_module_versions.py` & `clarifai-9.6.2/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/lister.py` & `clarifai-9.6.2/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/models.py` & `clarifai-9.6.2/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/module_versions.py` & `clarifai-9.6.2/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/listing/modules.py` & `clarifai-9.6.2/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/api.py` & `clarifai-9.6.2/clarifai/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/__init__.py` & `clarifai-9.6.2/clarifai/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/cli/__init__.py` & `clarifai-9.6.2/clarifai/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.2/clarifai/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/cli/model_zip.py` & `clarifai-9.6.2/clarifai/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/cli/repository.py` & `clarifai-9.6.2/clarifai/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/model_config/__init__.py` & `clarifai-9.6.2/clarifai/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/model_config/serializer.py` & `clarifai-9.6.2/clarifai/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/models/__init__.py` & `clarifai-9.6.2/clarifai/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/models/inference.py` & `clarifai-9.6.2/clarifai/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/models/pb_model.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/models/model_serving/pb_model_repository.py` & `clarifai-9.6.2/clarifai/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/modules/css.py` & `clarifai-9.6.2/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/modules/pages.py` & `clarifai-9.6.2/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/modules/style.css` & `clarifai-9.6.2/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/runners/api.py` & `clarifai-9.6.2/clarifai/runners/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai/urls/helper.py` & `clarifai-9.6.2/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai.egg-info/PKG-INFO` & `clarifai-9.6.2/clarifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.6.1
+Version: 9.6.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.6.1/clarifai.egg-info/SOURCES.txt` & `clarifai-9.6.2/clarifai.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -64,16 +64,25 @@
 clarifai/models/model_serving/cli/repository.py
 clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
 clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
 clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
 clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
 clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
 clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
 clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
 clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+clarifai/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+clarifai/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+clarifai/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
 clarifai/models/model_serving/model_config/__init__.py
 clarifai/models/model_serving/model_config/deploy.py
 clarifai/models/model_serving/model_config/serializer.py
 clarifai/models/model_serving/model_config/triton_config.py
 clarifai/models/model_serving/models/__init__.py
 clarifai/models/model_serving/models/inference.py
 clarifai/models/model_serving/models/model_types.py
@@ -143,16 +152,25 @@
 clarifai_utils/models/model_serving/cli/repository.py
 clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
 clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
 clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
 clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
 clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
 clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/__init__.py
+clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/inference.py
+clarifai_utils/models/model_serving/examples/text_to_text/bart-summarize/1/model.py
 clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
 clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/__init__.py
+clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/inference.py
+clarifai_utils/models/model_serving/examples/visual_embedding/vit-base/1/model.py
+clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/__init__.py
+clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/inference.py
+clarifai_utils/models/model_serving/examples/visual_segmentation/segformer-b2/1/model.py
 clarifai_utils/models/model_serving/model_config/__init__.py
 clarifai_utils/models/model_serving/model_config/deploy.py
 clarifai_utils/models/model_serving/model_config/serializer.py
 clarifai_utils/models/model_serving/model_config/triton_config.py
 clarifai_utils/models/model_serving/models/__init__.py
 clarifai_utils/models/model_serving/models/inference.py
 clarifai_utils/models/model_serving/models/model_types.py
```

### Comparing `clarifai-9.6.1/clarifai_utils/auth/helper.py` & `clarifai-9.6.2/clarifai_utils/auth/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         """
     # start with the env vars (potentially loaded from secrets.toml)
     # Don't validate yet as we'll layer on the query params next.
     auth = ClarifaiAuthHelper.from_env(validate=False)
 
     # Then add in the query params.
     try:
-      auth = auth.add_streamlit_query_params(query_params)
+      auth.add_streamlit_query_params(st.experimental_get_query_params())
     except Exception as e:
       st.error(e)
       st.stop()
       raise e
 
     # Then validate.
     try:
@@ -161,15 +161,15 @@
 
     """
 
     # Setup an empty one (not from env).
     auth = ClarifaiAuthHelper("", "", "", "", validate=False)
 
     # Then add in the query params.
-    auth = auth.add_streamlit_query_params(query_params)
+    auth.add_streamlit_query_params(query_params)
 
     # Then validate.
     auth.validate()
 
     return auth
 
   def add_streamlit_query_params(self, query_params: Any = "") -> "ClarifaiAuthHelper":
@@ -234,15 +234,15 @@
 
 Additionally, these optional params are supported:
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
     user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
-    token = os.environ("CLARIFAI_SESSION_TOKEN", "")
+    token = os.environ.get("CLARIFAI_SESSION_TOKEN", "")
     pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
     return cls(user_id, app_id, pat, token, base, ui, validate)
 
   def get_user_app_id_proto(
       self,
```

### Comparing `clarifai-9.6.1/clarifai_utils/client/abc.py` & `clarifai-9.6.2/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/client/stub.py` & `clarifai-9.6.2/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/convert_csv.py` & `clarifai-9.6.2/clarifai_utils/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.2/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/examples.py` & `clarifai-9.6.2/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/data_upload/upload.py` & `clarifai-9.6.2/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.2/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/concepts.py` & `clarifai-9.6.2/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/datasets.py` & `clarifai-9.6.2/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/inputs.py` & `clarifai-9.6.2/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.6.2/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/lister.py` & `clarifai-9.6.2/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/models.py` & `clarifai-9.6.2/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/module_versions.py` & `clarifai-9.6.2/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/listing/modules.py` & `clarifai-9.6.2/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/api.py` & `clarifai-9.6.2/clarifai_utils/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/__init__.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/__init__.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/model_zip.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/repository.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/text_to_text/bart-summarize/1/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
     from inference import InferenceModel
 
     self.inference_obj = InferenceModel()
-    self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
     self.input_name = [inp.name for inp in self.config_msg.input][0]
```

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/__init__.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/serializer.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/models/__init__.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/models/inference.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/models/pb_model.py` & `clarifai-9.6.2/clarifai/models/model_serving/examples/visual_embedding/vit-base/1/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
     from inference import InferenceModel
 
     self.inference_obj = InferenceModel()
-    self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
     self.input_name = [inp.name for inp in self.config_msg.input][0]
```

### Comparing `clarifai-9.6.1/clarifai_utils/models/model_serving/pb_model_repository.py` & `clarifai-9.6.2/clarifai_utils/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/modules/css.py` & `clarifai-9.6.2/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/modules/pages.py` & `clarifai-9.6.2/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/modules/style.css` & `clarifai-9.6.2/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/runners/api.py` & `clarifai-9.6.2/clarifai_utils/runners/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/clarifai_utils/urls/helper.py` & `clarifai-9.6.2/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/setup.py` & `clarifai-9.6.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.6.1",
+    version="9.6.2",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

### Comparing `clarifai-9.6.1/tests/test_auth.py` & `clarifai-9.6.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/tests/test_modules.py` & `clarifai-9.6.2/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.1/tests/test_stub.py` & `clarifai-9.6.2/tests/test_stub.py`

 * *Files identical despite different names*

