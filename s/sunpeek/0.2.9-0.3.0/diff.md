# Comparing `tmp/sunpeek-0.2.9-py3-none-any.whl.zip` & `tmp/sunpeek-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,65 +1,75 @@
-Zip file size: 160786 bytes, number of entries: 63
+Zip file size: 192799 bytes, number of entries: 73
 -rw-r--r--  2.0 unx     1035 b- defN 80-Jan-01 00:00 sunpeek/__init__.py
 -rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 sunpeek/api/__init__.py
 -rw-r--r--  2.0 unx      581 b- defN 80-Jan-01 00:00 sunpeek/api/dependencies.py
--rw-r--r--  2.0 unx     4170 b- defN 80-Jan-01 00:00 sunpeek/api/main.py
+-rw-r--r--  2.0 unx     5737 b- defN 80-Jan-01 00:00 sunpeek/api/main.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunpeek/api/routers/__init__.py
--rw-r--r--  2.0 unx     1713 b- defN 80-Jan-01 00:00 sunpeek/api/routers/api_jobs.py
+-rw-r--r--  2.0 unx     1718 b- defN 80-Jan-01 00:00 sunpeek/api/routers/api_jobs.py
 -rw-r--r--  2.0 unx     5692 b- defN 80-Jan-01 00:00 sunpeek/api/routers/config.py
--rw-r--r--  2.0 unx     3403 b- defN 80-Jan-01 00:00 sunpeek/api/routers/evaluations.py
--rw-r--r--  2.0 unx     2782 b- defN 80-Jan-01 00:00 sunpeek/api/routers/files.py
--rw-r--r--  2.0 unx    13410 b- defN 80-Jan-01 00:00 sunpeek/api/routers/plant.py
+-rw-r--r--  2.0 unx     5513 b- defN 80-Jan-01 00:00 sunpeek/api/routers/evaluations.py
+-rw-r--r--  2.0 unx     6582 b- defN 80-Jan-01 00:00 sunpeek/api/routers/files.py
+-rw-r--r--  2.0 unx    19436 b- defN 80-Jan-01 00:00 sunpeek/api/routers/plant.py
 -rw-r--r--  2.0 unx      780 b- defN 80-Jan-01 00:00 sunpeek/base_model.py
--rw-r--r--  2.0 unx      150 b- defN 80-Jan-01 00:00 sunpeek/common/__init__.py
+-rw-r--r--  2.0 unx      100 b- defN 80-Jan-01 00:00 sunpeek/common/__init__.py
 -rw-r--r--  2.0 unx     1248 b- defN 80-Jan-01 00:00 sunpeek/common/common_units.py
--rw-r--r--  2.0 unx     1446 b- defN 80-Jan-01 00:00 sunpeek/common/config_parser.py
--rw-r--r--  2.0 unx    19464 b- defN 80-Jan-01 00:00 sunpeek/common/context.py
--rw-r--r--  2.0 unx    17482 b- defN 80-Jan-01 00:00 sunpeek/common/data_uploader.py
--rw-r--r--  2.0 unx     1056 b- defN 80-Jan-01 00:00 sunpeek/common/errors.py
--rw-r--r--  2.0 unx    17621 b- defN 80-Jan-01 00:00 sunpeek/common/unit_uncertainty.py
--rw-r--r--  2.0 unx     6119 b- defN 80-Jan-01 00:00 sunpeek/common/utils.py
--rw-r--r--  2.0 unx      960 b- defN 80-Jan-01 00:00 sunpeek/components/__init__.py
--rw-r--r--  2.0 unx    12272 b- defN 80-Jan-01 00:00 sunpeek/components/base.py
--rw-r--r--  2.0 unx     2763 b- defN 80-Jan-01 00:00 sunpeek/components/components_factories.py
--rw-r--r--  2.0 unx    15276 b- defN 80-Jan-01 00:00 sunpeek/components/fluid_helpers.py
--rw-r--r--  2.0 unx    26357 b- defN 80-Jan-01 00:00 sunpeek/components/fluids.py
--rw-r--r--  2.0 unx    14915 b- defN 80-Jan-01 00:00 sunpeek/components/helpers.py
--rw-r--r--  2.0 unx    15711 b- defN 80-Jan-01 00:00 sunpeek/components/iam_methods.py
+-rw-r--r--  2.0 unx     1968 b- defN 80-Jan-01 00:00 sunpeek/common/config_parser.py
+-rw-r--r--  2.0 unx     1802 b- defN 80-Jan-01 00:00 sunpeek/common/errors.py
+-rw-r--r--  2.0 unx     6639 b- defN 80-Jan-01 00:00 sunpeek/common/time_zone.py
+-rw-r--r--  2.0 unx    17863 b- defN 80-Jan-01 00:00 sunpeek/common/unit_uncertainty.py
+-rw-r--r--  2.0 unx     5134 b- defN 80-Jan-01 00:00 sunpeek/common/utils.py
+-rw-r--r--  2.0 unx      986 b- defN 80-Jan-01 00:00 sunpeek/components/__init__.py
+-rw-r--r--  2.0 unx    13435 b- defN 80-Jan-01 00:00 sunpeek/components/base.py
+-rw-r--r--  2.0 unx     2800 b- defN 80-Jan-01 00:00 sunpeek/components/components_factories.py
+-rw-r--r--  2.0 unx    26948 b- defN 80-Jan-01 00:00 sunpeek/components/fluids.py
+-rw-r--r--  2.0 unx    14800 b- defN 80-Jan-01 00:00 sunpeek/components/fluids_wpd_models.py
+-rw-r--r--  2.0 unx    14886 b- defN 80-Jan-01 00:00 sunpeek/components/helpers.py
+-rw-r--r--  2.0 unx    15752 b- defN 80-Jan-01 00:00 sunpeek/components/iam_methods.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 sunpeek/components/jobs.py
--rw-r--r--  2.0 unx     2031 b- defN 80-Jan-01 00:00 sunpeek/components/operational_events.py
--rw-r--r--  2.0 unx    57176 b- defN 80-Jan-01 00:00 sunpeek/components/physical.py
--rw-r--r--  2.0 unx     2874 b- defN 80-Jan-01 00:00 sunpeek/components/results.py
--rw-r--r--  2.0 unx    18114 b- defN 80-Jan-01 00:00 sunpeek/components/sensor.py
--rw-r--r--  2.0 unx    10512 b- defN 80-Jan-01 00:00 sunpeek/components/sensor_types.py
--rw-r--r--  2.0 unx    21647 b- defN 80-Jan-01 00:00 sunpeek/components/types.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunpeek/core_methods/__init__.py
--rw-r--r--  2.0 unx     3203 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/__init__.py
--rw-r--r--  2.0 unx    13949 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/equation.py
--rw-r--r--  2.0 unx    27733 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/main.py
--rw-r--r--  2.0 unx    12817 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/plotting.py
--rw-r--r--  2.0 unx     3664 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/verify_validate.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/__init__.py
--rw-r--r--  2.0 unx    30187 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/main.py
--rw-r--r--  2.0 unx    33627 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/radiation.py
+-rw-r--r--  2.0 unx     3804 b- defN 80-Jan-01 00:00 sunpeek/components/operational_events.py
+-rw-r--r--  2.0 unx    49882 b- defN 80-Jan-01 00:00 sunpeek/components/physical.py
+-rw-r--r--  2.0 unx     3075 b- defN 80-Jan-01 00:00 sunpeek/components/results.py
+-rw-r--r--  2.0 unx    23359 b- defN 80-Jan-01 00:00 sunpeek/components/sensor.py
+-rw-r--r--  2.0 unx    11412 b- defN 80-Jan-01 00:00 sunpeek/components/sensor_types.py
+-rw-r--r--  2.0 unx    21504 b- defN 80-Jan-01 00:00 sunpeek/components/types.py
+-rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 sunpeek/core_methods/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunpeek/core_methods/common/__init__.py
+-rw-r--r--  2.0 unx    13669 b- defN 80-Jan-01 00:00 sunpeek/core_methods/common/main.py
+-rw-r--r--  2.0 unx     4570 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/__init__.py
+-rw-r--r--  2.0 unx    15126 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/equation.py
+-rw-r--r--  2.0 unx    31604 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/main.py
+-rw-r--r--  2.0 unx    22617 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/plotting.py
+-rw-r--r--  2.0 unx    10781 b- defN 80-Jan-01 00:00 sunpeek/core_methods/pc_method/wrapper.py
+-rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/__init__.py
+-rw-r--r--  2.0 unx    41535 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/algorithms.py
+-rw-r--r--  2.0 unx     4224 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/main.py
+-rw-r--r--  2.0 unx    35090 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/radiation.py
+-rw-r--r--  2.0 unx     3449 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/virtuals_array.py
+-rw-r--r--  2.0 unx     3868 b- defN 80-Jan-01 00:00 sunpeek/core_methods/virtuals/virtuals_plant.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunpeek/data_handling/__init__.py
+-rw-r--r--  2.0 unx    23508 b- defN 80-Jan-01 00:00 sunpeek/data_handling/context.py
+-rw-r--r--  2.0 unx    24335 b- defN 80-Jan-01 00:00 sunpeek/data_handling/data_uploader.py
+-rw-r--r--  2.0 unx     1849 b- defN 80-Jan-01 00:00 sunpeek/data_handling/wrapper.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 sunpeek/db_utils/__init__.py
--rw-r--r--  2.0 unx     4139 b- defN 80-Jan-01 00:00 sunpeek/db_utils/crud.py
--rw-r--r--  2.0 unx    14093 b- defN 80-Jan-01 00:00 sunpeek/db_utils/db_data_operations.py
--rw-r--r--  2.0 unx     1334 b- defN 80-Jan-01 00:00 sunpeek/db_utils/init_db.py
--rw-r--r--  2.0 unx      345 b- defN 80-Jan-01 00:00 sunpeek/definitions/__init__.py
--rw-r--r--  2.0 unx    18422 b- defN 80-Jan-01 00:00 sunpeek/definitions/collector_types.py
--rw-r--r--  2.0 unx    31721 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_definitions.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.csv
--rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.onnxbytes
--rw-r--r--  2.0 unx      241 b- defN 80-Jan-01 00:00 sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.csv
--rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.onnxbytes
+-rw-r--r--  2.0 unx     5593 b- defN 80-Jan-01 00:00 sunpeek/db_utils/crud.py
+-rw-r--r--  2.0 unx    16575 b- defN 80-Jan-01 00:00 sunpeek/db_utils/db_data_operations.py
+-rw-r--r--  2.0 unx     1921 b- defN 80-Jan-01 00:00 sunpeek/db_utils/init_db.py
+-rw-r--r--  2.0 unx      454 b- defN 80-Jan-01 00:00 sunpeek/definitions/__init__.py
+-rw-r--r--  2.0 unx    24370 b- defN 80-Jan-01 00:00 sunpeek/definitions/collector_types.py
+-rw-r--r--  2.0 unx      334 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/density.csv
+-rw-r--r--  2.0 unx      337 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/heat capacity.csv
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Pekasolar_FHW/density.csv
+-rw-r--r--  2.0 unx      241 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Pekasolar_FHW/heat capacity.csv
+-rw-r--r--  2.0 unx     3450 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Wocklum Thermum P/density.csv
+-rw-r--r--  2.0 unx     2532 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Wocklum Thermum P/heat capacity.csv
+-rw-r--r--  2.0 unx    33003 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_definitions.py
 -rw-r--r--  2.0 unx      528 b- defN 80-Jan-01 00:00 sunpeek/demo/__init__.py
--rw-r--r--  2.0 unx     1371 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant.py
--rw-r--r--  2.0 unx     4894 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant_script.py
--rw-r--r--  2.0 unx     2836 b- defN 80-Jan-01 00:00 sunpeek/exporter.py
--rw-r--r--  2.0 unx    14227 b- defN 80-Jan-01 00:00 sunpeek/serializable_models.py
--rw-r--r--  2.0 unx     7652 b- defN 80-Jan-01 00:00 sunpeek-0.2.9.dist-info/COPYING.LESSER
--rw-r--r--  2.0 unx    16989 b- defN 80-Jan-01 00:00 sunpeek-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 sunpeek-0.2.9.dist-info/COPYING
-?rw-r--r--  2.0 unx     5713 b- defN 16-Jan-01 00:00 sunpeek-0.2.9.dist-info/RECORD
-63 files, 586719 bytes uncompressed, 151636 bytes compressed:  74.2%
+-rw-r--r--  2.0 unx     1902 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant.py
+-rw-r--r--  2.0 unx     5168 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant_script.py
+-rw-r--r--  2.0 unx     6191 b- defN 80-Jan-01 00:00 sunpeek/exporter.py
+-rw-r--r--  2.0 unx    22264 b- defN 80-Jan-01 00:00 sunpeek/serializable_models.py
+-rw-r--r--  2.0 unx     7652 b- defN 80-Jan-01 00:00 sunpeek-0.3.0.dist-info/COPYING.LESSER
+-rw-r--r--  2.0 unx    15233 b- defN 80-Jan-01 00:00 sunpeek-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 sunpeek-0.3.0.dist-info/COPYING
+?rw-r--r--  2.0 unx     6642 b- defN 16-Jan-01 00:00 sunpeek-0.3.0.dist-info/RECORD
+73 files, 711544 bytes uncompressed, 182159 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -36,21 +36,18 @@
 
 Filename: sunpeek/common/common_units.py
 Comment: 
 
 Filename: sunpeek/common/config_parser.py
 Comment: 
 
-Filename: sunpeek/common/context.py
-Comment: 
-
-Filename: sunpeek/common/data_uploader.py
+Filename: sunpeek/common/errors.py
 Comment: 
 
-Filename: sunpeek/common/errors.py
+Filename: sunpeek/common/time_zone.py
 Comment: 
 
 Filename: sunpeek/common/unit_uncertainty.py
 Comment: 
 
 Filename: sunpeek/common/utils.py
 Comment: 
@@ -60,18 +57,18 @@
 
 Filename: sunpeek/components/base.py
 Comment: 
 
 Filename: sunpeek/components/components_factories.py
 Comment: 
 
-Filename: sunpeek/components/fluid_helpers.py
+Filename: sunpeek/components/fluids.py
 Comment: 
 
-Filename: sunpeek/components/fluids.py
+Filename: sunpeek/components/fluids_wpd_models.py
 Comment: 
 
 Filename: sunpeek/components/helpers.py
 Comment: 
 
 Filename: sunpeek/components/iam_methods.py
 Comment: 
@@ -96,38 +93,65 @@
 
 Filename: sunpeek/components/types.py
 Comment: 
 
 Filename: sunpeek/core_methods/__init__.py
 Comment: 
 
+Filename: sunpeek/core_methods/common/__init__.py
+Comment: 
+
+Filename: sunpeek/core_methods/common/main.py
+Comment: 
+
 Filename: sunpeek/core_methods/pc_method/__init__.py
 Comment: 
 
 Filename: sunpeek/core_methods/pc_method/equation.py
 Comment: 
 
 Filename: sunpeek/core_methods/pc_method/main.py
 Comment: 
 
 Filename: sunpeek/core_methods/pc_method/plotting.py
 Comment: 
 
-Filename: sunpeek/core_methods/pc_method/verify_validate.py
+Filename: sunpeek/core_methods/pc_method/wrapper.py
 Comment: 
 
 Filename: sunpeek/core_methods/virtuals/__init__.py
 Comment: 
 
+Filename: sunpeek/core_methods/virtuals/algorithms.py
+Comment: 
+
 Filename: sunpeek/core_methods/virtuals/main.py
 Comment: 
 
 Filename: sunpeek/core_methods/virtuals/radiation.py
 Comment: 
 
+Filename: sunpeek/core_methods/virtuals/virtuals_array.py
+Comment: 
+
+Filename: sunpeek/core_methods/virtuals/virtuals_plant.py
+Comment: 
+
+Filename: sunpeek/data_handling/__init__.py
+Comment: 
+
+Filename: sunpeek/data_handling/context.py
+Comment: 
+
+Filename: sunpeek/data_handling/data_uploader.py
+Comment: 
+
+Filename: sunpeek/data_handling/wrapper.py
+Comment: 
+
 Filename: sunpeek/db_utils/__init__.py
 Comment: 
 
 Filename: sunpeek/db_utils/crud.py
 Comment: 
 
 Filename: sunpeek/db_utils/db_data_operations.py
@@ -138,27 +162,33 @@
 
 Filename: sunpeek/definitions/__init__.py
 Comment: 
 
 Filename: sunpeek/definitions/collector_types.py
 Comment: 
 
-Filename: sunpeek/definitions/fluid_definitions.py
+Filename: sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/density.csv
+Comment: 
+
+Filename: sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/heat capacity.csv
 Comment: 
 
-Filename: sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.csv
+Filename: sunpeek/definitions/fluid_data/Pekasolar_FHW/density.csv
 Comment: 
 
-Filename: sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.onnxbytes
+Filename: sunpeek/definitions/fluid_data/Pekasolar_FHW/heat capacity.csv
 Comment: 
 
-Filename: sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.csv
+Filename: sunpeek/definitions/fluid_data/Wocklum Thermum P/density.csv
 Comment: 
 
-Filename: sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.onnxbytes
+Filename: sunpeek/definitions/fluid_data/Wocklum Thermum P/heat capacity.csv
+Comment: 
+
+Filename: sunpeek/definitions/fluid_definitions.py
 Comment: 
 
 Filename: sunpeek/demo/__init__.py
 Comment: 
 
 Filename: sunpeek/demo/demo_plant.py
 Comment: 
@@ -168,23 +198,23 @@
 
 Filename: sunpeek/exporter.py
 Comment: 
 
 Filename: sunpeek/serializable_models.py
 Comment: 
 
-Filename: sunpeek-0.2.9.dist-info/COPYING.LESSER
+Filename: sunpeek-0.3.0.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: sunpeek-0.2.9.dist-info/METADATA
+Filename: sunpeek-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sunpeek-0.2.9.dist-info/WHEEL
+Filename: sunpeek-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sunpeek-0.2.9.dist-info/COPYING
+Filename: sunpeek-0.3.0.dist-info/COPYING
 Comment: 
 
-Filename: sunpeek-0.2.9.dist-info/RECORD
+Filename: sunpeek-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sunpeek/api/main.py

```diff
@@ -2,90 +2,114 @@
 import json
 from fastapi import Depends, FastAPI, Request
 from fastapi.responses import JSONResponse
 from fastapi.middleware.cors import CORSMiddleware
 import sqlalchemy.exc
 import pint.errors
 import traceback
+import pytz
+from fastapi.responses import FileResponse, ORJSONResponse
 
 import sunpeek
-from sunpeek.common.utils import hit_logger
+from sunpeek.common.utils import sp_logger
 from sunpeek.common import errors
+import sunpeek.common.time_zone as tz
 from sunpeek.api.routers import files, evaluations, config, plant, api_jobs
-from sunpeek.api.dependencies import get_query_token
+from sunpeek.api.dependencies import get_query_token, session
 import sunpeek.serializable_models as smodels
+import sunpeek.exporter
 
 root_path = os.environ.get('HIT_API_ROOT_PATH', None)
-hit_logger.info(f"HarvestIT API started with root_path set to {root_path}")
+sp_logger.info(f"HarvestIT API started with root_path set to {root_path}")
 
 app = FastAPI(dependencies=[Depends(get_query_token)], title="SunPeek API", root_path=root_path,
+              version=sunpeek.__version__, default_response_class=ORJSONResponse,
               responses={400: {"description": "Bad Request", "model": smodels.Error}})
 
 app.include_router(files.files_router)
 app.include_router(evaluations.evaluations_router)
 app.include_router(evaluations.stored_evaluations_router)
 app.include_router(config.config_router)
 app.include_router(plant.plants_router)
 app.include_router(plant.plant_router)
 app.include_router(plant.any_plant_router)
 app.include_router(api_jobs.jobs_router)
 
 
 @app.exception_handler(sqlalchemy.exc.NoResultFound)
 def db_not_found(request, exc):
-    hit_logger.warning(traceback.format_tb(exc.__traceback__))
+    sp_logger.warning(traceback.format_tb(exc.__traceback__))
     return JSONResponse(
-            status_code=404,
-            content={"error": "NoResultFound",
-                     "message": exc.args[0],
-                     "detail": "The requested object, or one of it's child objects, cannot be found in the database"}
+        status_code=404,
+        content={"error": "NoResultFound",
+                 "message": exc.args[0],
+                 "detail": "The requested object, or one of it's child objects, cannot be found in the database"}
     )
 
 
-@app.exception_handler(errors.HitError)
+@app.exception_handler(errors.SunPeekError)
 @app.exception_handler(AssertionError)
 def general_hit_errors(request, exc):
-    hit_logger.warning(traceback.format_tb(exc.__traceback__))
+    sp_logger.warning(traceback.format_tb(exc.__traceback__))
     response = smodels.Error(error=exc.__class__.__name__,
-                                   message="The syntax of this request was valid, but there was an error processing it "
-                                        "further, see error detail",
-                                   detail=str(exc))
+                             message="The syntax of this request was valid, but there was an error processing it "
+                                     "further, see error detail",
+                             detail=str(exc))
     return JSONResponse(
-            status_code=400,
-            content=response.dict()
+        status_code=400,
+        content=response.dict()
+    )
+
+
+@app.exception_handler(pytz.exceptions.UnknownTimeZoneError)
+def unknown_tz_err(request, exc):
+    sp_logger.warning(traceback.format_tb(exc.__traceback__))
+    response = smodels.Error(error=exc.__class__.__name__,
+                             message="Unknown Timezone",
+                             detail=f"{str(exc)} was not recognised as a valid timezone identifier")
+    return JSONResponse(
+        status_code=400,
+        content=response.dict()
     )
 
 
 @app.exception_handler(sqlalchemy.exc.IntegrityError)
 def db_integrity_err(request, exc):
-    if "duplicate key value violates unique constraint" in str(exc):
-        hit_logger.warning(str(exc.orig))
+    if "duplicate key value violates unique constraint" in str(exc) or "UNIQUE constraint failed" in str(exc):
+        sp_logger.warning(str(exc.orig))
         return JSONResponse(
-                status_code=409,
-                content={"error": "IntegrityError",
-                         "message": "Item with duplicate identifier (e.g. name or id) exists",
-                         "detail": str(exc.orig)}
+            status_code=409,
+            content={"error": "IntegrityError",
+                     "message": "Item with duplicate identifier (e.g. name or id) exists",
+                     "detail": str(exc.orig)}
         )
-    if "is still referenced from table" in str(exc):
+    if "is still referenced from table" in str(exc) or "FOREIGN KEY constraint failed" in str(exc):
         return JSONResponse(
-                status_code=409,
-                content={"error": "IntegrityError",
-                         "message": "Cannot remove a component which is still referenced by other components",
-                         "detail": str(exc.orig)}
+            status_code=409,
+            content={"error": "IntegrityError",
+                     "message": "Cannot remove a component which is still referenced by other components",
+                     "detail": str(exc.orig)}
         )
 
+    else:
+        return JSONResponse(content = {"error": "IntegrityError",
+                                       "message": "A database integrity error occurred",
+                                       "detail": ''},
+                                       status_code=500)
+
+
 
 @app.exception_handler(pint.errors.UndefinedUnitError)
 def invalid_unit(_, exc):
     return JSONResponse(
         status_code=422,
         content={"error": "UndefinedUnitError",
                  "message": "One of the unit strings in your request was invalid",
                  "detail": str(exc)}
-        )
+    )
 
 
 origins = json.loads(os.environ.get('HIT_API_ALLOWED_ORIGINS',
                                     '["http://localhost", "http://127.0.0.1", "http://localhost:8080", \
                                     "http://127.0.0.1:8080", "http://localhost:8000"]')
                      )
 
@@ -93,18 +117,33 @@
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
+
 @app.get('/about')
-def about(request:Request):
+def about(request: Request):
     content = {'version': sunpeek.__version__,
                'interactive_docs_url': str(request.url).split(request.url.path)[0] + app.docs_url,
                'redoc_docs_url': str(request.url).split(request.url.path)[0] + app.redoc_url}
     return JSONResponse(status_code=200, content=content)
 
-#For Debugging
+
+@app.get('/debug_info', response_class=FileResponse, tags=["debug"])
+def about(include_plants: bool = True, include_db_structure: bool = True, session=Depends(session)):
+    content = sunpeek.exporter.dump_debug_info(include_plants, include_db_structure, session=session)
+    return JSONResponse(status_code=200, content=content)
+
+
+@app.get("/available_timezones", tags=["plant", "info", "timezones"],
+         summary="Show a list of timezones, including plant local time without DST")
+def list_timezones():
+    return JSONResponse(status_code=200, content=tz.available_timezones)
+
+
+# For Debugging
 if __name__ == '__main__':
     import uvicorn
+
     uvicorn.run("main:app", host='0.0.0.0', port=8000)
```

## sunpeek/api/routers/api_jobs.py

```diff
@@ -14,15 +14,15 @@
     prefix="/jobs",
     tags=["jobs"],
 )
 
 
 def create_result_url(job, request):
     if job.result_path:
-        job.result_url = request.url_for('result_file', id=job.id)
+        job.result_url = str(request.url_for('result_file', id=job.id))
     return job
 
 
 @jobs_router.get("/", response_model=List[smodels.Job], summary="List all jobs, or get one by id")
 @jobs_router.get("/{id}", response_model=smodels.Job, summary="Get a job by id")
 def jobs(request: Request, id: uuid.UUID = None, sess: Session=Depends(session), crd=Depends(crud)):
     jobs = crd.get_components(sess, "Job", id)
```

## sunpeek/api/routers/evaluations.py

```diff
@@ -1,16 +1,16 @@
 import datetime
-
+from typing import Union, List
 from fastapi import APIRouter, Depends, HTTPException
-from typing import Union
+
 from sunpeek.api.dependencies import session, crud
 from sunpeek.api.routers.plant import plant_router
 from sunpeek.api.routers.config import config_router
-from sunpeek.core_methods.pc_method import PCMethod
-import enum
+from sunpeek.core_methods.pc_method import AvailablePCEquations, AvailablePCMethods
+from sunpeek.core_methods.pc_method.wrapper import run_performance_check, list_pc_problems
 import sunpeek.serializable_models as smodels
 
 evaluations_router = APIRouter(
     prefix=plant_router.prefix + "/evaluations",
     tags=["methods", "evaluations"]
 )
 
@@ -21,51 +21,88 @@
 
 
 @evaluations_router.get("/run")
 @stored_evaluations_router.get("/run", tags=["methods", "evaluations"])
 def run(plant_id: int, stored_eval_id: int, method: str = None,
         eval_start: str = "1900-01-01 00:00:00", eval_end: str = "2021-01-01 00:00:00",
         sess=Depends(session), crd=Depends(crud)):
-    plant = crd.get_plants(sess, plant_id=plant_id)
+    crd.get_plants(sess, plant_id=plant_id)
     raise HTTPException(status_code=501,
                         detail="Stored evaluations are not yet implemented in HarvesIT", headers=
                         {"Retry-After": "Wed, 30 Nov 2022 23:59 GMT", "Cache-Control": "no-cache"})
 
 
-class available_pc_equations(enum.IntEnum):
-    one = 1
-    two = 2
-
-
-class available_pc_methods(enum.Enum):
-    iso = 'iso'
-    improved = 'improved'
-
-
 @evaluations_router.get("/pc_method", summary="Run the PC method", response_model=smodels.PCMethodOutput)
-def quick_run_pc_method(plant_id: int, method: available_pc_methods,
-                        equation: available_pc_equations,
-                        eval_start: Union[datetime.datetime, None] = None,
-                        eval_end: Union[datetime.datetime, None] = None,
-                        sess=Depends(session), crd=Depends(crud)):
+def run_pc_method(plant_id: int,
+                  method: Union[AvailablePCMethods, None] = None,
+                  equation: Union[AvailablePCEquations, None] = None,
+                  eval_start: Union[datetime.datetime, None] = None,
+                  eval_end: Union[datetime.datetime, None] = None,
+                  ignore_wind: Union[bool, None] = None,
+                  safety_pipes: Union[float, None] = None,
+                  safety_uncertainty: Union[float, None] = None,
+                  safety_others: Union[float, None] = None,
+                  sess=Depends(session), crd=Depends(crud)):
     """Runs the PC Method for the specified dates range"""
     plant = crd.get_plants(sess, plant_id=plant_id)
     plant.context.set_eval_interval(eval_start=eval_start, eval_end=eval_end)
-    pc_obj = PCMethod.create(method=method.name, plant=plant, equation_id=equation)
-    return pc_obj.run()
+    pc_output = run_performance_check(
+        plant=plant,
+        method=[method],
+        equation=[equation],
+        use_wind=None if ignore_wind is None else [not ignore_wind],
+        safety_pipes=safety_pipes,
+        safety_uncertainty=safety_uncertainty,
+        safety_others=safety_others,
+    ).output
+
+    return pc_output
+
+
+@evaluations_router.get("/pc_method_problems", summary="Report which PC method variants can be run",
+                        response_model=List[smodels.PCMethodProblem])
+def list_pc_problems_api(plant_id: int,
+                         method: Union[AvailablePCMethods, None] = None,
+                         equation: Union[AvailablePCEquations, None] = None,
+                         ignore_wind: Union[bool, None] = None,
+                         sess=Depends(session), crd=Depends(crud)) -> List[smodels.PCMethodProblem]:
+    """Runs the PC Method for the specified dates range"""
+    plant = crd.get_plants(sess, plant_id=plant_id)
+    pc_problems = list_pc_problems(
+        plant=plant,
+        method=[method],
+        equation=[equation],
+        use_wind=None if ignore_wind is None else [not ignore_wind],
+    )
+
+    return pc_problems
+
+# @evaluations_router.get("/pc_method", summary="Run the PC method", response_model=smodels.PCMethodOutput)
+# def quick_run_pc_method(plant_id: int, method: AvailablePCMethods,
+#                         equation: Union[AvailablePCEquations, None],
+#                         eval_start: Union[datetime.datetime, None] = None,
+#                         eval_end: Union[datetime.datetime, None] = None,
+#                         sess=Depends(session), crd=Depends(crud)):
+#     """Runs the PC Method for the specified dates range"""
+#     plant = crd.get_plants(sess, plant_id=plant_id)
+#     plant.context.set_eval_interval(eval_start=eval_start, eval_end=eval_end)
+#     pc_obj = PCMethod.create(method=method.name, plant=plant, equation=equation)
+#     pc_output = pc_obj.run()
+#     return pc_output
+
 
 # @methods_router.get("/get-dcat-method-results")
 # async def get_dcat_method_results(plant_id: str, start_date: str = "2021-05-20 13:00:00", end_date: str = "2021-05-21 13:00:00"):
 #     """Retrieves the results of the DCAT method for the specified dates range"""
 #     results_dict = {"plant_id": plant_id,"start_date":start_date, "end_date":end_date, "results_array": [1,1,2,1.5] }
 #     return results_dict
 
 
 # @methods_router.get("/run-pc-method")
-# async def run_pc_method(plant_id: str, start_date: str = "2021-05-20 13:00:00", end_date: str = "2021-05-21 13:00:00"):
+# async def run_performance_check(plant_id: str, start_date: str = "2021-05-20 13:00:00", end_date: str = "2021-05-21 13:00:00"):
 #     """Runs the PC method on the clean data stored between the specified dates range"""
 #
 #     results_dict = {"plant_id": plant_id,"start_date":start_date, "end_date":end_date, "results_array": [.35,.39,1.69,4.86,6.23,.51,5.25] }
 #
 #     return results_dict
```

## sunpeek/api/routers/files.py

```diff
@@ -1,20 +1,19 @@
 from typing import List
-from fastapi import APIRouter, Depends, HTTPException
+import warnings
+from fastapi import APIRouter, Depends, HTTPException, Response
 from fastapi.datastructures import UploadFile
 from sqlalchemy.orm import Session
 
-from sunpeek.common.utils import hit_logger
-from sunpeek.common.data_uploader import DataUploader_db
-from sunpeek.serializable_models import DataUploadResponse
+from sunpeek.common.utils import sp_logger
+from sunpeek.common.time_zone import process_timezone
+from sunpeek.data_handling.data_uploader import DataUploader_df, DataUploader_pq, DataUploadResponse, DataColumnsResponse
 from sunpeek.api.dependencies import session, crud
 from sunpeek.api.routers.plant import plant_router
-
-# from api.models import DataUploadResponse
-
+from sunpeek.common.utils import DatetimeTemplates
 
 files_router = APIRouter(
     prefix="/data",
     tags=["data"],
     # dependencies=[Depends(get_token_header)],
     responses={404: {"description": "Not found"}},
 )
@@ -25,55 +24,149 @@
     """This method server as a usage example only for the log class and the HTTP exception raising. It must be deleted for release"""
 
     try:
         x = 1 / 0
     except (Exception) as err:
 
         # how to use the logger to report an exception
-        hit_logger.exception(err)
+        sp_logger.exception(err)
         # how to manually report using the INFO level
-        hit_logger.info("This wont print in file because of loggers level")
+        sp_logger.info("This won't print in file because of loggers level")
         # str(err) gives the message related to the exception
         error_dict = {"message": "UPS something went wrong", "error": str(err)}
         # raise HTTPException so the API returns an error code instead of freezing
         raise HTTPException(status_code=500, detail=error_dict)
 
 
-@plant_router.post("/data", tags=["data"], response_model=DataUploadResponse)
+@plant_router.post("/data", tags=["data"], response_model=DataUploadResponse, status_code=201)
 def upload_measure_data(
         plant_id: int,
         files: List[UploadFile],
+        datetime_template: DatetimeTemplates = None,
+        datetime_format: str = None,
         timezone: str = None,
+        csv_separator: str = ';',
+        csv_decimal: str = '.',
+        csv_encoding: str = 'utf-8',
+        index_col: int = 0,
+        response: Response = Response(),
         sess: Session = Depends(session),
         crd: crud = Depends(crud)) -> DataUploadResponse:
     """Ingests csv files to database. For details, see docstring of the `data_uploader` module.
 
     Parameters
     ----------
     plant_id : A pre-configured plant with this name must exist in the database.
-    files : list, List of csv files that are batch ingested.
-    timezone : str, a timezone string like 'Europe/Vienna'
+    files : list
+        List of csv files that are batch ingested.
+    datetime_template : DatetimeTemplates
+        Templates to simplify the definition of a datetime format. Overridden by datetime_format (if not None).
+    datetime_format : str
+        Used to parse datetimes from csv file. Leave to None infers the format.
+    timezone : str or pytz.timezone.
+        Optional. To be provided if timestamps in the data have no time zone information.
+    csv_separator : str
+        Used in pd.read_csv as 'sep' kwarg
+    csv_decimal : str
+        Used in pd.read_csv as 'decimal' kwarg
+    csv_encoding : str
+        Used in pd.read_csv as 'encoding' kwarg
+    index_col : int
+        DataUploader will try to parse timestamps from this column.
     sess : sqlalchemy.orm.Session
     crd : api.dependencies.crud
 
     Returns
     -------
     upload_response : DataUploadResponse
 
     Raises
     ------
     ConnectionError
     HTTPException
     """
-    try:
-        up = DataUploader_db(plant=crd.get_plants(sess, plant_id),
-                             files=files,
+
+    with warnings.catch_warnings(record=True) as wrngs:
+        up = DataUploader_pq(plant=crd.get_plants(sess, plant_id),
+                             datetime_template=datetime_template,
+                             datetime_format=datetime_format,
+                             timezone=timezone,
+                             csv_separator=csv_separator,
+                             csv_decimal=csv_decimal,
+                             csv_encoding=csv_encoding,
+                             index_col=index_col)
+        out = up.do_upload(files=files)
+
+    if wrngs is not None:
+        response.headers['x-sunpeek-warnings'] = str([str(w.message) for w in wrngs])
+
+    return out  # DataUploadResponse
+
+
+@plant_router.post("/data/columns", tags=["data"], response_model=DataColumnsResponse, status_code=201)
+def get_sensor_names_and_index(
+        plant_id: int,
+        files: List[UploadFile],
+        csv_separator: str = ';',
+        csv_decimal: str = '.',
+        csv_encoding: str = 'utf-8',
+        index_col: int = 0,
+        datetime_template: DatetimeTemplates = None,
+        datetime_format: str = None,
+        timezone: str = None,
+        response: Response = Response(),
+        sess: Session = Depends(session),
+        crd: crud = Depends(crud)) -> DataColumnsResponse:
+    """Ingests csv files to database. For details, see docstring of the `data_uploader` module.
+
+    Parameters
+    ----------
+    plant_id : A pre-configured plant with this name must exist in the database.
+    files : list
+        List of csv files that are batch ingested.
+    csv_separator : str
+        Used in pd.read_csv as 'sep' kwarg
+    csv_decimal : str
+        Used in pd.read_csv as 'decimal' kwarg
+    csv_encoding : str
+        Used in pd.read_csv as 'encoding' kwarg
+    index_col : int
+        DataUploader will try to parse timestamps from this column.
+    datetime_template : DatetimeTemplates
+        Templates to simplify the definition of a datetime format. Overridden by datetime_format (if not None).
+    datetime_format : str
+        Used to parse datetimes from csv file. Leave to None infers the format.
+    timezone : str or pytz.timezone.
+        Optional. To be provided if timestamps in the data have no time zone information.
+    sess : sqlalchemy.orm.Session
+    crd : api.dependencies.crud
+
+    Returns
+    -------
+    upload_response : DataColumnsResponse
+
+    Raises
+    ------
+    ConnectionError
+    HTTPException
+    """
+
+    with warnings.catch_warnings(record=True) as wrngs:
+        plant = crd.get_plants(sess, plant_id)
+        timezone = process_timezone(timezone, plant)
+        up = DataUploader_df(plant=plant,
+                             datetime_template=datetime_template,
+                             datetime_format=datetime_format,
                              timezone=timezone,
-                             session=sess)
-        response = up.do_upload()
-        return response  # DataUploadResponse
-
-    except Exception as ex:
-        hit_logger.exception(ex)
-        raise HTTPException(status_code=500,
-                            detail="Something went wrong while uploading the files, please check the system log for "
-                                   "details and try again.")
+                             csv_separator=csv_separator,
+                             csv_decimal=csv_decimal,
+                             csv_encoding=csv_encoding,
+                             index_col=index_col)
+
+        sensor_names = up.get_sensor_names(files=files)
+        index_name = up.get_index_name(files=files)
+        out = {"sensors": list(sensor_names), "index": index_name}
+
+    if wrngs is not None:
+        response.headers['x-sunpeek-warnings'] = str([str(w.message) for w in wrngs])
+
+    return out  # DataColumnsResponse
```

## sunpeek/api/routers/plant.py

```diff
@@ -1,16 +1,23 @@
-from fastapi import APIRouter, Depends, BackgroundTasks, Request
 from typing import List, Union
+import datetime
+import pytz
+from fastapi import APIRouter, Depends, BackgroundTasks, Request
+from fastapi.responses import JSONResponse, Response
+
 from sqlalchemy.orm import Session
-from sunpeek.common import config_parser
-import sunpeek.exporter
-import sunpeek.components as cmp
 from sunpeek.api.dependencies import session, crud
 import sunpeek.serializable_models as smodels
 import sunpeek.demo.demo_plant as demo_plant_function
+import sunpeek.core_methods.virtuals as virtuals
+from sunpeek.common import config_parser
+import sunpeek.components as cmp
+from sunpeek.common.errors import TimeZoneError
+from sunpeek.data_handling.context import NanReportResponse
+import sunpeek.exporter
 
 plants_router = APIRouter(
     prefix="/plants",
     tags=["plants"],
     # dependencies=[Depends(get_token_header)],
     responses={404: {"description": "Not found"}},
 )
@@ -51,23 +58,18 @@
                     summary="create plants",
                     status_code=201,
                     responses={
                         409: {"description": "Conflict, most likely because the plant name or name of a child "
                                              "object already exists",
                               "model": smodels.Error}})
 def create_plant(plant: smodels.NewPlant, session: Session = Depends(session), crud=Depends(crud)):
-    """
-    Create a new plant. `name`, `latitude`, `longitude` are required. sensors can be mapped by passing a list of sensor
+    """ Create a new plant. `name`, `latitude`, `longitude` are required. sensors can be mapped by passing a list of sensor
     structures to `sensors`
     """
     plant = config_parser.make_full_plant(plant.dict(exclude_unset=True), session)
-    # plant = crud.create_component(session, plant)
-    # done at each plant update anyway
-    # plant.config_virtuals()
-    # plant = crud.update_component(session, plant)
     plant = crud.create_component(session, plant)
     return plant
 
 
 @plants_router.get("/create_demo_plant", response_model=smodels.Plant,
                    summary="Create demo plant config, optionally including data, if data is to be included, "
                            "accept_license must also be set to true")
@@ -95,26 +97,26 @@
 def export_conf(plant_id: int, session: Session = Depends(session), crud=Depends(crud)):
     plant = crud.get_plants(session, plant_id=plant_id)
     return smodels.ConfigExport(**sunpeek.exporter.create_export_config(plant))
 
 
 @plant_router.post("/export_complete", response_model=smodels.JobReference,
                    tags=["plants", "export"], summary="Export a plant with configuration and data",
-                   description="""Create an export job for a compleate plant with sensor types, collector types, 
+                   description="""Create an export job for a complete plant with sensor types, collector types, 
                    fluid definitions, and data. When the job completes a tar package containing a json file, 
                    and data 1 CSV file per calender year, is available for download""",
                    status_code=202)
 def create_complete_export(request: Request, background_tasks: BackgroundTasks, plant_id: int,
                            include_virtuals: bool = True,
                            session: Session = Depends(session), crud=Depends(crud)):
     plant = crud.get_plants(session, plant_id=plant_id)
     job = cmp.Job(status=cmp.helpers.ResultStatus.pending, plant=plant)
     crud.create_component(session, job)
     background_tasks.add_task(sunpeek.exporter.create_export_package, plant, include_virtuals, job)
-    return smodels.JobReference(job_id=job.id, href=request.url_for('jobs') + str(job.id))
+    return smodels.JobReference(job_id=job.id, href=str(request.url_for('jobs')) + str(job.id))
 
 
 def update_obj(obj, update_model):
     update_dict = update_model.dict(exclude_unset=True)
 
     for key, val in update_dict.items():
         if val != getattr(obj, key):
@@ -153,28 +155,77 @@
     name = p.name
     session.delete(p)
     session.commit()
 
     return str(f'plant {name} was deleted')
 
 
+@plant_router.get("/sensors/nan_report", tags=["sensors", "data"],
+                  summary="Triggers calculation of the daily-summarized NaN report for all sensors.")
+def nan_report(plant_id: int,
+               eval_start: Union[datetime.datetime, None] = None,
+               eval_end: Union[datetime.datetime, None] = None,
+               sess: Session = Depends(session), crd=Depends(crud)) -> NanReportResponse:
+    plant = crd.get_plants(sess, plant_id=plant_id)
+    plant.context.set_eval_interval(eval_start=eval_start, eval_end=eval_end)
+    nan_report = plant.context.get_nan_report(include_virtuals=True)
+
+    return nan_report
+
+
+@plant_router.get("/sensors/recalculate_virtuals", tags=["sensors, virtual"],
+                  summary="Triggers the recalculation of all virtual sensors of that plant")
+def recalculate_virtuals(plant_id: int, sess: Session = Depends(session), crd=Depends(crud)):
+    plant = crd.get_plants(sess, plant_id=plant_id)
+    virtuals.calculate_virtuals(plant)
+    return JSONResponse(status_code=200,
+                        content={"description": "Recalculation done!", "message": "Recalculation done!"})
+
+
 @plant_router.get("/sensors", response_model=Union[List[smodels.Sensor], smodels.Sensor],
                   tags=["sensors"],
                   summary="Get a list of sensors, or select by id or raw name")
+@plant_router.get("/sensors/{id}", response_model=smodels.Sensor, tags=["sensors"],
+                  summary="Get a single sensor by id")
 @any_plant_router.get("/sensors/{id}", response_model=smodels.Sensor, tags=["sensors"],
                       summary="Get a single sensor by id")
-def sensors(id: int = None, raw_name: str = None, plant_id: int = None,
+def sensors(id: int = None, raw_name: str = None, plant_id: Union[int, str] = None,
             session: Session = Depends(session), crud=Depends(crud)):
+    plant_id = None if plant_id == '-' else plant_id
     sensors = crud.get_sensors(session, id, raw_name, plant_id)
     return sensors
 
 
-@any_plant_router.post("/sensors", response_model=List[smodels.Sensor],
-                  tags=["sensors"],
-                  summary="Batch update a list of sensors, each passed sensor object must contain an id")
+@plant_router.get("/sensors/{id}/data", tags=["sensors", "data"],
+                  summary="Get measurement data of a single sensor by id")
+@any_plant_router.get("/sensors/{id}/data", response_model=smodels.Sensor, tags=["sensors"],
+                      summary="Get measurement data of a single sensor by id")
+def sensor_data(id: int = None, raw_name: str = None, plant_id: Union[int, str] = None,
+                eval_start: Union[datetime.datetime, None] = None,
+                eval_end: Union[datetime.datetime, None] = None,
+                session: Session = Depends(session), crud=Depends(crud)):
+    plant_id = None if plant_id == '-' else plant_id
+    plant = crud.get_plants(session, plant_id=plant_id)
+    plant.context.set_eval_interval(eval_start=eval_start, eval_end=eval_end)
+    sensor = crud.get_sensors(session, plant_id=plant_id, id=id)
+    data = sensor.data.pint.to(sensor.native_unit)
+    df = data.astype(float)  # to_json does not work with dtype pint.
+    return Response(df.to_json(), media_type="application/json")
+
+
+@plant_router.get("/sensors/recalculate_virtuals", tags=["sensors, virtual"],
+                  summary="Triggers the recalculation of all virtual sensors of that plant")
+def recalculate_virtuals(plant_id: int, sess: Session = Depends(session), crd=Depends(crud)):
+    plant = crd.get_plants(sess, plant_id=plant_id)
+    plant.calculate_virtuals()
+    return JSONResponse(status_code=200, content={"description": "Recalculation done!", "message": "Recalculation done!"})
+
+
+@any_plant_router.post("/sensors", response_model=List[smodels.Sensor], tags=["sensors"],
+                       summary="Batch update a list of sensors, each passed sensor object must contain an id")
 def update_sensors(sensors: List[smodels.BulkUpdateSensor], sess: Session = Depends(session), crd=Depends(crud)):
     for sensor in sensors:
         sensor_obj = crd.get_sensors(sess, sensor.id)
         crd.update_component(sess, update_obj(sensor_obj, sensor), commit=False)
     sess.commit()
     return sensors
 
@@ -214,46 +265,54 @@
     session.commit()
     return rets
 
 
 @any_plant_router.delete("/sensors/{id}", tags=["sensors"], summary="Delete a single sensor by id")
 def delete_sensor(id: int, sess: Session = Depends(session), crd=Depends(crud)):
     sensor_obj = crd.get_sensors(sess, id)
+    # if sensor_obj.plant is not None:
+    #     plant = sensor_obj.plant
+    #     plant.defer_configure_virtuals = True
+    # sensor_obj.remove_references(include_plant=False)
+    # crd.delete_component(sess, sensor_obj)
+    # plant.defer_configure_virtuals = False
+    # plant.arrays
+    with sess.no_autoflush:
+        sensor_obj.remove_references()
     crd.delete_component(sess, sensor_obj)
+    # plant.config_virtuals()
 
 
 @plant_router.get("/arrays", response_model=Union[List[smodels.Array], smodels.Array],
                   tags=["arrays"],
                   summary="Get a list of arrays, or select by id or name and plant")
 @any_plant_router.get("/arrays/{id}", response_model=smodels.Array, tags=["arrays"],
                       summary="Get a single array by id")
-def arrays(id: int = None, name: str = None, plant_id: int = None, plant_name: str = None,
+def arrays(id: int = None, name: str = None, plant_id: Union[int, str] = None, plant_name: str = None,
            session: Session = Depends(session), crud=Depends(crud)):
+    plant_id = None if plant_id == '-' else plant_id
     return crud.get_components(session, cmp.Array, id, name, plant_id, plant_name)
 
 
 @any_plant_router.post("/arrays/{id}", response_model=smodels.Array,
                        tags=["arrays"],
                        summary="Update an array by id")
-def arrays(id: int, array: smodels.Array, session: Session = Depends(session), crud=Depends(crud)):
+def update_array(id: int, array: smodels.Array, session: Session = Depends(session), crud=Depends(crud)):
     array_cmp = crud.get_components(session, component=cmp.Array, id=id)
-    array = array.dict(exclude_unset=True)
-
-    for key, val in array.items():
-        setattr(array_cmp, key, val)
-
+    array_cmp = update_obj(array_cmp, array)
     array_cmp = crud.update_component(session, array_cmp)
     return array_cmp
 
 
 @any_plant_router.delete("/arrays/{id}", tags=["arrays"],
                          summary="Delete an array by id")
 def arrays(id: int, session: Session = Depends(session), crud=Depends(crud)):
     array = crud.get_components(session, component=cmp.Array, id=id)
-    name = array.name
+    if array.plant is not None:
+        array.plant.arrays.pop(array.plant.arrays.index(array))
     session.delete(array)
     session.commit()
 
 
 @plant_router.post("/arrays/new",
                    response_model=Union[List[smodels.Array], smodels.Array],
                    tags=["arrays"], status_code=201,
@@ -292,7 +351,50 @@
 
 
 @plant_router.get("/fluids/{id}", response_model=smodels.Fluid,
                   tags=["fluids"],
                   summary="Get a single fluid by id")
 def fluids(id: int, session: Session = Depends(session), crud=Depends(crud)):
     return crud.get_components(session, cmp.Fluid, id=id)
+
+
+@plant_router.get("/operational_events", response_model=Union[smodels.OperationalEvent, List[smodels.OperationalEvent]],
+                  tags=["operational events"],
+                  summary="Get a list of operational_events for a plant, or select by date range, or id")
+def get_operational_events(plant_id: int, id: int = None, search_start: datetime.datetime = None,
+                           search_end: datetime.datetime = None, search_timezone: str = None,
+                           sess: Session = Depends(session), crd=Depends(crud)):
+    if ((search_start is not None) or (search_end is not None)) and (search_timezone is None):
+        raise TimeZoneError(
+            "The parameter 'timezone' must be specified in order to interpret search start and search end timestamps correctly")
+    if search_start is not None:
+        search_start = pytz.timezone(search_timezone).localize(search_start)
+        search_start = pytz.timezone('UTC').normalize(search_start)
+    if search_end is not None:
+        search_end = pytz.timezone(search_timezone).localize(search_end)
+        search_end = pytz.timezone('UTC').normalize(search_end)
+
+    return crd.get_operational_events(sess, id, plant_id, search_start=search_start, search_end=search_end)
+
+
+@any_plant_router.get("/operational_events/{id}", response_model=smodels.OperationalEvent,
+                      tags=["operational events"], summary="an operational event by id")
+def get_operational_event(id: int = None, sess: Session = Depends(session), crd=Depends(crud)):
+    return crd.get_operational_events(sess, id)
+
+
+@plant_router.post("/operational_events", response_model=smodels.OperationalEvent, tags=["operational events"],
+                   summary="Create an operational event")
+def create_operational_event(plant_id: int, event_start: datetime.datetime, timezone: str, description: str = None,
+                             event_end: datetime.datetime = None, ignored_range: bool = False,
+                             sess: Session = Depends(session), crd=Depends(crud)):
+    plant = crd.get_plants(sess, plant_id)
+    event = cmp.OperationalEvent(plant, event_start, tz=timezone, event_end=event_end, description=description,
+                                 ignored_range=ignored_range)
+    return crd.create_component(sess, event)
+
+
+@any_plant_router.delete("/operational_events/{id}", tags=["operational events"],
+                         summary="Delete an operational event by id")
+def delete_operational_event(id: int, sess: Session = Depends(session), crd=Depends(crud)):
+    event = crd.get_operational_events(sess, id)
+    crd.delete_component(sess, event)
```

## sunpeek/common/__init__.py

```diff
@@ -1,6 +1,4 @@
 from . import config_parser
-from . import context
-from . import data_uploader
 from . import errors
 from . import unit_uncertainty
 from . import utils
```

## sunpeek/common/config_parser.py

```diff
@@ -1,41 +1,61 @@
 import copy
+from sqlalchemy import exc
+
 import sunpeek.components as cmp
-from sunpeek.common.errors import ConfigurationError
+from sunpeek.common.errors import ConfigurationError, DuplicateNameError
+
+
+def _check_colltype_in_db(session, col_type_name):
+    if session is not None:
+        import sqlalchemy.exc
+        try:
+            session.query(cmp.CollectorType).filter(cmp.CollectorType.name == col_type_name).one()
+            return True
+        except sqlalchemy.exc.NoResultFound:
+            return False
+    return False
 
 
 def make_full_plant(conf, session=None):
     conf = copy.deepcopy(conf)
     collector_types = {}
     if 'collector_types' in conf:
         col_types = conf['collector_types']
         for col_type in col_types:
             test_type = col_type.pop('test_type')
-            if test_type in ['SST', "static"]:
+            if _check_colltype_in_db(session, col_type['name']):
+                type_obj = col_type['name']
+            elif test_type in ['SST', "static"]:
                 type_obj = cmp.CollectorTypeSST(**col_type)
             elif test_type in ['QDT', "dynamic"]:
                 type_obj = cmp.CollectorTypeQDT(**col_type)
             else:
-                raise ConfigurationError("CollectorType test_type parameter must be one of 'SST', 'static', 'QDT' or 'dynamic'")
+                raise ConfigurationError(
+                    "CollectorType test_type parameter must be one of 'SST', 'static', 'QDT' or 'dynamic'")
             collector_types[type_obj.name] = type_obj
     if 'plant' in conf:
         conf = conf['plant']
         for array in conf['arrays']:
             if array['collector_type'] in collector_types.keys():
                 array['collector_type'] = collector_types[array['collector_type']]
 
     plant = cmp.Plant(**conf)
 
     if session is not None:
         session.add(plant)
-        session.rollback()
+        # session.rollback()
 
     return plant
 
 
 def make_and_store_plant(conf, session):
-    p = make_full_plant(conf, session)
-    session.add(p)
-    # done at each plant update anyway
-    # p.config_virtuals()  # To ensure that sensor types, fluids etc. are available, do this after adding plant to session
-    session.commit()
-    return p
+    plant = make_full_plant(conf, session)
+    session.add(plant)
+
+    try:
+        session.flush()
+    except exc.IntegrityError:
+        session.rollback()
+        raise DuplicateNameError(f'Plant with name "{plant.name}" already exists.')
+
+    return plant
```

## sunpeek/common/errors.py

```diff
@@ -1,43 +1,78 @@
-class HitError(Exception):
+class SunPeekError(Exception):
     pass
 
 
-class ConfigurationError(HitError):
+class ConfigurationError(SunPeekError):
     pass
 
 
-class CollectorDefinitionError(HitError):
+class CollectorDefinitionError(SunPeekError):
     """Error in CollectorType definition.
     E.g. if supplied information is contradictory or not sufficient for full CollectorType definition.
     See #70 for valid CollectorType definitions.
     """
     pass
 
 
-class IncompatibleUnitError(HitError):
+class IncompatibleUnitError(SunPeekError):
     """Supplied unit (of raw sensor) is not compatible with the expected unit, e.g. as defined in SensorType.
     """
     pass
 
 
-class VirtualSensorConfigurationError(HitError):
+class VirtualSensorConfigurationError(SunPeekError):
     """Error in calcluation of virtual sensor due to missing input or input being None.
     """
     pass
 
 
-class VirtualSensorCalculationError(HitError):
+class PCMethodError(SunPeekError):
+    """General error in definition / configuration / calculation of PC method.
+    """
+    pass
+
+
+class CalculationError(SunPeekError):
     """General error in definition / handling of virtual senso.
     """
     pass
 
 
-class DuplicateNameError(HitError):
+class AlgorithmError(SunPeekError):
+    """Error in some core_method algorithm.
+    """
+    pass
+
+
+class DuplicateNameError(SunPeekError):
     """Error due to creating a component with a duplicate name, where this is not allowed"""
     pass
 
 
-class SensorNotFoundError(HitError):
+class SensorNotFoundError(SunPeekError):
     """Error due to not finding a sensor when one was expected to exist"""
     pass
 
+
+class SensorDataNotFoundError(SunPeekError):
+    """Error due to not finding a data column for a sensor in the current data store"""
+    pass
+
+
+class TimeIndexError(SunPeekError):
+    """Error handling or retrieving plant.time_index."""
+    pass
+
+
+class TimeZoneError(SunPeekError):
+    """Error related to time zone"""
+    pass
+
+
+class DataProcessingError(SunPeekError):
+    """Error related to data upload and processing"""
+    pass
+
+
+class DatabaseAlreadyExistsError(SunPeekError):
+    pass
```

## sunpeek/common/unit_uncertainty.py

```diff
@@ -72,18 +72,18 @@
 
 
 # units = create_unit_registry()
 pint_pandas.PintType.ureg = units
 Q = units.Quantity
 
 
-def get_unit_string(s):
-    """Returns unit of a pint unit-aware pd.Series as a string.
-    """
-    return s.pint.units.__str__()
+# def get_unit_string(s):
+#     """Returns unit of a pint unit-aware pd.Series as a string.
+#     """
+#     return s.pint.units.__str__()
 
 
 def to_s(num_arr_or_q, unit_str=''):
     """Return the input numeric array converted to pd.Series with dtype pint[unit_str]. No index."""
     if isinstance(num_arr_or_q, pint.Quantity):
         q = num_arr_or_q.to(unit_str)
         num_arr_or_q = q.m
@@ -93,15 +93,15 @@
     return pd.Series(num_arr_or_q).astype(f'pint[{unit_str}]')
 
 
 def to_numpy(s, unit_str=''):
     """Return the unit-aware pd.Series `s` to a numpy array after converting it to unit_str."""
     if isinstance(s, pint.Quantity):
         s = to_s(s, unit_str)
-    return s.pint.to(unit_str).astype('float64').to_numpy()
+    return s.pint.to(unit_str).astype(float).to_numpy()
 
 
 # def copy_unit(copy_from, copy_to):
 #     """Copies dtype pint unit from pd.Series `in1` and assigns it to s2 as .astype(pint[unit]).
 #     Same for DataFrame, applies to each column then. Both inputs have to be either Series or DataFrames.
 #     If inputs are DataFrames, it assumes all columns in in2 are found in in1.
 #     Parameters
@@ -231,157 +231,157 @@
     #     unc_m = unc.to(unit).magnitude
     # uarr = unumpy.uarray(x, unc_m)
     # pobj = units.Quantity(uarr, unit)
     pobj = units.Quantity(x, unit)
     return pobj
 
 
-def to_series(pobj, output_unit=None, direction='plus', k=1, n=1, index=None, name=None):
-    """
-    Converts a (vector) pint Quantity object to a pandas Series by stripping uncertainty and unit from pobj.
-
-    Notes
-    -----
-    Treatment of uncertainty can be controlled by parameters direction and k. This function returns the expanded
-    uncertainty, i.e. lower / upper bound of nominal_value +/- k * standard_uncertainty. For details on expanded
-    uncertainty, see e.g. [1]_
-
-    Parameters
-    ----------
-    pobj : `pint Quantity`
-    pobj
-        Pint object to convert.
-    
-    output_unit : `string`, optional
-        Unit string for pobj conversion. If `None`, output series will have the same unit as the input `pobj`.
-        Must be valid unit that can be passed as units(output_unit)
-    
-    direction : {'plus', 'minus'}
-        Direction in which uncertainty is added ('plus') or subtracted ('minus') from the nominal values to calculate
-        the expanded uncertainty.
-
-    k : `float`, default=1
-        Amount of uncertainty added to / subtracted from the nominal values to get the expanded uncertainty, in terms
-        of multiples of the standard uncertainty: expanded = nominal_value +/- k * standard_uncertainty
-        Assuming normal distribution, expanded uncertainty with k=1 yields 68% of values, k=2 95%, k=3 99.7%.
-
-    n : `float`, default=1
-        Multiplier of the nominal values in the returned pandas Series. You will in almost all cases leave this at
-        the default value of 1. So the true return formula is: expanded = n * nominal_value +/- k * standard_uncertainty
-
-    index : `pd.Index`, optional
-        pandas.Index that is attached to the output pandas Series.
-
-    name : `string`, optional
-        Name of the output pandas Series.
-
-    Returns
-    -------
-    s : `pd.Series`
-        A pandas Series, optionally with name and index, optionally converted to output_unit.
-    
-    References
-    ----------
-    .. [1] `What Does k=2 Mean in Accuracy and Uncertainty
-    Specifications?<https://blog.mensor.com/blog/what-does-k2-mean-in-accuracy-specification>`_
-
-    Examples
-    --------
-    # >>> s = to_series(x)
-    # >>> s = to_series(x, index=index, name='x')
-    # >>> s = to_series(x, direction='plus', k=1, index=index, name='x')
-    # >>> s = to_series(x, output_unit='mm', direction='plus', k=1, index=index, name='x')
-    """
-    # xm = pobj.magnitude
-    # nom = unumpy.nominal_values(xm)
-    # sd = unumpy.std_devs(xm)
-    # sgn = 1 if (direction.lower() == 'plus') else -1
-    # expanded = n * nom + k * sgn * sd
-
-    expanded = pobj.magnitude
-
-    if output_unit is not None:
-        expanded_u = units.Quantity(expanded, pobj.units)
-        expanded = expanded_u.to(output_unit).magnitude
-
-    s = pd.Series(data=expanded, index=index, name=name).astype(f'pint[{output_unit}]')
-    return s
-
-
-def nominal_values(pobj, output_unit=None, index=None, name=None):
-    """
-    Strips the uncertainty from a (vector) pint Quantity object and returns the nominal values in a given unit.
-
-    Parameters
-    ----------
-        pint object to convert.
-    pobj : `pint Quantity`
-        pint object to convert.
-    pobj
-        Pint object to convert.
-
-    output_unit : `string`, optional
-        Unit for the output conversion. If `None`, the output series will have the same unit as the input `pobj`.
-        Must be valid unit that can be passed as units(output_unit)
-
-    index : `pd.Index`, optional
-        pandas.Index that is attached to the output pandas Series.
-
-    name : `string`, optional
-        Name of the output pandas Series.
-
-    Returns
-    -------
-    s : `pd.Series`
-        A pandas Series, optionally with name and index, optionally converted to output_unit.
-
-    Examples
-    --------
-    uu.nominal_values(pobj)
-    uu.nominal_values(pobj, output_unit='m')
-    uu.nominal_values(pobj, output_unit='m', index=df.index)
-    uu.nominal_values(pobj, output_unit='m', index=df.index, name='x')
-    """
-    return to_series(pobj, output_unit=output_unit, k=0, index=index, name=name).astype(f'pint[{output_unit}]')
-
-
-def std_devs(pobj, output_unit=None, index=None, name=None):
-    """
-    Returns the uncertainty from a (vector) pint Quantity object and returns the uncertainty in a given unit.
-
-    Parameters
-    ----------
-    pobj : `pint Quantity`
-    pobj
-        Pint object to convert.
-
-    output_unit : `string`, optional
-        Unit for the output conversion. If `None`, the output series will have the same unit as the input `pobj`.
-        Must be valid unit that can be passed as units(output_unit)
+# def to_series(pobj, output_unit=None, direction='plus', k=1, n=1, index=None, name=None):
+#     """
+#     Converts a (vector) pint Quantity object to a pandas Series by stripping uncertainty and unit from pobj.
+#
+#     Notes
+#     -----
+#     Treatment of uncertainty can be controlled by parameters direction and k. This function returns the expanded
+#     uncertainty, i.e. lower / upper bound of nominal_value +/- k * standard_uncertainty. For details on expanded
+#     uncertainty, see e.g. [1]_
+#
+#     Parameters
+#     ----------
+#     pobj : `pint Quantity`
+#     pobj
+#         Pint object to convert.
+#
+#     output_unit : `string`, optional
+#         Unit string for pobj conversion. If `None`, output series will have the same unit as the input `pobj`.
+#         Must be valid unit that can be passed as units(output_unit)
+#
+#     direction : {'plus', 'minus'}
+#         Direction in which uncertainty is added ('plus') or subtracted ('minus') from the nominal values to calculate
+#         the expanded uncertainty.
+#
+#     k : `float`, default=1
+#         Amount of uncertainty added to / subtracted from the nominal values to get the expanded uncertainty, in terms
+#         of multiples of the standard uncertainty: expanded = nominal_value +/- k * standard_uncertainty
+#         Assuming normal distribution, expanded uncertainty with k=1 yields 68% of values, k=2 95%, k=3 99.7%.
+#
+#     n : `float`, default=1
+#         Multiplier of the nominal values in the returned pandas Series. You will in almost all cases leave this at
+#         the default value of 1. So the true return formula is: expanded = n * nominal_value +/- k * standard_uncertainty
+#
+#     index : `pd.Index`, optional
+#         pandas.Index that is attached to the output pandas Series.
+#
+#     name : `string`, optional
+#         Name of the output pandas Series.
+#
+#     Returns
+#     -------
+#     s : `pd.Series`
+#         A pandas Series, optionally with name and index, optionally converted to output_unit.
+#
+#     References
+#     ----------
+#     .. [1] `What Does k=2 Mean in Accuracy and Uncertainty
+#     Specifications?<https://blog.mensor.com/blog/what-does-k2-mean-in-accuracy-specification>`_
+#
+#     Examples
+#     --------
+#     # >>> s = to_series(x)
+#     # >>> s = to_series(x, index=index, name='x')
+#     # >>> s = to_series(x, direction='plus', k=1, index=index, name='x')
+#     # >>> s = to_series(x, output_unit='mm', direction='plus', k=1, index=index, name='x')
+#     """
+#     # xm = pobj.magnitude
+#     # nom = unumpy.nominal_values(xm)
+#     # sd = unumpy.std_devs(xm)
+#     # sgn = 1 if (direction.lower() == 'plus') else -1
+#     # expanded = n * nom + k * sgn * sd
+#
+#     expanded = pobj.magnitude
+#
+#     if output_unit is not None:
+#         expanded_u = units.Quantity(expanded, pobj.units)
+#         expanded = expanded_u.to(output_unit).magnitude
+#
+#     s = pd.Series(data=expanded, index=index, name=name).astype(f'pint[{output_unit}]')
+#     return s
 
-    index : `pd.Index`, optional
-        pandas.Index that is attached to the output pandas Series.
 
-    name : `string`, optional
-        Name of the output pandas Series.
+# def nominal_values(pobj, output_unit=None, index=None, name=None):
+#     """
+#     Strips the uncertainty from a (vector) pint Quantity object and returns the nominal values in a given unit.
+#
+#     Parameters
+#     ----------
+#         pint object to convert.
+#     pobj : `pint Quantity`
+#         pint object to convert.
+#     pobj
+#         Pint object to convert.
+#
+#     output_unit : `string`, optional
+#         Unit for the output conversion. If `None`, the output series will have the same unit as the input `pobj`.
+#         Must be valid unit that can be passed as units(output_unit)
+#
+#     index : `pd.Index`, optional
+#         pandas.Index that is attached to the output pandas Series.
+#
+#     name : `string`, optional
+#         Name of the output pandas Series.
+#
+#     Returns
+#     -------
+#     s : `pd.Series`
+#         A pandas Series, optionally with name and index, optionally converted to output_unit.
+#
+#     Examples
+#     --------
+#     uu.nominal_values(pobj)
+#     uu.nominal_values(pobj, output_unit='m')
+#     uu.nominal_values(pobj, output_unit='m', index=df.index)
+#     uu.nominal_values(pobj, output_unit='m', index=df.index, name='x')
+#     """
+#     return to_series(pobj, output_unit=output_unit, k=0, index=index, name=name).astype(f'pint[{output_unit}]')
 
-    Returns
-    -------
-    s : `pd.Series`
-        A pandas Series, optionally with name and index, optionally converted to output_unit.
 
-    Examples
-    --------
-    uu.std_devs(pobj)
-    uu.std_devs(pobj, output_unit='m')
-    uu.std_devs(pobj, output_unit='m', index=df.index)
-    uu.std_devs(pobj, output_unit='m', index=df.index, name='x')
-    """
-    return to_series(pobj, output_unit=output_unit, direction='plus', k=1, n=0, index=index, name=name).astype(
-        f'pint[{output_unit}]')
+# def std_devs(pobj, output_unit=None, index=None, name=None):
+#     """
+#     Returns the uncertainty from a (vector) pint Quantity object and returns the uncertainty in a given unit.
+#
+#     Parameters
+#     ----------
+#     pobj : `pint Quantity`
+#     pobj
+#         Pint object to convert.
+#
+#     output_unit : `string`, optional
+#         Unit for the output conversion. If `None`, the output series will have the same unit as the input `pobj`.
+#         Must be valid unit that can be passed as units(output_unit)
+#
+#     index : `pd.Index`, optional
+#         pandas.Index that is attached to the output pandas Series.
+#
+#     name : `string`, optional
+#         Name of the output pandas Series.
+#
+#     Returns
+#     -------
+#     s : `pd.Series`
+#         A pandas Series, optionally with name and index, optionally converted to output_unit.
+#
+#     Examples
+#     --------
+#     uu.std_devs(pobj)
+#     uu.std_devs(pobj, output_unit='m')
+#     uu.std_devs(pobj, output_unit='m', index=df.index)
+#     uu.std_devs(pobj, output_unit='m', index=df.index, name='x')
+#     """
+#     return to_series(pobj, output_unit=output_unit, direction='plus', k=1, n=0, index=index, name=name).astype(
+#         f'pint[{output_unit}]')
 
 
 # def isna(pobj):
 #     """
 #     Returns boolean array where nominal value or standard deviation of a pint object is NaN.
 #
 #     Parameters
@@ -461,15 +461,15 @@
         raise ValueError(f'Input `q` must be within limits {min_limit:~} and {max_limit:~}, but is {q:~}')
     return q
 
 
 def parse_quantity(value: Union[dict, list, Q, pd.Series]) -> Q:
     if isinstance(value, Q) or value is None:
         return value
-    elif ('magnitude' and 'units' in value):
+    elif 'magnitude' and 'units' in value:
         return Q(value['magnitude'], value['units'])
     elif isinstance(value, pd.Series):
         return Q(value.astype('float64').to_numpy(), value.pint.units.__str__())
     elif isinstance(value, list):
         try:
             return Q(value[0], value[1])
         except (IndexError, TypeError):
```

## sunpeek/common/utils.py

```diff
@@ -1,19 +1,25 @@
-import enum
 import logging
 import os
+import enum
 import pathlib
 import sys
 import dotenv
-import pandas as pd
 import sqlalchemy.orm
+import sqlalchemy.event
+import sqlalchemy.exc
 from pydantic import BaseModel
 from logging.config import dictConfig
 
-from sunpeek.common.unit_uncertainty import to_s
+try:
+    import uvicorn
+    api_modules_available = True
+except ModuleNotFoundError:
+    # API dependecies are not installed, log only to standard output, no file.
+    api_modules_available = False
 
 dotenv.load_dotenv()
 
 ROOT_DIR = os.path.abspath(pathlib.Path(__file__).parent.parent)
 log_dir = os.path.join(ROOT_DIR, 'logs')
 log_fname = os.path.join(log_dir, 'server.log')
 
@@ -42,53 +48,64 @@
     Notes
     -----
     Modified code snipped originally by "Yash Nag" taken from:
     https://stackoverflow.com/questions/63510041/adding-python-logging-to-fastapi-endpoints-hosted-on-docker-doesnt-display-api
 
     """
 
-    # LOGGER_NAME: str = "hit_logger"
+    # LOGGER_NAME: str = "sp_logger"
     FILE_LOG_FORMAT: str = "|%(asctime)s| [%(levelname)s -> %(module)s] : %(message)s"
     STD_OUT_LOG_FORMAT: str = "%(levelprefix)s |%(asctime)s| %(message)s"
     LOG_LEVEL: str = "DEBUG"
 
     # Create log directory if it does not exists
     if not os.path.exists(log_dir):
         os.makedirs(log_dir)
 
     # Logging config
     version = 1
     disable_existing_loggers = False
-    formatters = {
-        "std_out": {
-            "()": "uvicorn.logging.DefaultFormatter",
-            "fmt": STD_OUT_LOG_FORMAT,
-            "datefmt": "%Y-%m-%d %H:%M:%S",
-        },
-        "file_out": {
-            "format": FILE_LOG_FORMAT,
-            "datefmt": "%Y-%m-%d %H:%M:%S",
+
+    if api_modules_available:
+        formatters = {
+            "std_out": {
+                "()": "uvicorn.logging.DefaultFormatter",
+                "fmt": STD_OUT_LOG_FORMAT,
+                "datefmt": "%Y-%m-%d %H:%M:%S",
+            },
+            "file_out": {
+                "format": FILE_LOG_FORMAT,
+                "datefmt": "%Y-%m-%d %H:%M:%S",
+            }
+        }
+    else:
+        formatters = {
+            "std_out": {
+                "fmt": STD_OUT_LOG_FORMAT,
+                "datefmt": "%Y-%m-%d %H:%M:%S",
+            },
         }
-    }
+
     handlers = {
         "default": {
             "formatter": "std_out",
             "class": "logging.StreamHandler",
             "stream": "ext://sys.stderr",
-        },
-        "file": {
+        }}
+
+    loggers = {"sp_logger": {"handlers": ["default"], "level": LOG_LEVEL},}
+    if api_modules_available:
+        handlers["file"] = \
+            {
             "formatter": "file_out",
             "class": "logging.FileHandler",
             "level": "WARNING",
             "filename": log_fname
-        }
-    }
-    loggers = {
-        "hit_logger": {"handlers": ["default", "file"], "level": LOG_LEVEL},
-    }
+            }
+        loggers = {"sp_logger": {"handlers": ["default", "file"], "level": LOG_LEVEL},}
 
 
 def get_env(name):
     try:
         value = os.environ[name]
     except KeyError:
         raise MissingEnvVar(name)
@@ -97,94 +114,62 @@
 
 def get_db_conection_string():
     db_type = os.environ.get('HIT_DB_TYPE', 'postgresql')
     host = os.environ.get('HIT_DB_HOST', 'localhost:5432')
     user = os.environ.get('HIT_DB_USER')
     pw = os.environ.get('HIT_DB_PW')
     db_name = os.environ.get('HIT_DB_NAME', 'harvestit')
-    dialects = {'postgresql': 'postgresql+psycopg2'}
+    dialects = {'postgresql': 'postgresql+psycopg2', 'sqlite': 'sqlite'}
 
     db_str = '{}://'.format(dialects[db_type])
-    if user is not None:
+    if user is not None and db_type != 'sqlite':
         db_str = db_str + user
-    if pw is not None:
+    if pw is not None and db_type != 'sqlite':
         db_str = db_str + ':{}@'.format(pw)
-    db_str = db_str + '{}/{}'.format(host.strip('/'), db_name)
+    db_str = '{}{}'.format(db_str, host)
+    if db_type != 'sqlite':
+        db_str = '{}/{}'.format(db_str, db_name)
     return db_str
 
 
-def to_rd(*args):
-    """Converts numeric inputs to pd.Series with pint dtype W/m².
-    Useful to return radiation converter results.
-    """
-    out = *(None if elem is None else to_s(elem, unit_str='W m**-2') for elem in args),
-    out = out[0] if len(out) == 1 else out
-    return out
-
-
-def validate_timezone(idx: pd.DatetimeIndex, timezone) -> pd.DatetimeIndex:
-    """Validates timezone information, trying to match DataFrame timezone and timezone string.
-
-    Parameters
-    ----------
-    idx : pd.DatetimeIndex
-    timezone : timezone (str or pytz.timezone), examples: 'Europe/Berlin' or 'UTC' or pytz.FixedOffset(60)
-
-    Returns
-    -------
-    idx : pd.DatetimeIndex, timezone-aware index
-
-    Raises
-    ------
-    ValueError
+S = None
+db_engine = None
 
-    Notes
-    -----
-    Here is how all combinations are handled:
-    1. No timezone in df, but timezone string given: ok
-    2. Timezone in df, and no timezone string given: ok
-    3. No timezone in df, and no timezone string given: error (timezone info is missing)
-    4. Timezone both in df and as timezone string: error (because it's hard to check compatibility between a
-    dynamically-offset string-based timezone like 'Europe/Vienna' with a FixedOffset timezone info that is the
-    result of parsing timezone-aware timestamps).
-    See also: https://pvlib-python.readthedocs.io/en/v0.3.0/timetimezones.html
-    """
-
-    hit_logger.info("[validate_timezone] Started. Checking for timezone consistency...")
-
-    assert isinstance(idx, pd.DatetimeIndex), \
-        'Input index expected to be a pandas DatetimeIndex.'
-    tz_idx_none = idx.tzinfo is None
-
-    if (timezone is None) and tz_idx_none:
-        # No timezone information available at all -> error
-        raise ValueError(
-            'No timezone information found: Timezone string is None, '
-            'and no timezone information was found in the provided pandas index.')
-
-    if (timezone is not None) and not tz_idx_none:
-        # Both timezone informations available -> error (see docstring)
-        raise ValueError(
-            'Ambiguous timezone information found: A timezone string (resulting in a dynamic offset) is given, '
-            'and timezone information is also given in the pandas index (fixed offset).'
-            'These two pieces of timezone information are incompatible. Use only one of them, string or pandas index.')
-
-    if tz_idx_none:
-        idx = idx.tz_localize(timezone, ambiguous='NaT', nonexistent='NaT')
 
-    return idx
+def create_db_engine():
+    global S
+    global db_engine
+    try:
+        if os.environ.get('HIT_DB_TYPE', 'postgresql') == 'sqlite':
+            db_engine = sqlalchemy.create_engine(get_db_conection_string(), pool_pre_ping=True,
+                                                 connect_args={'timeout': 15, 'check_same_thread': False})
+        else:
+            db_engine = sqlalchemy.create_engine(get_db_conection_string(), pool_pre_ping=True)
+        S = sqlalchemy.orm.sessionmaker(db_engine)
+    except (ModuleNotFoundError, sqlalchemy.exc.ArgumentError):
+        db_engine = None
+        S = None
+
+
+# @sqlalchemy.event.listens_for(db_engine, "connect")
+# def connect(dbapi_connection, connection_record):
+#     cursor = dbapi_connection.cursor()
+#     cursor.execute(f"SET TIME ZONE utc;")
+#     cursor.close()
 
-try:
-    db_engine = sqlalchemy.create_engine(get_db_conection_string(), pool_pre_ping=True)
-    S = sqlalchemy.orm.sessionmaker(db_engine)
-except ModuleNotFoundError:
-    db_engine = None
-    S = None
 
 # logger
 dictConfig(LogConfig().dict())
-hit_logger = logging.getLogger("hit_logger")
+sp_logger = logging.getLogger("sp_logger")
+create_db_engine()
 
 
 class VerifyValidateMode(str, enum.Enum):
     validate = 'validate'
     verify = 'verify'
+
+
+class DatetimeTemplates(enum.Enum):
+    year_month_day = "year_month_day"
+    day_month_year = "day_month_year"
+    month_day_year = "month_day_year"
+
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## sunpeek/components/__init__.py

```diff
@@ -1,16 +1,17 @@
 from sunpeek.components import helpers
 from sunpeek.components.base import Component
 from sunpeek.components.components_factories import CollectorTypeQDT, CollectorTypeSST
-from sunpeek.components.fluids import Fluid, FluidDefinition, WPDFluid, CoolPropFluid, WPDFluidDefinition, \
-    CoolPropFluidDefinition, FluidFactory
-from sunpeek.components.fluid_helpers import ModelFactory
-from sunpeek.components.helpers import make_tables, SensorMap
+from sunpeek.components.fluids import Fluid, WPDFluid, CoolPropFluid, FluidFactory, \
+    FluidDefinition, CoolPropFluidDefinition, WPDFluidDefinition
+from sunpeek.components.fluids_wpd_models import ModelFactory
 from sunpeek.components.iam_methods import IAM_K50, IAM_ASHRAE, IAM_Interpolated, IAM_Ambrosetti
-from sunpeek.components.jobs import Job
 from sunpeek.components.operational_events import OperationalEvent
 from sunpeek.components.physical import Plant, Array, HeatExchanger
-from sunpeek.components.results import PCMethodOutput, PCMethodOutputArray
+from sunpeek.components.results import PCMethodOutput, PCMethodOutputPlant, PCMethodOutputArray
 from sunpeek.components.sensor import Sensor, SensorInfo
 from sunpeek.components.types import SensorType, CollectorType
 
+from sunpeek.components.jobs import Job
+from sunpeek.components.helpers import make_tables, SensorMap
+
 helpers.AttrSetterMixin.define_component_attrs()
```

## sunpeek/components/base.py

```diff
@@ -1,230 +1,264 @@
-import uuid
-from sqlalchemy.ext.associationproxy import association_proxy
-from typing import Union, Dict
+
+import warnings
+from typing import Union, Dict, Optional
+import enum
 import dataclasses
+from sqlalchemy.ext.associationproxy import association_proxy
+from sqlalchemy.orm import relationship, declared_attr
+from sqlalchemy import Column, Integer, Identity, String
+from sqlalchemy.orm.collections import attribute_mapped_collection
+
 from sunpeek.common.errors import ConfigurationError
 from sunpeek.common.unit_uncertainty import Q
-from sunpeek.common.utils import VerifyValidateMode
 from sunpeek.components import types
-from sunpeek.components.helpers import IsVirtual, AttrSetterMixin, SensorMap
+from sunpeek.components.helpers import IsVirtual, AttrSetterMixin, SensorMap, ORMBase
 from sunpeek.components.sensor import Sensor
 
 
+class AlgoCheckMode(str, enum.Enum):
+    config_only = 'config_only'
+    config_and_data = 'config_and_data'
+
+
 @dataclasses.dataclass
-class SensorSlot():
+class SensorSlot:
     """
     A pydantic class used to hold and validate information on a component sensor slot.
     
     Parameters
     ----------
     name : str
-        The name of the slot, which beahvaes like a component attribute and can be used to access the mapped sensor from 
+        The name of the slot, which behaves like a component attribute and can be used to access the mapped sensor from
         the component. e.g. te_amb. `name` only needs to be unique and understandable in the context of a specific
         component, e.g. the `tp` slot of a plant includes the total power of all arrays, whereas `tp` of an array is
         just that array's power.
     descriptive_name : str
         A longer more descriptive name, e.g. for display to a user in a front end client. Limited to 24 characters
     description : str
         A description of the purpose and use of the slot.
     virtual : enum
         Whether the sensor for a slot is always virtual, can be virtual given certain conditions, or is never virtual
     """
 
     name: str
     sensor_type: types.SensorType
-    descriptive_name: Union[str, None] = None
+    descriptive_name: Union[str] = None
     virtual: IsVirtual = IsVirtual.never
-    description: Union[str, None] = None
-    #
-    # def __init__(self,
-    #              name: str,
-    #              sensor_type: str,
-    #              descriptive_name: str,
-    #              virtual: Union[IsVirtual, str],
-    #              description: str = None):
-    #     super().__init__(name=name, sensor_type=sensor_type, descriptive_name=descriptive_name, virtual=virtual,
-    #                      description=description)
+    description: Union[str] = None
+    # Idea: Implement SensorSlot availability, also see ComponentParam.available
+    # available: Optional[bool] = None
+
 
+class Component(ORMBase, AttrSetterMixin):
+    """Base class to be used for physical components of a Plant, also specifies a DB table to allow polymorpic
+    references to any subclass (i.e. via FK on components.id)"""
 
-class Component(AttrSetterMixin):
-    """Abstract Class to be used for physical components of a Plant"""
+    __tablename__ = 'components'
+
+    component_id = Column(Integer, Identity(), primary_key=True)
 
     sensor_slots: Dict[str, SensorSlot] = {}
     sensors = association_proxy("_sensor_map", "sensor")
+    component_type = Column(String)
+    __mapper_args__ = {
+        "polymorphic_identity": "component",
+        "polymorphic_on": component_type,
+    }
+
+    @declared_attr
+    def _sensor_map(self):
+        return relationship("SensorMap",
+                            collection_class=attribute_mapped_collection("slot_name"),
+                            cascade="all, delete-orphan")
+
+    @property
+    def sensor_map(self):
+        return self._sensor_map
+
+    @sensor_map.setter
+    def sensor_map(self, str_map):
+        if isinstance(str_map, dict):
+            if not str_map:  # Nothing to do, avoid unnecessary call to plant.config_virtuals()
+                return
+            self.defer_post_config_changed_actions = True
+            for slot_name, sensor in str_map.items():
+                sensor = self.get_raw_sensor(sensor, raise_if_not_found=True)
+                self.map_sensor(sensor=sensor, slot_name=slot_name)
+                # elif sensor is None and slot_name in self.sensor_map:
+                #     del self.sensor_map[slot_name]
+
+            self.defer_post_config_changed_actions = False
+            if self.plant is not None:
+                [func(self.plant) for func in self.plant.post_config_changed_callbacks]
+
+        else:
+            raise ConfigurationError(f"sensor_map must be in the form {'slot_name:sensor_raw_name'}, got {str_map}.")
 
     def __setattr__(self, key, value):
         if key in self.sensor_slots:
             return self.map_sensor(value, key)
         return super().__setattr__(key, value)
 
+    def update_sensors(self, is_remove):
+        if is_remove:
+            # Not doing in for loop because of "RuntimeError: dictionary changed size during iteration"
+            vsensors = [s for s in self.sensors.values() if s.is_virtual]
+            for sensor in vsensors:
+                sensor.remove_references()
+        else:
+            for sensor in self.sensors.values():
+                sensor.plant = self.plant
+
+        return self
+
     def set_sensors(self, **kwargs):
-        self.defer_configure_virtuals = True
+        """Maps one or multiple sensors (by calling `map_sensor()`) and handles configuring virtual sensors.
+        """
+        self.defer_post_config_changed_actions = True
         for slot_name, sensor in kwargs.items():
             self.map_sensor(sensor, slot_name)
-        self.defer_configure_virtuals = False
+        self.defer_post_config_changed_actions = False
         if self.plant is not None:
-            self.plant.config_virtuals()
+            [func(self.plant) for func in self.plant.post_config_changed_callbacks]
 
     def map_sensor(self, sensor: Sensor, slot_name: str):
         """Maps sensor to slot_name of given component, including some sanity checks.
         """
         real_slots = [slot.name for slot in self.get_real_slots()]
         if sensor is not None and slot_name in real_slots:
-            SensorMap(slot_name, sensor, component=self,
-                      sensor_type=self.sensor_slots[slot_name].sensor_type)
+            remove_old = False
+            if self._sensor_map.get(slot_name) is not None:
+                # If there is a mapping to the slot already, we need to explicitly unmap it before remapping, otherwise
+                # we get 2 SensorMap objects referring to the same slot/component, the redundant one would be cleaned up
+                # but triggers `_unique_mapping_per_component_slot` first.
+                old_s = self.sensors[slot_name]
+                self._sensor_map[slot_name].unmap(include_sensor=True)
+                if old_s.is_virtual:
+                    # If mapping real sensor to a slot that was previously calculated: Remove virtual sensor
+                    remove_old = True
+
+            self._sensor_map[slot_name] = SensorMap(slot_name, sensor, component=self,
+                                                    sensor_type=self.sensor_slots[slot_name].sensor_type)
+            if remove_old:
+                # self.plant.raw_sensors.pop(self.plant.raw_sensors.index(old_s))
+                old_s.remove_references()
+
         elif (not self.sensors[slot_name].is_virtual if self.sensors.get(slot_name) is not None else False):
             # If slot is not empty and sensor currently in slot is not virtual
-            # TODO: Maybe replace this using association_proxy, see #288
-            # if slot_name in self.sensors:
-            del self.sensors[slot_name]._mappings[self.sensors[slot_name]._mappings.index(self.sensor_map[slot_name])]
-            del self.sensor_map[slot_name]
+            self.sensor_map[slot_name].unmap()
+        elif self.sensors[slot_name].is_virtual:
+            warnings.warn('You cannot set a virtual sensor directly. Virtual sensors are calculated automatically.')
 
-        if not self.defer_configure_virtuals and self.plant is not None:
-            self.plant.config_virtuals()
         return
 
-    def map_vsensor(self, slot_name: str, can_calculate: bool = True):
-        """Create virtual Sensor and map it to component.slot_name, or map None if can_calculate is not met."""
+    def map_vsensor(self, slot_name: str, problems: 'sunpeek.serializable_models.ProblemReport'):
+        """Create virtual Sensor and map it to component.slot_name, or map None if it cannot be calculated.
+
+        Parameters
+        ----------
+        slot_name : str, slot / channel name of the component self to which the virtual sensor will be mapped.
+        problems : ProblemReport, problems reported at config time, prior to vsensor calculation.
+        """
         if not self.has_virtual_slot_named(slot_name):
             raise ConfigurationError(f'Cannot map virtual sensor because slot {slot_name} of {self} '
                                      f'does not accept virtual sensors.')
+        # print(f'map_vsensor: component={self}, slot_name={slot_name}')
         try:
             sensor = self.sensors[slot_name]
         except KeyError:
             sensor = None
-        # Sensor already mapped? Update only
-        if sensor is not None and not sensor.is_virtual:
-            return  # Do not overwrite existing real sensor
-        elif sensor is not None:
-            sensor.can_calculate = can_calculate
-            # TODO could return reason _why_ this vsensor cannot be calculated, e.g. for WebUI
+
+        can_calculate = problems.success and (slot_name not in problems.problem_slots)
+
+        # Sensor already mapped? Update only, don't create new Sensor
+        if sensor is not None:
+            if sensor.is_virtual:
+                sensor.problems = problems
+                sensor.can_calculate = can_calculate
+            # Not virtual? Do nothing / Do not overwrite existing real sensor
             return
 
+        # Create new sensor
         vsensor_name = f"{slot_name}__virtual__{self.__class__.__name__}_{self.name}".replace(' ', '_').lower()
-        if self.plant.get_raw_sensor(vsensor_name) is not None if self.plant is not None else False:
-            # Plant is not None and vsensor with matching name already exists
-            vsensor = self.plant.get_raw_sensor(vsensor_name)
-            vsensor.can_calculate = can_calculate
+        if (self.plant is not None) and (self.plant.get_raw_sensor(vsensor_name) is not None):
+            # vsensor with matching name already exists in Plant
+            sensor = self.plant.get_raw_sensor(vsensor_name)
+            sensor.problems = problems
+            sensor.can_calculate = can_calculate
         else:
             # Create virtual sensor
-            # Needs to store compatible_unit of sensor_type, so it can later check if vsensor calc results are ok.
-            vsensor = Sensor(is_virtual=True,
-                             can_calculate=can_calculate,
-                             plant=self.plant,
-                             raw_name=vsensor_name,
-                             # a huge number of tests fail if vsensor doesn't know its compatible unit
-                             native_unit=self.sensor_slots[slot_name].sensor_type.compatible_unit_str
-                             # native_unit=get_sensor_type(self._get_type_name(slot_name)).compatible_unit_str,
-                             )
+            # Needs to store compatible_unit of sensor_type, so it can later check if vsensor calc result units are ok.
+            sensor = Sensor(is_virtual=True,
+                            plant=self.plant,
+                            raw_name=vsensor_name,
+                            problems=problems,
+                            can_calculate=can_calculate,
+                            native_unit=self.sensor_slots[slot_name].sensor_type.compatible_unit_str
+                            )
 
-        SensorMap(slot_name, vsensor, component=self, sensor_type=self.sensor_slots[slot_name].sensor_type)
+        SensorMap(slot_name, sensor, component=self, sensor_type=self.sensor_slots[slot_name].sensor_type)
 
     def has_virtual_slot_named(self, slot_name):
         """Assert component has a (possibly or always) virtual sensor slot named slot_name.
         """
         vnames = [slot.name for slot in self.sensor_slots.values() if slot.virtual != IsVirtual.never]
         return slot_name in vnames
 
     @classmethod
     def get_real_slots(cls):
         """Get component's slot names for (possibly or always) real (not virtual) sensors
         """
         return [slot for slot in cls.sensor_slots.values() if slot.virtual != IsVirtual.always]
 
-    def assert_verify_validate(self, check_mode: str, *attribs: str):
-        """Calls verify_validate, raises AssertionError if verify / validate failed.
+    def is_slot_missing(self, slot_name: str, check_mode) -> bool:
+        """Return True if component slot has no sensor mapped or sensor is not ready for calculations.
         """
-        response = self.verify_validate(check_mode, *attribs)
-        assert response[0], response[1]
-
-    def verify_validate(self, check_mode: str, *attribs: str):
-        """Return True if component attributes named `attribs` are wither ComponentParam / Quantity or
-        - if check_mode=='configured': is a virtual Sensor and .can_calculate
-        - if check_mode=='calculated': is a virtual Sensor and .validate_data
-
-        Parameters
-        ----------
-        check_mode : 'configured' or 'calculated'
-        attribs : str, keys of self.sensor_slots or ComponentParam attributes
-
-        Returns
-        -------
-        tuple
-            bool: 1 bool value, True only if ok for all attribs.
-            list: list of sensor_slots which broke the conditions.
-        """
-        # assert check_mode in ['configured', 'calculated'], f'Unknown "check_mode" parameter: {check_mode}.'
-        assert check_mode.lower() in [el.name for el in VerifyValidateMode], \
-            f'Unknown "check_mode" parameter: {check_mode}.'
-        if check_mode == VerifyValidateMode.validate:
-            assert len(self.plant.time_index) > 0, 'No data found for plant, "plant.time_index" is empty.'
-
-        problem_slots = []
-        for attrib in attribs:
-            try:
-                sensor_or_componentparam = getattr(self, attrib)
-            except AttributeError:
-                problem_slots.append(attrib)
-                continue
-            # Sensor
-            if attrib in self.sensor_slots:
-                if sensor_or_componentparam is None:
-                    problem_slots.append(attrib)
-                    continue
-                assert isinstance(sensor_or_componentparam, Sensor)
-                s = sensor_or_componentparam
-                if s.is_virtual:
-                    if (check_mode == VerifyValidateMode.verify) and (not s.can_calculate):
-                        problem_slots.append(attrib)
-                    elif (check_mode == VerifyValidateMode.validate) and s.data.notna().sum() == 0:
-                        problem_slots.append(attrib)
-            # ComponentParam
-            elif isinstance(sensor_or_componentparam, Q):
-                if sensor_or_componentparam is None:
-                    problem_slots.append(attrib)
-            # all others allow gracefully
-            else:
-                problem_slots.append(attrib)
-        return (len(problem_slots) == 0), problem_slots
-
-    # def can_calculate(self, *attribs: str):
-    #     """Return True if all component attributes are
-    #     - valid real Sensors or virtual Sensors with .can_calculate==True
-    #     - or ComponentParams
-    #     """
-    #     all_ok, problem_slots = self.verify_validate(check_mode='configured', *attribs)
-    #     return all_ok
-    #
-    # def validate_data(self, *attribs: str):
-    #     """Return True if all attribs are valid real Sensors or virtual Sensors with .validate_data==True"""
-    #     all_ok, problem_slots = self.verify_validate(check_mode='calculated', *attribs)
-    #     return all_ok
-
-    @property
-    def sensor_map(self):
-        return self._sensor_map
+        # May raise AttributeError
+        sensor = getattr(self, slot_name)
+        if sensor is None:
+            return True
+        if isinstance(sensor, Q):
+            raise TypeError(f'In {self.name}, {self.__class__.__name__}.{slot_name} exists, '
+                            f'but is a ComponentParam, not a sensor. Check the calling code.')
+        if sensor.is_virtual:
+            if check_mode == AlgoCheckMode.config_only:
+                is_slot_ok = sensor.can_calculate
+                return not is_slot_ok
+            elif check_mode == AlgoCheckMode.config_and_data:
+                is_slot_ok = sensor.data.notna().sum() > 0
+                return not is_slot_ok
+        return False
 
-    @sensor_map.setter
-    def sensor_map(self, str_map):
-        if isinstance(str_map, dict):
-            if not str_map:  # Nothing to do, avoid unnecessary call to plant.config_virtuals()
-                return
-            self.defer_configure_virtuals = True
-            for slot_name, sensor in str_map.items():
-                sensor = self.get_raw_sensor(sensor, raise_if_not_found=True)
-                self.map_sensor(sensor=sensor, slot_name=slot_name)
-                # elif sensor is None and slot_name in self.sensor_map:
-                #     del self.sensor_map[slot_name]
+    def is_real_slot_missing(self, slot_name: str, check_mode) -> bool:
+        """Like is_slot_missing, but additionally checks if sensor in named slot is real (not virtual).
+        """
+        sensor = getattr(self, slot_name)
+        if sensor is None:
+            return True
+        if isinstance(sensor, Q):
+            raise TypeError(f'In {self.name}, {self.__class__.__name__}.{slot_name} exists, '
+                            f'but is a ComponentParam, not a sensor. Check the calling code.')
+        if sensor.is_virtual:
+            return True
+        return False
 
-            self.defer_configure_virtuals = False
-            if self.plant is not None:
-                self.plant.config_virtuals()
-        else:
-            raise ConfigurationError(f"sensor_map must be in the form {'slot_name:sensor_raw_name'}, got {str_map}.")
+    def is_attrib_missing(self, attrib_name) -> bool:
+        """Return True if component attribute is None or not a ComponentParam holding a Quantity.
+        """
+        # May raise AttributeError
+        attrib = getattr(self, attrib_name)
+        if attrib is None:
+            return True
+        if isinstance(attrib, Sensor):
+            raise TypeError(f'In {self.name}, {self.__class__.__name__}.{attrib_name} exists, '
+                            f'but is a sensor, not a ComponentParam. Check the calling code.')
+        if not isinstance(attrib, Q):
+            return True
+        return False
 
     def get_raw_sensor(self, str_map, raise_if_not_found=False):
         if str_map is None:
             return None
         return self.plant.get_raw_sensor(str_map, raise_if_not_found)
 
     # 2022-10-11 Currenly this method is not in use. If re-activated, also uncomment the tests in get_display_name
```

## sunpeek/components/components_factories.py

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from datetime import datetime
 from sunpeek.common.unit_uncertainty import Q
+from pint import Quantity
 from sunpeek.components.types import CollectorType
-from sunpeek.components.iam_methods import _IAM_Method
+from sunpeek.components.iam_methods import IAM_Method
 
 
 class CollectorTypeSST:
     def __new__(cls, eta0hem: Q, a1: Q, a2: Q, ceff: Q, test_reference_area: Q, gross_length: Q,
-                iam_method: _IAM_Method, kd=None,
+                iam_method: IAM_Method, kd=None,
                 name: str = None, manufacturer_name: str = None, product_name: str = None, licence_number: str = None,
                 area_gr: Q = None, area_ap: Q = None, gross_width: Q = None, gross_height: Q = None,
                 description: str = None, certificate_date_issued: datetime = None, certificate_lab: str = None,
                 certificate_details: str = None, test_report_id: str = None, f_prime: Q = None
                 ):
         test_type = "SST"
         a5 = ceff
@@ -22,16 +23,16 @@
             test_report_id=test_report_id, licence_number=licence_number,
             certificate_date_issued=certificate_date_issued, certificate_lab=certificate_lab,
             certificate_details=certificate_details, area_gr=area_gr, area_ap=area_ap, gross_width=gross_width,
             gross_height=gross_height, a1=a1, a2=a2, a5=a5, kd=kd, eta0hem=eta0hem, iam_method=iam_method, f_prime=f_prime)
 
 
 class CollectorTypeQDT:
-    def __new__(cls, eta0b: Q, a1: Q, a2: Q, a5: Q, kd: Q, test_reference_area: str, gross_length: Q,
-                iam_method: _IAM_Method,
+    def __new__(cls, eta0b: Quantity, a1: Quantity, a2: Q, a5: Q, kd: Q, test_reference_area: str, gross_length: Q,
+                iam_method: IAM_Method,
                 name: str = None, manufacturer_name: str = None, product_name: str = None, licence_number: str = None,
                 area_gr: Q = None, area_ap: Q = None, gross_width: Q = None, gross_height: Q = None,
                 description: str = None, certificate_date_issued: datetime = None, certificate_lab: str = None,
                 certificate_details: str = None, test_report_id: str = None, f_prime: Q = None
                 ):
         test_type = "QDT"
         return CollectorType(
```

## sunpeek/components/fluids.py

```diff
@@ -1,8 +1,10 @@
 """
+Caveat: This docstring is outdated.
+
 Summary
 -------
 This module implements fluids and fluid properties for HarvestIT.
 
 Extended Summary
 ----------------
 A typical calculation involving fluid properties is getting thermal
@@ -45,16 +47,16 @@
 WPD fluids
 ----------
 
 This module supports
 
 - reading & interpolating csv data created with WebPlotDigitizer.
 - training sklearn models for interpolation / fitting, and visual checks of fit quality.
-- exporting the trained models as ONNX files (to be stored in database).
-- calculating fluid properties by using prediction based on ONNX model.
+# - exporting the trained models as ONNX files (to be stored in database).
+# - calculating fluid properties by using prediction based on ONNX model.
 - building WPDFluid instances from these ONNX files.
 
 Here is a step-by-step guide on how to add a fluid to HarvestIT for which only graphical information about fluid
 properties is given (see #73).
 An example is the FHW plant. Example workflows can be found under `tests/tests_fluids`.
 
 To enable property calculation for WPD fluids, follow this process:
@@ -117,42 +119,56 @@
     http://www.coolprop.org/fluid_properties/Incompressibles.html#id181
 .. _IAPWS-95:
     http://www.iapws.org/relguide/IAPWS-95.html
 
 """
 
 import numpy as np
+import pandas as pd
 import re
-import hashlib
 import warnings
 import sqlalchemy
 import CoolProp.CoolProp as Cp
-from sqlalchemy import Column, String, Integer, ForeignKey, Float, Boolean, Enum, LargeBinary, Identity, or_, \
-    CheckConstraint
+from sqlalchemy import Column, String, Integer, ForeignKey, Float, Boolean, Enum, Identity, or_, \
+    CheckConstraint, JSON, func
 from sqlalchemy.orm import relationship, declared_attr
 import sqlalchemy.event
+from typing import Union
 
 from sunpeek.common.unit_uncertainty import Q
-from sunpeek.common.utils import hit_logger
+from sunpeek.common.utils import sp_logger
 from sunpeek.common.errors import ConfigurationError
 import sunpeek.common.unit_uncertainty as uu
 from sunpeek.components.helpers import ORMBase, AttrSetterMixin
-from sunpeek.components.fluid_helpers import WPDModel, WPDModelPure, WPDModelMixed, ModelFactory
+from sunpeek.components.fluids_wpd_models import WPDModel, WPDModelPure, ModelFactory
+from sunpeek.definitions import FluidProps
 
 
 class FluidDefinition(ORMBase, AttrSetterMixin):
+    """Fluid with all information to store in database.
+
+    Attributes
+    ----------
+    name : str
+        Fluid name / Product name. Must be unique within SunPeek. Example: "Thermum P"
+    manufacturer : str
+        Manufacturer name. Example: "Thermum GmbH & Co. KG"
+    """
     __tablename__ = 'fluid_definitions'
 
     id = Column(Integer, Identity(0), primary_key=True)
     model_type = Column(Enum('CoolProp', 'WPD', name='fluid_definition_type'))
     name = Column(String, nullable=False, unique=True)
     manufacturer = Column(String)
     description = Column(String)
     is_pure = Column(Boolean)
 
+    _density_data = Column(JSON)
+    _heat_capacity_data = Column(JSON)
+
     __mapper_args__ = {
         'polymorphic_identity': 'fluid_def',
         'polymorphic_on': model_type,
         'with_polymorphic': '*'
     }
 
     def __init__(self, fluid_string=None, **kwargs):
@@ -190,37 +206,53 @@
         Raises
         ------
         ValueError
             If no or more than one fluid is found.
 
         """
         if fluid_string.lower() == 'water':
-            fluid = session.query(cls).filter(
-                cls.description.regexp_replace('[^A-Za-z0-9]', '', 'g').match('heoswater')).one()
+            fluid = session.query(cls).filter(cls.name == 'water').one()
             return fluid
         if fluid_string.isupper() and len(fluid_string) <= 8:
             try:
                 search_string = fluid_string.lower()
-                fluid = session.query(cls).filter(cls.name.match(search_string)).one()
+                fluid = session.query(cls).filter(cls.name == search_string).one()
                 return fluid
             except (sqlalchemy.exc.NoResultFound, sqlalchemy.exc.MultipleResultsFound):
                 pass
         try:
-            search_string = re.sub('[\W_]+', '', fluid_string)
+            # search_string = re.sub('[\W_]+', '', fluid_string)
+            search_string = fluid_string.replace(' ', '')
             fluid = session.query(cls).filter(or_(
-                cls.name.match(fluid_string.replace(' ', '')),
-                cls.description.regexp_replace('[^A-Za-z0-9]', '', 'g').ilike('%{}%'.format(search_string))
+                func.replace(func.lower(cls.name), ' ', '').ilike('%{}%'.format(search_string.lower())),
+                func.replace(func.lower(cls.description), ' ', '').ilike('%{}%'.format(search_string.lower()))
             )).one()
         except sqlalchemy.exc.NoResultFound:
             raise ConfigurationError(f'No entry found for {fluid_string}')
         except sqlalchemy.exc.MultipleResultsFound:
             raise ConfigurationError(f'{fluid_string} is not unique, more than 1 result found.')
 
         return fluid
 
+    @property
+    def density_data(self):
+        return pd.read_json(self._density_data)
+
+    @density_data.setter
+    def density_data(self, val):
+        self._density_data = val.to_json()
+
+    @property
+    def heat_capacity_data(self):
+        return pd.read_json(self._heat_capacity_data)
+
+    @heat_capacity_data.setter
+    def heat_capacity_data(self, val):
+        self._heat_capacity_data = val.to_json()
+
 
 class CoolPropFluidDefinition(FluidDefinition):
     __mapper_args__ = {
         'polymorphic_identity': 'CoolProp',
     }
 
 
@@ -244,150 +276,146 @@
     ```
     """
 
     __mapper_args__ = {
         'polymorphic_identity': 'WPD',
     }
 
-    heat_capacity_onnx = Column(LargeBinary)
-    density_onnx = Column(LargeBinary)
     dm_model_sha1 = Column(String)
     hc_model_sha1 = Column(String)
     heat_capacity_unit_te = Column(String)
     heat_capacity_unit_out = Column(String)
     heat_capacity_unit_c = Column(String)
     density_unit_te = Column(String)
     density_unit_out = Column(String)
     density_unit_c = Column(String)
 
     FluidDefinition.__table_args__ = (
         sqlalchemy.UniqueConstraint('dm_model_sha1', 'hc_model_sha1'),  # Constriant for WPDFluids
     )
 
-    def __init__(self, name, density_model, heat_capacity_model, manufacturer=None, description=None):
-        assert isinstance(density_model, WPDModel) and isinstance(heat_capacity_model, WPDModel), \
-            "Models must be instances of WPDModel"
+    @classmethod
+    def from_fluid_info(cls, fluid_info: 'sunpeek.definitions.fluid_definitions.WPDFluidInfo'):
+        rho_model = ModelFactory.from_info_and_property(fluid_info, FluidProps.density)
+        cp_model = ModelFactory.from_info_and_property(fluid_info, FluidProps.heat_capacity)
+
+        return WPDFluidDefinition(fluid_info.name,
+                                  density_model=rho_model,
+                                  heat_capacity_model=cp_model,
+                                  manufacturer=fluid_info.manufacturer,
+                                  description=fluid_info.description)
+
+    def __init__(self, name: str, density_model: WPDModel, heat_capacity_model: WPDModel,
+                 manufacturer=None, description=None):
         assert density_model.__class__.__name__ == heat_capacity_model.__class__.__name__, \
-            "density_model and heat_capacity_model must be of same type (pure or mixed)"
+            'Inputs "density_model" and "heat_capacity_model" must be of same type (pure or mixed WPD models).'
 
         self.name = name
         self.manufacturer = manufacturer
         self.description = description
 
         self.density_model = density_model
+        self.density_data = density_model.df
+
         self.heat_capacity_model = heat_capacity_model
-        self.heat_capacity_onnx = heat_capacity_model.onnx_model
-        self.density_onnx = density_model.onnx_model
+        self.heat_capacity_data = heat_capacity_model.df
 
         self.heat_capacity_unit_te = self.heat_capacity_model.unit['te']
         self.heat_capacity_unit_out = self.heat_capacity_model.unit['out']
         self.heat_capacity_unit_c = self.heat_capacity_model.unit.get('c')
         self.density_unit_te = self.density_model.unit['te']
         self.density_unit_out = self.density_model.unit['out']
         self.density_unit_c = self.density_model.unit.get('c')
 
-        self.dm_model_sha1 = hashlib.sha1(self.density_onnx.__repr__().encode()).hexdigest()
-        self.hc_model_sha1 = hashlib.sha1(self.heat_capacity_onnx.__repr__().encode()).hexdigest()
-
-        if isinstance(density_model, WPDModelPure):
-            self.is_pure = True
-        elif isinstance(density_model, WPDModelMixed):
-            self.is_pure = False
+        self.is_pure = isinstance(density_model, WPDModelPure)
 
     @sqlalchemy.orm.reconstructor
     def _init_on_load(self):
-        units_hc = {'te': self.heat_capacity_unit_te, 'out': self.heat_capacity_unit_out,
-                    'c': self.heat_capacity_unit_c}
-        units_d = {'te': self.density_unit_te, 'out': self.density_unit_out, 'c': self.density_unit_c}
-        self.heat_capacity_model = ModelFactory(units_hc, onnx_model_bytes=self.heat_capacity_onnx,
-                                                is_pure=self.is_pure)
-        self.density_model = ModelFactory(units_d, onnx_model_bytes=self.density_onnx, is_pure=self.is_pure)
+        units_hc = {'te': self.heat_capacity_unit_te,
+                    'out': self.heat_capacity_unit_out}
+        if self.heat_capacity_unit_c is not None:
+            units_hc['c'] = self.heat_capacity_unit_c
+
+        units_d = {'te': self.density_unit_te,
+                   'out': self.density_unit_out}
+        if self.density_unit_c is not None:
+            units_d['c'] = self.density_unit_c
+
+        self.density_model = ModelFactory(units_d, is_pure=self.is_pure, df=self.density_data)
+        self.heat_capacity_model = ModelFactory(units_hc, is_pure=self.is_pure, df=self.heat_capacity_data)
 
 
 class FluidFactory:
     def __new__(cls, **kwargs):
         if kwargs.get('fluid') is None:
             warnings.warn(
                 'This returns a generic fluid. You probably wanted FluidFactory(fluid=<fluid definition object>'
                 'attaching a fluid definition allows for a return of a concrete Fluid subtype')
             return Fluid(**kwargs)
 
-        elif isinstance(kwargs['fluid'], CoolPropFluidDefinition):
+        if isinstance(kwargs['fluid'], CoolPropFluidDefinition):
             return CoolPropFluid(**kwargs)
-        elif isinstance(kwargs['fluid'], WPDFluidDefinition):
+
+        if isinstance(kwargs['fluid'], WPDFluidDefinition):
             if kwargs['fluid'].is_pure:
                 if kwargs.pop('concentration', None) is not None:
-                    warnings.warn('You passed a "concentration" kwargs to a pure fluid (WPDFluidPure). I will '
-                                  'gracefully ignore the concentration.')
+                    warnings.warn('You passed a "concentration" kwargs to a pure fluid (WPDFluidPure). '
+                                  'I will gracefully ignore the concentration.')
                 return WPDFluidPure(**kwargs)
-            else:
-                return WPDFluidMixed(**kwargs)
+
+            return WPDFluidMixed(**kwargs)
+
         elif isinstance(kwargs['fluid'], str):
             return UninitialisedFluid(kwargs.pop('fluid'), kwargs)
 
 
 class Fluid(ORMBase):
     """
-    Stores basic information about fluids in HarvestIT and a high level, and implements a high level abstract fluid
-    interface for HarvestIT.
+    Stores basic information about fluids in SunPeek and a high level, and implements a high level abstract fluid
+    interface for SunPeek.
 
     Notes
     -----
     - Provides get_density() and get_heat_capacity() accessors for all fluids, accepting scalar or vector pint Quantity
     as temperature input.
     - Subclasses must implement _get_density() and _get_heat_capacity().
-    - Forms the base class for a joined table class hirarchy in the database, see https://docs.sqlalchemy.org/en/14/orm/inheritance.html
+    - Forms the base class for a joined table class hierarchy in the database,
+    see https://docs.sqlalchemy.org/en/14/orm/inheritance.html
     the polymorphic discriminator column is `model_type`, this parameter is set automatically, do not alter by hand.
 
-    Attributes
-    ----------
-    name : str
-        Fluid name, must be unique within HarvestIT.
-    manufacturer_name : str, optional
-        Manufacturer name. Example: "Thermum GmbH & Co. KG"
-    product_name : str, optional
-        Product name. Example: "Thermum P"
-    concentration : pint Quantity, optional
-        Volumetric or mass concentration, depending on how concentration is stated in the underlying manufacturer
-        data sheet or in `CoolProp`_.
-
     .. _CoolProp:
         http://www.coolprop.org/fluid_properties/Incompressibles.html#mixture-examples
     """
     __tablename__ = 'fluids'
 
     id = Column(Integer, Identity(0), primary_key=True)
     fluid_definition_id = Column(ForeignKey(WPDFluidDefinition.id))
     model_type = Column(Enum('CoolProp', 'WPD', 'WPDPure', 'WPDMixed', name='fluid_model_type'))
-    name = Column(String)
     fluid = relationship("FluidDefinition", foreign_keys=[fluid_definition_id])
     plant_id = Column(ForeignKey('plant.id', ondelete="CASCADE"))
-    # hx_hot_id = Column(ForeignKey('heat_exchangers.id', ondelete="CASCADE"))
-    # hx_cold_id = Column(ForeignKey('heat_exchangers.id', ondelete="CASCADE"))
     plant = relationship("Plant", foreign_keys=[plant_id], uselist=False)
-    # hx_hot = relationship("HeatExchanger", foreign_keys=[hx_hot_id], uselist=False)
-    # hx_cold = relationship("HeatExchanger", foreign_keys=[hx_cold_id], uselist=False)
+
     DENSITY_DEFAULT_UNIT = 'kg m**-3'
     HEAT_CAPACITY_DEFAULT_UNIT = 'J kg**-1 K**-1'
 
     __mapper_args__ = {
         'polymorphic_identity': 'fluid',
         'polymorphic_on': model_type,
         'with_polymorphic': '*'
     }
 
     __table_args__ = (
         CheckConstraint('_concentration between 0 and 1', name='concentration_check'),
     )
 
     def _get_density(self, te):
-        pass
+        raise NotImplementedError()
 
     def _get_heat_capacity(self, te):
-        pass
+        raise NotImplementedError()
 
     def get_density(self, te):
         """Calculate density of fluid at given temperature and self.concentration
         Parameters
         ----------
         te : pd.Series
             Temperature for which density is evaluated.
@@ -411,37 +439,45 @@
         -------
         pd.Series
         """
         cp = self._get_heat_capacity(te)
         cp.index = te.index
         return cp.pint.to(self.HEAT_CAPACITY_DEFAULT_UNIT)
 
+    @property
+    def name(self):
+        return self.fluid.name
+
 
 class UninitialisedFluid(Fluid):
+    __mapper_args__ = {
+        'polymorphic_identity': 'Uninitialised',
+    }
+
     def __init__(self, fluid_def_name, stored_args):
         self.fluid_def_name = fluid_def_name
         self.stored_args = stored_args
 
 
-def assert_valid_fluid(fluid):
+def assert_valid_fluid(fluid: Fluid):
     assert fluid is not None
     assert not isinstance(fluid, UninitialisedFluid)
 
 
 class CoolPropFluid(Fluid):
     """High level class for interface with CoolProp incompressible fluids.
 
     Input and output units to CoolProp are standardized and thus don't need to be specified.
 
     Attributes
     ----------
     fluid : CoolPropFluidDefinition
         User-supplied string that must uniquely define a fluid within the CoolProp incompressible fluids.
         See `CoolProp Incompressibles`_.
-    concentration : pint Quantity
+    concentration : Quantity or dict
         If fluid does not require concentration, leave at default None.
         `concentration` is interpreted as mass concentration for `mass-based binary mixtures`_.
         `concentration` is interpreted as volume concentration for `volume-based binary mixtures`_.
 
     Raises
     ------
     ValueError, TypeError
@@ -456,33 +492,38 @@
     def _concentration(cls):
         """concentration column, shared with WPDMixedFluid class"""
         return Fluid.__table__.c.get('_concentration', Column(Float))
 
     # Default pressure (in Pa) that is passed to CoolProp. See note in module docstring.
     P_DEFAULT = 101325
 
-    def __init__(self, fluid=None, concentration=None):
+    def __init__(self, fluid: CoolPropFluidDefinition = None, concentration: Union[Q, dict] = None):
         if fluid is not None:
             self.fluid = fluid
 
-        if (self.fluid is not None) and self.fluid.is_pure:
-            if concentration is not None:
-                raise ValueError('Non-None concentration was given for a pure fluid.')
-        elif (self.fluid is not None) and (not self.fluid.is_pure):
-            if concentration is None:
-                raise ValueError('None concentration was given a for a non-pure fluid.')
-            self._concentration = concentration.m_as('dimensionless') * 100
+            if self.fluid.is_pure:
+                if concentration is not None:
+                    raise ValueError('Non-None concentration was given for a pure fluid.')
+            else:
+                if concentration is None:
+                    raise ValueError('None concentration was given a for a non-pure fluid.')
+                self.concentration = concentration
 
     @property
     def concentration(self):
         if not self.fluid.is_pure:
-            return Q(self._concentration, 'percent')
+            return Q(self._concentration, 'dimensionless').to('percent')
         else:
             return None
 
+    @concentration.setter
+    def concentration(self, val):
+        val = uu.parse_quantity(val)
+        self._concentration = val.m_as('dimensionless')
+
     @property
     def query_str(self):
         """String to be sent to CoolProp backend, adds concentration to self.coolprop_fluid, if necessary.
         Return
         ------
         str
         """
@@ -507,33 +548,33 @@
         """Return density or heat capacity, with common error handling / CoolProp allowed temperature ranges.
         """
         coolprop_prop = "D" if prop == "density" else "C"
         try:
             val = Cp.PropsSI(coolprop_prop, "P", self.P_DEFAULT, "T", uu.to_numpy(te, 'K'), self.query_str)
             # If some (but not all) temperatures exceed the allowed fluid temperature range, they are returned as Inf.
             # Convert to NaN so all downstream methods can keep relying that everything is either ok or np.nan
-            hit_logger.warn(f'CoolProp returned Inf results in {prop} calculation of fluid "{self.query_str}". '
-                            f'This is probably because some of the given temperatures exceed the allowed '
-                            f'temperature range. '
-                            f'For more details, see http://www.coolprop.org/fluid_properties/Incompressibles.html')
+            sp_logger.warn(f'CoolProp returned Inf results in {prop} calculation of fluid "{self.query_str}". '
+                           f'This is probably because some of the given temperatures exceed the allowed '
+                           f'temperature range. '
+                           f'For more details, see http://www.coolprop.org/fluid_properties/Incompressibles.html')
         except ValueError:
             # This happens if all temperatures passed to CoolProp exceed the allowed fluid temperature range.
             # For allowed fluid temperatures, see http://www.coolprop.org/fluid_properties/Incompressibles.html
             val = np.full(len(te), np.inf)
-            hit_logger.warn(f'CoolProp raised ValueError in {prop} calculation of fluid "{self.query_str}". '
-                            f'This is probably because all given temperatures exceed the allowed temperature range. '
-                            f'For more details, see http://www.coolprop.org/fluid_properties/Incompressibles.html '
-                            f'All {prop} values have been set to Inf.')
+            sp_logger.warn(f'CoolProp raised ValueError in {prop} calculation of fluid "{self.query_str}". '
+                           f'This is probably because all given temperatures exceed the allowed temperature range. '
+                           f'For more details, see http://www.coolprop.org/fluid_properties/Incompressibles.html '
+                           f'All {prop} values have been set to Inf.')
 
         return val
 
 
 class WPDFluid(Fluid):
     """
-    Fluid with given trained ONNX models for density and heat capacity.
+    Fluid with given trained sklearn models for density and heat capacity.
     Accepts pint Quantity for temperature and (optionally) concentration. Returns fluid properties as pint Quantity.
     """
 
     __mapper_args__ = {
         'polymorphic_identity': 'WPD',
     }
 
@@ -548,68 +589,71 @@
     def _get_density(self, te):
         return self._get_property(self.density_model, te)
 
     def _get_heat_capacity(self, te):
         return self._get_property(self.heat_capacity_model, te)
 
     def _get_property(self, model, te):
-        pass
+        raise NotImplementedError()
 
 
 class WPDFluidPure(WPDFluid, ORMBase):
     """WPDFluid subclass for fluids that do not have a variable concentration, so they are either pure fluids or have
     a fixed concentration.
+
     Attributes
     ----------
     density_model, heat_capacity_model : WPDModel
         Trained WPDModel objects for density and heat capacity.
     """
 
     __mapper_args__ = {
         'polymorphic_identity': 'WPDPure',
     }
 
     def _get_property(self, model, te):
         """Return model property (density, heat capacity). Accepts & returns pd.Series with dtype pint unit."""
         te_ = te.pint.m_as(model.unit['te'])
         output = model.predict(te_)
-        # return uu.to_s(output, model.unit['out'])
         return uu.to_s(output.astype('float64'), model.unit['out'])
 
 
 class WPDFluidMixed(WPDFluid, ORMBase):
     """WPDFluid subclass for fluids that do have a variable concentration, either mass or volume concentration.
     Attributes
     ----------
-    concentration : float
+    concentration : Quantity or dict
         Scalar concentration value of fluid
     density_model, heat_capacity_model : WPDModel
         Trained WPDModel objects for density and heat capacity
     """
 
     __mapper_args__ = {
         'polymorphic_identity': 'WPDMixed',
     }
 
     @declared_attr
     def _concentration(cls):
         "concentration column, shared with WPDMixedFluid class"
         return Fluid.__table__.c.get('_concentration', Column(Integer))
 
-    def __init__(self, concentration, **kwargs):
-        self._concentration = concentration.to('percent').magnitude
+    def __init__(self, concentration: Union[Q, dict], **kwargs):
+        self.concentration = concentration
         # self.density_model = density_model
         # self.heat_capacity_model = heat_capacity_model
         super().__init__(**kwargs)
 
     @property
     def concentration(self):
-        return Q(self._concentration, 'percent')
+        return Q(self._concentration, 'dimensionless').to('percent')
+
+    @concentration.setter
+    def concentration(self, val):
+        val = uu.parse_quantity(val)
+        self._concentration = val.m_as('dimensionless')
 
     def _get_property(self, model, te):
-        # te_ = te.to(model.unit['te']).magnitude
         te_ = te.pint.m_as(model.unit['te'])
         c_ = self.concentration.m_as(model.unit['c'])
-        c_ = np.full(te.shape, c_)
         output = model.predict(te_, c_)
-        # return uu.units.Quantity(output, model.unit['out'])
+
         return uu.to_s(output, model.unit['out'])
```

## sunpeek/components/helpers.py

```diff
@@ -1,243 +1,263 @@
 """
 .. codeauthor:: Marnoch Hamilton-Jones <m.hamilton-jones@aee.at>
 .. codeauthor:: Philip Ohnewein <p.ohnewein@aee.at>
 """
 
 import numpy as np
 import sqlalchemy
-from sqlalchemy import Column, String, Integer, ForeignKey, Float, Identity, ARRAY
+from sqlalchemy import Column, String, Integer, ForeignKey, Float, Identity, ARRAY, Enum, UniqueConstraint, JSON
 from sqlalchemy.ext.declarative import declarative_base
 import sqlalchemy.orm
 import sqlalchemy.exc
-from sqlalchemy.orm import relationship, backref
-from sqlalchemy.orm.collections import attribute_mapped_collection
+from sqlalchemy.orm import relationship
 import sqlalchemy.event
 import enum
 
 from sunpeek.common.unit_uncertainty import Q
 import sunpeek.common.unit_uncertainty as uu
 from sunpeek.common.errors import ConfigurationError
+from sunpeek.common.utils import DatetimeTemplates
 
 ORMBase = declarative_base()
 
 
-# module_engine = utils.db_engine
-
-
 class ComponentParam:
     """Used to define parameters which are represented by Quantities, with optional limit checking.  
     
     Attributes
     ----------
     unit: compatible unit
     minimum: value of the paramters should not be below this
     maximum: value of the paramters should not be above this
-    type: either "scalar" or "array", defaults to used to create the correct database column types and apply checks correctly.
+    array_type: either "scalar" or "array", defaults to used to create the correct database column types and apply checks correctly.
     """
-    
-    def __init__(self, unit: str = None, minimum: float = -np.Inf, maximum: float = np.Inf, type: str = 'scalar'):
+
+    def __init__(self, unit: str = None, minimum: float = -np.Inf, maximum: float = np.Inf, param_type: str = 'scalar'):
         # self.name = name
         self.unit = unit
         self.minimum = minimum
         self.maximum = maximum
-        self.type = type
+        self.array_type = param_type
+        # Idea: Implement ComponentParam availability, also see ComponentParam.available
+        #  -> make this an ORM class, add "name" attrib, dataclass
+        # available: Optional[bool] = None
 
 
 class AttrSetterMixin:
     name = None
-    defer_configure_virtuals = False
+    defer_post_config_changed_actions = False
 
     @classmethod
     def define_component_attrs(cls):
         for sub_cls in cls.all_subclasses():
+            # get all ComponentParam from all component / subclass attributes
             params = {attr: obj for attr, obj in sub_cls.__dict__.items() if isinstance(obj, ComponentParam)}
             for attr, obj in params.items():
                 # delattr(sub_cls, attr)
-                sub_cls.add_component_attr(attr, obj.unit, obj.minimum, obj.maximum, obj.type)
+                sub_cls.add_component_attr(attr, obj.unit, obj.minimum, obj.maximum, obj.array_type)
 
     @classmethod
-    def add_component_attr(cls, name, unit=None, minimum=-np.Inf, maximum=np.Inf, type='scalar'):
-        if type == 'scalar':
-            setattr(cls, '_{}_mag'.format(name), Column(Float))
+    def add_component_attr(cls, name, unit=None, minimum=-np.Inf, maximum=np.Inf, array_type='scalar'):
+        if array_type == 'scalar':
+            setattr(cls, f'_{name}_mag', Column(Float))
         elif 'array':
-            setattr(cls, '_{}_mag'.format(name), Column(ARRAY(Float)))
-        setattr(cls, '_{}_unit'.format(name), Column(String))
-        prop = property(fset=lambda cls, value: cls.set_component_attribute(name, value, type),
+            setattr(cls, f'_{name}_mag', Column(JSON))
+        setattr(cls, f'_{name}_unit', Column(String))
+        prop = property(fset=lambda cls, value: cls.set_component_attribute(name, value, array_type),
                         fget=lambda cls: cls.get_component_attribute(name))
         setattr(cls, name, prop)
         if not hasattr(cls, '_attr_props'):
             cls._attr_props = {}
         cls._attr_props[name] = {'unit': unit, 'minimum': minimum, 'maximum': maximum}
         # print (self.attr_props[name])
 
     @classmethod
     def all_subclasses(cls, c=None):
         if c is None: c = cls
         return set(c.__subclasses__()).union(
             [s for c in cls.__subclasses__() for s in c.all_subclasses(c)])
 
-    def set_component_attribute(self, name, value, type):
+    @classmethod
+    def register_callback(cls, callback_type, func):
+        print(cls)
+        try:
+            getattr(cls, callback_type).append(func)
+        except AttributeError:
+            cls.post_config_changed_callbacks = [func]
+
+    def _check_value(self, name, value, type):
+        unit = self._attr_props[name]['unit']
+
+        uu.assert_compatible(value.units, unit)
+
+        val = value.to(unit).magnitude
+        min = self._attr_props[name]['minimum']
+        max = self._attr_props[name]['maximum']
+
+        if type == 'scalar' or type is None:
+            if isinstance(value.magnitude, np.ndarray):
+                raise ConfigurationError("Attempting to assign an array quantity to a scalar type parameter")
+            if val < min:
+                raise ConfigurationError(
+                    f"attempting to set a value for attribute {name} that is less than the minimum of {min}{unit}")
+            if val > max:
+                raise ConfigurationError(
+                    f"attempting to set a value for attribute {name} that is greater than the maximum of {max}{unit}")
+
+        if type == 'array':
+            if not isinstance(value.magnitude, np.ndarray):
+                raise ConfigurationError("Attempting to assign an array quantity to a scalar type parameter")
+            if (val < min).any():
+                raise ConfigurationError(
+                    f"attempting to set a value for attribute {name} that is less than the minimum of {min}{unit}")
+            if (val > max).any():
+                raise ConfigurationError(
+                    f"attempting to set a value for attribute {name} that is greater than the maximum of {max}{unit}")
+
+    def set_component_attribute(self, name, value, array_type):
         if value is not None:
             value = uu.parse_quantity(value)
             if not self._attr_props[name]['unit'] == 'no_check':
-                # assert uu.units.is_compatible_with(value.units, self._attr_props[name]['unit'])
-                uu.assert_compatible(value.units, self._attr_props[name]['unit'])
+                self._check_value(name, value, array_type)
 
-                if type == 'scalar' or type is None:
-                    assert not isinstance(value.magnitude, np.ndarray), "You are trying to assign an array quantity to a scalar type paramter"
-                    assert self._attr_props[name]['minimum'] <= value.to(self._attr_props[name]['unit']).magnitude
-                    assert value.to(self._attr_props[name]['unit']).magnitude <= self._attr_props[name]['maximum']
-                    mag = value.magnitude
-                if type == 'array':
-                    assert isinstance(value.magnitude, np.ndarray), "You are trying to assign a non-array quantity to an array type paramter"
-                    assert (self._attr_props[name]['minimum'] <= value.to(self._attr_props[name]['unit']).magnitude).all()
-                    assert (value.to(self._attr_props[name]['unit']).magnitude <= self._attr_props[name]['maximum']).all()
-                    mag = value.magnitude.tolist()
-            else:
+            if array_type == 'scalar' or array_type is None:
                 mag = value.magnitude
+            elif array_type == 'array':
+                mag = value.magnitude.tolist()
+            else:
+                raise ValueError("type must be either 'scalar' or 'array'")
 
-            setattr(self, '_{}_mag'.format(name), mag)
-            setattr(self, '_{}_unit'.format(name), str(value.units))
+            setattr(self, f'_{name}_mag', mag)
+            setattr(self, f'_{name}_unit', str(value.units))
         else:
             # setattr(self, name, None)
-            setattr(self, '_{}_mag'.format(name), None)
-            setattr(self, '_{}_unit'.format(name), None)
+            setattr(self, f'_{name}_mag', None)
+            setattr(self, f'_{name}_unit', None)
+
         if getattr(self, 'plant', None) is not None and (self.__class__.__name__ != 'Sensor'):
             # Update whether virtual sensor can be calculated with new plant information
-            if not self.defer_configure_virtuals:
-                self.plant.config_virtuals()
+            if not self.defer_post_config_changed_actions:
+                [func(self.plant) for func in self.plant.post_config_changed_callbacks]
 
     def get_component_attribute(self, name):
-        if self.__getattribute__('_{}_mag'.format(name)) is None:
+        if self.__getattribute__(f'_{name}_mag') is None:
             return None
-        return Q(self.__getattribute__('_{}_mag'.format(name)), self.__getattribute__('_{}_unit'.format(name)))
+        return Q(self.__getattribute__(f'_{name}_mag'), self.__getattribute__(f'_{name}_unit'))
 
     def __getattr__(self, item):
-                    # print('attr==sens')
-        if (item == "sensors") or ('_AssociationProxy__sensor_map' in item) or (item in ['_sa_instance_state', '_proxy_dicts']):
+        # print('attr==sens')
+        if (item == "sensors") or ('_AssociationProxy__sensor_map' in item) or (
+                item in ['_sa_instance_state', '_proxy_dicts']):
             raise AttributeError
 
         try:
             return self.sensors[item]
         except KeyError:
             if item in self.sensor_slots.keys():
                 return None
             else:
                 raise AttributeError(f"{item} not found in component {self}.")
-        except (AttributeError, AssertionError, sqlalchemy.exc.InvalidRequestError):
-            raise AttributeError(f"{item} not found in component {self}.")
+        except (AttributeError, AssertionError, sqlalchemy.exc.InvalidRequestError) as ex:
+            raise AttributeError(f"{item} not found in component {self}. Original exception: {ex}")
 
     def __str__(self):
         try:
             if self.name is not None:
-                return 'HarvestIT {} component called {}'.format(self.__class__.__name__, self.name)
+                return f'HarvestIT {self.__class__.__name__} component called {self.name}'
             else:
-                return 'HarvestIT {} object'.format(self.__class__.__name__)
+                return f'HarvestIT {self.__class__.__name__} object'
         except sqlalchemy.exc.InvalidRequestError:
             return "unknown SunPeek component"
 
     def __repr__(self):
         return self.__str__()
 
     def __dir__(self):
         try:
             return list(self.sensor_slots.keys()) + list(super().__dir__())
         except AttributeError:
             return super().__dir__()
 
 
-class AccuracyClass(enum.Enum):
+class AccuracyClass(str, enum.Enum):
     low = "low"
     medium = "medium"
     high = "high"
 
 
-class InstallCondition(enum.Enum):
+class InstallCondition(str, enum.Enum):
     perfect = "perfect"
     fair = "fair"
     bad = "bad"
 
 
-class IsVirtual(enum.Enum):
+class IsVirtual(str, enum.Enum):
     never = "never"
     possible = "possible"
     always = "always"
-    
-    
-class ResultStatus(enum.Enum):
+
+
+class ResultStatus(str, enum.Enum):
     pending = "pending"
     running = "running"
     done = "done"
     failed = "failed"
 
 
 class SensorMap(ORMBase):
     """Class which defines the many-to-many mapping table and performs required logic to map Sensor objects to sensor
     channels on components.
     The `sensor_type` argument to the __init__ method determines the SensorType that will be attached to the sensor.
     If a sensor type has already been attached, attempting to create another mapping with a different type, a ConfigurationError
     will be raised.
-    When a SensorMap is created, the sensor_type is not attached immediatly. Instead, the `sensor_type_name` attribute
+    When a SensorMap is created, the sensor_type is not attached immediately. Instead, the `sensor_type_name` attribute
     of the sensor is set. When the SensorMap object is attached to a database session, a lookup is performed against the
     sensor_types table, and an appropriate SensorType object loaded and attached to the sensor.
+
     Attributes
     ----------
-    sensor : Sensor
+
+    sensor : py:class:sunpeek.components.sensor.Sensor
         The sensor object to be mapped
     slot_name: str
         The name of the sensor channel being mapped to, e.g. `te_amb`
-    array : Array
+    array : physical.Array
         Array object, if the mapping is to an array
-    plant : Plant
+    plant : physical.Plant
         Plant object, if the mapping is to a plant
-    heat_exchanger : HeatExchanger
+    heat_exchanger : helpers.pyHeatExchanger
         HeatExchanger object, if the mapping is to a hx
     """
     __tablename__ = 'sensor_map'
 
     id = Column(Integer, Identity(0), primary_key=True)
     sensor_id = Column(Integer, ForeignKey('sensors.id', ondelete="CASCADE"))
     slot_name = Column(String)
 
-    plant_id = Column(Integer, ForeignKey('plant.id', ondelete="CASCADE"))
-    array_id = Column(Integer, ForeignKey('arrays.id', ondelete="CASCADE"))
-    heat_exchanger_id = Column(Integer, ForeignKey('heat_exchangers.id', ondelete="CASCADE"))
-    # row_id = Column(Integer, ForeignKey('rows.id'))
+    component_id = Column(Integer, ForeignKey('components.component_id', ondelete="CASCADE"))
 
     # reference to the "Sensor" object
-    sensor = relationship("Sensor", foreign_keys=[sensor_id], backref="_mappings")
+    sensor = relationship("Sensor", back_populates="mappings")
+    component = relationship("Component", back_populates="_sensor_map")
 
-    # Create association proxy relationships to parent components
-    array = relationship("Array",
-                         backref=backref("_sensor_map",
-                                         collection_class=attribute_mapped_collection("slot_name"),
-                                         cascade="all, delete-orphan"))
-    plant = relationship("Plant",
-                         backref=backref("_sensor_map",
-                                         collection_class=attribute_mapped_collection("slot_name"),
-                                         cascade="all, delete-orphan"))
-    heat_exchanger = relationship("HeatExchanger",
-                                  backref=backref("_sensor_map",
-                                                  collection_class=attribute_mapped_collection("slot_name"),
-                                                  cascade="all, delete-orphan"))
-
-    @property
-    def component(self):
-        for comp in [self.array, self.plant, self.heat_exchanger]:
-            if comp is not None:
-                return comp
 
-    def __init__(self, slot_name: str, sensor, sensor_type, component):
+    @sqlalchemy.orm.validates('sensor', include_removes=True)
+    def _handle_unmaps(self, _, val, is_remove):
+        if is_remove or val is None:
+            self.unmap(include_sensor=False)
+        return val
+
+    def __init__(self, slot_name: str, sensor, sensor_type=None, component=None):
         if sensor is None:
             return
         self.slot_name = slot_name
 
         if isinstance(sensor, str):
-            raise ConfigurationError(f'SensorMap was passed a string instead of a sensor obejct. This could be because '
+            raise ConfigurationError(f'SensorMap was passed a string instead of a sensor object. This could be because '
                                      f'channel {slot_name} of {component} was mapped to a raw sensor that does not exist.')
             # This should have been excluded by _on_array_append
         if component.plant is None:
             raise ConfigurationError(f'Cannot map sensor to channel {slot_name} of component {component} because '
                                      f'component.plant is None.')
 
         if isinstance(sensor_type, str):
@@ -251,28 +271,50 @@
         #     pass
         elif sensor.sensor_type.name != type_name:
             raise ConfigurationError(
                 f'Sensor {sensor.raw_name} already has type "{sensor.sensor_type.name}". Mapping to "{slot_name}" of '
                 f'{component} requires type "{type_name}". Check your config.')
 
         sensor.plant = component.plant
-        # else:
-        #     raise ConfigurationError(f'Sensor {sensor.raw_name} mapping to "{slot_name}" of {component}. There appears '
-        #                              f'to be a mismatch between sensor types and type_names names. '
-        #                              f'Type: "{sensor.sensor_type}", Type name: "{type_name}"')
 
         self.sensor = sensor
-        setattr(self,
-                {r.mapper.class_.__name__: r.key for r in SensorMap.__mapper__.relationships}
-                [component.__class__.__name__], component)
+
+        self.component = component
 
         # In case the attribute for channel name was already set to None, remove it so that __getattr__ looks in sensors
         component.__dict__.pop(slot_name, None)
         sensor.plant = component.plant
 
+    def unmap(self, include_sensor=True):
+        self.component = None
+        if include_sensor:
+            self.sensor = None
+        # session = sqlalchemy.orm.Session.object_session(self)
+        # if session is not None:
+        #     # Calling this inside an ORM object method isn't ideal, but seems to be necessary to avoid violating
+        #     # `_unique_mapping_per_component_slot` constraint under certain circumstances.
+        #     session.delete(self)
+        #     session.flush()
+
+
+class DataUploadDefaults(ORMBase):
+    __tablename__ = 'data_upload_defaults'
+
+    id = Column(Integer, Identity(0), primary_key=True)
+    plant_id = Column(Integer, ForeignKey('plant.id', ondelete="CASCADE"))
+    plant = relationship("Plant", back_populates='data_upload_defaults')
+
+    datetime_template = Column(Enum(DatetimeTemplates))
+    datetime_format = Column(String)
+    timezone = Column(String)
+    csv_separator = Column(String)
+    csv_decimal = Column(String)
+    csv_encoding = Column(String)
+    index_col = Column(Integer)
+
 
 # class Row(AttrSetterMixin, ORMBase):
 #     """
 #     Implements a single collector row with its inlet and outlet temperatures, as part of an Array.
 #
 #     Note
 #     ----
@@ -303,46 +345,22 @@
 #         self.te_in = te_in
 #         self.te_out = te_out
 #
 #         SensorMap('te_in', te_in, 'fluid_temperature', component=self)
 #         SensorMap('te_out', te_out, 'fluid_temperature', component=self)
 
 
-
-
-
 # array_results_association_table = sqlalchemy.Table('array_results_association', ORMBase.metadata,
 #                                                    Column('result_id', primary_key=True),
 #                                                    Column('result_time', primary_key=True),
 #                                                    Column('array_id', ForeignKey('arrays.id'), primary_key=True),
 #                                                    ForeignKeyConstraint(["result_id", "result_time"], ["pc_results.id",
 #                                                                                                        "pc_results.datetime_eval_done"]),
 #                                                    )
 
 
 # AttrSetterMixin.define_component_attrs()
 
 
-# TODO: make results table a hypertable, might not be possible due to Timescale limitiations: https://github.com/timescale/timescaledb/issues/498
-# sqlalchemy.event.listen(
-#     PCMethodOutput.__table__,
-#     'after_create',
-#     sqlalchemy.DDL(f"SELECT * FROM create_hypertable('{PCMethodOutput.__tablename__}', 'datetime_eval_done');")
-# )
-#
-# sqlalchemy.event.listen(
-#     PCMethodOutput.__table__,
-#     'after_create',
-#     sqlalchemy.DDL(f"CREATE INDEX ON "
-#                    f"{PCMethodOutput.__tablename__}(plant_id, datetime_eval_done);")
-# )
-#
-# sqlalchemy.event.listen(
-#     PCMethodOutput.__table__,
-#     'after_create
-#     sqlalchemy.DDL(f"CREATE INDEX ON "
-#                    f"{PCMethodOutput.__tablename__}(plant_id, datetime_eval_start, datetime_eval_end, datetime_eval_done);")
-# )
-
 def make_tables(engine):
     """Uses the table definitions contained in the component classes to create DB tables"""
     ORMBase.metadata.create_all(engine)
```

## sunpeek/components/iam_methods.py

```diff
@@ -23,15 +23,15 @@
 
 
 # -----------
 # Functions
 # -----------
 
 def get_iam_ASHRAE(aoi: pd.Series, b: Q):
-    """ Determines the incidence angle modifier using the ASHRAE transmission model, using pvlib.
+    """ Determines the incidence angle modifier using the ASHRAE transmission model, using :py:mod:pvlib.
 
     Parameters
     ----------
     aoi : pd.Series
         The angle of incidence (AOI) between the normal vector of the collector plane and the
         sun-beam vector, as pint (unit aware) pandas Series. Angles of NaN will result in NaN.
     b : float, default 0.05
@@ -41,15 +41,15 @@
     Returns
     -------
     `pd.Series`
         A unit-aware, dimensionless pandas Series containing the IAM values.
 
     See Also
     --------
-    components.iam_methods.IAM_ASHRAE
+    IAM_ASHRAE
     """
     aoi = to_numpy(aoi, 'deg')
     b = b.m_as('')
     iam = pvlib.iam.ashrae(aoi, b=b)
     return to_s(iam)
 
 
@@ -69,15 +69,15 @@
     Returns
     -------
     `pd.Series`
         A unit-aware, dimensionless pandas Series containing the IAM values.
 
     See Also
     --------
-    components.iam_methods.IAM_ASHRAE
+    sunpeek.components.iam_methods.IAM_ASHRAE
     """
     aoi = to_numpy(aoi, 'deg')
     k50 = k50.m_as('')
     rad_50 = 50 * np.pi / 180
     b = -(k50 - 1) / (1 / np.cos(rad_50) - 1)
     iam = pvlib.iam.ashrae(aoi, b=b)
     return to_s(iam)
@@ -114,47 +114,52 @@
 
 
 def get_iam_interpolated(aoi: pd.Series, iam_reference: Q, aoi_reference: Q, azimuth_diff: Q = Q(0, 'deg')):
     """ Determines the incidence angle modifier by interpolating over a set of given reference values.
 
     Parameters
     ----------
-    aoi : pd.Series
+    aoi : pandas.Series
         The angle of incidence between the module normal vector and the
         sun-beam vector, as pint (unit aware) pandas Series. Angles of NaN will result in NaN.
     aoi_reference : Quantity
         Vector of angles at which the IAM is known [degrees].
     iam_reference : Quantity
         IAM values for each angle in ``aoi_reference`` [unitless].
-    azimuth_diff : pd.Series
+    azimuth_diff : pandas.Series
         The difference between solar and collector azimuth angle [degrees].
 
     Returns
     -------
-    `pd.Series`
+    pandas.Series
         A unit-aware, dimensionless pandas Series containing the IAM values.
 
     Notes
     -----
-    Determines the IAM based on interpolating a set of reference values based on EN ISO 9806 Solar Energy Draft
-    p.53 Formula (22, 23, 25, 27). This is similar to pvlib.iam.interp, but allows separation in longitudinal and
-    transversal plane, whereas pvlib works only for symmetric collector IAMs.
+    Determines the IAM based on interpolating a set of reference values based on EN ISO 9806 [1]_. This is similar to
+    `pvlib.iam.interp`, but allows separation in longitudinal and transversal plane, whereas pvlib works only for
+    symmetric collector IAMs.
 
-    The IAM reference values `iam_reference` are usually measured values (as stated in the EN ISO 9806).
+    The IAM reference values `iam_reference` are usually measured values [1]_.
 
     ``aoi_reference`` must have two or more points and may span any range of angles. Typically there will be a dozen
     or more points in the range 0..90 degrees. Beyond the range of ``aoi_reference``, IAM values are extrapolated,
     but constrained to be non-negative.
 
     The sign of ``aoi`` is ignored; only the magnitude is used.
 
     See Also
     --------
     pvlib.iam.interp
+
+    References
+    ----------
+    .. [1] EN ISO 9806 Solar Energy Draft pp.53 Formula (22, 23, 25, 27)
     """
+
     aoi_reference = aoi_reference.m_as('deg')
     iam_reference = iam_reference.m_as('')
     aoi = to_numpy(aoi, 'deg')
     azimuth_diff = to_numpy(azimuth_diff, 'deg')
 
     aoi_reference, iam_reference = _normalize_iam_reference(aoi_reference=aoi_reference, iam_reference=iam_reference)
 
@@ -178,15 +183,15 @@
         The angle of incidence between the module normal vector and the
         sun-beam vector [degrees].
     azimuth_diff : numeric
         The difference between solar and collector azimuth angle [degrees].
 
     Notes
     -----
-    Calculation is based on equation_id 5 of this paper:
+    Calculation is based on equation 5 of this paper:
     S. Hess and V. I. Hanby, “Collector Simulation Model with Dynamic Incidence Angle Modifier for Anisotropic Diffuse
     Irradiance,” Energy Procedia, vol. 48, pp. 87–96, 2014, doi: 10.1016/j.egypro.2014.02.011.
     """
     aoi_rad = np.deg2rad(aoi)
     azimuth_diff_rad = np.deg2rad(azimuth_diff)
     aoi_transversal = np.rad2deg(-np.arctan(np.tan(aoi_rad) * np.cos(azimuth_diff_rad)))
     return np.abs(aoi_transversal)
@@ -201,15 +206,15 @@
         The angle of incidence between the module normal vector and the
         sun-beam vector [degrees].
     azimuth_diff : numeric
         The difference between solar and collector azimuth angle [degrees].
 
     Notes
     -----
-    Calculation is based on equation_id 4 of this paper:
+    Calculation is based on equation 4 of this paper:
     S. Hess and V. I. Hanby, “Collector Simulation Model with Dynamic Incidence Angle Modifier for Anisotropic Diffuse
     Irradiance,” Energy Procedia, vol. 48, pp. 87–96, 2014, doi: 10.1016/j.egypro.2014.02.011.
     """
     aoi_rad = np.deg2rad(aoi)
     azimuth_diff_rad = np.deg2rad(azimuth_diff)
     aoi_longitudinal = np.rad2deg(np.arctan(np.sin(aoi_rad) * np.sin(azimuth_diff_rad) / np.cos(aoi_rad)))
     return np.abs(aoi_longitudinal)
@@ -290,15 +295,15 @@
     return aoi, iam
 
 
 # -----------
 # CLASSES
 # -----------
 
-class _IAM_Method(ORMBase, AttrSetterMixin):
+class IAM_Method(ORMBase, AttrSetterMixin):
     __tablename__ = 'iam_methods'
     """ Abstract class for determining the incidence angle modifier (IAM) with different methods.
     """
     id = Column(Integer, Identity(0), primary_key=True)
     method_type = Column(Enum('Ambrosetti', 'ASHRAE', 'Interpolated', 'K50', name='iam_method_type'))
     collector_type_id = Column(Integer, ForeignKey('collector_types.id', ondelete="CASCADE"))
     collector_type = relationship("CollectorType", back_populates="iam_method")
@@ -321,15 +326,15 @@
             as pint (unit aware) pandas Series. Angles of NaN will result in NaN.
         azimuth_diff : pd.Series
             The difference between solar and collector azimuth angle, as pint (unit aware) pandas Series.
         """
         raise NotImplementedError("")
 
 
-class IAM_ASHRAE(_IAM_Method):
+class IAM_ASHRAE(IAM_Method):
     """ Determines the IAM for given incidence angles ``aoi`` [degrees], using the ASHRAE formula.
 
     Parameters
     ----------
     b : float, default 0.05
         A parameter to adjust the incidence angle modifier as a function of
         angle of incidence. Typical values are on the order of 0.05 [3].
@@ -348,15 +353,15 @@
     def __init__(self, b: Q, plant=None):
         self.b = b
 
     def get_iam(self, aoi: pd.Series, **kwargs):
         return get_iam_ASHRAE(aoi, b=self.b)
 
 
-class IAM_K50(_IAM_Method):
+class IAM_K50(IAM_Method):
     """ Determines the IAM for given incidence angles ``aoi`` [degrees], using the ASHRAE formula, if only `k50`, the
         IAM value at an incidence angle of 50°, is given.
 
     Parameters
     ----------
     k50 : float
         IAM value at an incidence angle of 50°
@@ -377,15 +382,15 @@
         self.b = -(self.k50 - 1) / (1 / np.cos(np.deg2rad(50)) - 1)
 
 
     def get_iam(self, aoi: pd.Series, **kwargs):
         return get_iam_ASHRAE(aoi, b=self.b)
 
 
-class IAM_Ambrosetti(_IAM_Method):
+class IAM_Ambrosetti(IAM_Method):
     """ Determines the IAM for given incidence angles ``aoi`` [degrees], using the Ambrosetti formula.
 
     Parameters
     ----------
     kappa : float
         exponent used for the Ambrosetti function
 
@@ -403,15 +408,15 @@
     def __init__(self, kappa: Q, plant=None):
         self.kappa = kappa
 
     def get_iam(self, aoi: pd.Series, **kwargs):
         return get_iam_ambrosetti(aoi, kappa=self.kappa)
 
 
-class IAM_Interpolated(_IAM_Method):
+class IAM_Interpolated(IAM_Method):
     """ Determines the incidence angle modifier by interpolating over a set of given reference values.
 
     Parameters
     ----------
     iam_reference: list
         Reference values for IAM values at certain incidence angles. (must match with `aoi_reference`)
     aoi_reference: list
@@ -422,16 +427,16 @@
     :func:`components.iam_methods.get_iam_interpolated`
     """
 
     __mapper_args__ = {
         'polymorphic_identity': 'Interpolated',
     }
 
-    aoi_reference = ComponentParam('deg', 0, 90, type='array')
-    iam_reference = ComponentParam('', 0, 2, type='array')
+    aoi_reference = ComponentParam('deg', 0, 90, param_type='array')
+    iam_reference = ComponentParam('', 0, 2, param_type='array')
 
     def __init__(self, iam_reference: Q, aoi_reference: Q, plant=None):
         # is then saved as a 2D list = 2 lists, one for longitudinal and one for transversal values
         aoi_reference, iam_reference = _normalize_iam_reference(aoi_reference=aoi_reference.m_as('deg'),
                                                                 iam_reference=iam_reference.m_as(''))
         self.aoi_reference = Q(aoi_reference, 'deg')
         self.iam_reference = Q(iam_reference)
```

## sunpeek/components/operational_events.py

```diff
@@ -1,58 +1,98 @@
+import sqlalchemy.orm
 from sqlalchemy import Column, Identity, ForeignKey, Integer, DateTime, String, Boolean
 from sqlalchemy.orm import relationship
+from sqlalchemy.ext.hybrid import hybrid_property
 import pytz
 from pandas import to_datetime
 
 from sunpeek.components.helpers import ORMBase
-from sunpeek.components.base import Component
+from sunpeek.common.errors import ConfigurationError, TimeZoneError
+
+
+def _check_has_tz(val, val_name):
+    if val.tzinfo is None:
+        raise ConfigurationError(f"Operational event {val_name} timestamp must be timezone aware. Pass a tz aware datetime"
+                                 f" object, or use set_start with a tz argument, or a string like 2022-1-1 00:00+02")
+
+
+def _check_tz_matches(val, tz):
+    if tz is not None and val.tzinfo is not None:
+        if not pytz.timezone(tz).utcoffset(val.combine(val.date(), val.time())) == val.utcoffset():
+            raise TimeZoneError('A timezone aware timestamp and a timezone argument were supplied, but the timezones did not match')
 
 
 class OperationalEvent(ORMBase):
     __tablename__ = 'operational_events'
 
     id = Column(Integer, Identity(0), primary_key=True)
     plant_id = Column(Integer, ForeignKey('plant.id', ondelete="CASCADE"))
     plant = relationship("Plant", back_populates="operational_events")
-    _start = Column(DateTime(timezone=True))
-    _end = Column(DateTime(timezone=True))
+    _event_start = Column(DateTime)
+    _event_end = Column(DateTime)
+    original_timezone = Column(String)
     ignored_range = Column(Boolean)
     description = Column(String)
 
-    def __init__(self, plant, start, tz=None, description=None, end=None, ignored_range=False):
+    def __init__(self, plant, event_start, event_end=None, tz=None, description=None, ignored_range=False):
         self.plant = plant
-        self.set_start(start, tz)
-        self.set_end(end, tz)
+        self.set_start(event_start, tz)
+        self.set_end(event_end, tz)
         self.ignored_range = ignored_range
         self.description = description
+        self.original_timezone = tz
 
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, val):
-        assert val.tzinfo is not None, "start must be timezone aware. Pass a tz aware datetime object, or use set_start " \
-                                       "with a tz argument, or a string like 2022-1-1 00:00+02"
-        self._start = val
+    @hybrid_property
+    def event_start(self):
+        try:
+            if self._event_start is None:
+                return self._event_start
+            elif self._event_start.tzinfo is None:
+                return pytz.timezone('utc').localize(self._event_start)
+            else:
+                return pytz.timezone('utc').normalize(self._event_start)
+        except AttributeError:
+            return self._event_start
+
+    @event_start.setter
+    def event_start(self, val):
+        _check_has_tz(val, 'start')
+        if val > self.event_end if self.event_end is not None else False:
+            raise ConfigurationError('OperationalEvent end must be after start')
+        self._event_start = pytz.timezone('utc').normalize(val)
 
     def set_start(self, val, tz=None):
         dt = to_datetime(val).to_pydatetime()
-        if tz is not None:
+        _check_tz_matches(dt, tz)
+        if tz is not None and dt.tzinfo is None:
             dt = pytz.timezone(tz).localize(dt)
-        self.start = dt
+        self.event_start = dt
 
-    @property
-    def end(self):
-        return self._end
-
-    @end.setter
-    def end(self, val):
-        assert val.tzinfo is not None, "end must be timezone aware. Pass a tz aware datetime object, or use set_end " \
-                                       "with a tz argument, or a string like 2022-1-1 00:00+02"
-        self._end = val
+    @hybrid_property
+    def event_end(self):
+        try:
+            if self._event_end is None:
+                return self._event_end
+            elif self._event_end.tzinfo is None:
+                return pytz.timezone('utc').localize(self._event_end)
+            else:
+                return pytz.timezone('utc').normalize(self._event_end)
+        except AttributeError:
+            return self._event_end
+
+    @event_end.setter
+    def event_end(self, val):
+        if val is None:
+            return
+        _check_has_tz(val, 'end')
+        if val < self.event_start if self.event_start is not None else False:
+            raise ConfigurationError('OperationalEvent end must be after start')
+        self._event_end = pytz.timezone('utc').normalize(val)
 
     def set_end(self, val, tz=None):
+        if val is None:
+            return
         dt = to_datetime(val).to_pydatetime()
-        if tz is not None:
+        _check_tz_matches(dt, tz)
+        if tz is not None and dt.tzinfo is None:
             dt = pytz.timezone(tz).localize(dt)
-        self.end = dt
+        self.event_end = dt
```

## sunpeek/components/physical.py

```diff
@@ -1,40 +1,39 @@
 import numpy as np
 import pandas as pd
-import time
-from typing import List
-from sqlalchemy.orm import relationship, Session
+from sqlalchemy.orm import relationship, Session, backref
 import sqlalchemy
-from sqlalchemy import Column, String, Integer, Enum, Identity, ForeignKey
+from sqlalchemy import Column, String, Integer, Float, Enum, ForeignKey, UniqueConstraint
 import sqlalchemy.event
 import os
-from typing import Union
+from typing import List
+import uuid
 
-from sunpeek.common.unit_uncertainty import Q
+from sunpeek.common.unit_uncertainty import Q, parse_quantity
 from sunpeek.common.errors import ConfigurationError, DuplicateNameError, SensorNotFoundError
-from sunpeek.common.utils import hit_logger
-import sunpeek.common.data_uploader
+import sunpeek.common.time_zone as tz
+# import sunpeek.common.data_uploader
 
-from sunpeek.components.helpers import ORMBase, AccuracyClass, ComponentParam, IsVirtual
+from sunpeek.components.helpers import AccuracyClass, ComponentParam, IsVirtual, DataUploadDefaults
 from sunpeek.components.operational_events import OperationalEvent
 from sunpeek.components.base import Component, SensorSlot
 from sunpeek.components.fluids import FluidFactory, FluidDefinition, UninitialisedFluid
 from sunpeek.components.sensor import Sensor
 from sunpeek.components.types import CollectorType, UninitialisedCollectorType
 from sunpeek.components import sensor_types as st
-from sunpeek.core_methods.virtuals import main as vs
 import sunpeek.db_utils.crud
 
 
-class Plant(Component, ORMBase):
+class Plant(Component):
     """
     Implements large solar thermal plant as the overarching component on which the kernel methods are applied.
 
     Attributes
     ----------
+
     name : str
         Plant name. Must be unique within HarvestIT 'plant' database.
     owner : str, optional
         Name of plant owner.
     operator : str, optional
         Name of plant operator.
     description : str, optional
@@ -43,14 +42,16 @@
         Name of the location. Example: 'Graz, Austria'
     latitude : pint Quantity
         Geographical latitude. Positive is north of the equator. See `pvlib Location`_.
     longitude : pint Quantity
         Geographical longitude. Positive is east of the prime meridian. See `pvlib Location`_.
     altitude : pint Quantity, optional
         Location altitude, e.g. Q(440, 'm'). If available, used to improve pvlib's solar position calculation.
+    data_upload_defaults : DataUploadDefaults,
+        Defaults for parsing raw data files for this plant. Defaults to an all null DataUploadDefaults
 
     fluid_solar : Fluid object
         Fluid in the solar circuit. Optional for the PC (Performance Check)
         method (but stated in the standard report, see Annex A1 in `ISO standard 24194`_),
         required for the D-CAT (Dynamic Collector Array Test) method.
     fluidvol_total : pint Quantity, optional
         Total fluid content of the solar side (including all pipes, collectors etc).
@@ -68,19 +69,19 @@
         Ambient relative humidity representative for the plant.
     te_dew_amb : Sensor, optional, or virtual Sensor
         Dew point temperature representative for the plant. Is calculated as a virtual sensor if both te_amb and
         rh_amb have data (are not None).
     pr_amb : Sensor, optional
         Ambient air pressure representative for the plant.
     te_in : Sensor, optional
-        Inlet / return temperature of the plant; this is the temperature received by all collector arrays together,
-        before the fluid enters the heat exchanger.
-    te_out : Sensor, optional
-        Outlet / flow temperature of the plant; this is the temperature after the heat exchanger, sent back to the
+        Inlet / return temperature of the plant; this is the temperature after the heat exchanger, sent back to the
         collector arrays.
+    te_out : Sensor, optional
+        Outlet / flow temperature of the plant; this is the temperature received by all collector arrays together,
+        before the fluid enters the heat exchanger.
     rd_ghi : virtual Sensor
         Global horizontal irradiance. Calculated by a radiation model from in_global, in_beam, in_diffuse, in_dni.
     rd_bhi : virtual Sensor
         Direct / beam horizontal irradiance. Calculated by a radiation model from in_global, in_beam, in_diffuse,
         in_dni.
     rd_dhi : virtual Sensor
         Diffuse horizontal irradiance. Calculated by a radiation model from in_global, in_beam, in_diffuse, in_dni.
@@ -123,52 +124,55 @@
     in_diffuse : Sensor, optional
         Diffuse radiation sensor to be used to calculate horizontal radiation components for the plant. The
         sensor may be installed at a non-zero tilt angle, in that case the horizontal radiation components will be
         calculated by a radiation model.
     in_dni : Sensor, optional
         Direct normal irradiance (DNI) sensor to be used to calculate horizontal radiation components for the plant.
 
+    References
+    ----------
     .. _pvlib:
         https://pvlib-python.readthedocs.io/en/stable/generated/pvlib.location.Location.html
     .. _IANA / tz database df_timezone string:
         https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
     .. _Timezonefinder library:
         https://github.com/jannikmi/timezonefinder
     .. _ISO standard 24194:
         https://www.iso.org/standard/78074.html
     """
+
     __tablename__ = 'plant'
 
-    id = Column(Integer, Identity(0), primary_key=True)
+    __mapper_args__ = {
+        "polymorphic_identity": "plant"
+    }
+    id = Column(Integer, ForeignKey('components.component_id'), primary_key=True)
     name = Column(String, unique=True)
     owner = Column(String)
     operator = Column(String)
     description = Column(String)
 
-    arrays = relationship(
-        "Array", back_populates="plant",
-        cascade="all, delete-orphan",
-        passive_deletes=True
-    )
+    raw_data_path = Column(String)
+    calc_data_path = Column(String)
 
-    operational_events = relationship("OperationalEvent", back_populates="plant", cascade="all, delete-orphan",
-                                      passive_deletes=True)
+    operational_events = relationship("OperationalEvent", back_populates="plant", cascade="all, delete-orphan")
 
-    latitude = ComponentParam('deg', -90, 90)
-    longitude = ComponentParam('deg', -180, 180)
+    _latitude = ComponentParam('deg', -90, 90)
+    _longitude = ComponentParam('deg', -180, 180)
+    _tz_data_offset = Column(Float)
     altitude = ComponentParam('m', -430.5, 8848.86)  # Anything between the Dead Sea and Everest
     location_name = Column(String)
 
-    fluid_solar = relationship("Fluid", back_populates='plant', uselist=False, cascade="all, delete",
-                               passive_deletes=True)
+    fluid_solar = relationship("Fluid", back_populates='plant', uselist=False, cascade="all, delete")
     fluid_vol = ComponentParam('m**3', 0, np.Inf)
 
     plant_measurement_accuracy = Column(Enum(AccuracyClass))
-    raw_sensors = relationship("Sensor", back_populates="plant", cascade="all, delete-orphan",
-                               passive_deletes=True)
+    raw_sensors = relationship("Sensor", back_populates="plant", cascade="all, delete-orphan")
+    data_upload_defaults = relationship("DataUploadDefaults", back_populates="plant", cascade="all, delete-orphan",
+                                        passive_deletes=True, uselist=False)
 
     raw_names = {}
 
     sensor_slots = {
         'tp': SensorSlot('tp', st.thermal_power,
                          'Thermal power', IsVirtual.possible,
                          description='Total thermal power of the plant, including all its collector arrays.'),
@@ -176,20 +180,20 @@
                          'Volume flow', IsVirtual.never,
                          description='Total volume flow in the solar circuit of the plant, for all collector arrays.'),
         'mf': SensorSlot('mf', st.mass_flow,
                          'Mass flow', IsVirtual.possible,
                          description='Total mass flow in the solar circuit of the plant, for all collector arrays.'),
         'te_in': SensorSlot('te_in', st.fluid_temperature,
                             'Inlet temperature', IsVirtual.never,
-                            description='Inlet / return temperature of the plant; this is the temperature received by '
-                                        'all collector arrays together, before the fluid enters the heat exchanger.'),
+                            description='Inlet / return temperature of the plant; this is the temperature after the '
+                                        'heat exchanger, sent back to the collector arrays.'),
         'te_out': SensorSlot('te_out', st.fluid_temperature,
                              'Outlet temperature', IsVirtual.possible,
-                             description='Outlet / flow temperature of the plant; this is the temperature after the '
-                                         'heat exchanger, sent back to the collector arrays.'),
+                             description='Inlet / return temperature of the plant; this is the temperature received by '
+                                         'all collector arrays together, before the fluid enters the heat exchanger.'),
         'te_amb': SensorSlot('te_amb', st.ambient_temperature,
                              'Ambient temperature', IsVirtual.never,
                              description='Ambient air temperature representative for the plant.'),
         've_wind': SensorSlot('ve_wind', st.wind_speed,
                               'Wind speed', IsVirtual.never,
                               description='Wind speed / wind velocity representative for the plant.'),
         'rh_amb': SensorSlot('rh_amb', st.float_0_1,
@@ -279,97 +283,149 @@
 
     def __init__(self, name=None, owner=None, operator=None, description=None, plant_measurement_accuracy=None,
                  location_name=None, latitude=None, longitude=None, altitude=Q(100, "m"),
                  fluid_solar=None, fluidvol_total=None, arrays=[], sensor_map={}, raw_sensors=[],
                  **kwargs):
 
         # to change plant context, explicitly attach a different Context object to plant in the calling code
-        from sunpeek.common.context import Context
+        from sunpeek.data_handling.context import Context
         self.context = Context(plant=self)
 
-        self.defer_configure_virtuals = True
-        self.name = name
+        self.defer_post_config_changed_actions = True
+        # TODO Remove
+        # self.defer_configure_virtuals = True
+
+        if name is not None:
+            self.name = name
+        else:
+            self.name = str(uuid.uuid4().hex[0:12])
         self.owner = owner
         self.operator = operator
         self.description = description
         self.plant_measurement_accuracy = plant_measurement_accuracy
         self.location_name = location_name
+        self._tz_data_offset = None
         self.latitude = latitude
         self.longitude = longitude
         self.altitude = altitude
 
         self.raw_sensors = raw_sensors
         self.fluid_solar = fluid_solar
         self.fluidvol_total = fluidvol_total
         self.arrays = arrays
 
+        self.raw_data_path = os.environ.get('SUNPEEK_RAW_DATA_PATH', './raw_data') + '/' + self.name
+        self.calc_data_path = os.environ.get('SUNPEEK_CALC_DATA_PATH', './calc_data') + '/' + self.name
+
+        self.data_upload_defaults = DataUploadDefaults()
+
         self.sensor_map = sensor_map
         if len(kwargs) > 0:
             self.set_sensors(**kwargs)
         else:
-            self.defer_configure_virtuals = False
-            self.config_virtuals()
+            self.defer_post_config_changed_actions = False
+            [func(self.plant) for func in self.plant.post_config_changed_callbacks]
 
     def add_array(self, arrays):
         """
         Convenience method for adding items to plant.arrays. Equivalent to plant.arrays += array or plant.arrays.append(array).
+
         Parameters
         ----------
-        arrays: Array or list of Array
+        arrays : `~sunpeek.components.physical.Array` or list of `~sunpeek.components.physical.Array`
 
         Returns
         -------
-        Updated list of arrays
+        Updated list of `~sunpeek.components.physical.Array` objects for the plant
         """
         if isinstance(arrays, Array):
             arrays = [arrays]
         for array in arrays:
             self.arrays.append(array)
         return self.arrays
 
     @sqlalchemy.orm.reconstructor
     def _init_on_load(self):
         # create default Context object
-        from sunpeek.common.context import Context
-        self.context = Context(plant=self, datasource='db')
+        from sunpeek.data_handling.context import Context
+        self.context = Context(plant=self, datasource='pq')
+
+    @property
+    def latitude(self):
+        return self._latitude
 
-    @sqlalchemy.orm.validates('arrays')
-    def _validate_arrays(self, attr_name, component):
-        """ used to automatically convert array dict represntations to components and
-        set sensors to plant when an array is added to the plant"""
+    @property
+    def longitude(self):
+        return self._longitude
+
+    @latitude.setter
+    def latitude(self, val):
+        val = parse_quantity(val)
+        if (val is not None) and (self.longitude is not None):
+            self._tz_data_offset = tz.get_timezone_offset_minutes(latitude=val, longitude=self.longitude)
+        self._latitude = val
+
+    @longitude.setter
+    def longitude(self, val):
+        val = parse_quantity(val)
+        if (val is not None) and (self.latitude is not None):
+            self._tz_data_offset = tz.get_timezone_offset_minutes(latitude=self.latitude, longitude=val)
+        self._longitude = val
+
+    @property
+    def tz_data(self):
+        return tz.get_data_timezone(self._tz_data_offset)
+
+    @property
+    def local_tz_string_with_DST(self):
+        if (self.latitude is None) or (self.longitude is None):
+            return None
+        return tz.get_timezone_string(latitude=self.latitude, longitude=self.longitude)
+
+    @sqlalchemy.orm.validates('arrays', include_removes=True)
+    def _validate_arrays(self, attr_name, component, is_remove):
+        """ Used to automatically convert array dict representations to components and
+        set sensors to plant when an array is added to the plant
+        """
         if isinstance(component, dict):
             return Array(plant=self, **component)
-        for sensor in component.sensors.values():
-            sensor.plant = self
+
+        component = component.update_sensors(is_remove=is_remove)
+
         return component
 
     @sqlalchemy.orm.validates('fluid_solar')
     def _validate_fluids(self, _, component):
-        """ used to automatically convert array dict represntations to components and
-        set sensors to plant when an array is added to the plant"""
+        """ Used to automatically convert fluid dict representations when a fluid is added to the plant.
+        """
         if isinstance(component, dict):
             return FluidFactory(**component)
         return component
 
-    @property
-    def raw_table_name(self):
-        return f"raw_data_{self.name.replace(' ', '_').lower()}"
+    @sqlalchemy.orm.validates('data_upload_defaults')
+    def _validate_data_upload_defaults(self, _, component):
+        """ Used to automatically convert dict representation to DataUploadDefaults object.
+        """
+        if isinstance(component, dict):
+            return DataUploadDefaults(**component)
+        return component
 
     @property
     def plant(self):
         return self
 
     @property
     def ignored_ranges(self) -> List[pd.Interval]:
         """Gets a list of time ranges to be ignored from the plant's `operational_events`
         """
         intervals = []
         for event in self.operational_events:
             if event.ignored_range:
-                intervals.append(pd.Interval(pd.to_datetime(event.start), pd.to_datetime(event.end), closed='both'))
+                intervals.append(
+                    pd.Interval(pd.to_datetime(event.event_start), pd.to_datetime(event.event_end), closed='both'))
 
         return list(set(intervals))
 
     def is_ignored(self, timestamp):
         """
         Checks if a timestamp is in an ignored range
 
@@ -395,172 +451,26 @@
         """
         Parameters
         ----------
         start : A datetime object, or a string. If the string does not contain a df_timezone like '2022-1-1 00:00+1',
             then the tz argument must also be specified.
         end : A datetime object, or a string. If the string does not contain a df_timezone like '2022-1-2 00:00+1',
             then the tz argument must also be specified.
-        tz : A df_timezone string like 'Europe/Vienna'
+        tz : A df_timezone string like 'Europe/Vienna' or any pytz time zone, like pytz.FixedOffset(60)
         description : str
             A description of the event or reason for ignored range.
         ignored_range : bool
             If data in the period specified in the event should be ignored
         """
-        if description is None:
-            raise ConfigurationError('Operational Events must have a description')
-        self.operational_events.append(
-            OperationalEvent(start=start, end=end, tz=tz, ignored_range=ignored_range, description=description,
-                             plant=self))
+
+        OperationalEvent(event_start=start, event_end=end, tz=tz, ignored_range=ignored_range, description=description,
+                         plant=self)
         if ignored_range:
             self.context.reset_cache()
 
-    def config_virtuals(self):
-        """Creates & maps virtual sensors for all components.
-        Raises
-        ------
-        VirtualSensorConfigurationError
-        """
-        self.config_virtuals_ambient()
-        self.config_virtuals_power()
-        self.config_virtuals_radiation_conversion()
-
-        for array in self.arrays:
-            array.config_virtuals_ambient()
-            array.config_virtuals_temperature()
-            array.config_virtuals_radiation_conversion()
-            # array.config_virtuals_te_out()
-
-    def calculate_virtuals(self, strategy_array_irradiance='feedthrough'):
-        """Implements all the logic of the virtual sensor calculation. Called as new data arrive.
-
-        Raises
-        ------
-        VirtualSensorCalculationError
-
-        Notes
-        -----
-        At the end of this method, there might be virtual sensors that have not been calculated, whatever the reason.
-        When queried for data (e.g. uncalculated_vsensor.data), Context.get_sensor_data() returns
-        an all-NaN series in the correct unit.
-        """
-        self.config_virtuals()
-        start_time = time.time()
-
-        hit_logger.info(f"[calculate_virtuals] Calculating virtual sensors data.")
-        self.context.verify_time_index()
-
-        self.calculate_virtuals_ambient()
-        self.calculate_virtuals_power()
-        self.calculate_virtuals_radiation_conversion()
-
-        # Arrays
-        for array in self.arrays:
-            array.calculate_virtuals_ambient()
-            array.calculate_virtuals_temperature()
-            array.calculate_virtuals_radiation_conversion(strategy=strategy_array_irradiance)
-            # array.calculate_virtuals_te_out()
-
-        hit_logger.info(f"[calculate_virtuals] --- Done after {(time.time() - start_time)} seconds ---")
-
-    def config_virtuals_ambient(self):
-        """Solar position, airmass, clearsky radiation, dew point"""
-        can_calculate = vs.CalcSolarPosition(self).verify_config()
-        self.map_vsensor('sun_azimuth', can_calculate)
-        self.map_vsensor('sun_zenith', can_calculate)
-        self.map_vsensor('sun_apparent_zenith', can_calculate)
-        self.map_vsensor('sun_elevation', can_calculate)
-        self.map_vsensor('sun_apparent_elevation', can_calculate)
-
-        # Dew point temperature
-        self.map_vsensor('te_dew_amb', can_calculate=vs.CalcDewPointTemperature(self).verify_config())
-
-        # Clearsky solar radiation
-        self.map_vsensor('rd_dni_extra', can_calculate=True)
-
-        # Airmass
-        can_calculate = vs.CalcAirmass(self).verify_config()
-        self.map_vsensor('rel_airmass', can_calculate)
-        self.map_vsensor('abs_airmass', can_calculate)
-
-        # Turbidity
-        self.map_vsensor('linke_turbidity', can_calculate=vs.CalcLinkeTurbidity(self).verify_config())
-
-        # Clearsky radiation
-        can_calculate = vs.CalcClearskyRadiation(self).verify_config()
-        self.map_vsensor('rd_ghi_clearsky', can_calculate)
-        self.map_vsensor('rd_dni_clearsky', can_calculate)
-
-    def calculate_virtuals_ambient(self):
-        azimuth, zenith, apparent_zenith, elevation, apparent_elevation = vs.CalcSolarPosition(self).calc()
-        self.sun_azimuth.update(azimuth)
-        self.sun_zenith.update(zenith)
-        self.sun_apparent_zenith.update(apparent_zenith)
-        self.sun_elevation.update(elevation)
-        self.sun_apparent_elevation.update(apparent_elevation)
-
-        # Dew point temperature
-        if (self.te_dew_amb is not None) and self.te_dew_amb.is_virtual:
-            te_dew_amb = vs.CalcDewPointTemperature(self).calc()
-            self.te_dew_amb.update(te_dew_amb)
-
-        # Clearsky solar radiation
-        dni_extra = vs.CalcDNIExtra(self).calc()
-        self.rd_dni_extra.update(dni_extra)
-
-        # Airmass
-        rel_airmass, abs_airmass = vs.CalcAirmass(self).calc()
-        self.rel_airmass.update(rel_airmass)
-        self.abs_airmass.update(abs_airmass)
-
-        # Turbidity
-        linke_turbidity = vs.CalcLinkeTurbidity(self).calc()
-        self.linke_turbidity.update(linke_turbidity)
-
-        # Clearsky radiation
-        ghi_clearsky, dni_clearsky = vs.CalcClearskyRadiation(self).calc()
-        self.rd_ghi_clearsky.update(ghi_clearsky)
-        self.rd_dni_clearsky.update(dni_clearsky)
-
-    def config_virtuals_power(self):
-        """Thermal power and mass flow"""
-        # Thermal power from volume flow: Allow that tp cannot be calculated, let downstream verify() methods check
-        self.map_vsensor('tp', can_calculate=vs.CalcPowerFromVolumeFlow(self).verify_config())
-
-        # Mass flow
-        self.map_vsensor('mf', can_calculate=vs.CalcMassFlowFromPower(self).verify_config())
-
-    def calculate_virtuals_power(self):
-        # Thermal power
-        if (self.tp is not None) and self.tp.is_virtual:
-            tp = vs.CalcPowerFromVolumeFlow(self).calc()
-            self.tp.update(tp)
-
-        # Mass flow
-        if (self.mf is not None) and self.mf.is_virtual:
-            mf = vs.CalcMassFlowFromPower(self).calc()
-            self.mf.update(mf)
-
-    def config_virtuals_radiation_conversion(self):
-        """Horizontal irradiance components from plant radiation input slots
-        """
-        can_calculate = vs.CalcHorizontalIrradiances(self).verify_config()
-        self.map_vsensor('rd_ghi', can_calculate)
-        self.map_vsensor('rd_bhi', can_calculate)
-        self.map_vsensor('rd_dhi', can_calculate)
-        self.map_vsensor('rd_dni', can_calculate)
-
-    def calculate_virtuals_radiation_conversion(self):
-        """Horizontal irradiance components from plant radiation input slots
-        """
-        ghi, bhi, dhi, dni = vs.CalcHorizontalIrradiances(self).calc()
-        self.rd_ghi.update(ghi)
-        self.rd_bhi.update(bhi)
-        self.rd_dhi.update(dhi)
-        self.rd_dni.update(dni)
-
     @property
     def radiation_input_slots(self):
         return self.in_global, self.in_beam, self.in_diffuse, self.in_dni
 
     @property
     def area_gr(self):
         return sum([a.area_gr for a in self.arrays])
@@ -569,17 +479,19 @@
     def area_ap(self):
         return sum([a.area_ap for a in self.arrays])
 
     @property
     def time_index(self):
         return self.context.time_index
 
-    @sqlalchemy.orm.validates('raw_sensors')
-    def _validate_raw_sensors(self, _, val):
+    @sqlalchemy.orm.validates('raw_sensors', include_removes=True)
+    def _validate_raw_sensors(self, _, val, is_remove):
         # assert isinstance(val, list), "raw_sensors must be a list of Sensor objects or dicts"
+        if is_remove:
+            val.remove_references(include_plant=False)
         if isinstance(val, dict):
             val = Sensor(**val)
         return val
 
     def get_raw_sensor(self, raw_name, raise_if_not_found=False):
         session = sqlalchemy.orm.object_session(self)
         if raw_name is None:
@@ -593,63 +505,23 @@
                 return sunpeek.db_utils.crud.get_sensors(session, plant_id=self.id, raw_name=raw_name)
             except (sqlalchemy.exc.NoResultFound, sqlalchemy.exc.MultipleResultsFound):
                 pass
         if raise_if_not_found:
             raise SensorNotFoundError(f"Either no sensor with raw_name '{raw_name}' was found, "
                                       f"or more than one such sensor was")
 
-    def get_raw_names(self, include_virtuals=False):
+    def get_raw_names(self, include_virtuals=False, only_virtuals=False):
         if include_virtuals:
             return [sensor.raw_name for sensor in self.raw_sensors]
-        else:
-            return [sensor.raw_name for sensor in self.raw_sensors if not sensor.is_virtual]
+        if only_virtuals:
+            return [sensor.raw_name for sensor in self.raw_sensors if (sensor.is_virtual and sensor.can_calculate)]
+        return [sensor.raw_name for sensor in self.raw_sensors if not sensor.is_virtual]
 
-    def validate_sensors(self):
-        assert self.context.datasource == 'df', \
-            'Can only call plant.validate_sensors() if plant.context datasource is "df" (DataFrame).'
-        sensor_validation = self.context.validate_sensors(self.context.df)
-        return sensor_validation
-
-    def use_dataframe(self, df: pd.DataFrame,
-                      calculate_virtuals: bool = True,
-                      **kwargs):
-        """Uses a dataframe as plant datasource. Includes configurable sanity checks on the given DataFrame.
 
-        Parameters
-        ----------
-        df : DataFrame to use as backend
-        calculate_virtuals : bool. Whether virtual sensor calculation should be triggered (might be slow).
-
-        Returns
-        -------
-        sensor_validation : dict, if calculate_sensor_validation == True, else nothing.
-        """
-        self.context.use_dataframe(df, **kwargs)
-        if calculate_virtuals:
-            self.calculate_virtuals()
-        sensor_validation = self.validate_sensors()
-
-        return sensor_validation
-
-    def use_csv(self,
-                csv_files: List[Union[str, os.PathLike]],
-                calculate_virtuals: bool = True,
-                **kwargs):
-        """Ingest csv files, calculate virtual sensors, set Context datasource to dataframe.
-
-        Returns
-        -------
-        import_info : DataUploadResponse, response from data upload process.
-        """
-        up = sunpeek.common.data_uploader.DataUploader_df(plant=self, files=csv_files, **kwargs)
-        up.do_upload(calculate_virtuals)
-        return up.output
-
-
-class Array(Component, ORMBase):
+class Array(Component):
     """
     Implements collector array with given area, homogeneous tilt and azimuth angles and exactly 1 collector_type.
 
     Attributes
     ----------
     name : str
         Name of array. Must be unique within parent plant.
@@ -760,20 +632,25 @@
 
     .. _Fixed Mount:
         https://pvlib-python.readthedocs.io/en/stable/generated/pvlib.pvsystem.FixedMount.html#pvlib.pvsystem.FixedMount
     """
 
     __tablename__ = 'arrays'
 
-    id = Column(Integer, Identity(0), primary_key=True)
+    __mapper_args__ = {
+        "polymorphic_identity": "array"
+    }
+
+    id = Column(Integer, ForeignKey('components.component_id'), primary_key=True)
+
     plant_id = Column(Integer, ForeignKey('plant.id', ondelete="CASCADE"))
-    plant = relationship("Plant", back_populates="arrays")
+    plant = relationship("Plant", foreign_keys=[plant_id], backref=backref("arrays", cascade="all, delete"))
     name = Column(String)
     collector_type_id = Column(Integer, ForeignKey('collector_types.id'))
-    _collector_type = relationship("CollectorType")
+    _collector_type = relationship("CollectorType", passive_deletes='all')
 
     area_gr = ComponentParam('m**2', 1, np.Inf)
     area_ap = ComponentParam('m**2', 1, np.Inf)
     azim = ComponentParam('deg', 0, 360)
     tilt = ComponentParam('deg', 0, 90)
     row_spacing = ComponentParam('m', 0, np.Inf)
     n_rows = ComponentParam('', 0, np.Inf)
@@ -782,15 +659,15 @@
     fluidvol_total = ComponentParam('m**3', 0, np.Inf)
     rho_ground = ComponentParam('', 0, 1)
     rho_colbackside = ComponentParam('', 0, 1)
     rho_colsurface = ComponentParam('', 0, 1)
     max_aoi_shadow = ComponentParam('deg', 30, 90)
     min_elevation_shadow = ComponentParam('deg', 0, 90)
 
-    # sensor_map = association_proxy("")
+    __table_args__ = (UniqueConstraint('name', 'plant_id', name='_unique_array_names_per_plant'),)
 
     sensor_slots = {
         'tp': SensorSlot('tp', st.thermal_power,
                          'Thermal power', IsVirtual.possible,
                          description='Thermal power of collector array.'),
         'vf': SensorSlot('vf', st.volume_flow,
                          'Volume flow', IsVirtual.never,
@@ -879,15 +756,15 @@
     }
 
     def __init__(self, name=None, plant=None, collector_type=None, area_gr=None, area_ap=None, azim=None, tilt=None,
                  row_spacing=None, n_rows=None, ground_tilt=Q(0, 'deg'), mounting_level=Q(0, 'm'),
                  fluidvol_total=None, rho_ground=None, rho_colbackside=None, rho_colsurface=Q(0),
                  max_aoi_shadow=Q(80, 'deg'), min_elevation_shadow=None, sensor_map={}, **kwargs):
 
-        self.defer_configure_virtuals = True
+        self.defer_post_config_changed_actions = True
         self.name = name
         self.collector_type = collector_type
 
         self.area_ap = area_ap
         self.area_gr = area_gr if area_gr is not None else self.calc_area_gr_from_collector()
         self.azim = azim
         self.tilt = tilt
@@ -904,15 +781,15 @@
         self.max_aoi_shadow = max_aoi_shadow
         self.min_elevation_shadow = min_elevation_shadow
         self.plant = plant
         self.sensor_map = sensor_map
         if len(kwargs) > 0:
             self.set_sensors(**kwargs)
 
-        self.defer_configure_virtuals = False
+        self.defer_post_config_changed_actions = False
 
     def calc_area_gr_from_collector(self):
         """Set array.area_gr from area_ap and collector_type information, if None
         """
         coll = self.collector_type
         if (self.area_ap is None) or (coll is None) or isinstance(coll, UninitialisedCollectorType):
             return None
@@ -928,103 +805,43 @@
     def collector_type(self):
         return self._collector_type
 
     @collector_type.setter
     def collector_type(self, value):
         if isinstance(value, CollectorType):
             self._collector_type = value
+        elif isinstance(value, str) and sqlalchemy.orm.object_session(self) is not None:
+            _convert_to_concrete_col_type(sqlalchemy.orm.object_session(self), self, 'collector_type',
+                                          UninitialisedCollectorType(value, parent=self, attribute='collector_type'))
         elif isinstance(value, str):
             self._collector_type = UninitialisedCollectorType(value, parent=self, attribute='collector_type')
         elif value is None:
             self._collector_type = None
         else:
             raise ConfigurationError("collector_type must be a CollectorType object, or the name of an existing "
                                      "collector_type")
 
     @property
     def fluid_solar(self):
         return self.plant.fluid_solar
 
-    def config_virtuals_ambient(self):
-        """Basic virtual sensors for sun- and shadow-related stuff in array:
-        Angle of incidence, is_shadowed, shadow angle, internal shading ratio"""
-        self.map_vsensor('aoi', can_calculate=vs.CalcAngleOfIncidence(self).verify_config())
-
-        can_calculate = vs.CalcInternalShading(self).verify_config()
-        self.map_vsensor('is_shadowed', can_calculate)
-        self.map_vsensor('internal_shading_ratio', can_calculate)
-        self.map_vsensor('shadow_angle', can_calculate)
-        self.map_vsensor('shadow_angle_midpoint', can_calculate)
-
-    def calculate_virtuals_ambient(self):
-        """Calculate general sun related array virtual sensors."""
-        # Angle of incidence
-        aoi = vs.CalcAngleOfIncidence(self).calc()
-        self.aoi.update(aoi)
-
-        # Shade ratio, shadow angle
-        is_shadowed, internal_shading_ratio, shadow_angle, shadow_angle_midpoint = vs.CalcInternalShading(self).calc()
-        if (self.is_shadowed is not None) and self.is_shadowed.is_virtual:
-            self.is_shadowed.update(is_shadowed)
-        self.internal_shading_ratio.update(internal_shading_ratio)
-        self.shadow_angle.update(shadow_angle)
-        self.shadow_angle_midpoint.update(shadow_angle_midpoint)
-
-    def config_virtuals_temperature(self):
-        """Virtual sensors for mean operating temperature, derivative etc.
-        """
-        can_calculate = vs.CalcArrayTemperatures(self).verify_config()
-        self.map_vsensor('te_op', can_calculate)
-        self.map_vsensor('te_op_deriv', can_calculate)
-
-    def calculate_virtuals_temperature(self):
-        te_op, te_op_deriv = vs.CalcArrayTemperatures(self).calc()
-        self.te_op.update(te_op)
-        self.te_op_deriv.update(te_op_deriv)
-
-    def config_virtuals_radiation_conversion(self):
-        """Virtual sensors for plane-of-array irradiance (global, beam, diffuse) including masking,
-        shading etc."""
-        can_calculate = vs.CalcTiltedIrradiances(self).verify_config()
-        self.map_vsensor('rd_gti', can_calculate)
-        self.map_vsensor('rd_bti', can_calculate)
-        self.map_vsensor('rd_dti', can_calculate)
-
-        self.map_vsensor('iam', can_calculate=vs.CalcIAM(self).verify_config())
-
-    def calculate_virtuals_radiation_conversion(self, strategy):
-        # array irradiance components, including beam shading and diffuse masking
-        gti, bti, dti = vs.CalcTiltedIrradiances(self, strategy).calc()
-        self.rd_gti.update(gti)
-        self.rd_bti.update(bti)
-        self.rd_dti.update(dti)
-
-        if (self.iam is not None) and self.iam.is_virtual:
-            iam = vs.CalcIAM(self).calc()
-            self.iam.update(iam)
-
-    # TODO virtual array.te_out required for St Ruprecht test plant?
-    # def config_virtuals_te_out(self):
-    #     """Average array `te_out` from outlet temperatures of several array row outlet temperatures."""
-    #     self.map_vsensor('te_out', can_calculate=True)
-    #
-    # def calculate_virtuals_te_out(self):
-    #     """Average array `te_out` from outlet temperatures of several rows that make up the array."""
-    #     if (self.te_out is not None) and self.te_out.is_virtual:
-    #         # te_out = vs.get_average_from_many(self.te_out)
-    #         self.te_out.update(None)
-
-    def get_orientation(self):
-        """Returns dictionary with array's "tilt" and "azim" values converted to deg, for radiation calculations.
+    @property
+    def orientation(self):
+        """Return dictionary with array's "tilt" and "azim" values converted to deg, for radiation calculations.
         """
         return {'tilt': self.tilt.m_as('deg'),
                 'azim': self.azim.m_as('deg')}
 
+    def has_orientation(self):
+        """Returns True if array has tilt and azimuth well-defined. Useful for radiation calculations.
+        """
+        return (self.tilt is not None) and (self.azim is not None)
+
 
-class HeatExchanger(Component, ORMBase):
+class HeatExchanger(Component):
     """
     Implements a heat exchangers including references to its hot- and cold-side fluids.
 
     Attributes
     ----------
     plant : Plant object
         Plant to which the heat exchanger belongs.
@@ -1033,35 +850,46 @@
     fluid_cold : Sensor, optional
         Fluid on the cold side of the heat exchanger (often water).
     ua_nom : pint Quantity, optional
         Nominal heat transfer coefficient.
     """
     __tablename__ = 'heat_exchangers'
 
-    id = Column(Integer, Identity(0), primary_key=True)
+    __mapper_args__ = {
+        "polymorphic_identity": "heat_exchanger"
+    }
+
+    id = Column(Integer, ForeignKey('components.component_id'), primary_key=True)
+
     plant_id = Column(Integer, ForeignKey('plant.id', ondelete="CASCADE"))
-    plant = relationship("Plant")
+    plant = relationship("Plant", foreign_keys=[plant_id],
+                         backref=backref("heat_exchangers", cascade="all, delete-orphan"))
     fluid_hot_id = Column(Integer, ForeignKey('fluids.id'))
     fluid_hot = relationship("Fluid", foreign_keys=[fluid_hot_id],
                              cascade="all, delete", uselist=False, passive_deletes=True)
     fluid_cold_id = Column(Integer, ForeignKey('fluids.id'))
     fluid_cold = relationship("Fluid", foreign_keys=[fluid_cold_id],
                               cascade="all, delete", uselist=False, passive_deletes=True)
     name = Column(String)
 
     ua_nom = ComponentParam('kW K**-1', 0, np.Inf)
 
     def __init__(self, name, plant, fluid_hot=None, fluid_cold=None, ua_nom=None):
-        self.defer_configure_virtuals = True
+        self.defer_post_config_changed_actions = True
         self.name = name
         self.plant = plant
         self.fluid_hot = fluid_hot
         self.fluid_cold = fluid_cold
         self.ud_nom = ua_nom
-        self.defer_configure_virtuals = False
+        self.defer_post_config_changed_actions = False
+
+
+# class RawData(ORMBase):
+#     ts = Column(DateTime(timezone=True))
+#     raw_name = Column(String)
 
 
 def _check_duplicate_col_type_defs(session, inst):
     try:
         db_col_type = session.query(CollectorType).filter(CollectorType.name == inst.name).one()
         if inst == db_col_type:
             return True
```

## sunpeek/components/results.py

```diff
@@ -1,73 +1,80 @@
 from sqlalchemy.orm import relationship
-from sqlalchemy import Column, String, Float, Integer, Identity, ForeignKey, DateTime, Enum, Interval, Boolean, ARRAY
+from sqlalchemy import Column, String, Float, Integer, Identity, ForeignKey, DateTime, Enum, Interval, Boolean, ARRAY, JSON
 from sunpeek.components.helpers import ORMBase, ComponentParam, AttrSetterMixin
-from sunpeek.components import Plant, Fluid
+from sunpeek.components import Fluid
 
 
 class PCMethodOutput(ORMBase, AttrSetterMixin):
     __tablename__ = 'pc_method_outputs'
 
     id = Column(Integer, Identity(0), primary_key=True)
 
     plant_id = Column(Integer, ForeignKey('plant.id'))
     plant = relationship("Plant")
 
     datetime_eval_start = Column(DateTime(timezone=True))
     datetime_eval_end = Column(DateTime(timezone=True))
 
-    # TODO Move these to the calling job, once we have a job system for PC calls
-    # datetime_job_start = Column(DateTime(timezone=True), primary_key=True)
-    # datetime_job_done = Column(DateTime(timezone=True), primary_key=True)
-
-    # Algorithm settings
+    # Algorithm / Strategy
     pc_method_name = Column(String)  # The version of the PC method used to reflect the plant hydraulic layout
-    evaluation_mode = Column(Enum('ISO', 'improved', name='pc_evaluation_modes'))
+    evaluation_mode = Column(Enum('ISO', 'extended', name='pc_evaluation_modes'))
     equation = Column(Integer)
-    check_accuracy_level = Column(Integer)
-
-    interval_length = Column(Interval)
-    safety_combined = Column(Float)
     wind_used = Column(Boolean)
 
-    max_nan_density = Column(Float)
-    min_data_in_interval = Column(Integer)
-    max_gap_in_interval = Column(Interval)
+    # PCSettings
+    settings = Column(JSON)
+
+    # Plant results
+    plant_output = relationship("PCMethodOutputPlant", uselist=False)
+
+    # Array results
+    array_output = relationship("PCMethodOutputArray")
+
+
+class PCMethodOutputPlant(ORMBase, AttrSetterMixin):
+    __tablename__ = 'pc_results_plant'
+
+    id = Column(Integer, Identity(0), primary_key=True)
+    parent_result_id = Column(Integer, ForeignKey('pc_method_outputs.id', ondelete="CASCADE"))
+
+    plant_id = Column(Integer, ForeignKey('plant.id'))
+    plant = relationship("Plant")
 
-    # Results
     n_intervals = Column(Integer)
 
-    datetime_intervals_start = Column(ARRAY(DateTime(timezone=True)))
-    datetime_intervals_end = Column(ARRAY(DateTime(timezone=True)))
+    datetime_intervals_start = Column(JSON)
+    datetime_intervals_end = Column(JSON)
 
-    # Plant results
-    tp_measured = ComponentParam('W', type='array')
-    tp_sp_measured = ComponentParam('W m**-2', type='array')
-    tp_sp_expected = ComponentParam('W m**-2', type='array')
-    tp_sp_expected_safety = ComponentParam('W m**-2', type='array')
+    tp_measured = ComponentParam('W', param_type='array')
+    tp_sp_measured = ComponentParam('W m**-2', param_type='array')
+    tp_sp_estimated = ComponentParam('W m**-2', param_type='array')
+    tp_sp_estimated_safety = ComponentParam('W m**-2', param_type='array')
+    mean_tp_sp_measured = ComponentParam('W m**-2')
+    mean_tp_sp_estimated = ComponentParam('W m**-2')
+    mean_tp_sp_estimated_safety = ComponentParam('W m**-2')
 
     target_actual_slope = ComponentParam('')
     target_actual_slope_safety = ComponentParam('')
 
-    # Array results
-    array_results = relationship("PCMethodOutputArray")
-
     fluid_solar_id = Column(ForeignKey(Fluid.id))
     fluid_solar = relationship("Fluid")
     mean_temperature = ComponentParam('K')
     mean_fluid_density = ComponentParam('kg m**-3')
     mean_fluid_heat_capacity = ComponentParam('J kg**-1 K**-1')
 
 
 class PCMethodOutputArray(ORMBase, AttrSetterMixin):
     __tablename__ = 'pc_results_arrays'
 
     id = Column(Integer, Identity(0), primary_key=True)
     parent_result_id = Column(Integer, ForeignKey('pc_method_outputs.id', ondelete="CASCADE"))
-    # parent_result = relationship("PCMethodOutput", back_populates="array_results")
 
     array_id = Column(ForeignKey('arrays.id'))
     array = relationship("Array")
 
-    tp_sp_measured = ComponentParam('W m**-2', type='array')
-    tp_sp_expected = ComponentParam('W m**-2', type='array')
-    tp_sp_expected_safety = ComponentParam('W m**-2', type='array')
+    tp_sp_measured = ComponentParam('W m**-2', param_type='array')
+    tp_sp_estimated = ComponentParam('W m**-2', param_type='array')
+    tp_sp_estimated_safety = ComponentParam('W m**-2', param_type='array')
+    mean_tp_sp_measured = ComponentParam('W m**-2')
+    mean_tp_sp_estimated = ComponentParam('W m**-2')
+    mean_tp_sp_estimated_safety = ComponentParam('W m**-2')
```

## sunpeek/components/sensor.py

```diff
@@ -1,16 +1,18 @@
+import warnings
 import pandas as pd
 import sqlalchemy
 from sqlalchemy import Column, String, Integer, ForeignKey, Boolean, Enum, Identity, JSON
 from sqlalchemy.orm import relationship
+from sqlalchemy.ext.associationproxy import association_proxy
 
 import sunpeek.common.unit_uncertainty as uu
 from sunpeek.common.unit_uncertainty import Q, units
-from sunpeek.common.errors import ConfigurationError, VirtualSensorConfigurationError, VirtualSensorCalculationError, DuplicateNameError
-from sunpeek.common.utils import hit_logger
+from sunpeek.common.errors import ConfigurationError, CalculationError, DuplicateNameError
+from sunpeek.common.utils import sp_logger
 from sunpeek.components.helpers import ORMBase, AttrSetterMixin, AccuracyClass, InstallCondition, ComponentParam
 from sunpeek.components import sensor_types as st
 
 
 class SensorInfo(ORMBase):
     __tablename__ = 'sensorinfo'
 
@@ -85,89 +87,118 @@
     plant = relationship("Plant", back_populates='raw_sensors')
     _given_sensor_type = Column(String)
     # hardware_type_id = Column(Integer, ForeignKey('hardware_types.id'))
     # hardware_type = relationship("HardwareType")
     description = Column(String)
     _native_unit = Column(String)
     is_virtual = Column(Boolean, nullable=False)
-    # is_calculated = Column(Boolean, nullable=False)
-    can_calculate = Column(Boolean, nullable=False)
+    can_calculate = Column(Boolean, nullable=True)
+
     _accuracy_class = Column(Enum(AccuracyClass))
     _installation_condition = Column(Enum(InstallCondition))
     _lower_replace_min = ComponentParam('no_check')
     _lower_replace_max = ComponentParam('no_check')
     lower_replace_value = ComponentParam('no_check')
     _upper_replace_min = ComponentParam('no_check')
     _upper_replace_max = ComponentParam('no_check')
     upper_replace_value = ComponentParam('no_check')
     info = relationship("SensorInfo", back_populates='sensor', uselist=False, cascade="all, delete",
                         passive_deletes=True, )
+    # map_ids = Column(Integer, ForeignKey('sensor_map.id', ondelete="CASCADE"))
+    mappings = relationship("SensorMap", back_populates='sensor', cascade="all, delete")
+    mapped_components = association_proxy("mappings", "component")
 
     __table_args__ = (
         sqlalchemy.UniqueConstraint('raw_name', 'plant_id'),
     )
 
     def __init__(self, raw_name, native_unit, plant=None, description=None, accuracy_class=None,
                  installation_condition=None, hardware_type=None, sensor_type=None,
-                 is_virtual=False, can_calculate=False, value_replacements={}, info={}):
+                 is_virtual=False, problems=None, can_calculate=None, value_replacements=None, info={}):
         self.raw_name = raw_name
         self.description = description
         self.accuracy_class = accuracy_class
         self._installation_condition = installation_condition
         self.plant = plant
         self.info = info
         self.hardware_type = hardware_type
+        self._sensor_type = None  # Never persisted in DB, used for in memory custom s_types and overrides.
         self.sensor_type = sensor_type
         self.is_virtual = is_virtual
+        self.problems = problems
         self.can_calculate = can_calculate
-        # self.is_calculated = False
         self.info = info
         self.native_unit = native_unit
-        self.value_replacements = value_replacements
+        if value_replacements is not None:
+            self.value_replacements = value_replacements
+        elif value_replacements is None and sensor_type is None:
+            self.value_replacements = {}
+
+    @sqlalchemy.orm.reconstructor
+    def _init_on_load(self):
+        self._sensor_type = None
+        self._problems = None
+
+    @property
+    def formatted_unit(self):
+        unit = f"{self.native_unit:~P}" if (self.native_unit is not None) else None
+        unit = "None" if unit == "" else unit
+        return unit
+
+    @formatted_unit.setter
+    def formatted_unit(self, str):
+        # needed so CRUD updates can try to update the "formatted_unit" property without failing.
+        pass
 
     @property
     def native_unit(self):
         if self._native_unit is not None and self._native_unit != 'None':
             return getattr(units, self._native_unit)
         elif self.sensor_type is not None:
-            return units[self.sensor_type.compatible_unit_str]
+            return getattr(units, self.sensor_type.compatible_unit_str)
         else:
             return None
 
     @native_unit.setter
     def native_unit(self, native_unit_str):
         sensor_type_unit = None
         if self.sensor_type is not None and self.sensor_type.compatible_unit_str is not None:
             sensor_type_unit = self.sensor_type.compatible_unit_str
 
         # None unit: get from sensor_type. Relevant for virtual sensors
         if native_unit_str is None:
             if sensor_type_unit is None:
-                # TODO reactivate this Exception?
                 pass
-                # raise TypeError('Sensor needs either a "native_unit" or a ".sensor_type.compatible_unit_str".')
             native_unit = sensor_type_unit
         else:
             # Check unit exists
             try:
                 native_unit = units[native_unit_str]
             except uu.pint.errors.UndefinedUnitError:
                 raise uu.pint.errors.UndefinedUnitError(
                     "'sensor_native_unit' must be a valid python pint library unit string")
             # Make sure native_unit is compatible with SensorType unit
             if sensor_type_unit is not None:
                 uu.assert_compatible(sensor_type_unit, native_unit)
-                # raise IncompatibleUnitError(f'Sensor unit {native_unit} is not compatible with SensorType expected '
-                #                             f'unit {str(self.sensor_type.min_limit.units)}')
         # normalise unit name, store as string for DB compatibility
         self._native_unit = str(native_unit)
 
+
     @property
-    def native_unit_str(self):
-        return str(self.native_unit)
+    def problems(self):
+        # self.problems is not persisted in the database, so if self._problems is None, on a virtual sensor,
+        # config_virtuals() is called on the plant which sets self.problems for all virtual sensors.
+        if self._problems is None and self.is_virtual:
+            if self.plant is not None:
+                [func(self.plant) for func in self.plant.post_config_changed_callbacks]
+        return self._problems
+
+    @problems.setter
+    def problems(self, val):
+        self._problems = val
 
     @sqlalchemy.orm.validates('info')
     def _set_info(self, _, info):
         if isinstance(info, SensorInfo):
             return info
         elif isinstance(info, dict):
             return SensorInfo(**info)
@@ -219,69 +250,93 @@
             self._accuracy_class = AccuracyClass[val]
 
     @property
     def sensor_type(self):
         if self._given_sensor_type is not None:
             return getattr(st, self._given_sensor_type)
         elif self.is_mapped:
-            return self._mappings[0].component.sensor_slots[self._mappings[0].slot_name].sensor_type
+            return self.mapped_components[0].sensor_slots[self.mappings[0].slot_name].sensor_type
         else:
-            return None
+            return self._sensor_type
 
     @sensor_type.setter
     def sensor_type(self, val):
         if val is None:
             return
         if isinstance(val, str):
             try:
                 val = getattr(st, val)
             except AttributeError:
                 raise ConfigurationError(f'{val} is not a known sensor type')
-
-        self._given_sensor_type = val.name
+        s_type_def = getattr(st, val.name, False)
+        wrn_txt = (f'Custom sensor types cannot be stored. If you are using a database to save configuration, '
+                   f'this sensor type will be lost on reload.')
+        if not s_type_def:
+            warnings.warn(f'Setting custom sensor type {val.name}. ' + wrn_txt)
+            self._sensor_type = val
+        elif s_type_def and val != s_type_def:
+            warnings.warn(f'Overriding built-in sensor type {s_type_def.name} with custom sensor type. ' + wrn_txt)
+            self._sensor_type = val
+        else:
+            self._given_sensor_type = val.name
         self.info.validate_all()
         if self.is_virtual:
             self.native_unit = val.compatible_unit_str
 
     @property
     def data(self):
         """Accessor for sensor data.
 
         Returns
         -------
         pandas Series object with 1 data column and DateTimeIndex depending on self.plant.context properties.
 
         Notes
-        -------
+        -----
         Does not change data time index, e.g. values are not resampled. To resample, use sensor.get_data()
         """
         if self.plant is None:
             raise ConfigurationError('Cannot access sensor.data because the sensor does not have a plant associated.')
+
         return self.plant.context.get_sensor_data(sensor=self)
 
     @property
     def is_mapped(self):
-        if len(self._mappings) > 0:
+        if len(self.mappings) > 0:
             return True
         return False
 
     @property
     def value_replacements(self):
         reps = {'upper': (self._upper_replace_min, self._upper_replace_max, self.upper_replace_value),
                 'lower': (self._lower_replace_min, self._lower_replace_max, self.lower_replace_value)}
 
-        if (self.sensor_type is not None) and (None in reps['upper']):
+        has_sensor_type = (self.sensor_type is not None)
+        all_none = lambda k: all((x is None for x in reps[k]))
+        if has_sensor_type and all_none('upper'):
             reps['upper'] = (self.sensor_type.upper_replace_min, self.sensor_type.upper_replace_max,
                              self.sensor_type.upper_replace_value)
-        if (self.sensor_type is not None) and (None in reps['lower']):
+        if has_sensor_type and all_none('lower'):
             reps['lower'] = (self.sensor_type.lower_replace_min, self.sensor_type.lower_replace_max,
                              self.sensor_type.lower_replace_value)
 
         return reps
 
+    @property
+    def value_replacements__native(self):
+        """Return self.value_replacements, but with all Quantities converted to floats in self.native_unit
+        """
+        reps = self.value_replacements
+        reps_native = {}
+        convert = lambda x: x.m_as(self.native_unit) if x is not None else None
+        for key in ['lower', 'upper']:
+            reps_native[key] = (convert(el) for el in reps[key])
+
+        return reps_native
+
     @value_replacements.setter
     def value_replacements(self, val):
         # assert isinstance(val, dict), 'Value replacement expected to be a dict.'
         # Changing value_replacements potentially affects cleaned value
         if self.plant is not None:
             self.plant.context.reset_cache()
 
@@ -291,15 +346,15 @@
                     'To define a sensor replacement interval, pass a dictionary with a 3-value tuple representing the '
                     'left and right interval boundaries and the replacement value.')
             left, right, replace = d[key]
             for x in [left, right, replace]:
                 if (x is not None) and (not x.is_compatible_with(s.native_unit)):
                     raise ValueError(
                         f'Cannot set replacement interval because unit is not compatible with sensor native_unit '
-                        f'{self.native_unit_str}')
+                        f'{self.native_unit}')
             if (left is not None) and (right is not None) and (left > right):
                 raise ValueError(
                     'In a lower replacement interval, the lower limit cannot be larger than the upper limit.')
             if (left is None) and (right is None) and (replace is not None):
                 raise ValueError(
                     'Cannot set replacement value for a replacement interval, because both left or right interval '
                     'boundaries are None.')
@@ -360,56 +415,119 @@
 
     def plot(self):
         """Create a simple development plot method for Sensor data."""
         # pd.set_option("plotting.backend", "plotly")
         # pio.renderers.default = 'browser'
         return self.data.astype('float64').plot().show()
 
-    def update(self, data: pd.Series = None):
+    def update(self, result_key: str, algo_result):
         """Save calculation results of virtual sensors to Context datasource.
 
         Parameters
         ----------
-        data : pd.Series, Data to be set as self.data
+        result_key : pd.Series is retrieved from algo_result.output with this key.
+        algo_result : AlgoResult object, output of virtual sensor algo run() method
 
         Raises
         ------
-        VirtualSensorError
-            If called on a normal (not virtual) sensor, so if self.virtual_sensor == False
+        CalculationError
+            If called on a normal (not virtual) sensor, or if required data not found in algo_result.
         """
-        if not self.is_virtual:
-            raise VirtualSensorConfigurationError(
-                'Can only update for virtual sensors, but got called on a regular sensor.')
+        if algo_result is None:
+            raise CalculationError('Got None algo_result. Check algo.run().')
 
-        if data is not None:
-            try:
-                data.pint
-            except AttributeError:
-                raise VirtualSensorCalculationError(
-                    'Calculated virtual sensor data expected to be pd.Series with dtype pint.')
-            if not self.native_unit.is_compatible_with(data.pint.units):
-                raise VirtualSensorCalculationError(
-                    f'Calculated virtual sensor data not compatible with expected unit {self.native_unit}.')
-            # Trying to minimize the changes made to sensor object: don't overwrite sensor native_unit
-            # self.native_unit = uu.get_unit_string(data)
-            data = data.pint.to(self.native_unit)
+        if (algo_result.output is not None) and (result_key not in algo_result.output):
+            raise CalculationError(
+                f'Trying to update data for virtual sensors, but required key "{result_key}" not found in algo result.')
+
+        if (algo_result.output is None) or (algo_result.output[result_key] is None):
+            # Save report of tried but not successful strategies.
+            self.problems = algo_result.problems
+            if self.is_virtual:
+                # No strategy succeeded, Context will store an all-NaN series for the vsensor.
+                sp_logger.debug(f'Sensor.update(): virtual sensor algo output is None. Storing with sensor.')
+                self.plant.context.store_data(self, None)
+            else:
+                sp_logger.debug(
+                    f'Sensor.update(): Got called on a real sensor with virtual sensor algo output None. '
+                    f'Will keep using the unchanged real sensor data.')
+            return
+        if not self.is_virtual:
+            raise CalculationError(
+                'Can only update data for virtual sensors, but got called on a real sensor with non-None output.')
 
-        hit_logger.info(f"[sensor.update] Storing data for sensor {self.raw_name }")
+        # Save report of tried but not successful strategies.
+        self.problems = algo_result.problems
 
+        # Save calculation results to virtual sensor
+        data = algo_result.output[result_key]
+        try:
+            data.pint
+        except AttributeError:
+            raise CalculationError(
+                'Calculated virtual sensor data expected to be pd.Series with dtype pint.')
+        if not self.native_unit.is_compatible_with(data.pint.units):
+            raise CalculationError(
+                f'Calculated virtual sensor data not compatible with expected unit {self.native_unit}.')
+        # Trying to minimize the changes made to sensor object: don't overwrite sensor native_unit
+        data = data.pint.to(self.native_unit)
         self.plant.context.store_data(self, data)
-        # If data is None / a vsensor calculation was not possible (for whatever reason), Context will store an all-NaN
-        # series.
 
-    def get_orientation(self):
-        """Returns dictionary with array's "tilt" and "azim" values converted to deg, for radiation calculations.
+        return
+
+    def remove_references(self, include_plant: bool = True):
+        """This makes sure SunPeek does not use the sensor anymore, and leaves the application in a consistent stage.
+        It does not do a database delete of the sensor.
+
+        Parameters
+        ----------
+        include_plant : bool
+            if false, method will not attempt to remove the sensor's reference to/from it's parent plant.
+        """
+
+        # Assigned here because removing sensor from plant.raw_sensors might lead to plant being set to None
+        plant = self.plant
+        if self.plant is not None and include_plant:
+            # self.plant = None     # Causes stack overflow by calling SQLAlchemy remove() code
+            self.plant.raw_sensors.pop(self.plant.raw_sensors.index(self))
+
+        self.mappings.clear()  # There might be mappings from sensor to a component that has no parent plant.
+
+        if plant is not None:
+            if not plant.defer_post_config_changed_actions:
+                # virtuals.config_virtuals(plant)
+                [func(plant) for func in plant.post_config_changed_callbacks]
+
+    def is_info_missing(self, info_item: str) -> bool:
+        """Make sure sensor info has an item with the specified key.
+        """
+        return (self.info is None) or (info_item not in self.info._info)
+
+    @property
+    def orientation(self):
+        """Return dictionary with array's "tilt" and "azim" values converted to deg, for radiation calculations.
         """
         return {'tilt': self.info['tilt'].m_as('deg'),
                 'azim': self.info['azim'].m_as('deg')}
 
-#
+    def has_orientation(self):
+        """Returns True if sensor has sensor info with tilt and azimuth well-defined. Useful for radiation calculations.
+        """
+        info = self.info._info
+        if not info:
+            return False
+        return ('tilt' in info) and ('azim' in info)
+
+# @event.listens_for(Sensor, 'before_delete')
+# def prevent_deletion_if_mapped(mapper, connection, target):
+#     "listen for the 'after_insert' event"
+#     if target.is_mapped:
+#         raise ConfigurationError(f"Deleting sensor {target.raw_name} is not allowed as it is mapped to a component! Please adapt your Sensor-Mapping accordingly")
+
+
 # @sqlalchemy.event.listens_for(Session, "transient_to_pending")
 # def _set_sensor_types(session, inst):
 #     if isinstance(inst, SensorMap):
 #         try:
 #             with session.no_autoflush:
 #                 type_def = session.query(SensorType).filter(SensorType.name == inst.sensor.sensor_type_name).one()
 #         except sqlalchemy.exc.NoResultFound:
```

## sunpeek/components/sensor_types.py

```diff
@@ -1,13 +1,12 @@
 import sys
 from sunpeek.common.unit_uncertainty import Q
 from sunpeek.common import common_units
 from sunpeek.components.types import SensorType
 
-
 # Some arguments to SensorType() are commented since uncertainty propagation is not implemented right now. Left
 # commented for later, just in case.
 
 '''
 This module contains a the definitions of all SensorTypes which are used to provide unit compatibility and data sanity 
 checks, depending on what a sensor does. Normally Sensors inherit their SensorType from any SensorSlots they are mapped 
 into on a component, but sensors can also be created with a type explicitly.
@@ -34,52 +33,58 @@
 global_radiation = SensorType(name='global_radiation',
                               description='Global irradiance',
                               compatible_unit_str='watt / meter**2',
                               lower_replace_min=Q(-10.0, 'watt / meter**2'),
                               lower_replace_max=Q(0.0, 'watt / meter**2'),
                               lower_replace_value=Q(0.0, 'watt / meter**2'),
                               upper_replace_max=Q(1700.0, 'watt / meter**2'),
-                              info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90},
-                                            'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360}},
-                              common_units=list(common_units.power/common_units.area),
+                              info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90,
+                                                    'description': 'Radiation sensor tilt angle.'},
+                                           'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360,
+                                                    'description': 'Radiation sensor azimuth angle.'}},
+                              common_units=list(common_units.power / common_units.area),
                               )
 
 direct_radiation = SensorType(name='direct_radiation',
                               description='Direct / beam irradiance',
                               compatible_unit_str='watt / meter**2',
                               lower_replace_min=Q(-10.0, 'watt / meter**2'),
                               lower_replace_max=Q(0.0, 'watt / meter**2'),
                               lower_replace_value=Q(0.0, 'watt / meter**2'),
                               upper_replace_max=Q(1400.0, 'watt / meter**2'),
-                              info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90},
-                                            'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360}},
-                              common_units=list(common_units.power/common_units.area),
+                              info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90,
+                                                    'description': 'Radiation sensor tilt angle.'},
+                                           'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360,
+                                                    'description': 'Radiation sensor azimuth angle.'}},
+                              common_units=list(common_units.power / common_units.area),
                               )
 
 diffuse_radiation = SensorType(name='diffuse_radiation',
                                description='Diffuse irradiance',
                                compatible_unit_str='watt / meter**2',
                                lower_replace_min=Q(-10.0, 'watt / meter**2'),
                                lower_replace_max=Q(0.0, 'watt / meter**2'),
                                lower_replace_value=Q(0.0, 'watt / meter**2'),
                                upper_replace_max=Q(1100.0, 'watt / meter**2'),
-                               info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90},
-                                             'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360}},
-                               common_units=list(common_units.power/common_units.area),
+                               info_checks={'tilt': {'unit': 'deg', 'minimum': 0, 'maximum': 90,
+                                                     'description': 'Radiation sensor tilt angle.'},
+                                            'azim': {'unit': 'deg', 'minimum': 0, 'maximum': 360,
+                                                     'description': 'Radiation sensor azimuth angle.'}},
+                               common_units=list(common_units.power / common_units.area),
                                )
 
 dni_radiation = SensorType(name='dni_radiation',
                            description='DNI (direct normal) irradiance',
                            compatible_unit_str='watt / meter**2',
                            lower_replace_min=Q(-10.0, 'watt / meter**2'),
                            lower_replace_max=Q(0.0, 'watt / meter**2'),
                            lower_replace_value=Q(0.0, 'watt / meter**2'),
                            upper_replace_max=Q(1400.0, 'watt / meter**2'),
                            info_checks=None,
-                           common_units=list(common_units.power/common_units.area),
+                           common_units=list(common_units.power / common_units.area),
                            )
 
 thermal_power = SensorType(name='thermal_power',
                            description='Thermal power',
                            compatible_unit_str='watt',
                            lower_replace_min=Q(-10.0, 'watt'),
                            lower_replace_max=Q(0.0, 'watt'),
@@ -91,44 +96,46 @@
 mass_flow = SensorType(name='mass_flow',
                        description=None,
                        compatible_unit_str='kilogram / second',
                        lower_replace_min=Q(-100.0, 'kilogram / second'),
                        lower_replace_max=Q(0.0, 'kilogram / second'),
                        lower_replace_value=Q(0.0, 'kilogram / second'),
                        info_checks=None,
-                       common_units=list(common_units.mass/common_units.time),
+                       common_units=list(common_units.mass / common_units.time),
                        )
 
 volume_flow = SensorType(name='volume_flow',
                          description=None,
                          compatible_unit_str='meter ** 3 / second',
                          lower_replace_min=Q(-0.1, 'meter ** 3 / second'),
                          lower_replace_max=Q(0.0, 'meter ** 3 / second'),
                          lower_replace_value=Q(0.0, 'meter ** 3 / second'),
-                         info_checks=None,
-                         common_units=list(common_units.volume/common_units.time),
+                         info_checks={'position': {'unit': '', 'minimum': 0, 'maximum': 1,
+                                                   'description': 'Position of the volume flow sensor, near te_in '
+                                                                  '(0), near te_out (1) or in between (0..1).'}},
+                         common_units=list(common_units.volume / common_units.time),
                          )
 
 wind_speed = SensorType(name='wind_speed',
                         description='Wind speed',
                         compatible_unit_str='meter / second',
                         lower_replace_min=Q(-1.0, 'meter / second'),
                         lower_replace_max=Q(0.0, 'meter / second'),
                         lower_replace_value=Q(0.0, 'meter / second'),
                         info_checks=None,
-                        common_units=list(common_units.length/common_units.time),
+                        common_units=list(common_units.length / common_units.time),
                         )
 
 temperature_derivative = SensorType(name='temperature_derivative',
                                     description='Temperature derivative',
                                     compatible_unit_str='kelvin / second',
                                     lower_replace_min=Q(-100.0, 'kelvin / second'),
                                     upper_replace_max=Q(100.0, 'kelvin / second'),
                                     info_checks=None,
-                                    common_units=list(common_units.temperature/common_units.time),
+                                    common_units=list(common_units.temperature / common_units.time),
                                     )
 
 pressure = SensorType(name='pressure',
                       description='Pressure',
                       compatible_unit_str='bar',
                       lower_replace_min=Q(-0.5, 'bar'),
                       lower_replace_max=Q(0.0, 'bar'),
@@ -163,15 +170,15 @@
                          lower_replace_min=Q(0.0),
                          upper_replace_max=Q(100.0),
                          info_checks=None,
                          )
 
 angle_0_180 = SensorType(name='angle_0_180',
                          description='Angle between 0 and 180',
-                         compatible_unit_str='',
+                         compatible_unit_str='degree',
                          lower_replace_min=Q(0.0, 'degree'),
                          upper_replace_max=Q(180.0, 'degree'),
                          info_checks=None,
                          common_units=list(common_units.angle),
                          )
 
 angle_0_360 = SensorType(name='angle_0_360',
@@ -197,9 +204,8 @@
                           compatible_unit_str='degree',
                           lower_replace_min=Q(-90.0, 'degree'),
                           upper_replace_max=Q(90.0, 'degree'),
                           info_checks=None,
                           common_units=list(common_units.angle),
                           )
 
-
 all_sensor_types = [x for x in sys.modules[__name__].__dict__.values() if isinstance(x, SensorType)]
```

## sunpeek/components/types.py

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy import inspect
 from typing import Union
 import datetime
 import copy
 import dataclasses
 
 from sunpeek.components import iam_methods
-from sunpeek.components.iam_methods import _IAM_Method
+from sunpeek.components.iam_methods import IAM_Method
 from sunpeek.common import unit_uncertainty as uu
 from sunpeek.common.unit_uncertainty import Q
 from sunpeek.common.errors import CollectorDefinitionError
 from sunpeek.components.helpers import ORMBase, AttrSetterMixin, ComponentParam
 
 
 @dataclasses.dataclass
@@ -46,28 +46,26 @@
         self._info_checks = val
 
 
 class CollectorType(AttrSetterMixin, ORMBase):
     """
     Implements a specific collector (product of some manufacturer), including all performance data acc. to data sheet.
 
-    Note
-    ----
     Stores two different collector type parameters, referring to the two test procedures defined in `ISO 9806`_,
     either quasi-dynamic or steady-state test. The type of test procedure is available from the standard collector
     data sheet / Solar Keymark certificate and must be specified in `test_type`.
 
     Test parameters may refer to either gross or aperture area. This must be specified in `test_reference_area`. The
     collector parameters stored in CollectorType _always_ refer to gross area.
 
-    IAM (incidence angle modifier) information may be given as an instance of the _IAM_Method class. This holds
+    IAM (incidence angle modifier) information may be given as an instance of the IAM_Method class. This holds
     several implementations where the IAM information can be given in either of these ways:
-    - If only IAM information at an aoi of 50 degrees is given, use `IAM_K50(k50)`. Internally, this uses the ASHRAE equation_id.
-    - To use the ASHRAE IAM equation_id with a known parameter `b`, use `IAM_ASHRAE(b)`.
-    - To use the Ambrosetti IAM equation_id with a known parameter `kappa`, use `IAM_Ambrosetti(kappa)`.
+    - If only IAM information at an aoi of 50 degrees is given, use `IAM_K50(k50)`. Internally, this uses the ASHRAE equation.
+    - To use the ASHRAE IAM equation with a known parameter `b`, use `IAM_ASHRAE(b)`.
+    - To use the Ambrosetti IAM equation with a known parameter `kappa`, use `IAM_Ambrosetti(kappa)`.
     - To use an IAM with given / known IAM values at given aoi angles, use `IAM_Interpolated()`. This requires a list
     of reference aoi's, and either a) 1 list of IAM values or b) 2 lists with transversal and longitudinal IAM
     values.
 
     Attributes
     ----------
     name : str
@@ -150,15 +148,14 @@
         Contains information about calculated collector parameters, where specific information was not given at 
         instantiation of the object, e.g. because the Solar Keymark data sheet does not include a specific parameter. 
         Some parameters can be calculated based on given ones, e.g. `Kd` (diffuse IAM) can be calculated based on 
         given IAM information. Dictionary keys are the names of calculated parameters (e.g. `kd`), dictionary values 
         hold information concerning specific calculation details (e.g. calculation method).    
     plant : None
         Not used, included for compatibility with other component types.
-        
 
     .. _ISO 9806:
         https://www.iso.org/standard/67978.html
     .. _ASHRAE model:
         https://pvlib-python.readthedocs.io/en/stable/generated/pvlib.iam.ashrae.html
     """
     __tablename__ = 'collector_types'
@@ -184,19 +181,19 @@
     manufacturer_name = Column(String)
     product_name = Column(String)
     licence_number = Column(String)
     test_report_id = Column(String)
     certificate_date_issued = Column(DateTime)
     certificate_lab = Column(String)
     certificate_details = Column(String)
-    iam_method = relationship("_IAM_Method", back_populates='collector_type', uselist=False, cascade="all, delete",
+    iam_method = relationship("IAM_Method", back_populates='collector_type', uselist=False, cascade="all, delete",
                               passive_deletes=True)
     test_type = Column(Enum(t_types))
     test_reference_area = Column(Enum(ref_a_types))
-    calculated_parameters = Column(JSON)  # TODO MHJ This is actually a dictionary. How to declare it for sqlalchemy?
+    calculated_parameters = Column(JSON)
 
     # No limit checks for these attributes to avoid code duplication with self._set_collector_parameters()
     area_gr = ComponentParam('m**2', minimum=0.1)
     area_ap = ComponentParam('m**2', minimum=0.1)
     gross_length = ComponentParam('cm', minimum=0)
     gross_width = ComponentParam('cm', minimum=0)
     gross_height = ComponentParam('cm', minimum=0)
@@ -207,15 +204,15 @@
     eta0b = ComponentParam('')
     eta0hem = ComponentParam('')
     b0 = ComponentParam('')
     kb_50 = ComponentParam('')
     khem_50 = ComponentParam('')
     f_prime = ComponentParam('', minimum=0, maximum=1)
 
-    def __init__(self, test_reference_area, test_type, gross_length, iam_method: _IAM_Method = None,
+    def __init__(self, test_reference_area, test_type, gross_length, iam_method: IAM_Method = None,
                  name=None, manufacturer_name=None, product_name=None, test_report_id=None, licence_number=None,
                  certificate_date_issued=None, certificate_lab=None, certificate_details=None,
                  area_gr=None, area_ap=None, gross_width=None, gross_height=None,
                  a1=None, a2=None, a5=None, kd=None, eta0b=None, eta0hem=None, f_prime=None, plant=None):
 
         self.test_reference_area = self._infer_test_reference_area(test_reference_area)
         self.test_type = self._infer_test_type(test_type)
@@ -347,14 +344,22 @@
         self.a5 = uu.check_quantity(a5, 'J m**-2 K**-1', min_limit=0, max_limit=100000)
         self.eta0hem = uu.check_quantity(eta0hem, min_limit=0, max_limit=1)
         self.eta0b = uu.check_quantity(eta0b, min_limit=0, max_limit=1)
         self.kd = uu.check_quantity(kd, min_limit=0, max_limit=1)
 
         return
 
+    def is_attrib_missing(self, attrib_name):
+        # May raise AttributeError
+        attrib = getattr(self, attrib_name)
+        if attrib is None:
+            return True
+        return False
+
+
     def __eq__(self, other):
         try:
             inst = inspect(self)
             attr_names = [c_attr.key for c_attr in inst.mapper.column_attrs if c_attr.key != 'id']
 
             for attr in attr_names:
                 if getattr(self, attr) != getattr(other, attr):
@@ -367,20 +372,14 @@
 class UninitialisedCollectorType(CollectorType):
     def __init__(self, collector_type_name, parent, attribute):
         self.name = collector_type_name
         self.parent = parent
         self.attribute = attribute
 
 
-def assert_valid_collector(coll):
-    assert coll is not None, 'Collector is None'
-    assert not isinstance(coll, UninitialisedCollectorType), \
-        'Collector is uninitialized, it is a "UninitialisedCollectorType"'
-
-
 def estimate_eta0hem(eta0b: Q, kd: Q):
     """
     Calculates the hemispherical peak collector efficiency 'eta_0hem'
     based on the QDT-SST conversion formulas in EN ISO 9806 ANNEX B.
 
     Parameters
     ----------
@@ -415,23 +414,23 @@
     """
     eta0b = eta0hem / (0.85 + 0.15 * kd)
     info = 'Parameter "eta0b" (beam peak collector efficiency) calculated based on "eta0hem" and diffuse incidence ' \
            'angle modifier "Kd" using the formula: eta0b = eta0hem / (0.85 + 0.15 * Kd)'
     return eta0b, info
 
 
-def estimate_kd_Hess_and_Hanby(iam_method: _IAM_Method):
+def estimate_kd_Hess_and_Hanby(iam_method: IAM_Method):
     """
     Estimates the diffuse IAM (incidence angle modifier) ``Kd`` by integrating the IAM values for beam irradiation
     over the hemispherical plane. Assumes isotropic diffuse radiation (which typically underestimates the derived ``Kd``
     values).
 
     Parameters
     ----------
-    iam_method : _IAM_Method
+    iam_method : IAM_Method
         instance based on a _IAM_Method class with a method ``get_iam(aoi, azimuth_diff)`` to calculate the iam based
         on the angle of incidence ``aoi`` and the solar azimuth angle ``phi``
 
     Returns
     -------
     kd: Quantity, estimated diffuse radiation incidence angle modifier
     info: string, information on calculation method used
```

## sunpeek/core_methods/__init__.py

```diff
@@ -0,0 +1,6 @@
+00000000: 6672 6f6d 2073 756e 7065 656b 2e63 6f72  from sunpeek.cor
+00000010: 655f 6d65 7468 6f64 732e 636f 6d6d 6f6e  e_methods.common
+00000020: 2e6d 6169 6e20 696d 706f 7274 2043 6f72  .main import Cor
+00000030: 6541 6c67 6f72 6974 686d 2c20 436f 7265  eAlgorithm, Core
+00000040: 5374 7261 7465 6779 2c20 416c 676f 5265  Strategy, AlgoRe
+00000050: 7375 6c74 0a0a 0a                        sult...
```

## sunpeek/core_methods/pc_method/__init__.py

```diff
@@ -1,18 +1,20 @@
 """
 Implements Performance Check (PC) Method according to technical standard ISO/DIS 24194.
 
-# HowTo
+HowTo
+=====
 
-See `main.py` docstring.
+See :py:mod:main docstring.
 
-# Why
+Why
+===
 
 The Performance Check (PC) method can be used to decide whether the measured performance of a solar thermal plant
-matches the performance expected based on given information (data sheets, boundary conditions etc).
+matches the performance estimated based on given information (data sheets, boundary conditions etc).
 
 From the ISO/DIS 24194:
 "
     # 1 Scope
     [This method allows to] verify the performance of solar thermal collector fields. The
     collectors in the fields can be glazed flat plate collectors, evacuated tube collectors and/or
     tracking, concentrating collectors.
@@ -29,17 +31,17 @@
     for the parameters in equation. The three possible equations are given in the next three subsections.
     The collector module efficiency parameters eta0_hem, eta0_b, Kb(theta) Kd, a1, a2, a5 [1] and a8 should be based on
     certified test results. When an estimate is given it shall always be stated which equation shall be used for
     checking the performance:
 
     a) Simple check, using total radiation on the collector plane when checking the power output
     (ISO this standard, eq 1).
-    b) Advanced check, using direct and diffuse radiation on collector plane wehn checking the power output
+    b) Advanced check, using direct and diffuse radiation on collector plane when checking the power output
     (ISO this standard, eq 2).
-    c) Advanced check, using only direct radiation on collector plane when checking the the power output
+    c) Advanced check, using only direct radiation on collector plane when checking the power output
     (ISO this standard, eq3)
 
     [1] in the older Solar Keymark data sheets a5 is denoted c_eff
 "
 
 # Notes & usage hints
 
@@ -49,13 +51,44 @@
 consider treating them as separate plants and running the PC method on each of them separately.
 - Current implementation assumes that temperatures (`te_in`, `te_out`) are available for all collector arrays.
 Application to other configurations is yet unclear.
 - Radiations (`rd_bti`, `rd_dti`) are defined and assumed to be available for each array.
 - Details concerning radiation modeling / radiation conversion algorithms are not in this algorithm.
 e.g. available = GHI, GTI, beam/diffuse separated, multiple radiation sensors for multiple arrays etc.
 
+# Collector parameter names
+
+The collector parameter names are taken from ISO 24194:2021 (ISO 24194:2022 introduced some name clashes /
+unusual symbols, as confirmed in personal communication with the standard developers):
+    `a1`: Heat loss coefficient at (theta_m - theta_a = 0)  (named a1_DeltaQ in ISO 24194:2022)
+    `a2`: Temperature dependence of the heat loss coefficient (named T_DeltaQ in ISO 24194:2022)
+    `a5`: Effective thermal capacity
+    `eta0b`: Peak collector efficiency (etab at theta_m -theta_a = 0 K) based on beam irradiance Gb
+    `eta0hem`: Peak collector efficiency (`eta0hem` at theta_m - theta_a = 0 K) based on
+              hemispherical irradiance G_hem
+    `kd`: Incidence angle modifier for diffuse solar radiation (named as Kd in ISO 24194:2022)
 """
 
-from .main import PCMethod
-from .equation import Equation1, Equation2
-from .plotting import plot_all, plot_square, plot_time, plot_sums
-from .verify_validate import verify_config, validate_data
+import enum
+# from .wrapper import run_performance_check
+from .plotting import plot_all, plot_square, plot_time, plot_sums, plot_sensor_data
+
+# from .wrapper import run_performance_check, pc_strategy_generator
+# from .main import PCMethod, PCSettings, PCMethodISO, PCMethodExtended
+# from .equation import Equation1, Equation2
+# from .verify_validate import verify_config, validate_data
+
+# OLD MAIN
+# from .main import PCMethod
+# from .equation import Equation1, Equation2
+# from .plotting import plot_all, plot_square, plot_time, plot_sums, plot_sensor_data
+# from .verify_validate import verify_config, validate_data
+
+
+class AvailablePCEquations(enum.IntEnum):
+    one = 1
+    two = 2
+
+
+class AvailablePCMethods(str, enum.Enum):
+    iso = 'iso'
+    extended = 'extended'
```

## sunpeek/core_methods/pc_method/equation.py

```diff
@@ -1,257 +1,287 @@
-# -*- coding: utf-8 -*-
-
 from abc import ABC, abstractmethod
-from typing import Callable
+from typing import Callable, Union
 import pandas as pd
 
 from sunpeek.common.unit_uncertainty import Q
-from sunpeek.common.utils import VerifyValidateMode
+from sunpeek.components.base import AlgoCheckMode
+from sunpeek.core_methods.common.main import is_valid_collector
 from sunpeek.components.physical import Plant, Array
-from sunpeek.components.types import assert_valid_collector
+from sunpeek.core_methods.pc_method import AvailablePCEquations
+from sunpeek.common.errors import PCMethodError
+from sunpeek.serializable_models import ProblemReport, ProblemType, AlgoProblem
+
+# Common to all equations
+MAX_DELTA_T_COLLECTOR = Q(5.0, 'K hour**-1')
+MIN_TE_AMB = Q(5.0, 'degC')
+MAX_WIND_SPEED = Q(10, 'm s**-1')
+
 
+# TODO Use this for all equations?
+MAX_AOI = Q(80, 'deg')
 
-def create_eq(equation_id):
-    if equation_id == 1:
-        return Equation1()
-    elif equation_id == 2:
-        return Equation2()
-    else:
-        raise ValueError(f'Unknown "equation_id" {equation_id}.')
+MAX_AOI_EQ2 = Q(75, 'deg')
 
+# Equation 1
+MIN_RD_GTI = Q(800, 'W m**-2')
 
+# Equation 2
+MIN_RD_BTI = Q(600, 'W m**-2')
+
+
+# noinspection PyArgumentList
 class Equation(ABC):
-    """
-    Template for the Equations as defined in the ISO DIS 241934:
-    It specifies how power is estimated and what filter criteria to need to be applied.
+    """Template class for the equations / formulae for calculating power output, as defined in the ISO 24194:
+
+    The equations are defined in ISO 24194 chapter 5.2.1. The equations specify
+    1. how power output is calculated / estimated
+    2. and what restrictions are applied to data: the criteria in ISO 24194 Table 1 depend on the equation choice.
 
     "
     # 5.1 Stating an estimate for the thermal power output of a collector field
-    The estimated power output of the collector array is given as an equation_id depending on the collector parameters
+    The estimated power output of the collector array is given as an equation depending on the collector parameters
     according to ISO 9806 and operation conditions. The measured power shall comply with the corresponding calculated
-    power according to this equation_id. Measured and calculated power are nly compared under some specific conditions
+    power according to this equation. Measured and calculated power are only compared under some specific conditions
     to avoid too large uncertainties - see section 5.4
 
-    The estimate is given by stating the equation_id to be used for calculating the power output, including specific
-    values for the parameters in equation_id. The three possible equations are given in the next three subsections.
+    The estimate is given by stating the equation to be used for calculating the power output, including specific
+    values for the parameters in equation. The three possible equations are given in the next three subsections.
     The collector module efficiency parameters eta0_hem, eta0_b, Kb(theta) Kd, a1, a2, a5 [1] and a8 should be based on
-    certified test results. When an estimate is given it shall always be stated which equation_id shall be used for
+    certified test results. When an estimate is given it shall always be stated which equation shall be used for
     checking the performance:
 
     a) Simple check, using total radiation on the collector plane when checking the power output (ISO this standard,
     eq 1).
-    b) Advanced check, using direct and diffuse radiation on collector plane wehn checking the power output
+    b) Advanced check, using direct and diffuse radiation on collector plane when checking the power output
     (ISO this standard, eq 2).
-    c) Advanced check, using only direct radiation on collector plane when checking the the power output
+    c) Advanced check, using only direct radiation on collector plane when checking the power output
     (ISO this standard, eq3)
 
     [1] in the older Solar Keymark data sheets a5 is denoted c_eff
     "
     """
 
     id = None
 
-    # Restricions on operating conditions based on Table 1 of standard ISO 24194.
-    # Only data that pass these restrictions (as averages over given time range) are used for calculation of expected
+    # Restrictions on operating conditions based on Table 1 of ISO 24194.
+    # Only data that pass these restrictions (as averages over given time range) are used for calculation of estimated
     # array power.
     # Common to equations 1 & 2
-    max_deltat_collector = Q(5.0, 'K hour**-1')
-    min_te_amb = Q(5.0, 'degC')
-    max_wind_speed = Q(10, 'm s**-1')
+    max_deltat_collector = MAX_DELTA_T_COLLECTOR
+    min_te_amb = MIN_TE_AMB
+    max_wind_speed = MAX_WIND_SPEED
+
+    @classmethod
+    def create(cls, equation: Union[AvailablePCEquations, int], use_wind: bool) -> 'Equation':
+        if equation == AvailablePCEquations.one:
+            return Equation1(use_wind)
+
+        elif equation == AvailablePCEquations.two:
+            return Equation2(use_wind)
+
+        else:
+            raise PCMethodError(f'Unknown equation number "{equation}". '
+                                f'Valid equations: {", ".join(map(str, AvailablePCEquations))}.')
+            # f'Valid equations: {", ".join([str(e.value) for e in AvailablePCEquations])}.')
 
-    def __init__(self, ignore_wind: bool = False):
+    def __init__(self, use_wind: bool):
         """
         Parameters
         ----------
-        ignore_wind : bool
-            if True, the wind speed parameter is ignored during fining valid data records.
-            Default: False
+        use_wind : bool
+            if False, the wind speed sensor is ignored as a restriction to finding valid intervals
+            in the data filtering process for meeting the ISO 24194 requirements.
         """
-        self.ignore_wind = ignore_wind
+        self.use_wind = use_wind
         return
 
-    @staticmethod
-    def _assert_available_common(array, check_mode):
-        assert array.area_gr is not None, \
-            f'Array {array}: array gross area "area_gr" is None.'
-
-        assert_valid_collector(array.collector_type)
-        for param in ['a1', 'a2', 'a5', 'eta0b', 'kd']:
-            assert getattr(array.collector_type, param) is not None, \
-                f'Array {array}: collector coefficient "{param}" is required to run the PC method but not available.'
-
-        array_ok, problem_slots = array.verify_validate(check_mode, 'te_op', 'te_op_deriv', 'is_shadowed', 'iam')
-        assert array_ok, \
-            f"Array {array}: sensors are required to run the PC method but not available: {problem_slots}."
-
-    @abstractmethod
-    def assert_available(self,
-                         array: Array,
-                         verify_validate: VerifyValidateMode):
-        """Asserts whether equation fulfills all requirements == can be applied to array, either in
-        'verify' (config only) or in 'validate' (with data) mode.
+    def report_problems(self, array: Array, check_mode: AlgoCheckMode) -> ProblemReport:
+        r = ProblemReport()
 
-        Parameters
-        ----------
-        array : Array to check
-        verify_validate : str, 'verify' or 'validate' (see check_mode module docstring for details)
+        for attrib in ['area_gr']:
+            if array.is_attrib_missing(attrib):
+                r.add_own(AlgoProblem(ProblemType.component_attrib, array, attrib))
+
+        if not is_valid_collector(array.collector_type, check_mode):
+            r.add_own(AlgoProblem(ProblemType.component_attrib,
+                                  array, 'collector_type',
+                                  'Collector type is None or UninitialisedCollectorType.'))
+        else:
+            for attrib in ['a1', 'a2', 'a5', 'eta0b', 'kd']:
+                if getattr(array.collector_type, attrib) is None:
+                    r.add_own(AlgoProblem(ProblemType.component_attrib,
+                                          array.collector_type, attrib,
+                                          f'Collector coefficient "{attrib}" is required but is None / not available.'))
+
+        for slot_name in ['te_op', 'te_op_deriv', 'is_shadowed', 'iam']:
+            if array.is_slot_missing(slot_name, check_mode):
+                r.add_own(AlgoProblem(ProblemType.component_slot, array, slot_name))
+
+        if self.use_wind:
+            if array.plant.is_slot_missing('ve_wind', check_mode):
+                r.add_own(AlgoProblem(ProblemType.component_slot, array.plant, 've_wind'))
 
-        Returns
-        -------
-        Nothing
-        """
-        raise NotImplementedError
+        return r
 
     @abstractmethod
-    def get_nan_mask(self, plant: Plant, ignore_wind: bool):
+    def get_nan_mask(self, plant: Plant):
         """This method checks whether all sensors required to apply an equations are available.
 
         Returns
         -------
         bool : True where any of the sensors required to calculate equation are NaN.
 
         Notes
         -----
         In this PC Method implementation, only data records are used where none of the needed sensor records is NaN.
-        Make sure _set_equation() has been called before, so self.equation_id is not None.
+        Make sure _set_equation() has been called before, so self.equation is not None.
         """
         raise NotImplementedError
 
-    @staticmethod
-    def _get_nan_mask_common(plant, ignore_wind):
+    def _get_nan_mask_common(self, plant):
         """This method checks sensors common to both equations 1 and 2.
         """
+
         # Plant
         mask = plant.te_amb.data.isna()
         mask = mask | plant.tp.data.isna()
         mask = mask | plant.sun_apparent_elevation.data.isna()
-        if not ignore_wind:
+        if self.use_wind:
             mask = mask | plant.ve_wind.data.isna()
 
         # Arrays
         for array in plant.arrays:
             mask = mask | array.te_op.data.isna()
             mask = mask | array.te_op_deriv.data.isna()
             mask = mask | array.is_shadowed.data.isna()
 
         return mask
 
     @abstractmethod
-    def calc_pc_restrictions(self, plant: Plant, ignore_wind: bool, resampler: Callable) -> pd.Series:
+    def calc_pc_restrictions(self, plant: Plant, resampler: Callable) -> pd.Series:
         """Check the operating condition restrictions of ISO 24194. Implements Table 1, chapter 5.4.
 
         Parameters
         ----------
         plant : Plant
-        ignore_wind : bool
         resampler : Callable
             Aggregates single records into an aggregated value, e.g. hourly mean.
 
         Returns
         -------
         pd.Series : bool mask, True where any of the sensors required to calculate equation are NaN.
 
         Notes
         -----
-        From the ISO DIS 241934:
+        From the ISO 24194:
             # 6.2 Valid data records
             Only data records (hourly average values) fulfilling the requirements in section 5.4 are valid.
             For checking the collector performance, the measuring period shall have at least 20 datapoints.
             [...]
             All valid datapoints should be used unless it is obvious that errors in the data or very atypical
             operating conditions occur (omitting valid data points shall be reported and justified).
         """
         raise NotImplementedError
 
-    def _calc_pc_restrictions_common(self, plant, ignore_wind, resampler) -> pd.Series:
+    def _calc_pc_restrictions_common(self, plant, resampler) -> pd.Series:
         """Checks the operating condition restrictions that are common to Equation 1 and Equation 2.
 
         Returns
         -------
         pd.Series : bool mask
         """
-        # minimum ambient temperature
+        # Minimum ambient temperature
         is_valid = resampler(plant.te_amb.data) >= self.min_te_amb
-        if not ignore_wind:
-            # maximum wind speed
+        if self.use_wind:
+            # Maximum wind speed
             is_valid = is_valid & (resampler(plant.ve_wind.data) <= self.max_wind_speed)
 
         for array in plant.arrays:
-            # shading
+            # Shading
             is_valid = is_valid & (resampler(array.is_shadowed.data, 'sum') == 0)
-            # maximum temperature change
+            # Maximum temperature change
             is_valid = is_valid & (resampler(array.te_op_deriv.data).abs() <= self.max_deltat_collector)
 
         return is_valid
 
     @abstractmethod
-    def calc_expected_power(self, array: Array, aggregator: Callable) -> pd.Series:
-        """Calculates the estimated specific power output of the collector based on the ISO equation_id formula.
+    def calc_estimated_power(self, array: Array, aggregator: Callable) -> pd.Series:
+        """Calculates the estimated specific power output of the collector based on the ISO equation formula.
 
         Parameters
         ----------
         array : Array
         aggregator : Callable
             Aggregates single records into an aggregated value, e.g. hourly mean.
 
         Returns
         -------
         pd.Series : Estimated power output of the collector, unit-aware series compatible to unit [W m**-2]
         """
         raise NotImplementedError
 
 
+# noinspection PyArgumentList
 class Equation1(Equation):
     """ Implements Equation 1 of the ISO 24194. See Equation base class for more infos.
     """
     id = 1
 
     # Restrictions specific to equation 1
     # max_aoi = Q(30, 'deg')
     # Deliberately set maximum incidence angle (not defined in ISO 24194) to avoid numerical problems and problems
     # with calculated Kd values at high incidence angles.
-    max_aoi_khem = Q(75, 'deg')
-    min_rd_gti = Q(800, 'W m**-2')
-
-    def assert_available(self, array, verify_validate):
-        """Asserts whether all requirements are fulfilled to apply equation 1 to given array.
-        """
-        self._assert_available_common(array, verify_validate)
 
-        assert array.collector_type.eta0hem is not None, \
-            f'Array {array}: collector coefficient "eta0hem" is required to run PC method eq. 1 but not available.'
+    # TODO change for newest ISO 24194 version
+    max_aoi_eq1 = MAX_AOI_EQ2
+    min_rd_gti = MIN_RD_GTI
+
+    def report_problems(self, array: Array, check_mode: AlgoCheckMode) -> ProblemReport:
+        r = super().report_problems(array, check_mode)
+
+        for attrib in ['eta0hem']:
+            if getattr(array.collector_type, attrib) is None:
+                r.add_own(AlgoProblem(ProblemType.component_attrib,
+                                      array.collector_type, attrib,
+                                      f'Collector coefficient "{attrib}" is required for equation 1 but '
+                                      f'is None / not available.'))
+
+        for slot_name in ['rd_gti', 'aoi']:
+            if array.is_slot_missing(slot_name, check_mode):
+                r.add_own(AlgoProblem(ProblemType.component_slot, array, slot_name))
+
+        return r
+
+    def get_nan_mask(self, plant:Plant):
+        # Common sensors
+        mask = self._get_nan_mask_common(plant)
 
-        array_ok, problem_slots = array.verify_validate(verify_validate, 'rd_gti', 'aoi')
-        assert array_ok, \
-            f"Array {array}: sensors are required to run PC method eq. 1 but not available: {problem_slots}."
-
-    def get_nan_mask(self, plant: Plant, ignore_wind: bool):
-        mask = self._get_nan_mask_common(plant, ignore_wind)
+        # Specific to equation 1
         for array in plant.arrays:
             mask = mask | array.rd_gti.data.isna()
             mask = mask | array.aoi.data.isna()
 
         return mask
 
-    def calc_pc_restrictions(self, plant, ignore_wind, resampler) -> pd.Series:
-        is_valid = self._calc_pc_restrictions_common(plant, ignore_wind, resampler)
+    def calc_pc_restrictions(self, plant, resampler) -> pd.Series:
+        is_valid = self._calc_pc_restrictions_common(plant, resampler)
 
         for array in plant.arrays:
             # Minimum diffuse radiation
             is_valid = is_valid & (resampler(array.rd_gti.data) >= self.min_rd_gti)
             # Question: Use max aoi here, or mean, or...? Fails occasionally with 'max', not sure why, see #268
             # maximum incidence angle --> This criterion got removed in version ISO 24194:2022(E).
             # is_valid = is_valid & (resampler(array.aoi.data, 'mean') <= self.max_aoi)
             # Maximum incidence angle: not included as a criterion in ISO 24194:2022(E), but necessary to ensure
             # stability  
-            is_valid = is_valid & (resampler(array.aoi.data, 'mean') <= self.max_aoi_khem)
+            is_valid = is_valid & (resampler(array.aoi.data, 'mean') <= self.max_aoi_eq1)
 
         return is_valid
 
-    def calc_expected_power(self, array, aggregator) -> pd.Series:
+    def calc_estimated_power(self, array, aggregator) -> pd.Series:
         """Calculates the estimated power output of a collector array based on equation 1 formula in ISO 24194.
         """
         # Collector coefficients
         a1 = array.collector_type.a1
         a2 = array.collector_type.a2
         a5 = array.collector_type.a5
         eta0b = array.collector_type.eta0b
@@ -266,59 +296,61 @@
 
         # Calculation of hemispheric incidence angle modifier for global tilted radiation:
         # Calculation is based on ISO 9806:2017 annex B, with variable name iam_xx used here instead of K_xx
         # G * iam_hem * eta0hem = G * eta0b * (0.85 * iam_b + 0.15 * iam_d)
         kb = aggregator(array.iam.data)
         khem = (eta0b / eta0hem) * (0.85 * kb + 0.15 * kd)
 
-        tp_expected_specific = eta0hem * khem * rd_gti \
-                               - a1 * (te_op - te_amb) \
-                               - a2 * (te_op - te_amb) ** 2 \
-                               - a5 * te_op_deriv
+        tp_estimated_specific = eta0hem * khem * rd_gti \
+                                - a1 * (te_op - te_amb) \
+                                - a2 * (te_op - te_amb) ** 2 \
+                                - a5 * te_op_deriv
 
-        return tp_expected_specific.astype('pint[W m**-2]')
+        return tp_estimated_specific.astype('pint[W m**-2]')
 
 
 class Equation2(Equation):
     """ Implements Equation 2 of the ISO 24194. See Equation base class for more infos.
     """
-
     id = 2
 
-    # Restrictions specific to equation 1
-    min_rd_bti = Q(600, 'W m**-2')
+    # Restrictions specific to equation 2
+    min_rd_bti = MIN_RD_BTI
 
-    def get_nan_mask(self, plant: Plant, ignore_wind: bool):
-        mask = self._get_nan_mask_common(plant, ignore_wind)
+    def get_nan_mask(self, plant: Plant):
+        # Common sensors
+        mask = self._get_nan_mask_common(plant)
+
+        # Specific to equation 2
         for array in plant.arrays:
             mask = mask | array.rd_bti.data.isna()
             mask = mask | array.rd_dti.data.isna()
             mask = mask | array.iam.data.isna()
 
         return mask
 
-    def assert_available(self, array, check_mode):
-        """Asserts whether all requirements are fulfilled to apply equation 2 to given array.
-        """
-        self._assert_available_common(array, check_mode)
+    def report_problems(self, array: Array, check_mode: AlgoCheckMode) -> ProblemReport:
+        r = super().report_problems(array, check_mode)
+
+        for slot_name in ['rd_bti', 'rd_dti']:
+            if array.is_slot_missing(slot_name, check_mode):
+                r.add_own(AlgoProblem(ProblemType.component_slot, array, slot_name))
 
-        array_ok, problem_slots = array.verify_validate(check_mode, 'rd_bti', 'rd_dti')
-        assert array_ok, \
-            f"Array {array}: sensors are required to run PC method eq. 2 but not available: {problem_slots}."
+        return r
 
-    def calc_pc_restrictions(self, plant, ignore_wind, resampler) -> pd.Series:
-        is_valid = self._calc_pc_restrictions_common(plant, ignore_wind, resampler)
+    def calc_pc_restrictions(self, plant, resampler) -> pd.Series:
+        is_valid = self._calc_pc_restrictions_common(plant, resampler)
 
         for array in plant.arrays:
             # Minimum beam radiation
             is_valid = is_valid & (resampler(array.rd_bti.data) >= self.min_rd_bti)
 
         return is_valid
 
-    def calc_expected_power(self, array, aggregator) -> pd.Series:
+    def calc_estimated_power(self, array, aggregator) -> pd.Series:
         """Calculates the estimated specific power output of a collector array based on equation 2 formula in ISO 24194.
         """
         # Collector coefficients
         a1 = array.collector_type.a1
         a2 = array.collector_type.a2
         a5 = array.collector_type.a5
         eta0b = array.collector_type.eta0b
@@ -328,13 +360,13 @@
         rd_bti = aggregator(array.rd_bti.data)
         rd_dti = aggregator(array.rd_dti.data)
         iam_b = aggregator(array.iam.data)
         te_amb = aggregator(array.plant.te_amb.data)
         te_op = aggregator(array.te_op.data)
         te_op_deriv = aggregator(array.te_op_deriv.data)
 
-        tp_expected_specific = eta0b * iam_b * rd_bti + eta0b * kd * rd_dti \
-                               - a1 * (te_op - te_amb) \
-                               - a2 * (te_op - te_amb) ** 2 \
-                               - a5 * te_op_deriv
+        tp_estimated_specific = eta0b * iam_b * rd_bti + eta0b * kd * rd_dti \
+                                - a1 * (te_op - te_amb) \
+                                - a2 * (te_op - te_amb) ** 2 \
+                                - a5 * te_op_deriv
 
-        return tp_expected_specific.astype('pint[W m**-2]')
+        return tp_estimated_specific.astype('pint[W m**-2]')
```

## sunpeek/core_methods/pc_method/main.py

```diff
@@ -1,93 +1,128 @@
 """
 Implements Performance Check (PC) Method according to technical standard ISO/DIS 24194.
 
-# HowTo
+HowTo
+=====
 
 To create instances, use
-- PCMethod.create_iso()
-- PCMethod.create_improved()
+- ISO mode: PCMethod.from_method('iso')
+- Extended mode: PCMethod.from_method('extended')
 
 Main method to run an analysis is pc_method.run()
 Results: pc_method.get_results() returns a components.results.PCMethodOutput object.
 
 See docstring in __init__ for more details.
 
-# Implementations
-
-## PCMethodISO
+Implementations
+===============
+PCMethodISO
+-----------
 
 The implementation variant that aligns as closely as possible to the ISO 24194 standard is in class PCMethodISO.
-Create an analysis with PCMethod.create_iso(**kwargs).
+Create an analysis with PCMethod.from_method('iso', **kwargs).
 
-## PCMethodImproved
+PCMethodExtended
+----------------
 
 Reasoning: Some of the data analysis recommendations described in the ISO standard apprently assume the use of Excel or
 other spreadsheet based software. For instance, analysis is based on fixed 1-hourly that start at full hours. This
 does not necessarily lead to the best / most useful results.
 
-This software package implements a variant of the PC method that overcomes some limitations of the strictly ISO-based
-variant. It has a few slight but significant improvements in data analysis and offers some more flexibility,
-while sticking as closely as possible to the intentions and purpose of the ISO 24194 standard.
+This software package implements an extended variant of the Performance Check method that overcomes some limitations of
+the strictly fixed-hour variant described in ISO 24194.
+This 'extended' implementation has a few slight but significant improvements in data analysis,
+while sticking as closely as possible to the intentions and purpose of the ISO 24194 standard:
+It tends to produce more and less noisy intervals in a Performance Check analysis. Numerically, comparable in range to
+PCMethodISO in terms of measured vs expected power. The extended version tends to include more intervals that are
+limit cases compared to the requirements stated in the ISO 24194, hence its results have somewhat higher generality.
+By default, the extended implementation uses a 1-hour averaging, as described in ISO 24194. It can be set to a
+different value. All other PCMethodExtended settings are the same as PCMethodISO.
 
-First analysis validations on real-plant data confirmed that the PCMethodImproved variant reduces
-noise in the analysis output and improves the regression between measured and expected power, the main KPI of the PC
+First analysis validations on real-plant data confirmed that the PCMethodExtended variant reduces
+noise in the analysis output and improves the regression between measured and estimated power, the main KPI of the PC
 method.
 
-Differences of PCMethodImproved over PCMethodISO in detail:
+Differences of PCMethodExtended over PCMethodISO in detail:
 - Uses rolling resampling instead of fixed-hour resampling in PCMethodISO. Consequently, data intervals used for the
 analysis (performance equations) are not restricted to start at full hours.
 - Uses a minimum-noise (minimum relative standard deviation) criterion to select among overlapping interval candidates.
 - Allows different interval lengths, not restricted to 1 hour.
 - Minimum number of non-NaN data records per interval not restricted to 20.
 
 .. codeauthor:: Philip Ohnewein <p.ohnewein@aee.at>
 .. codeauthor:: Lukas Feierl <l.feierl@solid.at>
 .. codeauthor:: Daniel Tschopp <d.tschopp@aee.at>
 """
 
 from abc import ABC, abstractmethod
 import warnings
+import enum
 import datetime as dt
 import pandas as pd
 import numpy as np
-import numbers
+from typing import Union, Optional, Dict, Any
 from statsmodels.formula import api as smf
 
+from sunpeek.common.utils import sp_logger
 from sunpeek.common.unit_uncertainty import Q
-from sunpeek.common.errors import ConfigurationError
-from sunpeek.components import Plant, PCMethodOutput, PCMethodOutputArray
-from sunpeek.core_methods.pc_method import equation as eq
+from sunpeek.components import Plant
+import sunpeek.components.results as results
+from sunpeek.common.errors import PCMethodError
+from sunpeek.components.base import AlgoCheckMode
+from sunpeek.core_methods.pc_method import AvailablePCMethods, AvailablePCEquations
+from sunpeek.core_methods.pc_method.equation import Equation
+from sunpeek.serializable_models import ProblemReport, ProblemType, AlgoProblem
+
+# ------------------------------------------------------------------------------------
+# PC Method parameters
 
-# Default Parameter for PC Method
+# Default values that appear in ISO 24194:
 INTERVAL_LENGTH_ISO = dt.timedelta(hours=1)  # 1 hour = specified in ISO standard
+MIN_INTERVALS_IN_OUTPUT = 20
+
+# Default settings defined in this implementation:
+DEFAULT_ACCURACY_LEVEL = "II"
+# Safety factors
 F_PIPES = 0.98
 F_UNCERTAINTY = 0.90
 F_OTHERS_EQ1 = 0.98
 F_OTHERS_EQ2 = 0.99
+
+# Data
 MIN_DATA_IN_INTERVAL = 10
+LOWER_BOUND__MIN_DATA_IN_INTERVAL = 5
+MAX_NAN_DENSITY = 0.05
+
+# Intervals & gaps
+MAX_INTERVAL_LENGTH = dt.timedelta(hours=12)
 MAX_GAP_IN_INTERVAL = dt.timedelta(minutes=30)
-MAX_NAN_DENSITY = 0.05  # maximum allowed NaN share per interval (0 = no NaNs allowed, 1 = all NaNs is ok)
-MIN_INTERVALS_IN_OUTPUT = 20
+DEFAULT_RATIO__MAX_GAP__TO__INTERVAL_LENGTH = 0.5
+MIN_INTERVAL_LENGTH_EXTENDED = dt.timedelta(minutes=15)
 
 
-class PCMethod(ABC):
-    """Superclass for various variants of the Performance Check Method.
+class PCAccuracyClasses(str, enum.Enum):
+    one = "I"
+    two = "II"
+    three = "III"
 
-    Parameters
-    ----------
-    plant : Plant
-        Fully-configured plant with at least one array, and with virtual sensors calculated.
-    equation_id : {1, 2} (optional)
-        equation_id to be used for the pc method. If 'None', equation_id is chosen based on the input data.
-        Default: None
-    ignore_wind : bool (optional)
-        if True, the wind speed sensor is ignored as a restriction to finding valid intervals for the PC method.
-        Automatically set to True if plant has no wind measurement (plant.ve_wind is None).
-        Default: False
+
+# TODO This is a stub. Probably not needed anymore with the new ISO 24194? Check issue 383
+# def get_default_safety_factors(accuracy_level: PCAccuracyClasses = DEFAULT_ACCURACY_LEVEL):
+#     if accuracy_level == PCAccuracyClasses.one:
+#         pass
+#
+#     raise NotImplementedError()
+
+
+# ------------------------------------------------------------------------------------
+#
+class PCSettings:
+    """PC Method settings: Holds defaults, parses and validates a PC method settings dictionary, replacing None or
+    missing settings with defaults.
 
     safety_pipes : float (optional)
         Safety factor considering heat losses from pipes etc. in the collector loop. To be estimated based on an
         evaluation of the pipe losses - normally only a few %.
         Default: None (0.98)
     safety_uncertainty : float (optional)
         Safety factor considering measurement uncertainty. To be estimated - with the requirements given in 6.1,
@@ -97,204 +132,259 @@
         Safety factor for other uncertainties e.g. related to non-ideal conditions such as: • non-ideal flow
         distribution. To be estimated - should be close to one. • unforeseen heat losses. To be estimated - should
         be close to one. • uncertainties in the model/procedure itself. To be estimated - should be close to one.
         Note - it is recommended to put fO ≤ 1 when eq. (1) is used, as eq. (1) does not consider the influence of
         incidence angle modifiers.
         Default: None (will be set according to used equation)
 
-    check_accuracy_level : {1, 2} (optional)
+    check_accuracy_level : {"I", "II", "III"} (optional)
         Level of accuracy of sensor as specified in ISO chapter 6. Will only be used for reporting and does not
         influence the output of the pc method.
     interval_length : dt.datetime (optional)
         Length of the interval over which single data records are averaged.
-        This is set to 1 hour in the ISO 24194 standard, but can be changed for PCMethodImproved.
+        This is set to 1 hour in the ISO 24194 standard, but can be changed for PCMethodExtended.
 
     max_nan_density : float (optional)
-        maximum percentage of missing data allowed. Intervals which have higher nan density will be discarded.
+        maximum percentage of missing data allowed per interval. Intervals which have higher nan density will be
+        discarded. 0 = no NaNs allowed, 1 = all NaNs is ok.
     min_data_in_interval : int (optional)
-        Minimum non-NaN values per interval (defined by self.interval_length).
+        Minimum non-NaN values per interval (defined by self.settings.interval_length).
         The default value of 20 is stated in ISO 24194 chapter 6.2.
-        Explanation: Independently from NaNs, the situation could arise where there are only a few values in an
+        Explanation: Independently of NaNs, the situation could arise where there are only a few values in an
         interval, and it doesn't make much sense to include such intervals.
     max_gap_in_interval : dt.timedelta
         Even if an interval has a minimum number of intervals (at least min_data_in_interval), those records might be
         clustered e.g. at the beginning or end of the interval, with large gaps without data records in between.
+
+    Notes
+    -----
+    Some settings for the Performance Check calculations depend on the chosen method (ISO | extended) and equation.
+    That is why method and equation must be known at __init__ time.
     """
+    safety_pipes: Optional[float]
+    safety_uncertainty: Optional[float]
+    safety_others: Optional[float]  # has no single default, depends on & needs to be set by Equation
+    interval_length: Optional[dt.timedelta]
+    max_gap_in_interval: Optional[dt.timedelta]
+    min_data_in_interval: Optional[int]
+    max_nan_density: Optional[float]
+    min_intervals_in_output: Optional[int]
+    check_accuracy_level: Optional[str]
+
+    default_settings = dict(
+        safety_pipes=F_PIPES,
+        safety_uncertainty=F_UNCERTAINTY,
+        safety_others=None,  # Has no single default, depends on & needs to be set by Equation
+        interval_length=INTERVAL_LENGTH_ISO,
+        min_data_in_interval=MIN_DATA_IN_INTERVAL,
+        max_gap_in_interval=None,  # Default: fixed ratio of interval_length
+        max_nan_density=MAX_NAN_DENSITY,
+        min_intervals_in_output=MIN_INTERVALS_IN_OUTPUT,
+        check_accuracy_level=DEFAULT_ACCURACY_LEVEL,
+    )
 
-    method_name = ""
-    mode = ""
+    @property
+    def safety_combined(self):
+        return self.safety_uncertainty * self.safety_pipes * self.safety_others
+
+    @property
+    def names(self):
+        return self.default_settings.keys()
 
     def __init__(self,
-                 plant: Plant,
-                 equation_id: int = None,
-                 ignore_wind: bool = False,
-                 safety_pipes: float = None,
-                 safety_uncertainty: float = None,
-                 safety_others: float = None,
-                 check_accuracy_level: int = 2,
-                 interval_length: dt.timedelta = INTERVAL_LENGTH_ISO,
-                 min_data_in_interval: int = MIN_DATA_IN_INTERVAL,
-                 max_gap_in_interval: dt.timedelta = MAX_GAP_IN_INTERVAL,
-                 max_nan_density: float = MAX_NAN_DENSITY,
-                 ):
-        self.plant = plant
-        self.equation_id_in = equation_id
-        self.equation = None
-        self.ignore_wind = True if (plant.ve_wind is None) else ignore_wind
-        self.check_accuracy_level = check_accuracy_level
-
-        self.safety_combined = None
-        for f in [safety_pipes, safety_uncertainty, safety_others]:
-            assert (f is None) or ((f > 0) and (f <= 1)), \
-                'All PC method safety factors must be floats between 0 and 1.'
-        self._safety_pipes = safety_pipes
-        self._safety_others = safety_others
-        self._safety_uncertainty = safety_uncertainty
-
-        self._interval_length = None
-        self.max_gap_in_interval = max_gap_in_interval
-        self.interval_length = interval_length
-        self.max_nan_density = max_nan_density
-        self.min_data_in_interval = min_data_in_interval
+                 method: Union[AvailablePCMethods, str],
+                 equation: Union[AvailablePCEquations, int],
+                 **kwargs):
+
+        settings = kwargs.copy()
+        defaults = self.default_settings
+
+        for k in settings:
+            if k not in self.names:
+                raise PCMethodError(f'Unkown Performance Check method setting: {k}.'
+                                    f'Known settings: {", ".join(self.names)}.')
+
+        # Replace None / missing with default
+        settings = {k: v for k, v in settings.items() if v is not None}
+        for key in self.names:
+            self.__setattr__(key, settings.get(key, defaults[key]))
+
+        # Safety factors
+        if self.safety_others is None:
+            if equation == AvailablePCEquations.one:
+                self.safety_others = F_OTHERS_EQ1
+            elif equation == AvailablePCEquations.two:
+                self.safety_others = F_OTHERS_EQ2
+
+        # Safety factors
+        safety_ok = lambda x: (x is None) or ((x > 0) and (x <= 1))
+        for f in ['safety_pipes', 'safety_uncertainty', 'safety_others']:
+            if not safety_ok(self.__getattribute__(f)):
+                raise PCMethodError(
+                    f'All Performance Check safety factors must be either None or floats between 0 and 1. '
+                    f'Got "{f}" = {str(f)}.')
+
+        # interval length
+        if self.interval_length > MAX_INTERVAL_LENGTH:
+            raise PCMethodError(
+                f'Performance Check maximum allowed interval length is {str(MAX_INTERVAL_LENGTH)}.')
+
+        if method == AvailablePCMethods.iso:
+            if self.interval_length != INTERVAL_LENGTH_ISO:
+                raise PCMethodError(
+                    f'For a Performance Check evaluation following the fixed-hour ("ISO") scheme, '
+                    f'the "interval_length" is fixed to 1 hour, as defined in the ISO 24194.')
+
+        if method == AvailablePCMethods.extended:
+            if self.interval_length < MIN_INTERVAL_LENGTH_EXTENDED:
+                raise PCMethodError(
+                    f'For a Performance Check evaluation following the rolling-hour ("extended") scheme, '
+                    f'"interval_length" should not be lower than {str(MIN_INTERVAL_LENGTH_EXTENDED)}.')
 
-        self._mask = None
-        self._bins = None
-        self._output = {}
-        return
+        # max_gap_in_interval
+        if self.max_gap_in_interval is None:
+            self.max_gap_in_interval = self.interval_length * DEFAULT_RATIO__MAX_GAP__TO__INTERVAL_LENGTH
+        if self.max_gap_in_interval > self.interval_length:
+            warnings.warn(f'Performance Check "max_gap_in_interval" cannot be longer than "interval_length". '
+                          f'Setting "max_gap_in_interval" to {self.interval_length}.')
+            self.max_gap_in_interval = self.interval_length
 
-    @classmethod
-    def create(cls, method: str, plant: Plant, **kwargs):
-        method = method.lower()
-        assert method in ['iso', 'improved'], f'Unknown PC method: {method}.'
-        if method == 'iso':
-            return PCMethodISO(plant, **kwargs)
-        if method == 'improved':
-            return PCMethodImproved(plant, **kwargs)
+        # min_data_in_interval
+        if self.min_data_in_interval < LOWER_BOUND__MIN_DATA_IN_INTERVAL:
+            raise PCMethodError(
+                f'Performance Check method option "min_data_in_interval" too low ({settings["min_data_in_interval"]}): '
+                f'Setting "min_data_in_interval" to less than '
+                f'{LOWER_BOUND__MIN_DATA_IN_INTERVAL} most likely yields poor results.')
 
-    @classmethod
-    def create_iso(cls, plant, **kwargs):
-        # kwargs.update({
-        #     # 'evaluation_mode': 'ISO',
-        #     # 'interval_length': INTERVAL_LENGTH_ISO
-        # })
-        return PCMethodISO(plant, **kwargs)
+        # max_nan_density
+        if self.max_nan_density > 1 or self.max_nan_density < 0:
+            raise PCMethodError(
+                f'Performance Check option "max_nan_density" must be None or a float between 0 and 1. evaluation '
+                f'Got {str(self.max_nan_density)}.')
+
+        # min_intervals_in_output
+        if self.min_intervals_in_output <= 0:
+            raise PCMethodError(
+                f'Performance Check option "min_intervals_in_output" must be None or greater than 0. '
+                f'Got {str(self.min_intervals_in_output)}.')
+        if method == AvailablePCMethods.iso:
+            if self.min_intervals_in_output != MIN_INTERVALS_IN_OUTPUT:
+                raise PCMethodError(
+                    f'For a Performance Check evaluation following the fixed-hour ("ISO") scheme, '
+                    f'"min_intervals_in_output" is fixed to {MIN_INTERVALS_IN_OUTPUT}, as defined in the ISO 24194.')
+
+        # check_accuracy_level
+        if self.check_accuracy_level is None:
+            self.check_accuracy_level = DEFAULT_ACCURACY_LEVEL
+        if self.check_accuracy_level not in list(PCAccuracyClasses):
+            raise PCMethodError(
+                f'Performance Check option "check_accuracy_level" invalid. '
+                f'Must be one of {", ".join(list(PCAccuracyClasses))}. '
+                f'Got {str(self.check_accuracy_level)}.')
+
+        # Now all settings should have been set / no None left
+        none_settings = [s for s in self.names if self.__getattribute__(s) is None]
+        if none_settings:
+            raise PCMethodError(f'Some settings are None after initializing PCSettings. This is an internal error. '
+                                f'None settings: {", ".join(none_settings)}')
 
-    @classmethod
-    def create_improved(cls, plant, **kwargs):
-        # kwargs.update({
-        #     # 'evaluation_mode': 'improved'
-        # })
-        return PCMethodImproved(plant, **kwargs)
 
-    @property
-    def interval_length(self):
-        return self._interval_length
+# ------------------------------------------------------------------------------------
+# PC Method
 
-    @interval_length.setter
-    def interval_length(self, val: dt.timedelta):
-        self._set_interval_length(val)
+# noinspection PyArgumentList
+class PCMethod(ABC):
+    """Superclass for various variants of the Performance Check Method.
 
-    @abstractmethod
-    def _set_interval_length(self, val: dt.timedelta):
-        raise NotImplementedError
+    Parameters
+    ----------
+    plant : Plant
+        Fully-configured plant with at least one array, and with virtual sensors calculated.
+    equation : Equation
+        Equation to be used for the PC method. See ISO 24194 chapter 5.2.1.
+    kwargs : passed to PCSettings
+    """
 
-    @property
-    def min_data_in_interval(self):
-        return self._min_data_in_interval
+    method_name = ""
+    mode = ""
 
-    @min_data_in_interval.setter
-    def min_data_in_interval(self, val: int):
-        if val is None:
-            self._min_data_in_interval = MIN_DATA_IN_INTERVAL
-            return
-        assert val >= 5, \
-            'Setting PC method "min_data_in_interval" to less than 5 most likely yields poor results.'
-        self._min_data_in_interval = val
+    @classmethod
+    def from_method(cls,
+                    method: Union[AvailablePCMethods, str],
+                    plant: Plant,
+                    equation: Union[AvailablePCEquations, int],
+                    use_wind: bool = True,
+                    **kwargs):
+
+        if method == AvailablePCMethods.iso:
+            return PCMethodISO(plant, equation, use_wind, **kwargs)
+        elif method == AvailablePCMethods.extended:
+            return PCMethodExtended(plant, equation, use_wind, **kwargs)
+        else:
+            raise PCMethodError(f'Cannot create PC method, unknown method "{method}".')
 
-    @property
-    def max_gap_in_interval(self):
-        return self._max_gap_in_interval
+    def __init__(self,
+                 plant: Plant,
+                 equation: Union[AvailablePCEquations, int],
+                 use_wind: bool = True,
+                 **kwargs):
+        self.plant = plant
+        self.equation = Equation.create(equation, use_wind)
+        self.settings = PCSettings(method=self.mode, equation=equation, **kwargs)
 
-    @max_gap_in_interval.setter
-    def max_gap_in_interval(self, val: dt.timedelta):
-        if val is None:
-            self._max_gap_in_interval = 0.5 * self.interval_length
-            return
-        if self.interval_length is not None:
-            assert val < self.interval_length, \
-                f'Value of "max_gap_in_interval" ({val}) cannot be longer than interval_length {self.interval_length}.'
-        self._max_gap_in_interval = val
+        self._mask = None
+        self._bins = None
+        self._output = {}
+        return
 
-    @property
-    def max_nan_density(self):
-        return self._max_nan_density
+    def run(self) -> results.PCMethodOutput:
+        """ Applies the Performance Check on the plant and returns the estimated and calculated power.
+        """
+        start_time = dt.datetime.now(dt.timezone.utc)
 
-    @max_nan_density.setter
-    def max_nan_density(self, val: float):
-        assert (val >= 0) and (val < 1), \
-            'PC Method parameter "max_nan_density" must be a float between 0 and 1.'
-        if val is None:
-            self._max_nan_density = MAX_NAN_DENSITY
-        else:
-            self._max_nan_density = val
+        if self._filter_intervals():
+            self._calc_output()
 
-    @property
-    def equation_id_in(self):
-        return self._equation_id_in
+        pc_method_output = self._create_output_object(start_time)
+        return pc_method_output
 
-    @equation_id_in.setter
-    def equation_id_in(self, val):
-        if val is not None:
-            assert isinstance(val, numbers.Number) and (val in [1, 2]), \
-                f'Invalid PC method parameter "equation_id": {val}. Valid inputs are: 1, 2.'
-        self._equation_id_in = val
+    def report_problems(self, check_mode: AlgoCheckMode) -> ProblemReport:
+        r = ProblemReport()
 
-    @property
-    def equation_id(self):
-        return None if (self.equation is None) else self.equation.id
+        if not self.plant.arrays:
+            r.add_own(AlgoProblem(ProblemType.component_missing, self.plant, 'arrays',
+                                  'To run the Performance Check method, you need to add arrays to the plant.'))
+
+        for slot_name in ['te_amb', 'tp']:
+            if self.plant.is_slot_missing(slot_name, check_mode):
+                r.add_own(AlgoProblem(ProblemType.component_slot, self.plant, slot_name))
+
+        for i, array in enumerate(self.plant.arrays):
+            r_array = self.equation.report_problems(array, check_mode)
+            if not r_array.success:
+                r.add_sub(f'Array {i + 1} called "{array.name}"', r_array)
+
+        return r
 
-    # --------------------
-    # RUN related methods
-    # --------------------
     @abstractmethod
     def _aggregate_candidates(self, s: pd.Series, agg_fun: str):
-        """Implements the aggregation of sensor data records, e.g. hourly mean (ISO) or rolling mean (improved),
+        """Implements the aggregation of sensor data records, e.g. hourly mean (ISO) or rolling mean (extended),
         into candidate intervals that may be selected as the final PC method intervals.
 
         Parameters
         ----------
         s : pd. Series
         agg_fun : str, passed to pandas aggregate
 
         Returns
         -------
         pd.Series : resampled data
         """
         raise NotImplementedError
 
-    def _aggregate_intervals(self, s: pd.Series):
-        """Implements the aggregation of sensor data records for the final intervals selected among the candidates.
-
-        Parameters
-        ----------
-        s : pd. Series
-
-        Returns
-        -------
-        pd.Series : resampled data
-
-        Notes
-        -----
-        - The final intervals meet data quality requirements and the restrictions of PC method Table 1.
-        - The number of intervals is usually much smaller than the number of candidates. Thus groupby should be
-        faster than resampling / rolling again and then filtering on self._mask['best_intervals']
-        - The same aggregation is used for PCMethodISO and PCMethodImproved.
-        """
-        return s.groupby(self._bins).mean()
-
     @abstractmethod
     def _select_best_intervals(self):
         """Among all possible intervals, select the best non-overlapping intervals to be evaluated with the PC method.
         Returns pd.Series (with index self.plant.time_index) which is True at the starting points of the intervals.
         """
         raise NotImplementedError
 
@@ -316,318 +406,276 @@
         - max_nan_density
         - DataFrame index is self.plant.time_index.
         """
         self._mask = pd.DataFrame()
 
         # min_data_in_interval
         value_count = self._aggregate_candidates(self.plant.time_index.to_series(), 'count')
-        self._mask['min_data_ok'] = (value_count >= self.min_data_in_interval)
+        self._mask['min_data_ok'] = (value_count >= self.settings.min_data_in_interval)
 
         # max_nan_density
         # nan_mask: True where _any_ of the sensors used in the PC method is NaN. Those records are rejected.
-        nan_mask = self.equation.get_nan_mask(self.plant, self.ignore_wind)
+        nan_mask = self.equation.get_nan_mask(self.plant)
         nan_density = self._aggregate_candidates(nan_mask, 'sum') / value_count
-        self._mask['nan_density_ok'] = (nan_density <= self.max_nan_density)
+        self._mask['nan_density_ok'] = (nan_density <= self.settings.max_nan_density)
 
         # max_gap_in_interval
         # Define gap of an index as average between backward and forward gap.
         bwd = self.plant.time_index.to_series().diff().dt.total_seconds()
         fwd = bwd.shift(-1)
         gaps = pd.concat([bwd, fwd], axis=1).mean(axis=1)
         max_gap = self._aggregate_candidates(gaps, 'max')
-        self._mask['max_gap_ok'] = (max_gap <= self.max_gap_in_interval.total_seconds())
+        self._mask['max_gap_ok'] = (max_gap <= self.settings.max_gap_in_interval.total_seconds())
 
         # Restrictions to interval filtering described in ISO 24194 Table 1, chapter 5.4.
         self._mask['pc_restrictions'] = \
             self.equation.calc_pc_restrictions(plant=self.plant,
-                                               ignore_wind=self.ignore_wind,
                                                resampler=lambda s, fun='mean': self._aggregate_candidates(s, fun))
 
         self._mask['best_intervals'] = self._select_best_intervals()
         n_intervals = self._mask['best_intervals'].sum()
         self._output['n_intervals'] = n_intervals
 
-        if n_intervals < MIN_INTERVALS_IN_OUTPUT:
-            warnings.warn(
-                f'PC method analysis found {n_intervals} intervals. For checking the collector performance, '
-                f'the ISO 24194 standard recommends to have at least {MIN_INTERVALS_IN_OUTPUT} intervals.')
+        if (n_intervals < self.settings.min_intervals_in_output) and (self.mode == AvailablePCMethods.iso):
+            # TODO transport this warning over the API
+            sp_logger.warn(
+                f'Performance check analysis found {n_intervals} intervals. For checking the collector performance, '
+                f'the ISO 24194 recommends to have at least {MIN_INTERVALS_IN_OUTPUT} intervals.')
         if n_intervals == 0:
             return False
 
         # Out of the marked best intervals, create bins for groupby
         self._bins = pd.Series(data=np.nan, index=self.plant.time_index)
         for i, end in enumerate(self._mask.index[self._mask['best_intervals']]):
-            mask = (self._bins.index > end - self.interval_length) & (self._bins.index <= end)
+            mask = (self._bins.index > end - self.settings.interval_length) & (self._bins.index <= end)
             self._bins.loc[mask] = i
 
         return True
 
-    def run(self):
-        """ Applies the Performance Check on the plant and returns the estimated and calculated power."""
-        # Set equation based on given equation_id_in and make sure PC method can be applied.
-        # Under the hood, _set_equation() calls verify_validate.validate_data(),
-        # so we can be sure plant config and data are ok to run the PC method.
-        start_time = dt.datetime.now(dt.timezone.utc)
-        self._set_equation()
-        self.set_safety_factor()  # cannot be done before, depends on self.equation
-
-        if self._filter_intervals():
-            self._calc_output()
-
-        pc_method_output = self._create_output_object(start_time)
-        return pc_method_output
-
     def _calc_output(self):
-        """Calculates expected power for plant and all arrays, saves results in self attributes.
+        """Calculates estimated power for plant and all arrays, saves results in self attributes.
 
         Returns
         -------
         Nothing. Sets self._output_plant, self._slopes and self._output_arrays
         """
-        tp_expected = 0
+        tp_estimated = 0
         te_op_mean_area = 0
         self._output['arrays'] = {}
-        aggregator = self._aggregate_intervals
+
+        # Aggregation of sensor data records for the final intervals selected among the candidates.
+        #  - The final intervals meet data quality requirements and the restrictions of PC method Table 1.
+        #  - The number of intervals is usually much smaller than the number of candidates. Thus groupby should be
+        #    faster than resampling / rolling again and then filtering on self._mask['best_intervals']
+        #  - The same aggregation is used for PCMethodISO and PCMethodExtended.
+        # aggregator = self._aggregate_intervals
+        aggregator = lambda s: s.groupby(self._bins).mean()
 
         for array in self.plant.arrays:
-            df = self.equation.calc_expected_power(array, aggregator).to_frame(name='tp_sp_expected')
-            df['tp_sp_expected_safety'] = df['tp_sp_expected'] * self.safety_combined
-            df['tp_expected'] = df['tp_sp_expected'] * array.area_gr
-            if array.tp is not None:
+            df = self.equation.calc_estimated_power(array, aggregator).to_frame(name='tp_sp_estimated')
+            df['tp_sp_estimated_safety'] = df['tp_sp_estimated'] * self.settings.safety_combined
+            df['tp_estimated'] = df['tp_sp_estimated'] * array.area_gr
+            if (not array.tp.is_virtual) or (array.tp.is_virtual and array.tp.can_calculate):
                 df['tp_sp_measured'] = aggregator(array.tp.data) / array.area_gr
             # save DataFrame with array results in dict
             self._output['arrays'][array] = df
-            tp_expected += df['tp_expected']
+            tp_estimated += df['tp_estimated']
             te_op_mean_area += aggregator(array.te_op.data) * array.area_gr
 
         df = aggregator(self.plant.tp.data.astype('pint[kW]')).to_frame(name='tp_measured')
         df['tp_sp_measured'] = df['tp_measured'].astype('pint[W]') / self.plant.area_gr
-        df['tp_sp_expected'] = tp_expected / self.plant.area_gr
-        df['tp_expected'] = tp_expected.astype('pint[kW]')
-        df['tp_sp_expected_safety'] = df['tp_sp_expected'] * self.safety_combined
+        df['tp_sp_estimated'] = tp_estimated / self.plant.area_gr
+        df['tp_estimated'] = tp_estimated.astype('pint[kW]')
+        df['tp_sp_estimated_safety'] = df['tp_sp_estimated'] * self.settings.safety_combined
         # area-weighted mean operating temperature over all arrays
         te_op_mean = te_op_mean_area / self.plant.area_gr
         df['te_op_mean'] = te_op_mean.astype('pint[degC]')
         self._output['plant'] = df
 
-        # Slope between measured and expected power, for plant
-        df_slopes = self._output['plant'].loc[:, ['tp_sp_measured', 'tp_sp_expected', 'tp_sp_expected_safety']]
+        # Slope between measured and estimated power, for plant
+        df_slopes = self._output['plant'].loc[:, ['tp_sp_measured', 'tp_sp_estimated', 'tp_sp_estimated_safety']]
         df_slopes = df_slopes.astype('float64')
 
         self._output['slopes'] = {}
-        fit = smf.ols('tp_sp_measured ~ tp_sp_expected -1', data=df_slopes).fit()
+        fit = smf.ols('tp_sp_measured ~ tp_sp_estimated -1', data=df_slopes).fit()
         self._output['slopes']['target_actual'] = Q(fit.params.to_numpy()[0], '')
 
-        fit = smf.ols('tp_sp_measured ~ tp_sp_expected_safety -1', data=df_slopes).fit()
+        fit = smf.ols('tp_sp_measured ~ tp_sp_estimated_safety -1', data=df_slopes).fit()
         self._output['slopes']['target_actual_safety'] = Q(fit.params.to_numpy()[0], '')
 
-    def set_safety_factor(self, safety_pipes=None, safety_uncertainty=None, safety_others=None):
-        safety_pipes = self._safety_pipes if (safety_pipes is None) else safety_pipes
-        safety_uncertainty = self._safety_uncertainty if (safety_uncertainty is None) else safety_uncertainty
-        safety_others = self._safety_others if (safety_others is None) else safety_others
-
-        safety_pipes = F_PIPES if (safety_pipes is None) else safety_pipes
-        safety_uncertainty = F_UNCERTAINTY if (safety_uncertainty is None) else safety_uncertainty
-
-        assert self.equation_id is not None, \
-            'Cannot determine PC method safety factor "safety_others" because equation_id is None.'
-        if safety_others is None:
-            if self.equation_id == 1:
-                safety_others = F_OTHERS_EQ1
-            elif self.equation_id == 2:
-                safety_others = F_OTHERS_EQ2
-
-        self.safety_combined = safety_others * safety_pipes * safety_uncertainty
-
-    # --------------------
-    # OUTPUT related methods
-    # --------------------
-    def _create_output_object(self, start_time):
+    def _create_output_object(self, start_time) -> results.PCMethodOutput:
         """Gather all PC method calculation outputs required for ISO 24194 Annex A1, and a few more.
 
         Returns
         -------
         PCMethodOutput object
         """
-        out = PCMethodOutput()
+        out = results.PCMethodOutput()
+
         out.plant = self.plant
+
         out.datetime_eval_start = self.plant.context.eval_start
         out.datetime_eval_end = self.plant.context.eval_end
 
-        # Algorithm settings
+        # Algorithm / Strategy
         out.pc_method_name = self.method_name
-        out.evaluation_mode = self.mode
-        out.equation = self.equation_id
-        out.check_accuracy_level = self.check_accuracy_level
-
-        out.interval_length = self.interval_length
-        out.safety_combined = self.safety_combined
-        out.wind_used = not self.ignore_wind
-
-        out.max_nan_density = self.max_nan_density
-        out.min_data_in_interval = self.min_data_in_interval
-        out.max_gap_in_interval = self.max_gap_in_interval
-
-        # Results
-        out.n_intervals = self._output['n_intervals']
-        if out.n_intervals == 0:
-            return out
+        out.evaluation_mode = self.mode.value
+        out.equation = self.equation.id
+        out.wind_used = self.equation.use_wind
+
+        # Strategy PCSettings
+        out.settings = dict(
+            safety_pipes=self.settings.safety_pipes,
+            safety_uncertainty=self.settings.safety_uncertainty,
+            safety_others=self.settings.safety_others,
+            safety_combined=self.settings.safety_combined,
+            interval_length=self.settings.interval_length,
+            max_gap_in_interval=self.settings.max_gap_in_interval,
+            min_data_in_interval=self.settings.min_data_in_interval,
+            max_nan_density=self.settings.max_nan_density,
+            min_intervals_in_output=self.settings.min_intervals_in_output,
+            check_accuracy_level=self.settings.check_accuracy_level,
+        )
+
+        # Plant results
+        plant_out = results.PCMethodOutputPlant()
+        plant_out.plant = self.plant
+        plant_out.n_intervals = self._output['n_intervals']
 
         intervals_end = self._mask.index[self._mask['best_intervals']].to_pydatetime()
-        out.datetime_intervals_start = intervals_end - self.interval_length
-        out.datetime_intervals_end = intervals_end
+        plant_out.datetime_intervals_start = intervals_end - self.settings.interval_length
+        plant_out.datetime_intervals_end = intervals_end
 
-        # Plant results
-        df = self._output['plant']
-        unit_tp = 'pint[kW]'
-        unit_tp_sp = 'pint[W m**-2]'
-        out.tp_measured = df['tp_measured'].astype(unit_tp)
-        out.tp_sp_measured = df['tp_sp_measured'].astype(unit_tp_sp)
-        out.tp_sp_expected = df['tp_sp_expected'].astype(unit_tp_sp)
-        out.tp_sp_expected_safety = df['tp_sp_expected_safety'].astype(unit_tp_sp)
+        has_intervals = (self._output['n_intervals'] > 0)
 
-        out.target_actual_slope = self._output['slopes']['target_actual']
-        out.target_actual_slope_safety = self._output['slopes']['target_actual_safety']
+        if has_intervals:
+            df = self._output['plant']
+            unit_tp = 'pint[kW]'
+            unit_tp_sp = 'pint[W m**-2]'
+
+            # This is necessary to prevent unneeded calls of config_virtuals -> PCMethodOutputPlant is AttrSetterMixin
+            try:
+                plant_out.defer_post_config_changed_actions = True
+                plant_out.tp_measured = df['tp_measured'].astype(unit_tp)
+                plant_out.tp_sp_measured = df['tp_sp_measured'].astype(unit_tp_sp)
+                plant_out.tp_sp_estimated = df['tp_sp_estimated'].astype(unit_tp_sp)
+                plant_out.tp_sp_estimated_safety = df['tp_sp_estimated_safety'].astype(unit_tp_sp)
+                plant_out.mean_tp_sp_measured = plant_out.tp_sp_measured.mean()
+                plant_out.mean_tp_sp_estimated = plant_out.tp_sp_estimated.mean()
+                plant_out.mean_tp_sp_estimated_safety = plant_out.tp_sp_estimated_safety.mean()
+                plant_out.target_actual_slope = self._output['slopes']['target_actual']
+                plant_out.target_actual_slope_safety = self._output['slopes']['target_actual_safety']
+
+                te = self._output['plant']['te_op_mean'].mean().to('degC')
+                plant_out.mean_temperature = te
+                te_s = pd.Series(data=te.to('K').magnitude).astype('pint[K]')
+
+                plant_out.fluid_solar = self.plant.fluid_solar
+                no_fluid = (self.plant.fluid_solar is None)
+                plant_out.mean_fluid_density = None if no_fluid else Q(self.plant.fluid_solar.get_density(te_s)[0])
+                plant_out.mean_fluid_heat_capacity = None if no_fluid else Q(
+                    self.plant.fluid_solar.get_heat_capacity(te_s)[0])
+            finally:
+                plant_out.defer_post_config_changed_actions = False
+
+        out.plant_output = plant_out
 
         # Array results
         array_results = []
         for array in self.plant.arrays:
-            df = self._output['arrays'][array]
-            arr_out = PCMethodOutputArray()
+            arr_out = results.PCMethodOutputArray()
             arr_out.array = array
-            arr_out.tp_sp_measured = df['tp_sp_measured'].astype(unit_tp_sp) if ('tp_sp_measured' in df.columns) \
-                else None
-            arr_out.tp_sp_expected = df['tp_sp_expected'].astype(unit_tp_sp)
-            arr_out.tp_sp_expected_safety = df['tp_sp_expected_safety'].astype(unit_tp_sp)
-            array_results.append(arr_out)
-        out.array_results = array_results
 
-        out.fluid_solar = self.plant.fluid_solar
-        te = self._output['plant']['te_op_mean'].mean().to('degC')
-        out.mean_temperature = te
-        te_s = pd.Series(data=te.to('K').magnitude).astype('pint[K]')
-        out.mean_fluid_density = Q(self.plant.fluid_solar.get_density(te_s)[0])
-        out.mean_fluid_heat_capacity = Q(self.plant.fluid_solar.get_heat_capacity(te_s)[0])
+            if has_intervals:
+                df = self._output['arrays'][array]
+                # This is necessary to prevent unneeded calls of config_virtuals -> PCMethodOutputArray is AttrSetterMixin
+                try:
+                    plant_out.defer_post_config_changed_actions = True
+                    if 'tp_sp_measured' in df.columns:
+                        arr_out.tp_sp_measured = df['tp_sp_measured'].astype(unit_tp_sp)
+                        arr_out.mean_tp_sp_measured = arr_out.tp_sp_measured.mean()
+                    else:
+                        arr_out.tp_sp_measured = None
+                        arr_out.mean_tp_sp_measured = None
+
+                    arr_out.tp_sp_estimated = df['tp_sp_estimated'].astype(unit_tp_sp)
+                    arr_out.tp_sp_estimated_safety = df['tp_sp_estimated_safety'].astype(unit_tp_sp)
+                    arr_out.mean_tp_sp_estimated = arr_out.tp_sp_estimated.mean()
+                    arr_out.mean_tp_sp_estimated_safety = arr_out.tp_sp_estimated_safety.mean()
+                finally:
+                    plant_out.defer_post_config_changed_actions = False
 
-        return out
-
-    # --------------------
-    # EQUATION related methods
-    # --------------------
-    def _set_equation(self):
-        """Returns the requested equation_id class based on the requested eq_id or the sensors available to plant.
-        """
-        if self.equation_id_in is None:
-            self.equation = self._get_optimal_equation()
-        elif self._equation_available(self.equation_id_in)[0]:
-            self.equation = eq.create_eq(self.equation_id_in)
-        else:
-            raise ConfigurationError(
-                f'Requirements to apply PC Method equation {self.equation_id_in} to the plant and its arrays '
-                f'are not fulfilled. '
-                f'Reason: {self._equation_available(self.equation_id_in)[1]}. '
-                f'For details, run pc_method.verify_validate.validate_data() on the plant.')
-
-    def _get_optimal_equation(self):
-        """Return optimal / best equation_id based on available information in plant sensors and plant config.
-        Precendence is given to Equation2 if all requirements are fulfilled.
-        See: https://gitlab.com/sunpeek/sunpeek/-/issues/174
-        """
-        if self._equation_available(2)[0]:
-            return eq.create_eq(2)
-        elif self._equation_available(1)[0]:
-            return eq.create_eq(1)
-        else:
-            raise ConfigurationError(
-                f'Requirements to apply PC Method equation 1 or equation 2 to the plant and its arrays '
-                f'are not fulfilled. '
-                f'Reason for equation 1: {self._equation_available(1)[1]}. '
-                f'Reason for equation 2: {self._equation_available(2)[1]}. '
-                f'For details, run pc_method.verify_validate.validate_data() on the plant.')
+            array_results.append(arr_out)
 
-    def _equation_available(self, equation_id):
-        """Returns whether PC equation (1 or 2) is available (all requirements fulfilled) for plant config + data.
+        out.array_output = array_results
 
-        Returns
-        -------
-        tuple : False if not available, reason
-        """
-        from sunpeek.core_methods.pc_method import validate_data
-        try:
-            validate_data(self.plant, equation_id, self.ignore_wind)
-        except AssertionError as ex:
-            return False, ex.__str__()
-        return True, ''
+        return out
 
 
 class PCMethodISO(PCMethod):
     """This PC method implementation aligns as strictly as possible to the method as defined in the technical
-    standard ISO/DIS 24194.
+    standard ISO 24194.
     """
 
-    method_name = "PC Method 'ISO DIS 24194'"
-    mode = 'ISO'
-
-    def _set_interval_length(self, val: dt.timedelta):
-        assert val == INTERVAL_LENGTH_ISO, \
-            'For a PC Method ISO evaluation, the "interval_length" is fixed to 1 hour as defined in the ISO 24194.'
-        self._interval_length = val
-        # Invalid max_gap? Reset to default value
-        if self.max_gap_in_interval >= self.interval_length:
-            self.max_gap_in_interval = None
+    method_name = "PC Method 'ISO 24194'"
+    mode = AvailablePCMethods.iso
 
     def _aggregate_candidates(self, s, agg_fun):
-        s = s.resample(self.interval_length, closed='right', label='right').aggregate(agg_fun)
+        s = s.resample(self.settings.interval_length, closed='right', label='right').aggregate(agg_fun)
         return s
 
     def _select_best_intervals(self):
         """Due to the fixed-hour resampling pattern used in the PCMethodISO data aggregation, we have no overlapping
         intervals, so all intervals that fulfill all constraints (self._mask) are ok.
         """
         return self._mask.all(axis='columns')
 
 
-class PCMethodImproved(PCMethod):
-    """This class implements an alternative variant of the PC method, with improvements in data analysis.
+class PCMethodExtended(PCMethod):
+    """This class implements the "extended" variant of the Performance Check method, with improvements in data
+    analysis. See class docstring for more info.
     """
 
-    method_name = "PC Method 'ISO DIS 24194', improved"
-    mode = 'improved'
-
-    def _set_interval_length(self, val: dt.timedelta):
-        assert val >= dt.timedelta(minutes=15), \
-            'Setting PC method "interval_length" to less than 15 minutes most likely yields poor results.'
-        self._interval_length = val
-        # Invalid max_gap? Reset to default value
-        if self.max_gap_in_interval >= self.interval_length:
-            self.max_gap_in_interval = None
+    method_name = "PC Method 'ISO 24194' extended"
+    mode = AvailablePCMethods.extended
 
     def _aggregate_candidates(self, s, agg_fun='mean'):
-        s_out = s.rolling(window=self.interval_length, closed='right').aggregate(agg_fun)
+        s_out = s.rolling(window=self.settings.interval_length, closed='right').aggregate(agg_fun)
+        # For some reason, the "rolling" operation drops the pint dtype.
         if agg_fun not in ['sum', 'count']:
-            s_out = s_out.astype(s.dtype)  # rolling drops pint dtype...
+            s_out = s_out.astype(s.dtype)
         return s_out
 
     def _select_best_intervals(self):
+        """Due to the rolling averaging used in the PCMethodExtended data aggregation, we might have overlapping
+        intervals that fulfill all ISO 24194 requirements.
+        This algorithm ranks intervals according to a score, which is relative standard deviation of thermal power,
+        evaluiated over the interval.
+        This algorithm chooses the best interval, then excludes all overlapping intervals, goes on with the
+        remaining intervals etc. until no intervals are left.
+        """
         # Intervals that fulfill all constraints so far:
         is_candidate = self._mask.all(axis='columns')
 
         # Criterion to find "best" interval among overlapping: smallest relative standard deviation of plant power.
         tp = self.plant.tp.data
-        variation = (self._aggregate_candidates(tp, 'mean') / self._aggregate_candidates(tp, 'std')).astype('float64')
+        variation = (self._aggregate_candidates(tp, 'mean') / self._aggregate_candidates(tp, 'std')).astype(
+            'float64')
         score = 1 / variation
         score[~is_candidate] = 0
 
-        # Iteratively add best interval and remove overlapping from candidates.
+        # Iteratively add the best interval and remove overlapping intervals from candidates.
         idx = self.plant.time_index
         best_intervals_mask = pd.Series(index=idx, data=False)
         while any(is_candidate):
             # Mark best-scoring interval. Exit if score is NaN in all remaining candidates:
             if score.where(is_candidate).isna().all():
                 break
             # If idxmax is not unique --> returns first occurrence of maximum
             best_idx = score.where(is_candidate).idxmax()
             best_intervals_mask.loc[best_idx] = True
             # Remove overlapping intervals (past and future) from candidates
-            is_candidate.loc[(idx > best_idx - self.interval_length) & (idx < best_idx + self.interval_length)] = False
+            is_candidate.loc[
+                (idx > best_idx - self.settings.interval_length) & (
+                        idx < best_idx + self.settings.interval_length)] = False
 
         return best_intervals_mask
```

## sunpeek/core_methods/pc_method/plotting.py

```diff
@@ -1,104 +1,229 @@
 """Plotting module. Development plots only.
 """
 
-import os
 import warnings
-
+from pathlib import Path
 import numpy as np
 import pandas as pd
-import uuid
 import datetime as dt
+import pint
+import matplotlib.pyplot as plt
+import matplotlib.dates as mdates
+import matplotlib.transforms as transforms
+
+from sunpeek.common.utils import ROOT_DIR, sp_logger
+from sunpeek.components.results import PCMethodOutput
 
-from sunpeek.common.utils import ROOT_DIR
+PLOTS_MISSING_TXT = 'Modules "plotly" or "pendulum" not found. Install them to use development plots.'
 
 try:
     from plotly import graph_objects as go
     from plotly.subplots import make_subplots
-    PLOTS_AVAILABLE = True
+    import pendulum
+
+    plots_available = True
 except ModuleNotFoundError:
-    warnings.warn('module plotly not found, install it to use development plots')
-    PLOTS_AVAILABLE = False
+    warnings.warn(PLOTS_MISSING_TXT)
+    plots_available = False
 
 
-def plot_all(pc_output, mode='screen', use_safety=True, write_image=False, anonymize=False):
+def assert_modules():
+    if not plots_available:
+        raise ModuleNotFoundError(PLOTS_MISSING_TXT)
+
+
+# Color: matplotlib style 'tableau-colorblind10'
+# Style: https://viscid-hub.github.io/Viscid-docs/docs/dev/styles/tableau-colorblind10.html
+# Color names https://stackoverflow.com/questions/74830439/list-of-color-names-for-matplotlib-style-tableau-colorblind10
+COLORS = {
+    'blue': '#5F9ED1',
+    'sky_blue': '#006BA4',
+    'sail_blue': '#A2C8EC',
+    'pumpkin': '#FF800E',
+    'orange': '#C85200',
+    'cheese': '#FFBC79',
+    'gray': '#595959',
+    'warm_gray': '#898989',
+    'light_gray': '#CFCFCF',
+    'dark_gray': '#ABABAB',
+    'almost_black': '#373737',
+}
+
+FULL_WIDTH = 16.59 / 2.54  # full page width, cm to inches
+FONT_SIZE = 6
+plt.rcParams.update({
+    'figure.dpi': 600,
+    # 'font.family': 'Times New Roman',
+    'font.family': 'Open Sans',
+    'font.size': FONT_SIZE,
+    'text.usetex': False,
+    'axes.labelsize': FONT_SIZE,
+    'axes.titlesize': FONT_SIZE,
+    'axes.labelpad': 2,
+    'axes.titlepad': 4,
+    'axes.linewidth': 0.5,
+    'xaxis.labellocation': 'left',
+    'grid.alpha': 0.5,
+    'grid.linewidth': 0.5,
+    'lines.linewidth': 0.75,
+    'patch.linewidth': 0.25,
+    'legend.fontsize': FONT_SIZE - 1,
+    'legend.title_fontsize': FONT_SIZE - 1,
+    'legend.framealpha': 0.8,
+    'legend.borderpad': 0.2,
+    'legend.columnspacing': 1.5,
+    'legend.labelspacing': 0.25,
+    'xtick.labelsize': FONT_SIZE - 1,
+    'ytick.labelsize': FONT_SIZE,
+    'xtick.major.size': 2,
+    'xtick.major.pad': 1,
+    'xtick.major.width': 0.5,
+    'ytick.major.size': 2,
+    'ytick.major.pad': 1,
+    'ytick.major.width': 0.5,
+    'xtick.minor.size': 2,
+    'xtick.minor.pad': 1,
+    'xtick.minor.width': 0.5,
+    'ytick.minor.size': 2,
+    'ytick.minor.pad': 1,
+    'ytick.minor.width': 0.5,
+})
+# Avoid black unless necessary
+# Taken from https://atchen.me/research/code/data-viz/2022/01/04/plotting-matplotlib-reference.html
+plt.rcParams.update({
+    'text.color': COLORS['almost_black'],
+    'patch.edgecolor': COLORS['gray'],
+    'patch.force_edgecolor': True,
+    'hatch.color': COLORS['almost_black'],
+    'axes.edgecolor': COLORS['almost_black'],
+    'axes.labelcolor': COLORS['almost_black'],
+    'xtick.color': COLORS['almost_black'],
+    'ytick.color': COLORS['almost_black']
+})
+
+
+def plot_all(pc_output: PCMethodOutput,
+             mode='screen',
+             show_image=True,
+             write_image=False,
+             use_safety=True,
+             anonymize=False):
+    """Create all defined plots.
+    """
+    assert_modules()
     assert mode in ['screen', 'presentation']
-    if not PLOTS_AVAILABLE:
-        raise ModuleNotFoundError('module plotly not found, install it to use development plots')
-    if pc_output.n_intervals == 0:
-        print('Nothing to plot, no PC intervals found.')
+    if pc_output is None or (pc_output.plant_output.n_intervals == 0):
+        sp_logger.info('Nothing to plot, no Performance Check intervals found.')
+        # print('Nothing to plot, no Performance Check intervals found.')
         return
 
+    settings = dict(
+        mode=mode,
+        show_image=show_image,
+        write_image=write_image,
+        use_safety=use_safety,
+        anonymize=anonymize,
+    )
+
     figures = dict(
-        square=plot_square(pc_output, mode=mode, use_safety=use_safety, write_image=write_image, anonymize=anonymize),
-        time=plot_time(pc_output, mode=mode, use_safety=use_safety, write_image=write_image, anonymize=anonymize),
-        sums=plot_sums(pc_output, mode=mode, write_image=write_image, anonymize=anonymize),
+        square=plot_square(pc_output, **settings),
+        time=plot_time(pc_output, **settings),
+        sums=plot_sums(pc_output, **settings),
     )
 
     return figures
 
 
-def plot_square(pc_output, mode, use_safety=False, write_image=False, anonymize=False):
-    """Plot measured vs. estimated power in intervals + trendline.
+def plot_square(pc_output,
+                mode: str,
+                use_safety=True,
+                show_image=True,
+                write_image=False,
+                anonymize=False,
+                axis_range=None,
+                tick0=None):
+    """Plot measured vs. estimated power in intervals + trend line.
     """
-    if not PLOTS_AVAILABLE:
-        raise ModuleNotFoundError('module plotly not found, install it to use development plots')
-    if pc_output.n_intervals == 0:
+
+    assert_modules()
+    if pc_output is None or (pc_output.plant_output.n_intervals == 0):
         print('Nothing to plot, no PC intervals found.')
         return
 
-    measured = pc_output.tp_sp_measured.magnitude
-    estimated = pc_output.tp_sp_expected_safety.magnitude if use_safety else pc_output.tp_sp_expected.magnitude
-    slope =pc_output.target_actual_slope_safety.magnitude if use_safety else pc_output.target_actual_slope.magnitude
+    if axis_range is None:
+        axis_range = [250, 650]
+    if tick0 is None:
+        tick0 = 300
+
+    pout = pc_output.plant_output
+    measured = pout.tp_sp_measured.magnitude
+    estimated = pout.tp_sp_estimated_safety.magnitude if use_safety else pout.tp_sp_estimated.magnitude
+    # slope = pout.target_actual_slope_safety.magnitude if use_safety else pout.target_actual_slope.magnitude
     font_size = 24 if mode == 'presentation' else 14
 
     fig = go.Figure()
     fig.add_scatter(x=estimated, y=measured,
-                    name='interval averages',
+                    name=f"Interval averages ("
+                         f"{pendulum.duration(seconds=pc_output.settings['interval_length'].total_seconds()).in_words(locale='en')}"
+                         f")",
                     mode='markers', marker_size=10, marker_opacity=0.8)
 
+    fig.update_layout(legend=dict(
+        orientation="h",
+        yanchor="bottom",
+        y=1.01,
+        xanchor="right",
+        x=1
+    ))
+
     # Linear trendline with 0 intercept
     # rng = [estimated.min(), estimated.max()]
     # fig.add_scatter(x=rng, y=slope * np.array(rng),
     #                 name=f'y = {slope:.3f} x',
     #                 mode='lines', line_color='grey', line_width=3)
 
     # Bisection line
-    # axis_range = [np.min([estimated.min(), measured.min()]).round(-2) - 100,
-    #               np.max([estimated.max(), measured.max()]).round(-2)]
-    # axis_range = [350, 700]
-    axis_range = [300, 600]
     fig.add_scatter(x=axis_range, y=axis_range, name='', showlegend=False,
                     mode='lines',
                     # line_dash='dash',
                     line_color='grey', line_width=0.5)
     fig.update_layout(
-        # title=dict(text=_get_title(pc_output, anonymize),
-        #            xanchor='left', yanchor='top',
-        #            font_size=font_size + 1,
-        #            ),
-        # margin=dict(l=250, r=20, t=70, b=150),
         width=1000,
         height=1000,
-        xaxis=dict(title="<b>Estimated</b> power [W/m²]",
-                   linecolor="#BCCCDC",
-                   range=axis_range,
-                   title_font_size=font_size,
-                   tickfont_size=font_size,
-                   ),
-        yaxis=dict(title="<b>Measured</b> power [W/m²]",
-                   linecolor="#BCCCDC",
-                   range=axis_range,
-                   scaleanchor="x",
-                   scaleratio=1,
-                   title_font_size=font_size,
-                   tickfont_size=font_size,
-                   ),
+        autosize=False,
+        xaxis=dict(
+            type='linear',
+            constrain="domain",
+            title="<b>Estimated</b> power [W/m²]",
+            linecolor="#BCCCDC",
+            range=axis_range,
+            title_font_size=font_size,
+            tickfont_size=font_size,
+            tick0=tick0,
+            dtick=100,
+        ),
+        yaxis=dict(
+            type='linear',
+            constrain="domain",
+            title="<b>Measured</b> power [W/m²]",
+            title_font_size=font_size,
+            title_standoff=30,
+            linecolor="#BCCCDC",
+            range=axis_range,
+            scaleanchor="x",
+            scaleratio=1,
+            autorange=False,
+            tickfont_size=font_size,
+            tick0=tick0,
+            dtick=100,
+        ),
         legend_font_size=font_size,
     )
+
     # fig.update_xaxes(
     #     showspikes=True,
     #     spikecolor="grey",
     #     spikesnap="cursor",
     #     spikemode="across",
     #     spikedash="solid",
     # )
@@ -106,164 +231,178 @@
     #     showspikes=True,
     #     spikecolor="grey",
     #     spikesnap="cursor",
     #     spikemode="across",
     #     spikedash="solid",
     # )
 
-    _show(fig)
+    if show_image:
+        _show(fig)
     if write_image:
-        fig.write_image(_get_filename())
+        fig.write_image(_get_filename('square', pc_output))
 
     return fig
 
 
-def plot_time(pc_output, mode, use_safety=False, write_image=False, anonymize=False, plot_trend=True):
-    """Plots ratio of measured vs. estimated power over time."""
-    if not PLOTS_AVAILABLE:
-        raise ModuleNotFoundError('module plotly not found, install it to use development plots')
-    if pc_output.n_intervals == 0:
+def plot_time(pc_output,
+              mode: str,
+              use_safety=True,
+              show_image=True,
+              write_image=False,
+              anonymize=False,
+              plot_trend=True,
+              yrange=None,
+              ):
+    """Plots ratio of measured vs. estimated power over time.
+    """
+    assert_modules()
+    if pc_output is None or (pc_output.plant_output.n_intervals == 0):
         print('Nothing to plot, no PC intervals found.')
         return
 
-    estimated = pc_output.tp_sp_expected_safety.magnitude if use_safety else pc_output.tp_sp_expected.magnitude
-    measured = pc_output.tp_sp_measured.magnitude
+    if yrange is None:
+        yrange = [0.8, 1.2]
+
+    pout = pc_output.plant_output
+    estimated = pout.tp_sp_estimated_safety.magnitude if use_safety else pout.tp_sp_estimated.magnitude
+    measured = pout.tp_sp_measured.magnitude
     ratio = measured / estimated
     # Plotting ratio against midpoint of intervals
-    time_display = pc_output.datetime_intervals_start + 0.5 * pc_output.interval_length
+    time_display = pout.datetime_intervals_start + 0.5 * pc_output.settings['interval_length']
     font_size = 24 if mode == 'presentation' else 14
 
     fig = go.Figure()
     fig.add_scatter(x=time_display, y=ratio,
                     mode='markers', marker_size=10, marker_opacity=0.5,
                     showlegend=False)
 
     if plot_trend:
         rm = pd.Series(data=ratio, index=time_display) \
             .rolling(dt.timedelta(days=45), min_periods=25, center=True, closed='both').median()
         fig.add_scatter(y=rm, x=rm.index, mode='lines', line_color='grey', line_width=5, showlegend=False)
 
-    # print_data = lambda i: data.index[i].strftime('%Y-%m-%d')
     fig.update_layout(
-        # title=dict(text=_get_title(pc_output, anonymize),
-        #            xanchor='left', yanchor='top',
-        #            font_size=font_size + 1,
-        #            ),
-        # margin=dict(l=250, r=20, t=70, b=150),
         width=2000,
         height=600,
         xaxis=dict(title="",
                    title_font_size=font_size,
                    tickfont_size=font_size,
                    linecolor="#BCCCDC"),
         yaxis=dict(title="<b>Ratio measured vs. estimated</b> power [-]",
-                   # range=[0.5, 1.2],
-                   range=[0.8, 1.2],
-                   # range=[ratio.min(), np.max([1, ratio.max()])],
+                   title_standoff=30,
                    title_font_size=font_size,
                    tickfont_size=font_size,
+                   tickformat='0%',
+                   range=yrange,
+                   dtick=0.1,
                    linecolor="#BCCCDC")
 
     )
-    _show(fig)
+    if show_image:
+        _show(fig)
     if write_image:
-        fig.write_image(_get_filename())
+        fig.write_image(_get_filename('time', pc_output))
 
     return fig
 
 
-def plot_sums(pc_output, mode, write_image=False, anonymize=False):
+def plot_sums(pc_output,
+              mode: str,
+              use_safety=False,
+              show_image=True,
+              write_image=False,
+              anonymize=False,
+              ):
     """Plot sums / average powers in intervals, measured vs. estimated.
     """
-    if not PLOTS_AVAILABLE:
-        raise ModuleNotFoundError('module plotly not found, install it to use development plots')
-    if pc_output.n_intervals == 0:
+    assert_modules()
+    if pc_output is None or (pc_output.plant_output.n_intervals == 0):
         print('Nothing to plot, no PC intervals found.')
         return
 
-    # estimated = np.mean(pc_output.tp_sp_expected.magnitude)
-    esimated_safe = np.mean(pc_output.tp_sp_expected_safety.magnitude)
-    measured = np.mean(pc_output.tp_sp_measured.magnitude)
+    pout = pc_output.plant_output
+    # estimated = np.mean(pout.tp_sp_estimated.magnitude)
+    estimated_safe = np.mean(pout.tp_sp_estimated_safety.magnitude)
+    measured = np.mean(pout.tp_sp_measured.magnitude)
 
     fig = make_subplots(rows=1, cols=2, specs=[[{}, {}]],
                         shared_xaxes=False,
                         shared_yaxes=False, vertical_spacing=0.001)
 
     font_size = 18 if mode == 'presentation' else 14
     labels = ['Average power<br><b>measured</b>', 'Average power<br><b>estimated</b>']
-    x = [measured, esimated_safe]
+    x = [measured, estimated_safe]
     colors = ['rgba(192, 0, 0, 0.6)', 'rgba(68, 114, 196, 0.6)']
 
     text = [str(np.round(val, decimals=1)) + ' W/m²' for val in x]
     fig.append_trace(go.Bar(
-        x=x, y=labels,
+        x=x,
+        y=labels,
         marker=dict(
             color=colors,
             line=dict(color='rgba(90, 90, 90, 1.0)', width=1),
         ),
         orientation='h',
         width=0.4,
         text=text,
         textposition="outside",
         insidetextanchor="end",
         outsidetextfont_size=font_size
     ), 1, 1)
 
+    plant_name = '<anonymized>' if anonymize else pout.plant.name
+    if plant_name.startswith('FHW Arcon South'):
+        plant_name = 'FHW Fernheizwerk Graz, Arcon South'
+    title = (f"<b>Check of Performance</b> ({pc_output.pc_method_name}).<br>"
+             f"Mode: {pc_output.evaluation_mode}. "
+             f"Equation: {pc_output.equation}. "
+             f"Wind: {'' if pc_output.wind_used else 'Not '}used.<br>"
+             # f"Plant name: <b>{plant_name}</b>.<br>"
+             f"n={pout.n_intervals} intervals. Interval duration: "
+             f"{pendulum.duration(seconds=pc_output.settings['interval_length'].total_seconds()).in_words(locale='en')}."
+             f"<br>Data from {pc_output.datetime_eval_start.tz_convert(pout.plant.tz_data)} to "
+             f"{pc_output.datetime_eval_end.tz_convert(pout.plant.tz_data)}.<br>"
+             )
     axis_range = [0, np.max(x).round(-1) + 100]
     fig.update_layout(
-        title=dict(text=_get_title(pc_output, anonymize),
-                   xanchor='left', yanchor='top',
+        title=dict(text=title,
+                   xanchor='left',
+                   xref='paper',
+                   x=fig.layout.xaxis.domain[0],
+                   # yanchor='top',
+                   yanchor='bottom',
+                   y=fig.layout.height,
                    font_size=font_size + 1,
                    ),
         autosize=False,
-        height=500,
-        width=2200,
-        # legend=dict(x=0.029, y=1.038, font_size=10),
-        margin=dict(l=250, r=20, t=70, b=150),
-        # paper_bgcolor='rgb(248, 248, 255)',
-        # plot_bgcolor='rgb(248, 248, 255)',
+        height=700,
+        width=2400,
+        margin=dict(l=250, r=20, t=70, b=250),
         yaxis=dict(
             tickfont=dict(size=font_size),
+            title_standoff=30,
             showgrid=False,
             showline=False,
             showticklabels=True,
             domain=[0, 0.85],
         ),
-        # yaxis2=dict(
-        #     range=axis_range,
-        #     showgrid=False,
-        #     showline=True,
-        #     showticklabels=False,
-        #     linecolor='rgba(102, 102, 102, 0.8)',
-        #     linewidth=2,
-        #     domain=[0, 0.85],
-        # ),
         xaxis=dict(
             title=dict(text='Specific thermal power [W/m²]',
-                   font_size=font_size - 1,
-                   ),
+                       font_size=font_size,
+                       ),
             # title='Specific thermal power [W/m²]',
-            title_font_size=font_size-1,
-            tickfont=dict(size=font_size-1),
+            title_font_size=font_size - 1,
+            tickfont=dict(size=font_size),
             range=axis_range,
             zeroline=False,
             showline=False,
             showticklabels=True,
             showgrid=True,
             domain=[0, 0.42],
         ),
-        # xaxis2=dict(
-        #     zeroline=False,
-        #     showline=False,
-        #     showticklabels=True,
-        #     showgrid=True,
-        #     domain=[0.47, 1],
-        #     side='top',
-        #     dtick=25000,
-        # ),
     )
 
     # Adding labels
     # x_power = np.round([measured, estimated], decimals=1)
     # for xp, yp in zip(x_power, labels):
     #     # labeling the bar net worth
     #     annotations.append(dict(xref='x1', yref='y1',
@@ -271,42 +410,66 @@
     #                             text=str(xp) + ' W/m²',
     #                             align="left",
     #                             font=dict(family='Arial', size=font_size,
     #                                       color='rgb(0, 0, 0)'),
     #                             showarrow=False))
 
     # Guarantee fulfilled statement
-    ratio = measured / esimated_safe
+    ratio = measured / estimated_safe
     fulfill_txt = 'not ' if ratio < 1 else ''
+    min_intervals_ok = (pout.n_intervals >= pc_output.settings['min_intervals_in_output'])
     ratio_text = (f'<b>Performance Check {fulfill_txt}fulfilled:'
                   f'</b> Ratio measured / estimated power = {ratio:.1%}'
-                  f'<br>Combined safety factor f<sub>safe</sub> = {pc_output.safety_combined:.2} taken into account.')
-    fig.add_annotation(dict(xref='paper', yref='paper', xanchor='left',
-                            x=0, y=-0.45,
-                            text=ratio_text,
-                            align='left',
-                            font_size=font_size,
-                            showarrow=False))
+                  f'<br>Combined safety factor f<sub>safe</sub> = {pc_output.settings["safety_combined"]:.2} '
+                  f'taken into account.'
+                  f'<br>{pout.n_intervals} intervals found: '
+                  f'The minimum number of intervals ({pc_output.settings["min_intervals_in_output"]}) '
+                  f'has {"" if min_intervals_ok else "not "}been reached.'
+                  )
+    # fig.add_annotation(dict(
+    #     text=ratio_text,
+    #     font_size=font_size,
+    #     yref='paper',
+    #     yanchor="bottom",
+    #     y=-1.02,
+    #     xref='paper',
+    #     xanchor="left",
+    #     x=0,
+    #     # align='left',
+    #     showarrow=False))
+
+    # Calculate position of annotation
+    fig.add_annotation(
+        text=ratio_text,
+        font_size=font_size,
+        xref='paper',
+        x=fig.layout.xaxis.domain[0],
+        align='left',
+        # xanchor='left',
+        y=-230 / fig.layout.height,
+        yref='paper',
+        showarrow=False,
+    )
 
     fig.update_layout(showlegend=False)
 
-    _show(fig)
+    if show_image:
+        _show(fig)
     if write_image:
-        fig.write_image(_get_filename())
+        fig.write_image(_get_filename('sums', pc_output))
 
     return fig
 
 
 def plot_mask(pc_output, mask):
     """Produces a subplot figure with the PC criteria mask.
     mask is usually pc_obj._mask
     """
-    if not PLOTS_AVAILABLE:
-        raise ModuleNotFoundError('module plotly not found, install it to use development plots')
-    if pc_output.n_intervals == 0:
+    assert_modules()
+    if pc_output is None or (pc_output.plant_output.n_intervals == 0):
         print('Nothing to plot, no PC intervals found.')
         return
 
     subplot_cols = mask.columns
     fig = make_subplots(rows=1 + len(subplot_cols), shared_xaxes=True, subplot_titles=subplot_cols)
 
     t = mask.index
@@ -318,32 +481,177 @@
 
     fig.layout.update(showlegend=False)
     _show(fig)
 
     return fig
 
 
+def format_xaxis(ax,
+                 tz,
+                 interval,
+                 # date_start=DAY_START, date_end=DAY_END,
+                 minor_locator=mdates.MinuteLocator(interval=5),
+                 major_locator=mdates.MinuteLocator(interval=15),
+                 major_formatter=None):
+    ax.set_xlim(interval[0], interval[1], auto=None)
+    if major_formatter is None:
+        major_formatter = mdates.DateFormatter("%#H:%M", tz=tz)
+    ax.xaxis_date(tz)
+    ax.xaxis.set_minor_locator(minor_locator)
+    ax.xaxis.set_major_locator(major_locator)
+    ax.xaxis.set_major_formatter(major_formatter)
+    # adjust_xlabel_positions(ax, 4, remove_last=True)
+
+    # Position extra text below x axis
+    vertical_offset_points = 10
+    offset = transforms.ScaledTranslation(0, vertical_offset_points / 72, ax.figure.dpi_scale_trans)
+    ax.text(0, 0, f'{mdates.num2date(ax.get_xlim()[0]):%Y-%m-%d} ({str(tz)})', ha='left',
+            transform=ax.transAxes - offset, va='top', fontsize=plt.rcParams['axes.labelsize'] - 1)
+
+    return ax
+
+
+def plot_sensor_data(array,
+                     interval,
+                     anonymize=False,
+                     ):
+    """Plot main sensor values in given interval.
+    Using matplotlib here because plotly doesn't behave with subplot grid legends...
+    """
+    a = array
+    p = array.plant
+
+    fig, ax = plt.subplots(ncols=2, nrows=3, sharex=True,
+                           constrained_layout=True,
+                           gridspec_kw=dict(width_ratios=[1, 1], height_ratios=[3, 3, 2]),
+                           )
+    fig.subplots_adjust(left=.15, bottom=.16, right=.99, top=.97)
+
+    def _get_plot_data(sensor, unit):
+        idx = sensor.data.index
+        mask = (idx > interval[0]) & (idx <= interval[1])
+        sub_series = sensor.data.loc[mask]
+        sub_series = sub_series.pint.to(unit).pint.magnitude
+
+        remove_virtual = lambda s: s.split('__', 1)[0] if '__' in s else s
+        sub_series.rename(remove_virtual(sensor.raw_name), inplace=True)
+
+        return sub_series
+
+    def _format_subplot(ax_, title_txt, unit, ylims=None, has_legend=True):
+        ax_.set_title(title_txt, loc='center')
+        print_unit = lambda s: f"[{pint.Unit(s):~P}]" if s else "[dimensionless]"
+        if isinstance(unit, list):
+            ylabel_txt = ", ".join([print_unit(s) for s in unit])
+        else:
+            ylabel_txt = print_unit(unit)
+        ax_.set_ylabel(ylabel_txt)
+        if ylims is not None:
+            ax_.set_ylim(ylims[0], ylims[1])
+        if has_legend:
+            # ax.get_legend().remove()
+            legend = ax_.legend(loc="upper right")
+            legend.get_frame().set_facecolor((1, 1, 1, 0.8))
+            legend.set_zorder(1000)
+        ax_.grid()
+        ax_.set_axisbelow('line')
+
+    # plot data (Fluid Temperatures)
+    ax_ = ax[0][0]
+    unit = 'degC'
+    data = _get_plot_data(a.te_out, unit)
+    ax_.plot(data, color=COLORS['orange'], label=data.name, zorder=10)
+    data = _get_plot_data(a.te_op, unit)
+    ax_.plot(data, color=COLORS['warm_gray'], label=data.name, zorder=15)
+    data = _get_plot_data(a.te_in, unit)
+    ax_.plot(data, color=COLORS['blue'], label=data.name, zorder=5)
+    _format_subplot(ax_, "(a) Fluid Temperatures", unit)
+
+    # plot data (Thermal Power)
+    ax_ = ax[0][1]
+    data = _get_plot_data(p.tp, 'kW')
+    ax_.plot(data, color=COLORS['warm_gray'], label=data.name, zorder=5)
+    _format_subplot(ax_, "(b) Thermal Power", 'kW', has_legend=False)
+
+    # plot data (Solar Radiation)
+    ax_ = ax[1][0]
+    unit = 'W m**-2'
+    if a.rd_gti is not None:
+        data = _get_plot_data(a.rd_gti, unit)
+        ax_.plot(data, color=COLORS['orange'], label=data.name, zorder=15)
+    if a.rd_bti is not None:
+        data = _get_plot_data(a.rd_bti, unit)
+        ax_.plot(data, color=COLORS['cheese'], label=data.name, zorder=10)
+    if a.rd_dti is not None:
+        data = _get_plot_data(a.rd_dti, unit)
+        ax_.plot(data, color=COLORS['dark_gray'], label=data.name, zorder=5)
+    _format_subplot(ax_, "(c) Solar Radiation", unit, ylims=[0, 1200])
+
+    # plot data (Ambient)
+    ax_ = ax[1][1]
+    data = _get_plot_data(p.te_amb, 'degC')
+    ax_.plot(data, color=COLORS['cheese'], label=data.name, zorder=15)
+    if p.ve_wind is not None:
+        data = _get_plot_data(p.ve_wind, 'm s**-1')
+        ax_.plot(data, color=COLORS['light_gray'], label=data.name, zorder=10)
+        _format_subplot(ax_, "(d) Ambient", ['degC', 'm s**-1'])
+    else:
+        _format_subplot(ax_, "(d) Ambient", 'degC')
+
+    # plot data (Angle of Incidence)
+    ax_ = ax[2][0]
+    data = _get_plot_data(a.aoi, 'deg')
+    ax_.plot(data, color=COLORS['almost_black'], label=data.name, zorder=15)
+    _format_subplot(ax_, "(e) Angle of Incidence", 'deg', has_legend=False)
+
+    # plot data (Incidence Angle Modifier)
+    ax_ = ax[2][1]
+    data = _get_plot_data(a.iam, '')
+    ax_.plot(data, color=COLORS['almost_black'], label=data.name, zorder=15)
+    _format_subplot(ax_, "(f) Incidence Angle Modifier", '', has_legend=False)
+
+    fig.set_size_inches(w=FULL_WIDTH, h=FULL_WIDTH / 1.9)
+    fig.tight_layout()
+    format_xaxis(ax[2][0], tz=p.tz_data, interval=interval)
+    format_xaxis(ax[2][1], tz=p.tz_data, interval=interval)
+
+    plant_name = '<anonymized>' if anonymize else array.plant.name
+    if plant_name.startswith('FHW Arcon South'):
+        plant_name = 'FHW Fernheizwerk Graz, Arcon South'
+    title_txt = (f"Sensor data for plant: {plant_name}. "
+                 # f"Data from {interval[0]} to {interval[1]}."
+                 )
+    plt.suptitle(title_txt, fontweight='bold',
+                 x=0.05, y=0.98,
+                 horizontalalignment='left')
+
+    plt.tight_layout()
+
+    plt.savefig(_get_filename('sensor_data'))
+    plt.close()
+    print(f'Saved plot "sensor_data".')
+
+
 def _show(fig):
     fig.update_layout(dragmode='pan')
     config = {'scrollZoom': True,
               'displayModeBar': True,
               'modeBarButtonsToRemove': ['zoomIn', 'zoomOut'],
               'modeBarButtonsToAdd': ['drawline',
                                       'drawrect',
                                       'eraseshape'
                                       ]}
     fig.show(config=config)
 
 
-def _get_title(pc_output, anonymize):
-    plant_name = '<anonymized>' if anonymize else pc_output.plant.name
-    return (f"<b>Check of Performance</b> ({pc_output.pc_method_name}, "
-            f"equation {pc_output.equation}).<br>"
-            # f"Plant <b>{plant_name}</b>.<br>"
-            f"<b>Data from</b> {pc_output.datetime_eval_start} to {pc_output.datetime_eval_end}.<br>"
-            f"n={pc_output.n_intervals} intervals with duration {pc_output.interval_length}."
-            )
-
+def _get_filename(plot_name, pc_output=None):
+    """Generate png file name from method, equation and plot name.
+    """
+    save_folder = Path(ROOT_DIR).parent / 'tests' / 'resources'
+    if pc_output is None:
+        filename = f'{plot_name}__{dt.datetime.now().strftime("%Y%m%d_%H%M%S")}.png'
+    else:
+        m = pc_output.evaluation_mode
+        e = pc_output.equation
+        filename = f'{m}_eq{e}__{plot_name}__{dt.datetime.now().strftime("%Y%m%d_%H%M%S")}.png'
 
-def _get_filename():
-    resource_fldr = os.path.join(ROOT_DIR, 'tests', 'resources')
-    return os.path.join(resource_fldr, f"{uuid.uuid4().hex}.png")
+    return save_folder / filename
```

## sunpeek/core_methods/virtuals/__init__.py

```diff
@@ -0,0 +1,6 @@
+00000000: 6672 6f6d 2073 756e 7065 656b 2e63 6f72  from sunpeek.cor
+00000010: 655f 6d65 7468 6f64 732e 7669 7274 7561  e_methods.virtua
+00000020: 6c73 2e6d 6169 6e20 696d 706f 7274 2063  ls.main import c
+00000030: 6f6e 6669 675f 7669 7274 7561 6c73 2c20  onfig_virtuals, 
+00000040: 6361 6c63 756c 6174 655f 7669 7274 7561  calculate_virtua
+00000050: 6c73 0a                                  ls.
```

## sunpeek/core_methods/virtuals/main.py

```diff
@@ -1,760 +1,106 @@
-"""
-Module implementing functionality needed for virtual sensor calculation.
-
-Contains functions to calculate virtual sensors. Main calculation methods start with "get_()"
-Includes functions to verify / assert calculation inputs.
 
-All get_() methods
-- accept inputs (for scalars): pint.Quantity, and (for series): cmp.Sensor objects
-- return unit-aware pd.Series objects (pd.Series with dtype pint[unit])
+"""
+This module implements functionality for calculation and verification of virtual sensors.
 
-Internal functions (underscore functions) accept and return things as numeric values in appropriate units
-(like radiation in W/m² etc); see docstrings for details.
+It contains two entry-point functions for doing virtual sensor stuff.
+- config_virtuals():
+   - Is fast to run, only depends on plant config, no calculations.
+   - Attaches a ProblemReport to all virtual sensors, stating if it _can_ be calculated / why not
+- calculate_virtuals():
+   - Actually calculates virtual sensors for all components.
+   - Calculation logic is hard coded.
+
+## Details
+
+- Implements functions that calculate groups of virtual sensors
+  (one calculation call returns data for multiple virtual sensors).
+- Calculations generally return unit-aware pd.Series objects, `pd.Series with dtype pint[unit]`.
+- Internal functions (underscore functions) may also accept and return arguments as numeric values in appropriate units
+(as opposed to the main calculations which work with pint Quantities). See local docstrings for details.
+- The module also implements functions to verify / assert calculation inputs.
+
+## Note for developers:
+- Virtual sensors may use data and parameters of various objects in their calculations (e.g. plant latitude,
+array irradiance, array area etc.). Therefore, virtual sensors are associated to one and only one component. They
+may not be linked / associated with more than one component, like real sensors which
+can be "shared" by multiple components.
 
 .. codeauthor:: Philip Ohnewein <p.ohnewein@aee.at>
 .. codeauthor:: Daniel Tschopp <d.tschopp@aee.at>
+.. codeauthor:: Marnoch Hamilton-Jones <m.hamilton-jones@aee.at>
 """
 
 from abc import ABCMeta, abstractmethod
 from typing import Union
-import pandas as pd
-import numpy as np
-import scipy.signal
-import pvlib as pv
-
-import sunpeek.common.unit_uncertainty as uu
-from sunpeek.common.utils import to_rd, VerifyValidateMode
-from sunpeek.common.errors import VirtualSensorCalculationError
-from sunpeek.components.types import assert_valid_collector
-from sunpeek.components.fluids import assert_valid_fluid
-from sunpeek.core_methods.virtuals.radiation import RadiationConversionHorizontal, RadiationConversionTilted
-from metpy.calc import dewpoint_from_relative_humidity
-
-
-def validate_radiation_inputs(comp):
-    """Checks if component has been assigned sufficient radiation data/sensors to perform radiation conversion.
-
-    Parameters
-    ----------
-    comp : components.Plant or components.Array
-        Plant or Array object for which radiation components will be calculated.
-
-    Notes
-    -----
-    This function can be used on a Plant and also Array level.
-    Sensor tilt angle and required output angles are not taken into account.
-    For a brief discussion, see https://gitlab.com/sunpeek/sunpeek/-/issues/128
-    Expects component to return 4 input radiations of type global, beam, diffuse and DNI from a call to
-    component.get_radiation_input_slots()
-    """
-    input_pattern = _get_radiation_input_pattern(*comp.radiation_input_slots)
-
-    # No inputs
-    reason = ''
-    if input_pattern == '0000':
-        reason = 'No radiation inputs given.'
-    # 1 input, but not global
-    elif input_pattern in ['0100', '0010', '0001']:
-        reason = 'Cannot calculate radiation components with only 1 input which is not a global radiation.'
-    # Inputs beam + DNI
-    elif input_pattern == '0101':
-        reason = 'Cannot calculate radiation components with only beam and DNI radiations as inputs.'
-
-    return *(reason == '', reason),
-
-
-def _get_radiation_input_pattern(*args):
-    """Returns input pattern as string, where 1 if input is not None, else 0.
-    Example: beam and diffuse radiation given, while global and DNI are None: pattern=='0110'.
-    """
-    is_given = [x is not None for x in args]
-    return f'{sum([x * np.power(10, 3 - i) for i, x in enumerate(is_given)]):04d}'
-
-
-class VirtualsMeta(ABCMeta):
-    required_attributes = []
-
-    def __call__(self, *args, **kwargs):
-        obj = super(VirtualsMeta, self).__call__(*args, **kwargs)
-        for attr_name in obj.required_attributes:
-            if not getattr(obj, attr_name):
-                raise ValueError(f'Required attribute "{attr_name}" not set.')
-        return obj
-
-
-class VirtualSensorCalculation(object, metaclass=VirtualsMeta):
-    required_attributes = ['n_results']
-
-    @abstractmethod
-    def __init__(self):
-        pass
-
-    @abstractmethod
-    def _core(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def _do_assert(self, check_mode: VerifyValidateMode) -> Union[bool, None]:
-        return True
-
-    @property
-    def none_output(self):
-        out = (None,) * self.n_results
-        out = out[0] if (self.n_results == 1) else out
-        return out
-
-    def calc(self, *args, **kwargs):
-        if not self.validate_data():
-            return self.none_output
-
-        try:
-            return self._core(*args, **kwargs)
-        except Exception as ex:
-            raise VirtualSensorCalculationError(ex)
-
-    def verify_config(self):
-        try:
-            self._do_assert(check_mode=VerifyValidateMode.verify)
-        except AssertionError:
-            return False
-        return True
-
-    def validate_data(self):
-        try:
-            self._do_assert(check_mode=VerifyValidateMode.validate)
-        except AssertionError:
-            return False
-        return True
-
-
-class CalcPowerFromVolumeFlow(VirtualSensorCalculation):
-    """For plants and arrays, calculate thermal power from fluid, volume flow and inlet & outlet temperatures.
-    """
-
-    # def __init__(self, comp: Union[Plant, Array]):
-    def __init__(self, comp):
-        # if isinstance(comp, Array):
-        #     raise NotImplementedError('array.fluid -> array.plant.fluid_solar not yet implemented')
-
-        self.comp = comp
-        self.n_results = 1
-
-    def _core(self):
-        """
-        Returns
-        -------
-        tp : pd.Series
-            Calculated thermal power.
-        """
-        tp = self.calc_tp_from_vf_pos(fluid=self.comp.fluid_solar,
-                                      vf=self.comp.vf.data,
-                                      te_in=self.comp.te_in.data,
-                                      te_out=self.comp.te_out.data,
-                                      pos=self.comp.vf.info['position'].m_as(''))
-        return tp
-
-    def _do_assert(self, check_mode):
-        assert_valid_fluid(self.comp.fluid_solar)
-        self.comp.assert_verify_validate(check_mode, 'vf', 'te_in', 'te_out')
-
-    @staticmethod
-    def calc_tp_from_vf_pos(fluid, vf, te_in, te_out, pos):
-        """Calculates thermal power from given fluid, volume flow and inlet & outlet temperatures.
-
-        Parameters
-        ----------
-        fluid : components.Fluid
-        vf : pd.Series
-        te_in : pd.Series
-        te_out : pd.Series
-        pos : float, 0 == Volume flow sensor installed close to inlet / te_in, 1 == close to outlet / te_out
-
-        Returns
-        -------
-        tp : pd.Series
-            Calculated thermal power
-
-        Notes
-        -----
-        Position of volume flow sensor decides which temperature has to be used for density / mass flow calculation.
-        """
-        rho = fluid.get_density(
-            te=_get_weighted_temperature(te_in, te_out, 1 - pos, pos))
-        cp = fluid.get_heat_capacity(
-            te=_get_weighted_temperature(te_in, te_out))
-
-        mf = vf * rho * cp
-        tp = mf * (te_out - te_in)
-        return tp.pint.to('kW')
-        # pd.concat([rho.astype('float64'),
-        #            cp.astype('float64'),
-        #            mf.astype('float64'),
-        #
-        #            ], axis=1).to_clipboard()
-
-
-class CalcMassFlowFromPower(VirtualSensorCalculation):
-    """For plants and arrays, calculate mass flow from fluid, thermal power and inlet & outlet temperatures.
-    """
-
-    # def __init__(self, comp: Union[Plant, Array]):
-    def __init__(self, comp):
-        # if isinstance(comp, Array):
-        #     raise NotImplementedError('array.fluid -> array.plant.fluid_solar not yet implemented')
-        self.comp = comp
-        self.n_results = 1
-
-    def _core(self):
-        """
-        Returns
-        -------
-        tp : pd.Series
-            Calculated mass flow.
-        """
-        mf = self.calc_mf_from_tp(fluid=self.comp.fluid_solar,
-                                  tp=self.comp.tp.data,
-                                  te_in=self.comp.te_in.data,
-                                  te_out=self.comp.te_out.data)
-        return mf
-
-    def _do_assert(self, check_mode):
-        assert_valid_fluid(self.comp.fluid_solar)
-        self.comp.assert_verify_validate(check_mode, 'tp', 'te_in', 'te_out')
-
-    @staticmethod
-    def calc_mf_from_tp(fluid, tp, te_in, te_out):
-        """Calculates mass flow from fluid, thermal power and inlet & outlet temperatures.
-
-        Parameters
-        ----------
-        fluid : components.Fluid
-        tp : pd.Series
-        te_in : pd.Series
-        te_out : pd.Series
-
-        Returns
-        -------
-        mf : pd.Series
-            Calculated mass flow.
-        """
-        cp = fluid.get_heat_capacity(te=_get_weighted_temperature(te_in, te_out))
-        mf = tp / (cp * (te_out - te_in))
-        return mf.pint.to('kg s**-1')
-
-
-class CalcSolarPosition(VirtualSensorCalculation):
-    """Calculates solar angles (azimuth, elevation, zenith) for Plant, based on pvlib.
-    """
-
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 5
-
-    def _core(self):
-        """Calculates solar angles (azimuth, elevation, zenith) for Plant, based on pvlib.
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.solarposition.get_solarposition.html
-
-        Returns
-        -------
-        azimuth, zenitz, apparenzt_zenith, elevation, apparent_elevation : pd.Series
-            Angles defining the solar position.
-        """
-        longitude = self.plant.longitude.m_as('deg')
-        latitude = self.plant.latitude.m_as("deg")
-        altitude = None if (self.plant.altitude is None) else self.plant.altitude.m_as('m')
-        te_amb = self.plant.te_amb
-        if te_amb is None:
-            # returns pd.DataFrame
-            sol_pos = pv.solarposition.get_solarposition(time=self.plant.time_index,
-                                                         latitude=latitude,
-                                                         longitude=longitude,
-                                                         altitude=altitude)
-        else:
-            te_amb = te_amb.data.pint.to('degC')
-            # 12 degC is the pvlib default in case no ambient temperature is known
-            te_amb = te_amb.fillna(12).astype('float64').to_numpy()
-            sol_pos = pv.solarposition.get_solarposition(time=self.plant.time_index,
-                                                         latitude=latitude,
-                                                         longitude=longitude,
-                                                         altitude=altitude,
-                                                         temperature=te_amb)
-
-        return uu.to_s(sol_pos['azimuth'], 'deg'), \
-               uu.to_s(sol_pos['zenith'], 'deg'), \
-               uu.to_s(sol_pos['apparent_zenith'], 'deg'), \
-               uu.to_s(sol_pos['elevation'], 'deg'), \
-               uu.to_s(sol_pos['apparent_elevation'], 'deg')
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode, 'latitude', 'longitude')
-
-
-class CalcDewPointTemperature(VirtualSensorCalculation):
-    """Calculates ambient dew point temperature based on ambient temperature and ambient relative humidity of plant.
-    """
-
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 1
-
-    def _core(self):
-        """Calculates ambient dew point temperature based on ambient temperature and ambient relative humidity of plant.
-
-        Returns
-        -------
-        te_dew : pd.Series
-            Calculated ambient dew point temperature as pd.Series with dtype pint.
-        """
-        te_dew = self.calc_te_dew_from_te_rh_amb(te_amb=self.plant.te_amb.q_as('degC'),
-                                                 rh_amb=self.plant.rh_amb.q_as(''))
-        return te_dew
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode, 'te_amb', 'rh_amb')
-
-    @staticmethod
-    def calc_te_dew_from_te_rh_amb(te_amb, rh_amb):
-        te_dew = dewpoint_from_relative_humidity(te_amb, rh_amb)
-        te_dew = uu.to_s(te_dew, 'degC')
-        return te_dew
-
-
-class CalcDNIExtra(VirtualSensorCalculation):
-    """Calculates extraterrestrial solar radiation.
-    """
-    n_results = 1
-
-    def __init__(self, plant):
-        self.plant = plant
-
-    def _core(self):
-        """Calculates extraterrestrial solar radiation using pvlib function.
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.get_extra_radiation.html
-
-        Returns
-        -------
-        dni_extra : pd.Series
-            Extraterrestrial solar radiation in W/m².
-        """
-        dni_extra = pv.irradiance.get_extra_radiation(self.plant.time_index)
-        return to_rd(dni_extra)
-
-
-class CalcAirmass(VirtualSensorCalculation):
-    """Calculates relative and absolute airmass.
-    """
-
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 2
-
-    def _core(self):
-        """Calculate absolute airmass using pvlib function.
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.atmosphere.get_absolute_airmass.html
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.atmosphere.get_relative_airmass.html
-
-        Returns
-        -------
-        rel_airmass : pd.Series
-            Relative airmass (numeric value).
-        abs_airmass : pd.Series
-            Absolute, pressure-corrected airmass (numeric value).
-        """
-        rel_airmass = pv.atmosphere.get_relative_airmass(zenith=self.plant.sun_apparent_zenith.s_as('deg'))
-        abs_airmass = pv.atmosphere.get_absolute_airmass(airmass_relative=rel_airmass)
-        return rel_airmass.astype('pint[dimensionless]'), abs_airmass.astype('pint[dimensionless]')
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode, 'sun_apparent_zenith')
+import time
 
-
-class CalcLinkeTurbidity(VirtualSensorCalculation):
-    """Calculate Linke turbidity.
-    """
-
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 1
-
-    def _core(self):
-        """Calculate Linke turbidity using pvlib, required for clearsky irradiance calculation.
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.clearsky.lookup_linke_turbidity.html#pvlib.clearsky.lookup_linke_turbidity
-
-        Returns
-        -------
-        linke_turbidity : pd.Series, Linke turbidity
-        """
-        linke_turbidity = pv.clearsky.lookup_linke_turbidity(self.plant.time_index,
-                                                             self.plant.latitude.m_as('deg'),
-                                                             self.plant.longitude.m_as('deg'))
-        return uu.to_s(linke_turbidity, 'dimensionless')
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode, 'latitude', 'longitude')
+from sunpeek.common.utils import sp_logger
+import sunpeek.core_methods.virtuals.virtuals_plant as vp
+import sunpeek.core_methods.virtuals.virtuals_array as va
+from sunpeek.components.base import Component
 
 
-class CalcClearskyRadiation(VirtualSensorCalculation):
-    """Calcualte clearsky global horizontal irradiance and DNI using pvlib.
-    """
-
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 2
-
-    def _core(self):
-        """Calculate clearsky global horizontal irradiance and DNI using pvlib.
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.clearsky.ineichen.html#pvlib.clearsky.ineichen
-        Alternative models:
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.clearsky.haurwitz.html
-        https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.clearsky.simplified_solis.html
-
-        Returns
-        -------
-        rd_ghi_clearsky : pd.Series
-            Global horizontal clearsky radiation
-        rd_dni_clearsky : pd.Series
-            Clearsky DNI radiation
-        """
-        altitude = 0 if self.plant.altitude is None else self.plant.altitude.m_as('m')
-        clearsky = pv.clearsky.ineichen(self.plant.sun_apparent_zenith.m_as('deg'),
-                                        self.plant.abs_airmass.m_as(''),
-                                        self.plant.linke_turbidity.m_as('dimensionless'),
-                                        altitude,
-                                        self.plant.rd_dni_extra.m_as('W m**-2'))
-        # TODO This generates a RuntimeWarning: divide by zero, but the results all look good. How to treat?
-        return to_rd(clearsky['ghi'], clearsky['dni'])
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode,
-                                          'sun_apparent_zenith', 'abs_airmass', 'linke_turbidity', 'rd_dni_extra')
+def config_virtuals(plant):
+    """Creates & maps virtual sensors for all components.
 
-
-class CalcHorizontalIrradiances(VirtualSensorCalculation):
-    """For a plant, calculate horizontal irradiance components from plant radiation input slots.
+    Raises
+    ------
+    VirtualSensorConfigurationError
     """
+    # TODO Remove debug statement?
+    sp_logger.debug('In config_virtuals().')
+    start_time = time.time()
 
-    def __init__(self, plant):
-        self.plant = plant
-        self.n_results = 4
-
-    def _core(self):
-        """Calculate plant horizontal irradiance components.
-
-        Returns
-        -------
-        rd_ghi : pd.Series
-            Global horizontal irradiance
-        rd_bhi : pd.Series
-            Beam horizontal irradiance
-        rd_dhi : pd.Series
-            Diffuse horizontal irradiance
-        rd_dni : pd.Series
-            DNI irradiance
-        """
-        rc = RadiationConversionHorizontal(plant=self.plant,
-                                           in_global=self.plant.in_global,
-                                           in_beam=self.plant.in_beam,
-                                           in_diffuse=self.plant.in_diffuse,
-                                           in_dni=self.plant.in_dni)
-        rd_ghi, rd_bhi, rd_dhi, rd_dni = rc.get_irradiance_components()
-        return rd_ghi, rd_bhi, rd_dhi, rd_dni
+    vp.config_virtuals_ambient(plant)
+    vp.config_virtuals_power(plant)
+    # TODO Uncomment if plant horizontal radiations are needed e.g. for KPIs.
+    # vp.config_virtuals_radiation_conversion(plant)
 
-    def _do_assert(self, check_mode):
-        assert validate_radiation_inputs(self.plant)[0]
+    for array in plant.arrays:
+        va.config_virtuals_ambient(array)
+        va.config_virtuals_power(array)
+        va.config_virtuals_temperature(array)
+        va.config_virtuals_radiation_conversion(array)
+        # TODO Uncomment if vsensor array.te_out (averaged over row outlet temperatures) is required.
+        # va.config_virtuals_te_out(array)
 
+    sp_logger.debug(f"  [config_virtuals] --- Done in {(time.time() - start_time):.1f} seconds ---")
 
-class CalcTiltedIrradiances(VirtualSensorCalculation):
-    """For an array, calculate global, beam and diffuse irradiance from array radiation input slots.
-    """
 
-    def __init__(self, array, strategy='feedthrough'):
-        self.array = array
-        self.strategy = strategy
-        self.n_results = 3
-
-    def _core(self, **kwargs):
-        """Calculate array tilted irradiance components.
-
-        Returns
-        -------
-        rd_gti : pd.Series
-            Global tilted irradiance
-        rd_bti : pd.Series
-            Beam tilted irradiance
-        rd_dti : pd.Series
-            Diffuse tilted irradiance
-        """
-        rc = RadiationConversionTilted(array=self.array,
-                                       strategy=self.strategy,
-                                       in_global=self.array.in_global,
-                                       in_beam=self.array.in_beam,
-                                       in_diffuse=self.array.in_diffuse,
-                                       in_dni=self.array.in_dni,
-                                       **kwargs)
-        gti, bti, dti = rc.get_irradiance_components()
-        return gti, bti, dti
-
-    def _do_assert(self, check_mode):
-        assert self.strategy == 'feedthrough', \
-            'Only "feedthrough" strategy implemented so far.'
-        assert validate_radiation_inputs(self.array)[0]
-
-
-# def get_poa_irradiances(array, **kwargs):
-#     rc = RadiationConversionTilted(array=array, strategy='poa',
-#                                    in_global=array.in_global, in_beam=array.in_beam,
-#                                    in_diffuse=array.in_diffuse, in_dni=array.in_dni,
-#                                    **kwargs)
-#     dni, poa_diff_iso, poa_diff_circumsolar, poa_diff_horizon = rc.get_irradiance_components()
-#     return dni, poa_diff_iso, poa_diff_circumsolar, poa_diff_horizon
-
-
-# rd_bti_iam not needed? Currently using CalcIAM instead.
-# class CalcIAMRadiation(VirtualSensorCalculation):
-#     """Calculate incidence angle modifier (IAM) and IAM-corrected beam radiation for array.
-#     """
-#
-#     def __init__(self, array):
-#         self.array = array
-#         self.n_results = 2
-#
-#     def _core(self):
-#         """Calculate IAM and IAM-corrected beam radiation.
-#
-#         Returns
-#         -------
-#         iam : pd.Series
-#             Incidence Angle Modifier
-#         rd_bti_iam : pd.Series
-#             IAM-corrected (reduced) beam irradiance on array
-#         """
-#         ar = self.array
-#         iam = ar.collector_type.iam_method.get_iam(aoi=ar.aoi.data,
-#                                                    azimuth_diff=ar.plant.sun_azimuth.data - ar.azim)
-#
-#         try:
-#             self.array.assert_verify_validate(VerifyValidateMode.validate, 'rd_bti')
-#             rd_bti_iam = uu.to_numpy(iam) * self.array.rd_bti.data
-#         except AssertionError:
-#             rd_bti_iam = None
-#
-#         return iam, rd_bti_iam
-#
-#     def _do_assert(self, check_mode):
-#         assert not isinstance(self.array.collector_type, UninitialisedCollectorType)
-#         self.array.assert_verify_validate(check_mode, 'aoi', 'azim')
-#         self.array.plant.assert_verify_validate(check_mode, 'sun_azimuth')
+def calculate_virtuals(plant):
+    """Implements all the logic of the virtual sensor calculation. Typically called by data upload.
 
+    Raises
+    ------
+    CalculationError
 
-class CalcIAM(VirtualSensorCalculation):
-    """Calculate incidence angle modifier (IAM) for array.
-    """
-
-    def __init__(self, array):
-        self.array = array
-        self.n_results = 1
-
-    def _core(self):
-        """Calculate IAM.
-
-        Returns
-        -------
-        iam : pd.Series
-            Incidence Angle Modifier
-        """
-        ar = self.array
-        iam = ar.collector_type.iam_method.get_iam(aoi=ar.aoi.data,
-                                                   azimuth_diff=ar.plant.sun_azimuth.data - ar.azim)
-        return iam
-
-    def _do_assert(self, check_mode):
-        assert_valid_collector(self.array.collector_type)
-        self.array.assert_verify_validate(check_mode, 'aoi', 'azim')
-        self.array.plant.assert_verify_validate(check_mode, 'sun_azimuth')
-
-
-class CalcAngleOfIncidence(VirtualSensorCalculation):
-    """Calculate the angle of incidence of sun on plane of array using pvlib function.
-    """
-
-    def __init__(self, array):
-        self.array = array
-        self.plant = array.plant
-        self.n_results = 1
-
-    def _core(self):
-        """https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.aoi.html
-
-        Returns
-        -------
-        aoi : pd.Series
-            Angle of incidence
-        """
-        aoi = pv.irradiance.aoi(surface_tilt=self.array.tilt.m_as('deg'),
-                                surface_azimuth=self.array.azim.m_as('deg'),
-                                solar_zenith=self.plant.sun_zenith.m_as('deg'),
-                                solar_azimuth=self.plant.sun_azimuth.m_as('deg'))
-        return uu.to_s(aoi, 'deg')
-
-    def _do_assert(self, check_mode):
-        self.plant.assert_verify_validate(check_mode, 'sun_zenith', 'sun_azimuth')
-        self.array.assert_verify_validate(check_mode, 'tilt', 'azim')
-
-
-class CalcInternalShading(VirtualSensorCalculation):
-    """Calculates internal shading (row-to-row shading) related virtual sensors of a collector array.
-    """
-
-    def __init__(self, array):
-        self.array = array
-        self.plant = array.plant
-        self.n_results = 4
-
-    def _core(self):
-        """Calculates internal shading (row-to-row shading) and several related virtual sensors of a collector array.
-
-        Returns
-        -------
-        is_shadowed : pd.Series
-            bool. True if there is any (internal) shadow on the collector array. This takes into account: maximum
-            angle of incidence, minimum sun elevation, no internal (row-to-row) shading.
-        internal_shading_ratio : pd.Series
-            Float between 0 and 1. Degree of shading of the collectors due to row-to-row shading,
-            from not shaded (0) to completely shaded (1).
-        shadow_angle : pd.Series
-            Shadow angle between collector rows: Required minimum sun elevation in order not to have beam shading.
-        shadow_angle_midpoint : pd.Series
-            Shadow angle between collector rows, at half of the collector's slant height (i.e. the "midpoint"): Sun
-            elevation that corresponds to an internal_shading_ratio of 0.5. This can be used as a typical angle for
-            diffuse masking.
-
-        Notes
-        -----
-        Calculation based on [1].
-
-        internal_shading_ratio calculation taken from ADA implementation:
-        https://gitlab.com/sunpeek/sunpeek/uploads/d383e5e42f77516953810e13ac0f42cb/vDP_CollectorField_rd_bT_shaded.m
-        This implementation has been extended and takes array.ground_tilt into account.
-        Not used in algorithms: plant pressure, plant humidity / dewpoint
-        See also discussion in https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-
-        References
-        ----------
-        .. [1] Bany, J. and Appelbaum, J. (1987): "The effect of shading on the design of a field of solar collectors",
-            Solar Cells 20, p. 201 - 228
-            :doi:`https://doi.org/10.1016/0379-6787(87)90029-9`
-        """
-        pl = self.plant
-        ar = self.array
-
-        aoi_projection = pv.irradiance.aoi_projection(surface_tilt=ar.tilt.m_as('deg'),
-                                                      surface_azimuth=ar.azim.m_as('deg'),
-                                                      solar_zenith=pl.sun_zenith.m_as('deg'),
-                                                      solar_azimuth=pl.sun_azimuth.m_as('deg'))
-        sun_behind_coll = (aoi_projection < 0)
-        sun_below_horizon = (pl.sun_elevation.m_as('deg') <= 0)
-
-        # Formula (18), nomenclature according to BANY and APPELBAUM (1987)
-        beta = ar.tilt.m_as('rad') - ar.ground_tilt.m_as('rad')
-        sb = np.sin(beta)
-        cb = np.cos(beta)
-
-        A = ar.collector_type.gross_length.m_as('m')
-
-        Hc = A * np.sin(beta)
-        D = ar.row_spacing.m_as('m') - A * cb
-        # Relative collector spacing:
-        Drel = D / Hc
-        gamma = pl.sun_azimuth.m_as('rad') - ar.azim.m_as('rad')
-        alpha = pl.sun_elevation.m_as('rad')
-
-        # hs: shadow height [0..1]
-        cg = np.cos(gamma)
-        hs = 1 - ((Drel * sb + cb) / (cb + sb * cg / np.tan(alpha)))
-        hs[hs > 1] = 1
-        hs[hs < 0] = 0
-        hs[sun_behind_coll * sun_below_horizon] = 1
-        internal_shading_ratio = uu.to_s(hs, 'dimensionless')
-
-        # From formula of hs calculate shadow angle (as minimum sun elevation: no beam shading if sun above this angle)
-        alpha_min = np.arctan(cg / Drel)
-        shadow_angle = uu.to_s(alpha_min, 'rad').pint.to('deg')
-
-        # Shadow_angle_midpoint is the shadow angle at half of the collector's slant height.
-        alpha_min = np.arctan(cg / (2 * Drel + cb / sb))
-        shadow_angle_midpoint = uu.to_s(alpha_min, 'rad').pint.to('deg')
-
-        # is_shadowed: tells if the array generally is to be considered as affected by shadow or not.
-        is_not_shadowed = np.ones(len(shadow_angle))
-        if ar.max_aoi_shadow is not None:
-            is_not_shadowed *= (ar.aoi.m_as('deg') <= ar.max_aoi_shadow.m_as('deg'))
-        if ar.min_elevation_shadow is not None:
-            is_not_shadowed *= (ar.plant.sun_apparent_elevation.m_as('deg') >= ar.min_elevation_shadow.m_as('deg'))
-        is_not_shadowed *= (internal_shading_ratio == 0)
-        is_shadowed = uu.to_s(1-is_not_shadowed, 'dimensionless')
-
-        return is_shadowed, internal_shading_ratio, shadow_angle, shadow_angle_midpoint
-
-    def _do_assert(self, check_mode):
-        assert_valid_collector(self.array.collector_type)
-        assert self.array.collector_type.gross_length is not None
-        self.array.assert_verify_validate(check_mode, 'tilt', 'azim', 'row_spacing', 'aoi')
-        self.plant.assert_verify_validate(check_mode, 'sun_zenith', 'sun_azimuth', 'sun_elevation')
-
+    Notes
+    -----
+    At the end of calculate_virtuals, there might be virtual sensors that have not been calculated, for a variety of
+    possible reasons. Such an uncalculated virtual sensor, when queried for data (vsensor.data), it returns an
+    all-NaN series with the correct physical unit (pint dtype) attached.
+    """
+    config_virtuals(plant)
+    start_time = time.time()
+
+    sp_logger.debug(f"[calculate_virtuals] Calculating virtual sensors data.")
+    plant.context.verify_time_index()
+
+    vp.calculate_virtuals_ambient(plant)
+    vp.calculate_virtuals_power(plant)
+    # TODO Uncomment if horizontal radiations needed
+    # vp.calculate_virtuals_radiation_conversion(plant)
+
+    # Arrays
+    for array in plant.arrays:
+        va.calculate_virtuals_ambient(array)
+        va.calculate_virtuals_power(array)
+        va.calculate_virtuals_temperature(array)
+        va.calculate_virtuals_radiation_conversion(array)
+        # TODO Uncomment if vsensor array.te_out (averaged over row outlet temperatures) is required.
+        # va.calculate_virtuals_te_out(array)
 
-class CalcArrayTemperatures(VirtualSensorCalculation):
-    """Calculate mean operating temperature of collector array and its temperature derivative.
-    """
+    sp_logger.debug(f"[calculate_virtuals] --- Done in {(time.time() - start_time):.1f} seconds ---")
 
-    def __init__(self, array):
-        self.array = array
-        self.n_results = 2
-
-    def _core(self):
-        """Calculate mean operating temperature of collector array and its temperature derivative.
-
-        Returns
-        -------
-        te_op : pd.Series
-            Mean operating temperature
-        te_op_deriv : pd.Series
-            Derivative of mean operating temperature
-
-        Notes
-        -----
-        Implementation explanation:
-        `te_op` is smoothened with a Savitzky-Golay for more robust differentiation. Bad / noisy: te_op.diff()
-        Mathematically, we just have (te(t_N) - t(t_0))/dt, for regularly spaced data.
-        Using 'te_op_deriv' is preferred over this because instantaneous changes in `te_in` and `te_out`
-        make `te_op` a bad predictor for real mean temperature.
-        Integrating over a smoothened `te_op_deriv` is probably a better option, as the calculation then depends
-        not only on 2 single measurements, avoiding negative effects like meas. uncertainty of single measurements,
-        measurement delay and transport effects etc. So smoothing over all data should improve results.
-        More research on this should be done, especially on non-regularly spaced data.
-        """
-        # Mean operating temperature
-        te_op = _get_weighted_temperature(self.array.te_in.data, self.array.te_out.data)
-        te_op = pd.Series(uu.to_numpy(te_op, 'K'), index=self.array.plant.time_index)
-
-        # Derivative of mean operating temperature
-        mean_sampling_rate = self.array.plant.time_index.to_series().diff().min()
-        # Filling NaNs, otherwise savgol fails. Downstream methods need to filter intervals with too many NaNs out.
-        te_op.fillna(method='pad', inplace=True)
-        te_op_deriv = scipy.signal.savgol_filter(te_op, mode='mirror', window_length=15, polyorder=3, deriv=1)
-        te_op_deriv_final = te_op_deriv / mean_sampling_rate.total_seconds()  # now in K / s
-
-        return uu.to_s(te_op, 'K'), uu.to_s(te_op_deriv_final, 'K s**-1')
-
-    def _do_assert(self, check_mode):
-        self.array.assert_verify_validate(check_mode, 'te_in', 'te_out')
-
-
-def _get_weighted_temperature(te1, te2, w1=0.5, w2=0.5):
-    """Return weighted average between temperature pd.Series te1 and te2.
-    Takes care of converting things to K before doing the weighting. Result will be unit-aware pd.Series in degC.
-    """
-    # te_weighted = w1 * te1.pint.to('K') + w2 * te2.pint.to('K')
-    # return uu.to_s(te_weighted, 'degC')
-    # This greatly improves speed, especially in presence of many NaNs in data
-    te_weighted = w1 * te1.pint.to('K').astype('float64') + w2 * te2.pint.to('K').astype('float64')
-    return uu.to_s(te_weighted, 'K')
 
+Component.register_callback('post_config_changed_callbacks', config_virtuals)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## sunpeek/core_methods/virtuals/radiation.py

```diff
@@ -1,57 +1,111 @@
 from abc import ABC, abstractmethod
 import numpy as np
 import enum
 
 import pvlib as pv
-from sunpeek.common.errors import VirtualSensorConfigurationError, VirtualSensorCalculationError
-from sunpeek.common.utils import to_rd
+from sunpeek.common.errors import VirtualSensorConfigurationError, CalculationError
+from sunpeek.common.unit_uncertainty import to_s
 
 
-# import sunpeek.components as cmp
+## Utility functions
+
+def get_radiation_inputs(component):
+    """Return list with the 4 standard input slots of an Array of Plant.
+    """
+    return [component.in_global, component.in_beam, component.in_diffuse, component.in_dni]
 
 
-## Utility functions
+def unpack_radiations(component):
+    """Tries to read radiation as numeric value from self attributes (Sensor) in unit W/m**2.
+    Useful to prepare input sensors for radiation converters.
+    Returns
+    -------
+    tuple : pd.Series
+        For each Sensor, returns pd.Series of Sensor.data, converted to W/m², None if Sensor is None.
+    """
+    return (None if elem is None else elem.m_as('W m**-2') for elem in get_radiation_inputs(component))
+
+
+def to_rd(*args):
+    """Converts numeric inputs to pd.Series with pint dtype W/m².
+    Useful to return radiation converter results.
+    """
+    out = *(None if elem is None else to_s(elem, unit_str='W m**-2') for elem in args),
+    out = out[0] if len(out) == 1 else out
+    return out
+
+
+def get_radiation_pattern(component):
+    """Returns input pattern as string, where 1 if input is not None, else 0.
+    Example: beam and diffuse radiation given, while global and DNI are None: pattern=='0110'.
+    """
+    is_given = [x is not None for x in get_radiation_inputs(component)]
+    return f'{sum([x * np.power(10, 3 - i) for i, x in enumerate(is_given)]):04d}'
+
+
+# def _get_radiation_input_pattern(*args):
+#     """Returns input pattern as string, where 1 if input is not None, else 0.
+#     Example: beam and diffuse radiation given, while global and DNI are None: pattern=='0110'.
+#     """
+#     is_given = [x is not None for x in args]
+#     return f'{sum([x * np.power(10, 3 - i) for i, x in enumerate(is_given)]):04d}'
+
 
 def _get_orientation(c_in):
     """Returns tilt and orientation of a cmp.Array or a cmp.Sensor, assuming a radiation sensor for global, beam or diffuse (not for dni)
+
     Parameters
     ----------
-    c_in : cmp.Sensor or cmp.Array
+    c_in : Sensor or Array
+
     Returns
     -------
-    Returns tilt and azimuth in degrees or None if input is None.
+    tilt: tilt angle in degrees, or None if input is None.
+    azim: azim angle in degrees, or None if input is None.
     """
     if c_in is None:
         return None
-    orientation_dict = c_in.get_orientation()
-    return orientation_dict['tilt'], orientation_dict['azim']
+    return c_in.orientation['tilt'], c_in.orientation['azim']
 
 
-def _is_horizontal(*args):
+def is_horizontal(*args):
     """Returns tuple with bool for each arg.
     True if arg is horizontal (sensor.info.tilt==0 or array.tilt==0), False otherwise.
     """
-    return *(None if elem is None else (_get_orientation(elem) == 0) for elem in args),
+    # return *(None if elem is None else (_get_orientation(elem) == 0) for elem in args),
+    return [None if elem is None else (_get_orientation(elem) == 0) for elem in args]
 
 
-def _same_orientation(*args):
+def same_orientation(*args):
     """Checks whether two radiation sensors or arrays have same tilt & orientation.
+
     Parameters
     ----------
-    args : cmp.Sensor or cmp.Array
+    args : Sensor or Array
+
     Returns
     -------
     True if either all args are horizontal (tilt==0) or tilt and orientation are all the same.
     """
-    is_horizontal = [_is_horizontal(x) for x in args]
-    if all(is_horizontal):
-        return True
-    tilts = {x._get_orientation()[0] for x in args}
-    azims = {x._get_orientation()[1] for x in args}
+    args = [x for x in args if x is not None]
+
+    orientations_available = [x.has_orientation() for x in args]
+    if not all(orientations_available):
+        return False
+
+    # if all(_is_horizontal(*args)):
+    #     return True
+    #
+    # tilts = {_get_orientation(x)[0] for x in args}
+    # azims = {_get_orientation(x)[1] for x in args}
+
+    tilts = {_get_orientation(x)[0] for x in args if x is not None}
+    azims = {_get_orientation(x)[1] for x in args if x is not None}
+
     return len(tilts) == 1 and len(azims) == 1
 
 
 ## Elementary functions for radiation converter
 
 def _get_aoi(plant, tilt, azim):
     # TODO add docstring
@@ -61,690 +115,649 @@
     aoi = pv.irradiance.aoi(surface_tilt=tilt,
                             surface_azimuth=azim,
                             solar_zenith=plant.sun_zenith.m_as('deg'),
                             solar_azimuth=plant.sun_azimuth.m_as('deg'))
     return aoi
 
 
-def _get_dni_from_ghi(plant, ghi):
-    # TODO add docstring
-
-    # ghi : array-like in W/m²
-    # Decomposition
-    # DNI from global horitzonal (ghi) using dirindex model
-    # Returns: DNI in W/m²
-    # case [b] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-    # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dirindex.html
-    # TODO Philip Note that dirindex needs timeseries data! (vector of at least length 2), may not be case for all vs calculations
-    #  https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.dirindex.html
-    # TODO Philip I think we should have a parameter for radiation decompositon model to allow for other models in the future, e.g. https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.erbs.html
-    #  decomposition models are usually very easy to implement (e.g. Engerer)
-    dni = pv.irradiance.dirindex(ghi=ghi,
-                                 ghi_clearsky=plant.rd_ghi_clearsky.m_as('W m**-2'),
-                                 dni_clearsky=plant.rd_dni_clearsky.m_as('W m**-2'),
-                                 zenith=plant.sun_zenith.m_as('deg'),
-                                 times=plant.time_index)
-    return dni
-
-
-def _get_beam_from_dni(plant, dni, tilt=0, azim=180):
-    # TODO add docstring
-    # Calculates beam irradiance on arbitrary surface (tilt, azim) from DNI
-    # Returns: beam irradiane (bhi or bti, depending on tilt) in W/m²
-
-    bti = pv.irradiance.beam_component(surface_tilt=tilt,
-                                       surface_azimuth=azim,
-                                       solar_zenith=plant.sun_zenith.m_as('deg'),
-                                       solar_azimuth=plant.sun_azimuth.m_as('deg'),
-                                       dni=dni)
-    return bti
-
-
-def _get_horizontal_from_ghi(plant, ghi, dni=None):
-    # TODO Philip - add a function _get_horizontal_from_ghi_dni (confusing if we have _get_horizontal_from_ghi_bhi)
-    # TODO add docstring
-
-    # ghi : array-like in W/m²
-    # Returns: ghi, bhi, dhi, DNI in W/m²
-    # Decomposition
-
-    if dni is None:
-        dni = _get_dni_from_ghi(plant, ghi)
-    bhi = _get_beam_from_dni(plant, dni)
-    # bhi = pv.irradiance.beam_component(0, 180, plant.sun_zenith.to('deg'), plant.sun_azimuth.to('deg'), dni)
-    dhi = ghi - bhi
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_gti(plant, gti, tilt, azim):
-    """Inverse decomposition. Returns horizontal components from global tilted irradiance with given tilt and azimuth.
-
-    Parameters
-    ----------
-    gti : numeric array
-        Global titled irradiance in W/m².
-    tilt : float
-    azim : float
-        Tilt and azimuth angle at which the global tilted irradiance is given.
-
-    Returns
-    -------
-    global, beam, diffuse and DNI irradiances
-    """
-    # TODO add docstring
-    # TODO Philip: "Model performance is poor for AOI greater than approximately 80 degrees and plane of array irradiance greater than approximately 200 W/m^2."
-    #   (https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.gti_dirint.html) - do we need a virtual sensors which tells us if conversion is ok? and also some
-    #   basic quality checks (don't know if gti_dirint does this?)
-    # gti : array-like in W/m²
-    # tilt, azim : in degrees
-    # albedo: currently fixed to pvlib default of 0.25
-    # Returns: ghi, bhi, dhi, DNI in W/m²
-    # Case [a] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-    # Inverse decomposition
-    # Horizontal components (ghi, dhi, DNI) from global tilted (gti) using gti_dirint model
-    # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.gti_dirint.html
-
-    # TODO calculate_gt_90 should be True, but then gti_dirint throws IndexError
-    # gti[gti<0]=0
-
-    # TODO use plant dew point if available
-    horiz = pv.irradiance.gti_dirint(poa_global=gti,
-                                     aoi=_get_aoi(plant, tilt, azim),
-                                     solar_zenith=plant.sun_zenith.m_as('deg'),
-                                     solar_azimuth=plant.sun_azimuth.m_as('deg'),
-                                     times=plant.time_index,
-                                     surface_tilt=tilt,
-                                     surface_azimuth=azim,
-                                     calculate_gt_90=False,
-                                     use_delta_kt_prime=False,
-                                     model='perez',
-                                     model_perez='allsitescomposite1990',
-                                     temp_dew=None,
-                                     albedo=.25,
-                                     max_iterations=50)
-
-    horiz.index = plant.time_index
-    horiz = horiz.assign(gti=gti)
-    # horiz.plot()
-
-    bhi = horiz['ghi'] - horiz['dhi']
-    return horiz['ghi'], bhi, horiz['dhi'], horiz['dni']
-
-
-def _get_horizontal_from_ghi_dhi(plant, ghi, dhi):
-    # TODO add docstring
-    # ghi, dhi : array-like in W/m²
-    # Returns: ghi, bhi, dhi, DNI in W/m²
-
-    dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
-    bhi = _get_beam_from_dni(plant, dni)
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_dhi_dni(plant, dhi, dni):
-    # TODO add docstring
-    # Calculates global irradiance components from diffuse horizontal and DNI
-
-    bhi = _get_beam_from_dni(plant, dni)
-    ghi = bhi + dhi
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_dti_dni(plant, dti, dni):
-    # TODO add docstring
-    # Calculates global irradiance components from diffuse tilted and DNI
-    # by calculating global tilted irradiance in plane of dti sensor, then converting that gti to horizontal.
-
-    tilt, azim = _get_orientation(plant.in_diffuse)
-    bti = _get_beam_from_dni(plant, dni, tilt, azim)
-    gti = bti + dti
-    ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt, azim)
-
-    return ghi, bhi, dhi, dni
-
-
-def _get_dni_from_ghi_dhi(plant, ghi, dhi):
-    # TODO add docstring
-
-    # ghi, dhi : array-like in W/m²
-    # Returns: DNI in W/m²
-    # Case [c] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-    # uses pvlib dni: https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dni.html
-
-    dni = pv.irradiance.dni(ghi=ghi,
-                            dhi=dhi,
-                            zenith=plant.sun_zenith.m_as('deg'),
-                            clearsky_dni=plant.rd_dni_clearsky.m_as('W m**-2'))
-    return dni
-
-
-def _get_horizontal_from_ghi_bhi(plant, ghi, bhi):
-    # TODO add docstring
-    # Calculates horizontal irradiance components from ghi and bhi
-    # ghi, bhi : array-like in W/m²
-    # Returns: ghi, bhi, dhi, DNI in W/m²
-    dhi = ghi - bhi
-    dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_ghi_bti(plant, ghi, bti, tilt, azim):
-    # TODO add docstring
-    # Calculates horizontal irradiance components from ghi and bti
-    # ghi, bhi : array-like in W/m²
-    # Returns: ghi, bhi, dhi, DNI in W/m²
-    dni = _get_dni_from_beam(plant, bti, tilt, azim)
-    bhi = _get_beam_from_dni(plant, dni)
-    dhi = ghi - bhi
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_bti_dti(plant, bti, dti):
-    # TODO add docstring
-    # Calculate hotizontal irradiance components from beam and diffuse tilted radiations.
-    # This works also if bti and dti do not have the same tile & orientation.
-
-    tilt_d, azim_d = _get_orientation(plant.in_diffuse)
-    if _same_orientation(plant.in_beam, plant.in_diffuse):
-        gti = bti + dti
-    else:
-        # Convert bti to the plane where dti is given
-        tilt_b, azim_b = _get_orientation(plant.in_beam)
-        dni = _get_dni_from_beam(plant, bti, tilt_b, azim_b)
-        bti_d = _get_beam_from_dni(plant, dni, tilt_d, azim_d)
-        gti = bti_d + dti
-
-    ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt_d, azim_d)
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_bti_dhi(plant, bti, dhi):
-    # TODO add docstring
-    # Calculates horizontal irradiance components from beam tilted and diffuse horizontal measurements.
-
-    tilt, azim = _get_orientation(plant.in_beam)
-    dni = _get_dni_from_beam(plant, bti, tilt, azim)
-    bhi = _get_beam_from_dni(plant, dni)
-    ghi = bhi + dhi
-
-    return ghi, bhi, dhi, dni
-
-
-def _get_horizontal_from_bhi_dti(plant, bhi, dti):
-    # TODO add docstring
-    # Calcualtes horizontal irradiance components from beam horizontal and diffuse tilted
-
-    dni = _get_dni_from_beam(plant, bhi)
-    tilt, azim = _get_orientation(plant.in_diffuse)
-    bti = _get_beam_from_dni(plant, dni, tilt, azim)
-    gti = dti + bti
-    ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt, azim)
-    return ghi, bhi, dhi, dni
-
-
-def _get_dni_from_beam(plant, bti, tilt=0, azim=180, max_zenith=87):
-    # TODO add docstring
-    # Calculates DNI from beam horizontal or beam tilted irradiance
-    # ghi, bhi : array-like in W/m²
-    # tilt, azim
-    # Returns: DNI in W/m²
-    # max_zenith follows recommendation in
-    # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dirindex.html
-    aoi = _get_aoi(plant, tilt, azim)
-    aoi_ok = (aoi <= max_zenith)
-    dni = np.zeros_like(bti)
-    dni[aoi_ok] = bti[aoi_ok] / np.cos(aoi[aoi_ok])
-    return dni
-
-
-def _get_horizontal_from_bhi_dhi(plant, bhi, dhi):
-    # TODO add docstring
-    ghi = dhi - bhi
-    dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
-    return ghi, bhi, dhi, dni
+# To be uncommented, once radiation conversion for Arrays is implemented.
+# def _get_dni_from_ghi(plant, ghi):
+#     # TODO add docstring
+#
+#     # ghi : array-like in W/m²
+#     # Decomposition
+#     # DNI from global horitzonal (ghi) using dirindex model
+#     # Returns: DNI in W/m²
+#     # case [b] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+#     # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dirindex.html
+#     # TODO Philip Note that dirindex needs timeseries data! (vector of at least length 2), may not be case for all vs calculations
+#     #  https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.dirindex.html
+#     # TODO Philip I think we should have a parameter for radiation decompositon model to allow for other models in the future, e.g. https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.erbs.html
+#     #  decomposition models are usually very easy to implement (e.g. Engerer)
+#     dni = pv.irradiance.dirindex(ghi=ghi,
+#                                  ghi_clearsky=plant.rd_ghi_clearsky.m_as('W m**-2'),
+#                                  dni_clearsky=plant.rd_dni_clearsky.m_as('W m**-2'),
+#                                  zenith=plant.sun_zenith.m_as('deg'),
+#                                  times=plant.time_index)
+#     return dni
+
+
+# To be uncommented, once radiation conversion for Arrays is implemented.
+# def _get_beam_from_dni(plant, dni, tilt=0, azim=180):
+#     # TODO add docstring
+#     # Calculates beam irradiance on arbitrary surface (tilt, azim) from DNI
+#     # Returns: beam irradiane (bhi or bti, depending on tilt) in W/m²
+#
+#     bti = pv.irradiance.beam_component(surface_tilt=tilt,
+#                                        surface_azimuth=azim,
+#                                        solar_zenith=plant.sun_zenith.m_as('deg'),
+#                                        solar_azimuth=plant.sun_azimuth.m_as('deg'),
+#                                        dni=dni)
+#     return bti
+
+# To be uncommented, once radiation conversion for Arrays is implemented.
+# def _get_horizontal_from_ghi(plant, ghi, dni=None):
+#     # TODO Philip - add a function _get_horizontal_from_ghi_dni (confusing if we have _get_horizontal_from_ghi_bhi)
+#     # TODO add docstring
+#
+#     # ghi : array-like in W/m²
+#     # Returns: ghi, bhi, dhi, DNI in W/m²
+#     # Decomposition
+#
+#     if dni is None:
+#         dni = _get_dni_from_ghi(plant, ghi)
+#     bhi = _get_beam_from_dni(plant, dni)
+#     # bhi = pv.irradiance.beam_component(0, 180, plant.sun_zenith.to('deg'), plant.sun_azimuth.to('deg'), dni)
+#     dhi = ghi - bhi
+#     return ghi, bhi, dhi, dni
+
+
+# def _get_horizontal_from_gti(plant, gti, tilt, azim):
+#     """Inverse decomposition. Returns horizontal components from global tilted irradiance with given tilt and azimuth.
+#
+#     Parameters
+#     ----------
+#     gti : numeric array
+#         Global titled irradiance in W/m².
+#     tilt : float
+#     azim : float
+#         Tilt and azimuth angle at which the global tilted irradiance is given.
+#
+#     Returns
+#     -------
+#     global, beam, diffuse and DNI irradiances
+#     """
+#     # TODO add docstring
+#     # TODO Philip: "Model performance is poor for AOI greater than approximately 80 degrees and plane of array irradiance greater than approximately 200 W/m^2."
+#     #   (https://pvlib-python.readthedocs.io/en/v0.6.3/generated/pvlib.irradiance.gti_dirint.html) - do we need a virtual sensors which tells us if conversion is ok? and also some
+#     #   basic quality checks (don't know if gti_dirint does this?)
+#     # gti : array-like in W/m²
+#     # tilt, azim : in degrees
+#     # albedo: currently fixed to pvlib default of 0.25
+#     # Returns: ghi, bhi, dhi, DNI in W/m²
+#     # Case [a] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+#     # Inverse decomposition
+#     # Horizontal components (ghi, dhi, DNI) from global tilted (gti) using gti_dirint model
+#     # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.gti_dirint.html
+#
+#     # TODO calculate_gt_90 should be True, but then gti_dirint throws IndexError
+#     # gti[gti<0]=0
+#
+#     # TODO use plant dew point if available
+#     horiz = pv.irradiance.gti_dirint(poa_global=gti,
+#                                      aoi=_get_aoi(plant, tilt, azim),
+#                                      solar_zenith=plant.sun_zenith.m_as('deg'),
+#                                      solar_azimuth=plant.sun_azimuth.m_as('deg'),
+#                                      times=plant.time_index,
+#                                      surface_tilt=tilt,
+#                                      surface_azimuth=azim,
+#                                      calculate_gt_90=False,
+#                                      use_delta_kt_prime=False,
+#                                      model='perez',
+#                                      model_perez='allsitescomposite1990',
+#                                      temp_dew=None,
+#                                      albedo=.25,
+#                                      max_iterations=50)
+#
+#     horiz.index = plant.time_index
+#     horiz = horiz.assign(gti=gti)
+#     # horiz.plot()
+#
+#     bhi = horiz['ghi'] - horiz['dhi']
+#     return horiz['ghi'], bhi, horiz['dhi'], horiz['dni']
+#
+#
+# def _get_horizontal_from_ghi_dhi(plant, ghi, dhi):
+#     # TODO add docstring
+#     # ghi, dhi : array-like in W/m²
+#     # Returns: ghi, bhi, dhi, DNI in W/m²
+#
+#     dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
+#     bhi = _get_beam_from_dni(plant, dni)
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_dhi_dni(plant, dhi, dni):
+#     # TODO add docstring
+#     # Calculates global irradiance components from diffuse horizontal and DNI
+#
+#     bhi = _get_beam_from_dni(plant, dni)
+#     ghi = bhi + dhi
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_dti_dni(plant, dti, dni):
+#     # TODO add docstring
+#     # Calculates global irradiance components from diffuse tilted and DNI
+#     # by calculating global tilted irradiance in plane of dti sensor, then converting that gti to horizontal.
+#
+#     tilt, azim = _get_orientation(plant.in_diffuse)
+#     bti = _get_beam_from_dni(plant, dni, tilt, azim)
+#     gti = bti + dti
+#     ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt, azim)
+#
+#     return ghi, bhi, dhi, dni
+
+
+# To be uncommented, once radiation conversion for Arrays is implemented.
+# def _get_dni_from_ghi_dhi(plant, ghi, dhi):
+#     # TODO add docstring
+#
+#     # ghi, dhi : array-like in W/m²
+#     # Returns: DNI in W/m²
+#     # Case [c] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+#     # uses pvlib dni: https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dni.html
+#
+#     dni = pv.irradiance.dni(ghi=ghi,
+#                             dhi=dhi,
+#                             zenith=plant.sun_zenith.m_as('deg'),
+#                             clearsky_dni=plant.rd_dni_clearsky.m_as('W m**-2'))
+#     return dni
+
+
+# def _get_horizontal_from_ghi_bhi(plant, ghi, bhi):
+#     # TODO add docstring
+#     # Calculates horizontal irradiance components from ghi and bhi
+#     # ghi, bhi : array-like in W/m²
+#     # Returns: ghi, bhi, dhi, DNI in W/m²
+#     dhi = ghi - bhi
+#     dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_ghi_bti(plant, ghi, bti, tilt, azim):
+#     # TODO add docstring
+#     # Calculates horizontal irradiance components from ghi and bti
+#     # ghi, bhi : array-like in W/m²
+#     # Returns: ghi, bhi, dhi, DNI in W/m²
+#     dni = _get_dni_from_beam(plant, bti, tilt, azim)
+#     bhi = _get_beam_from_dni(plant, dni)
+#     dhi = ghi - bhi
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_bti_dti(plant, bti, dti):
+#     # TODO add docstring
+#     # Calculate hotizontal irradiance components from beam and diffuse tilted radiations.
+#     # This works also if bti and dti do not have the same tile & orientation.
+#
+#     tilt_d, azim_d = _get_orientation(plant.in_diffuse)
+#     if same_orientation(plant.in_beam, plant.in_diffuse):
+#         gti = bti + dti
+#     else:
+#         # Convert bti to the plane where dti is given
+#         tilt_b, azim_b = _get_orientation(plant.in_beam)
+#         dni = _get_dni_from_beam(plant, bti, tilt_b, azim_b)
+#         bti_d = _get_beam_from_dni(plant, dni, tilt_d, azim_d)
+#         gti = bti_d + dti
+#
+#     ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt_d, azim_d)
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_bti_dhi(plant, bti, dhi):
+#     # TODO add docstring
+#     # Calculates horizontal irradiance components from beam tilted and diffuse horizontal measurements.
+#
+#     tilt, azim = _get_orientation(plant.in_beam)
+#     dni = _get_dni_from_beam(plant, bti, tilt, azim)
+#     bhi = _get_beam_from_dni(plant, dni)
+#     ghi = bhi + dhi
+#
+#     return ghi, bhi, dhi, dni
+#
+#
+# def _get_horizontal_from_bhi_dti(plant, bhi, dti):
+#     # TODO add docstring
+#     # Calcualtes horizontal irradiance components from beam horizontal and diffuse tilted
+#
+#     dni = _get_dni_from_beam(plant, bhi)
+#     tilt, azim = _get_orientation(plant.in_diffuse)
+#     bti = _get_beam_from_dni(plant, dni, tilt, azim)
+#     gti = dti + bti
+#     ghi, bhi, dhi, dni = _get_horizontal_from_gti(plant, gti, tilt, azim)
+#     return ghi, bhi, dhi, dni
+
+
+# To be uncommented, once radiation conversion for Arrays is implemented.
+# def _get_dni_from_beam(plant, bti, tilt=0, azim=180, max_zenith=87):
+#     # TODO add docstring
+#     # Calculates DNI from beam horizontal or beam tilted irradiance
+#     # ghi, bhi : array-like in W/m²
+#     # tilt, azim
+#     # Returns: DNI in W/m²
+#     # max_zenith follows recommendation in
+#     # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.dirindex.html
+#     aoi = _get_aoi(plant, tilt, azim)
+#     aoi_ok = (aoi <= max_zenith)
+#     dni = np.zeros_like(bti)
+#     dni[aoi_ok] = bti[aoi_ok] / np.cos(aoi[aoi_ok])
+#     return dni
+
+
+# def _get_horizontal_from_bhi_dhi(plant, bhi, dhi):
+#     # TODO add docstring
+#     ghi = dhi - bhi
+#     dni = _get_dni_from_ghi_dhi(plant, ghi, dhi)
+#     return ghi, bhi, dhi, dni
 
 
 ## Radiation conversion classes
 
-class RadiationConversion(ABC):
-    def __init__(self, in_global, in_beam, in_diffuse, in_dni):
-        self.in_global = in_global
-        self.in_beam = in_beam
-        self.in_diffuse = in_diffuse
-        self.in_dni = in_dni
-        self.input_pattern = self._get_input_pattern()
-
-    @abstractmethod
-    def get_irradiance_components(self):
-        pass
+# class RadiationConversion(ABC):
+#     def __init__(self, in_global, in_beam, in_diffuse, in_dni):
+#         self.in_global = in_global
+#         self.in_beam = in_beam
+#         self.in_diffuse = in_diffuse
+#         self.in_dni = in_dni
+#         self.input_pattern = self.get_radiation_pattern()
+#
+#     @abstractmethod
+#     def get_irradiance_components(self):
+#         pass
 
     # @staticmethod
-    # def _from_rd(*args):
+    # def unpack_radiations(*args):
     #     """Tries to read radiation as numeric value from Sensor.data (of 1 or several cmp.Sensors) in unit W/m**2.
     #     Useful to prepare component sensors for radiation converter.
     #     Parameters
     #     ----------
     #     args : cmp.Sensor
     #     Returns
     #     -------
     #     tuple : pd.Series
     #         For each Sensor, returns pd.Series of Sensor.data, converted to W/m², None if Sensor is None.
     #     """
     #     return (None if elem is None else elem.m_as('W m**-2') for elem in args)
 
-    def _from_rd(self):
-        """Tries to read radiation as numeric value from self attributes (Sensor) in unit W/m**2.
-        Useful to prepare input sensors for radiation converters.
-        Returns
-        -------
-        tuple : pd.Series
-            For each Sensor, returns pd.Series of Sensor.data, converted to W/m², None if Sensor is None.
-        """
-        args = [self.in_global, self.in_beam, self.in_diffuse, self.in_dni]
-        return (None if elem is None else elem.m_as('W m**-2') for elem in args)
-
-    def _get_input_pattern(self):
-        """Returns input pattern as string, where 1 if input is not None, else 0.
-        Example: beam and diffuse radiation given, while global and DNI are None: pattern=='0110'.
-        """
-        is_given = [x is not None for x in [self.in_global, self.in_beam, self.in_diffuse, self.in_dni]]
-        return f'{sum([x * np.power(10, 3 - i) for i, x in enumerate(is_given)]):04d}'
-
-    def _is_horizontal(self):
-        """Returns tuple with bool for each of the radiation Sensors self.in_global, .in_beam, .in_diffuse.
-        """
-        return _is_horizontal(self.in_global, self.in_beam, self.in_diffuse)
-
-
-class RadiationConversionHorizontal(RadiationConversion):
-    """Calculates horizontal irradiance components (global, beam, diffuse, DNI) for the plant.
-    """
-
-    def __init__(self, plant, *args, **kwargs):
-        self.plant = plant
-        super().__init__(*args, **kwargs)
-        return
-
-    def get_irradiance_components(self):
-        return self.get_horizontal_irradiances()
-
-    def get_horizontal_irradiances(self):
-        """Calculates horizontal irradiance components (global, beam, diffuse, DNI) for the plant.
-        radiation input sensors
-        TODO correct docstring, state the selection pattern for the different cases
-        Returns horizontal irradiance components for global, beam / direct, diffuse and DNI.
-        Returns: horizontal ghi, bhi, dhi, dni
-        Logic is described in detail in https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-        """
-
-        glob, beam, diff, dni = self._from_rd()
-        is_glob_horizontal, is_beam_horizontal, is_diff_horizontal = self._is_horizontal()
-
-        # self.input_pattern:
-        # 1 input:
-        #  1000 ok, global only
-        #  0100, 0010, 0001: not ok, not enough inputs
-        # 2 inputs:
-        #  1100 ok, global + beam
-        #  1010 ok, global + diffuse
-        #  1001 ok, global + DNI
-        #  0110 ok, beam + diffuse
-        #  0011 ok, diffuse + DNI
-        # 3 inputs: not yet implemented (
-        #  1110 ok, global + beam + diffuse -> same as 0110 (ignore global)
-        #  1101 ok, global + beam + dni     -> same as 1001 (ignore beam)
-        #  1011 ok, global + diffuse + dni  -> same as 0101 (ignore global)
-        #  0111 ok, beam + diffuse + dni    -> same as 0011 (ignore beam)
-        # 4 inputs: not yet implemented
-        #  1111 ok, global + beam + diffuse + dni -> same as 0101 (ignore global and beam)
-
-        # raise NotImplementedError
-
-        # no radiation inputs
-        if self.input_pattern == '0000':
-            ghi, bhi, dhi, dni = None, None, None, None
-        # TODO Philip - I suggest to change to selection order for the overdetermined case,
-        #  see https://gitlab.com/sunpeek/sunpeek/-/issues/128
-        # global only
-        elif self.input_pattern == '1000':
-            if is_glob_horizontal:
-                # Input glob is ghi: decomposition
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob)
-            else:
-                # Input glob is some gti: inverse decomposition
-                tilt, azim = _get_orientation(self.in_global)
-                ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
-
-        # global + beam
-        elif self.input_pattern == '1100':
-            if is_glob_horizontal and is_beam_horizontal:
-                # Inputs are ghi and bhi
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bhi(self.plant, glob, beam)
-            elif is_glob_horizontal:
-                # Inputs are ghi and bti
-                tilt, azim = _get_orientation(self.in_beam)
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bti(self.plant, glob, beam, tilt, azim)
-            else:
-                # TODO Philip - To ignore beam is not intuitive to me here
-                #  1) calcuate ghi, use bhi as measured? or 2) use other model with gti, bti inputs?
-                # Inputs are gti and (bhi or bti): beam input is ignored
-                tilt, azim = _get_orientation(self.in_global)
-                ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
-
-        # global + diffuse
-        elif self.input_pattern == '1010':
-            if is_glob_horizontal and is_diff_horizontal:
-                # Inputs are ghi and dhi
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi_dhi(self.plant, glob, diff)
-            elif is_glob_horizontal:
-                # Inputs are ghi and dti: diffuse input is ignored
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob)
-            else:
-                # TODO Philip - same problem as with ignoring beam:
-                #  if gti and dti are in SAME plane --> calcuate + use beam
-                # Inputs are gti and (dhi or dti): diffuse input is ignored
-                tilt, azim = _get_orientation(self.in_global)
-                ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
-
-        # global + DNI
-        elif self.input_pattern == '1001':
-            if is_glob_horizontal:
-                # Inputs are ghi and DNI
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob, dni)
-            else:
-                # Inputs are gti and DNI
-                tilt, azim = _get_orientation(self.in_global)
-                ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
-
-        # diffuse + DNI
-        elif self.input_pattern == '0011':
-            if is_diff_horizontal:
-                # Inputs are dhi and DNI
-                ghi, bhi, dhi, dni = _get_horizontal_from_dhi_dni(self.plant, diff, dni)
-            else:
-                # Inputs are dti and DNI
-                ghi, bhi, dhi, dni = _get_horizontal_from_dti_dni(self.plant, diff, dni)
-
-        # beam + diffuse (and other subsumed cases that include beam + diffuse)
-        elif self.input_pattern in ['0110', '1110', '0111', '1111']:
-            if is_beam_horizontal and is_diff_horizontal:
-                # Inputs are bhi and dhi
-                ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bhi(self.plant, beam, diff)
-            elif ~is_beam_horizontal and ~is_diff_horizontal:
-                # Inputs are bti and dti
-                ghi, bhi, dhi, dni = _get_horizontal_from_bti_dti(self.plant, beam, diff)
-            elif is_diff_horizontal:
-                # Inputs are bti and dhi
-                ghi, bhi, dhi, dni = _get_horizontal_from_bti_dhi(self.plant, beam, diff)
-            else:
-                # Inputs are bhi and dti
-                ghi, bhi, dhi, dni = _get_horizontal_from_bhi_dti(self.plant, beam, diff)
-
-        elif self.input_pattern in ['0100', '0010', '0001', '0101']:
-            # Not permitted, cannot calculate horizontal radiation components with these inputs
-            # These cases should have been caught by assert_enough_radiation_inputs().
-            raise VirtualSensorConfigurationError(
-                'Cannot calculate horizontal radiation components with the given radiation inputs.')
-        else:
-            raise NotImplementedError()
-
-        return to_rd(ghi, bhi, dhi, dni)
-
-
-class TiltedStrategy(enum.Enum):
-    poa = 0  # Return plane of array irradiance components.
-    feedthrough = 1  # Return only input sensor values, if orientation matches; no radiation modeling.
-    detailed = 2  # Return all irradiance components using radiation modeling.
-
+    # def _is_horizontal(self):
+    #     """Returns tuple with bool for each of the radiation Sensors self.in_global, .in_beam, .in_diffuse.
+    #     """
+    #     return is_horizontal(self.in_global, self.in_beam, self.in_diffuse)
 
-class RadiationConversionTilted(RadiationConversion):
-    """
-    TODO update docstring
-    """
 
-    def __init__(self, array, strategy='feedthrough',
-                 use_diffuse_masking=True,
-                 use_beam_shading=True,
-                 ground_diffuse_strategy='ghi',
-                 ground_albedo=0.25,
-                 treat_circumsolar_as_diffuse=True,
-                 horizon_brightness_strategy='ignore',
-                 *args, **kwargs):
-        self.array = array
-        self.tilt = array.tilt.m_as('deg')
-        self.azim = array.azim.m_as('deg')
-        self.plant = array.plant
-        self.strategy = strategy
-        self.use_diffuse_masking = use_diffuse_masking
-        self.use_beam_shading = use_beam_shading
-        self.ground_diffuse_strategy = ground_diffuse_strategy
-        self.ground_albedo = ground_albedo
-        self.treat_circumsolar_as_diffuse = treat_circumsolar_as_diffuse
-        self.horizon_brightness_strategy = horizon_brightness_strategy
-        super().__init__(*args, **kwargs)
-        return
-
-    @property
-    def strategy(self):
-        return self._strategy
-
-    @strategy.setter
-    def strategy(self, val):
-        if val is not None:
-            self._strategy = TiltedStrategy[val]
-
-    def get_irradiance_components(self):
-        if self._strategy is TiltedStrategy.feedthrough:
-            return to_rd(*self._get_array_irradiances_feedthrough())
-        elif self.strategy is TiltedStrategy.poa:
-            return to_rd(*self._get_poa_irradiances())
-        elif self.strategy is TiltedStrategy.detailed:
-            return to_rd(*self._get_array_irradiances_detailed())
-        else:
-            return AttributeError(f'Invalid tilted strategy {self.strategy}.')
-
-    def _get_array_irradiances_feedthrough(self):
-        """Returns global, beam, diffuse irradiances on array, only if input sensor and array orientations match.
-        Does not do any further calculations like applying radiation models.
-        Returns
-        -------
-        gti, bti, dti : numeric array
-            Global, beam and diffuse tilted radiation components in W/m².
-        """
-
-        glob, beam, diff, dni = self._from_rd()
-        gti, bti, dti = None, None, None
-        if not _same_orientation(self.array, self.in_global, self.in_beam, self.in_diffuse):
-            raise VirtualSensorCalculationError('Array irradiance calculation with strategy "feedthrough" can only '
-                                                'be applied if array and sensor have the same orientation.')
-
-        # no radiation inputs
-        if self.input_pattern == '0000':
-            gti, bti, dti = None, None, None
-        # global only
-        elif self.input_pattern == '1000':
-            gti = glob
-        # beam + diffuse
-        elif self.input_pattern == '0110':
-            bti, dti = beam, diff
-        # global + beam + diffuse
-        elif self.input_pattern in ['1110', '1111']:
-            gti, bti, dti = glob, beam, diff
-        else:
-            raise VirtualSensorCalculationError(
-                'Array irradiance calculation with strategy "feedthrough" only accepts either global or beam + diffuse '
-                'or all 3 radiations together as inputs. Got input pattern' + self.input_pattern)
-        return gti, bti, dti
-
-    def _get_array_irradiances_detailed(self):
-        """Returns global, beam, diffuse irradiances on array, applying detailed modeling with plane-of-array irradiances.
-        Returns
-        -------
-        gti : numeric array
-          Global irradiance on array in W/m².
-        bti : numeric array
-          Beam / direct irradiance on array in W/m².
-        dti : numeric array
-          Diffuse irradiance on array in W/m².
-
-        Notes
-        -----
-        Calculates array irradiance components global, beam / direct and diffuse.
-        Components of poa diffuse (e.g. horizon brightness) can be combined specifically.
-        Calls _get_poa_irradiances() to yield DNI and poa diffuse components (diffuse sky, diffuse horizon etc.)
-        For diffuse masking, uses shadow_angle_midpoint, i.e. the angle at half of the collector's slant height.
-        """
-        # TODO Daniel would be good to get your ideas about details on how to calculate dti
-        # TODO Make sure array virtual sensors exist: shadow_angle_midpoint, internal_shading_ratio, plant.ghi
-        # TODO Philip - conversion strategies should be 'consistent', i.e. if we apply inverse, then forward direction for a sensor, this should return the sensor value
-        #   - step 1:
-        #   - a) using gti (in same plane as array) --> apply dirint --> keep gti, calculate bti based on DNI, "normalize" shares for iffuse_iso + diffuse_circ + diffuse_horz
-        #   - b) using gti (in different plane than array) --> apply dirint --> use perez model
-        #   - step 2:
-        #   - calcuate reduction (masking, horizon) RELATIVE to measurement at the top of the collector --> we need to define the default settings here
-        #   - later:
-        #   - alternatively, we could think of implementing our own radiation conversion model to make this consistent, e.g. like https://www.sciencedirect.com/science/article/pii/S0038092X21000633,
-        #     for the solar community it would be help to have a very general radiation conversion algorithm for all possible measurement setups
-
-        # Plane-of-array irradiance components
-        dni, poa_diffuse_iso, poa_diffuse_circ, poa_diffuse_horiz = self._get_poa_irradiances()
-        bti = _get_beam_from_dni(self.plant, dni, self.tilt, self.azim)
-
-        # Diffuse masking
-        if self.use_diffuse_masking:
-            # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.shading.sky_diffuse_passias.html
-            iso_blocked = pv.shading.sky_diffuse_passias(masking_angle=self.array.shadow_angle_midpoint.m_as('deg'))
-            poa_diffuse_iso *= np.ones_like(poa_diffuse_iso) - iso_blocked
-            # TODO Philip - This calculation is NOT correct, it does not take the tilt angle of the array into account!
-        dti = poa_diffuse_iso
-
-        # Circumsolar diffuse
-        if self.treat_circumsolar_as_diffuse:
-            dti += poa_diffuse_circ
-        else:  # treat circumsolar as beam
-            bti += poa_diffuse_circ
-
-        # Beam shading
-        if self.use_beam_shading:
-            bti *= np.ones_like(bti) - self.array.internal_shading_ratio.m_as('dimensionless')
-
-        # Horizon brightness
-        if self.horizon_brightness_strategy == 'ignore':
-            pass
-        else:
-            dti += poa_diffuse_horiz
-
-        # Ground diffuse
-        # TODO Philip - these models need to be consistent with the transposition model - I would include the options
-        #  - a) ground reflection as in Perez
-        #  - b) ignore ground reflection (substract this from the diffuse irradiance?)
-        #  - b) correct ground reflection (with view factor from sensors versus towards ground)
-        if self.ground_diffuse_strategy == 'ignore':
-            pass
-        elif self.ground_diffuse_strategy == 'ghi':
-            if self.plant.ghi is None:
-                raise VirtualSensorCalculationError(
-                    'Calculating array irradiances with strategy "ghi" requires plant.ghi to be not None.')
-                # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.get_ground_diffuse.html
-            dti += pv.irradiance.get_ground_diffuse(surface_tilt=self.tilt,
-                                                    ghi=self.plant.ghi.m_as('W m**-2'),
-                                                    albedo=self.ground_albedo)
-        else:
-            raise NotImplementedError
-
-        gti = bti + dti
-        return gti, bti, dti
-
-    def _get_poa_irradiances(self):
-        """Calculates in-plane radiation components from array radiation input sensors in_global, in_beam, in_diffuse,
-        in_dni. Returns tilted in-plane (poa, plane-of-array) irradiance components for DNI, sky and ground diffuse.
-        Returns
-        -------
-        rd_dni : numeric array
-          DNI (Direct Normal Irradiance) in W/m².
-        rd_poa_diffuse_sky : numeric array
-          Plane-of-array (poa) in-plane diffuse irradiance from the sky in W/m².
-        rd_poa_diffuse_ground : numeric array
-          Plane-of-array (poa) in-plane diffuse irradiance from the ground in W/m².
-
-        Note:
-        -----
-        Does not take beam shading and diffuse masking of the array into account.
-        Logic is described in https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-        """
-
-        glob, beam, diff, dni = self._from_rd()
-        is_glob_horizontal, is_beam_horizontal, is_diff_horizontal = self._is_horizontal()
-
-        # no radiation inputs
-        if self.input_pattern == '0000':
-            dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = None, None, None, None
-        # global only
-        elif self.input_pattern == '1000':
-            if is_glob_horizontal:
-                # Input glob is ghi
-                dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = self._get_poa_from_ghi(glob)
-            else:
-                # Input glob is some gti: inverse decomposition
-                raise NotImplementedError
-                # tilt, azim = _get_sensor_orientation(array._in_glob)
-                # dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = _get_poa_from_gti(plant, glob, tilt, azim)
-        else:
-            # TODO implement more tilted radiation strategies here
-            raise NotImplementedError
-
-        return dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz
-
-    def _get_poa_from_ghi(self, ghi):
-        # TODO add docstring
-        # Calculates plane-of-array radiation components from global horizontal irradiance / measurement.
-        # Combines decomposition (dirindex) and transposition (Perez)
-        # Returns plane-of-array irradiance, i.e. does not take beam shading and diffuse masking into account.
-        # Returns: DNI, isotropic diffuse, circumsolar diffuse, horizon brightness radiations, all in W/m²
-
-        dni = _get_dni_from_ghi(self.plant, ghi)
-        bhi = _get_beam_from_dni(self.plant, dni)
-        dhi = ghi - bhi
-        poa_diff_iso, poa_diff_circ, poa_diff_horiz = self._get_poadiffuse_from_dhi(dhi, dni)
-        return dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz
-
-    def _get_poa_from_gti(self, gti):
-        # TODO add docstring
-        # Calculates plane-of-array radiation components from global tilted irradiance / measurement.
-        raise NotImplementedError
-        # tilt, azim = _get_sensor_orientation(array.in_global)
-        # gti_dirint
-
-    def _get_poadiffuse_from_dhi(self, dhi, dni):
-        # TODO add docstring
-        # dhi, dni : array-like in W/m²
-        # Returns:
-        # --------
-        # poa_diff_iso : numeric
-        #   Tilted / poa isotropic diffuse radiation, in W/m²
-        # poa_diff_circ : numeric
-        #   Tilted / poa circumsolar radiation, in W/m²
-        # poa_diff_horiz : numeric
-        #   Tilted /poa horizon brightness radiation, in W/m²
-        # Transposition: Calculates sky diffuse irradiance in plane of array from global and diffuse horizontal.
-        # This implementation uses the Perez method:
-        # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.perez.html
-        # case [f] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
-        # TODO Make sure the necessary sensors like plant.sun_apparent_zenit, plant.rel_airmass exist / not None
-
-        diffuse = pv.irradiance.perez(surface_tilt=self.tilt,
-                                      surface_azimuth=self.azim,
-                                      dhi=dhi,
-                                      dni=dni,
-                                      dni_extra=self.plant.rd_dni_extra.m_as('W m**-2'),
-                                      solar_zenith=self.plant.sun_apparent_zenith.m_as('deg'),
-                                      solar_azimuth=self.plant.sun_azimuth.m_as('deg'),
-                                      airmass=self.plant.rel_airmass.m_as(''),
-                                      return_components=True)
-        return diffuse['isotropic'], diffuse['circumsolar'], diffuse['horizon']
+# class RadiationConversionHorizontal(RadiationConversion):
+#     """Calculates horizontal irradiance components (global, beam, diffuse, DNI) for the plant.
+#     """
+#
+#     def __init__(self, plant, *args, **kwargs):
+#         self.plant = plant
+#         super().__init__(*args, **kwargs)
+#         return
+#
+#     def get_irradiance_components(self):
+#         return self.get_horizontal_irradiances()
+#
+#     def get_horizontal_irradiances(self):
+#         """Calculates horizontal irradiance components (global, beam, diffuse, DNI) for the plant.
+#         radiation input sensors
+#         TODO correct docstring, state the selection pattern for the different cases
+#         Returns horizontal irradiance components for global, beam / direct, diffuse and DNI.
+#         Returns: horizontal ghi, bhi, dhi, dni
+#         Logic is described in detail in https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+#         """
+#
+#         glob, beam, diff, dni = self.unpack_radiations()
+#         is_glob_horizontal, is_beam_horizontal, is_diff_horizontal = self._is_horizontal()
+#
+#         # self.input_pattern:
+#         # 1 input:
+#         #  1000 ok, global only
+#         #  0100, 0010, 0001: not ok, not enough inputs
+#         # 2 inputs:
+#         #  1100 ok, global + beam
+#         #  1010 ok, global + diffuse
+#         #  1001 ok, global + DNI
+#         #  0110 ok, beam + diffuse
+#         #  0011 ok, diffuse + DNI
+#         # 3 inputs: not yet implemented (
+#         #  1110 ok, global + beam + diffuse -> same as 0110 (ignore global)
+#         #  1101 ok, global + beam + dni     -> same as 1001 (ignore beam)
+#         #  1011 ok, global + diffuse + dni  -> same as 0101 (ignore global)
+#         #  0111 ok, beam + diffuse + dni    -> same as 0011 (ignore beam)
+#         # 4 inputs: not yet implemented
+#         #  1111 ok, global + beam + diffuse + dni -> same as 0101 (ignore global and beam)
+#
+#         # raise NotImplementedError
+#
+#         # no radiation inputs
+#         if self.input_pattern == '0000':
+#             ghi, bhi, dhi, dni = None, None, None, None
+#         # TODO Philip - I suggest to change to selection order for the overdetermined case,
+#         #  see https://gitlab.com/sunpeek/sunpeek/-/issues/128
+#         # global only
+#         elif self.input_pattern == '1000':
+#             if is_glob_horizontal:
+#                 # Input glob is ghi: decomposition
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob)
+#             else:
+#                 # Input glob is some gti: inverse decomposition
+#                 tilt, azim = _get_orientation(self.in_global)
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
+#
+#         # global + beam
+#         elif self.input_pattern == '1100':
+#             if is_glob_horizontal and is_beam_horizontal:
+#                 # Inputs are ghi and bhi
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bhi(self.plant, glob, beam)
+#             elif is_glob_horizontal:
+#                 # Inputs are ghi and bti
+#                 tilt, azim = _get_orientation(self.in_beam)
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bti(self.plant, glob, beam, tilt, azim)
+#             else:
+#                 # TODO Philip - To ignore beam is not intuitive to me here
+#                 #  1) calcuate ghi, use bhi as measured? or 2) use other model with gti, bti inputs?
+#                 # Inputs are gti and (bhi or bti): beam input is ignored
+#                 tilt, azim = _get_orientation(self.in_global)
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
+#
+#         # global + diffuse
+#         elif self.input_pattern == '1010':
+#             if is_glob_horizontal and is_diff_horizontal:
+#                 # Inputs are ghi and dhi
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi_dhi(self.plant, glob, diff)
+#             elif is_glob_horizontal:
+#                 # Inputs are ghi and dti: diffuse input is ignored
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob)
+#             else:
+#                 # TODO Philip - same problem as with ignoring beam:
+#                 #  if gti and dti are in SAME plane --> calcuate + use beam
+#                 # Inputs are gti and (dhi or dti): diffuse input is ignored
+#                 tilt, azim = _get_orientation(self.in_global)
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
+#
+#         # global + DNI
+#         elif self.input_pattern == '1001':
+#             if is_glob_horizontal:
+#                 # Inputs are ghi and DNI
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi(self.plant, glob, dni)
+#             else:
+#                 # Inputs are gti and DNI
+#                 tilt, azim = _get_orientation(self.in_global)
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_gti(self.plant, glob, tilt, azim)
+#
+#         # diffuse + DNI
+#         elif self.input_pattern == '0011':
+#             if is_diff_horizontal:
+#                 # Inputs are dhi and DNI
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_dhi_dni(self.plant, diff, dni)
+#             else:
+#                 # Inputs are dti and DNI
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_dti_dni(self.plant, diff, dni)
+#
+#         # beam + diffuse (and other subsumed cases that include beam + diffuse)
+#         elif self.input_pattern in ['0110', '1110', '0111', '1111']:
+#             if is_beam_horizontal and is_diff_horizontal:
+#                 # Inputs are bhi and dhi
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_ghi_bhi(self.plant, beam, diff)
+#             elif ~is_beam_horizontal and ~is_diff_horizontal:
+#                 # Inputs are bti and dti
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_bti_dti(self.plant, beam, diff)
+#             elif is_diff_horizontal:
+#                 # Inputs are bti and dhi
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_bti_dhi(self.plant, beam, diff)
+#             else:
+#                 # Inputs are bhi and dti
+#                 ghi, bhi, dhi, dni = _get_horizontal_from_bhi_dti(self.plant, beam, diff)
+#
+#         elif self.input_pattern in ['0100', '0010', '0001', '0101']:
+#             # Not permitted, cannot calculate horizontal radiation components with these inputs
+#             # These cases should have been caught by assert_enough_radiation_inputs().
+#             raise VirtualSensorConfigurationError(
+#                 'Cannot calculate horizontal radiation components with the given radiation inputs.')
+#         else:
+#             raise NotImplementedError()
+#
+#         return to_rd(ghi, bhi, dhi, dni)
+
+
+# TODO delete
+# class TiltedStrategy(enum.Enum):
+#     poa = 0  # Return plane of array irradiance components.
+#     feedthrough = 1  # Return only input sensor values, if orientation matches; no radiation modeling.
+#     detailed = 2  # Return all irradiance components using radiation modeling.
+
+
+# class RadiationConversionTilted(RadiationConversion):
+#     """
+#     TODO update docstring
+#     """
+#
+#     def __init__(self, array, strategy='feedthrough',
+#                  use_diffuse_masking=True,
+#                  use_beam_shading=True,
+#                  ground_diffuse_strategy='ghi',
+#                  ground_albedo=0.25,
+#                  treat_circumsolar_as_diffuse=True,
+#                  horizon_brightness_strategy='ignore',
+#                  *args, **kwargs):
+#         self.array = array
+#         self.tilt = array.tilt.m_as('deg')
+#         self.azim = array.azim.m_as('deg')
+#         self.plant = array.plant
+#         self.strategy = strategy
+#         self.use_diffuse_masking = use_diffuse_masking
+#         self.use_beam_shading = use_beam_shading
+#         self.ground_diffuse_strategy = ground_diffuse_strategy
+#         self.ground_albedo = ground_albedo
+#         self.treat_circumsolar_as_diffuse = treat_circumsolar_as_diffuse
+#         self.horizon_brightness_strategy = horizon_brightness_strategy
+#         super().__init__(*args, **kwargs)
+#         return
+#
+#     @property
+#     def strategy(self):
+#         return self._strategy
+#
+#     @strategy.setter
+#     def strategy(self, val):
+#         if val is not None:
+#             self._strategy = TiltedStrategy[val]
+#
+#     def get_irradiance_components(self):
+#         if self._strategy is TiltedStrategy.feedthrough:
+#             return to_rd(*self._get_array_irradiances_feedthrough())
+#         elif self.strategy is TiltedStrategy.poa:
+#             return to_rd(*self._get_poa_irradiances())
+#         elif self.strategy is TiltedStrategy.detailed:
+#             return to_rd(*self._get_array_irradiances_detailed())
+#         else:
+#             return AttributeError(f'Invalid tilted strategy {self.strategy}.')
+
+    # To be uncommented, once radiation conversion for Arrays is implemented.
+    # def _get_array_irradiances_detailed(self):
+    #     """Returns global, beam, diffuse irradiances on array, applying detailed modeling with plane-of-array irradiances.
+    #     Returns
+    #     -------
+    #     gti : numeric array
+    #       Global irradiance on array in W/m².
+    #     bti : numeric array
+    #       Beam / direct irradiance on array in W/m².
+    #     dti : numeric array
+    #       Diffuse irradiance on array in W/m².
+    #
+    #     Notes
+    #     -----
+    #     Calculates array irradiance components global, beam / direct and diffuse.
+    #     Components of poa diffuse (e.g. horizon brightness) can be combined specifically.
+    #     Calls _get_poa_irradiances() to yield DNI and poa diffuse components (diffuse sky, diffuse horizon etc.)
+    #     For diffuse masking, uses shadow_angle_midpoint, i.e. the angle at half of the collector's slant height.
+    #     """
+    #     # TODO Daniel would be good to get your ideas about details on how to calculate dti
+    #     # TODO Make sure array virtual sensors exist: shadow_angle_midpoint, internal_shading_ratio, plant.ghi
+    #     # TODO Philip - conversion strategies should be 'consistent', i.e. if we apply inverse, then forward direction for a sensor, this should return the sensor value
+    #     #   - step 1:
+    #     #   - a) using gti (in same plane as array) --> apply dirint --> keep gti, calculate bti based on DNI, "normalize" shares for iffuse_iso + diffuse_circ + diffuse_horz
+    #     #   - b) using gti (in different plane than array) --> apply dirint --> use perez model
+    #     #   - step 2:
+    #     #   - calcuate reduction (masking, horizon) RELATIVE to measurement at the top of the collector --> we need to define the default settings here
+    #     #   - later:
+    #     #   - alternatively, we could think of implementing our own radiation conversion model to make this consistent, e.g. like https://www.sciencedirect.com/science/article/pii/S0038092X21000633,
+    #     #     for the solar community it would be help to have a very general radiation conversion algorithm for all possible measurement setups
+    #
+    #     # Plane-of-array irradiance components
+    #     dni, poa_diffuse_iso, poa_diffuse_circ, poa_diffuse_horiz = self._get_poa_irradiances()
+    #     bti = _get_beam_from_dni(self.plant, dni, self.tilt, self.azim)
+    #
+    #     # Diffuse masking
+    #     if self.use_diffuse_masking:
+    #         # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.shading.sky_diffuse_passias.html
+    #         iso_blocked = pv.shading.sky_diffuse_passias(masking_angle=self.array.shadow_angle_midpoint.m_as('deg'))
+    #         poa_diffuse_iso *= np.ones_like(poa_diffuse_iso) - iso_blocked
+    #         # TODO Philip - This calculation is NOT correct, it does not take the tilt angle of the array into account!
+    #     dti = poa_diffuse_iso
+    #
+    #     # Circumsolar diffuse
+    #     if self.treat_circumsolar_as_diffuse:
+    #         dti += poa_diffuse_circ
+    #     else:  # treat circumsolar as beam
+    #         bti += poa_diffuse_circ
+    #
+    #     # Beam shading
+    #     if self.use_beam_shading:
+    #         bti *= np.ones_like(bti) - self.array.internal_shading_ratio.m_as('dimensionless')
+    #
+    #     # Horizon brightness
+    #     if self.horizon_brightness_strategy == 'ignore':
+    #         pass
+    #     else:
+    #         dti += poa_diffuse_horiz
+    #
+    #     # Ground diffuse
+    #     # TODO Philip - these models need to be consistent with the transposition model - I would include the options
+    #     #  - a) ground reflection as in Perez
+    #     #  - b) ignore ground reflection (substract this from the diffuse irradiance?)
+    #     #  - b) correct ground reflection (with view factor from sensors versus towards ground)
+    #     if self.ground_diffuse_strategy == 'ignore':
+    #         pass
+    #     elif self.ground_diffuse_strategy == 'ghi':
+    #         if self.plant.ghi is None:
+    #             raise VirtualSensorCalculationError(
+    #                 'Calculating array irradiances with strategy "ghi" requires plant.ghi to be not None.')
+    #             # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.get_ground_diffuse.html
+    #         dti += pv.irradiance.get_ground_diffuse(surface_tilt=self.tilt,
+    #                                                 ghi=self.plant.ghi.m_as('W m**-2'),
+    #                                                 albedo=self.ground_albedo)
+    #     else:
+    #         raise NotImplementedError
+    #
+    #     gti = bti + dti
+    #     return gti, bti, dti
+
+    # To be uncommented, once radiation conversion for Arrays is implemented.
+    # def _get_poa_irradiances(self):
+    #     """Calculates in-plane radiation components from array radiation input sensors in_global, in_beam, in_diffuse,
+    #     in_dni. Returns tilted in-plane (poa, plane-of-array) irradiance components for DNI, sky and ground diffuse.
+    #     Returns
+    #     -------
+    #     rd_dni : numeric array
+    #       DNI (Direct Normal Irradiance) in W/m².
+    #     rd_poa_diffuse_sky : numeric array
+    #       Plane-of-array (poa) in-plane diffuse irradiance from the sky in W/m².
+    #     rd_poa_diffuse_ground : numeric array
+    #       Plane-of-array (poa) in-plane diffuse irradiance from the ground in W/m².
+    #
+    #     Note:
+    #     -----
+    #     Does not take beam shading and diffuse masking of the array into account.
+    #     Logic is described in https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+    #     """
+    #
+    #     glob, beam, diff, dni = self.unpack_radiations()
+    #     is_glob_horizontal, is_beam_horizontal, is_diff_horizontal = self.is_horizontal()
+    #
+    #     # no radiation inputs
+    #     if self.input_pattern == '0000':
+    #         dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = None, None, None, None
+    #     # global only
+    #     elif self.input_pattern == '1000':
+    #         if is_glob_horizontal:
+    #             # Input glob is ghi
+    #             dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = self._get_poa_from_ghi(glob)
+    #         else:
+    #             # Input glob is some gti: inverse decomposition
+    #             raise NotImplementedError
+    #             # tilt, azim = _get_sensor_orientation(array._in_glob)
+    #             # dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz = _get_poa_from_gti(plant, glob, tilt, azim)
+    #     else:
+    #         # TODO implement more tilted radiation strategies here
+    #         raise NotImplementedError
+    #
+    #     return dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz
+
+    # To be uncommented, once radiation conversion for Arrays is implemented.
+    # def _get_poa_from_ghi(self, ghi):
+    #     # TODO add docstring
+    #     # Calculates plane-of-array radiation components from global horizontal irradiance / measurement.
+    #     # Combines decomposition (dirindex) and transposition (Perez)
+    #     # Returns plane-of-array irradiance, i.e. does not take beam shading and diffuse masking into account.
+    #     # Returns: DNI, isotropic diffuse, circumsolar diffuse, horizon brightness radiations, all in W/m²
+    #
+    #     dni = _get_dni_from_ghi(self.plant, ghi)
+    #     bhi = _get_beam_from_dni(self.plant, dni)
+    #     dhi = ghi - bhi
+    #     poa_diff_iso, poa_diff_circ, poa_diff_horiz = self._get_poadiffuse_from_dhi(dhi, dni)
+    #     return dni, poa_diff_iso, poa_diff_circ, poa_diff_horiz
+
+    # To be uncommented, once radiation conversion for Arrays is implemented.
+    # def _get_poa_from_gti(self, gti):
+    #     # TODO add docstring
+    #     # Calculates plane-of-array radiation components from global tilted irradiance / measurement.
+    #     raise NotImplementedError
+    #     # tilt, azim = _get_sensor_orientation(array.in_global)
+    #     # gti_dirint
+
+    # To be uncommented, once radiation conversion for Arrays is implemented.
+    # def _get_poadiffuse_from_dhi(self, dhi, dni):
+    #     # TODO add docstring
+    #     # dhi, dni : array-like in W/m²
+    #     # Returns:
+    #     # --------
+    #     # poa_diff_iso : numeric
+    #     #   Tilted / poa isotropic diffuse radiation, in W/m²
+    #     # poa_diff_circ : numeric
+    #     #   Tilted / poa circumsolar radiation, in W/m²
+    #     # poa_diff_horiz : numeric
+    #     #   Tilted /poa horizon brightness radiation, in W/m²
+    #     # Transposition: Calculates sky diffuse irradiance in plane of array from global and diffuse horizontal.
+    #     # This implementation uses the Perez method:
+    #     # https://pvlib-python.readthedocs.io/en/stable/reference/generated/pvlib.irradiance.perez.html
+    #     # case [f] in design https://gitlab.com/sunpeek/sunpeek/-/issues/128/
+    #     # TODO Make sure the necessary sensors like plant.sun_apparent_zenit, plant.rel_airmass exist / not None
+    #
+    #     diffuse = pv.irradiance.perez(surface_tilt=self.tilt,
+    #                                   surface_azimuth=self.azim,
+    #                                   dhi=dhi,
+    #                                   dni=dni,
+    #                                   dni_extra=self.plant.rd_dni_extra.m_as('W m**-2'),
+    #                                   solar_zenith=self.plant.sun_apparent_zenith.m_as('deg'),
+    #                                   solar_azimuth=self.plant.sun_azimuth.m_as('deg'),
+    #                                   airmass=self.plant.rel_airmass.m_as(''),
+    #                                   return_components=True)
+    #     return diffuse['isotropic'], diffuse['circumsolar'], diffuse['horizon']
 
 ## old stuff
 # pvlib surfaces (for Array definition)
 # https://pvlib-python.readthedocs.io/en/stable/_modules/pvlib/irradiance.html?highlight=surface_albedos
 # SURFACE_ALBEDOS = {'urban': 0.18,
 #                    'grass': 0.20,
 #                    'fresh grass': 0.26,
```

## sunpeek/db_utils/crud.py

```diff
@@ -1,10 +1,14 @@
+import datetime
+from typing import Union
+
 from sqlalchemy.orm import Session
+from sqlalchemy import or_, and_
 import sunpeek.components as cmp
-from typing import Union
+from sunpeek.common.errors import SensorNotFoundError
 
 
 def get_plants(session: Session, plant_id: int=None, plant_name: str=None):
     """
     Gets a plant by name from the database, or all plants if no `plant_name` or `plant_id` parameter is supplied
     Parameters
     ----------
@@ -45,35 +49,39 @@
     """
 
     if isinstance(component, str):
         component = cmp.__dict__[component]
 
     qry = session.query(component)
     if id is not None:
+        obj = qry.filter(component.id == id).one()
+        if plant_id is not None and obj.plant_id != plant_id:
+            raise SensorNotFoundError(f"{component.__name__} with id {id} has a plant_id that does not match the passed "
+                                      f"plant_id. This means that the component is associated with a different plant or "
+                                      f"no plant, probably an incorrect id or plant_id was passed.")
         return qry.filter(component.id == id).one()
     if plant_id is not None:
-        qry = qry.join(cmp.Plant).filter(cmp.Plant.id == plant_id)
+        qry = qry.filter(component.plant_id == plant_id)
     if name is not None and component != cmp.Sensor:
         return qry.filter(component.name == name).one()
     elif name is not None and component == cmp.Sensor:
         return qry.filter(component.raw_name == name).one()
     if plant_name is not None:
-        qry = qry.join(cmp.Plant).filter(cmp.Plant.name == plant_name)
+        qry = qry.join(cmp.Plant, component.plant_id == cmp.Plant.id).filter(cmp.Plant.name == plant_name)
     return qry.all()
 
 
 def get_sensors(session: Session, id: int = None, raw_name: str = None, plant_id: int=None, plant_name: str=None):
     """
     Get all sensors, all sensors of a given plant, or a specific sensor. Note, parameters have the following precedence:
     id, name, plant_id, plant_name. So if a component name is given, all further parameters are ignored
 
     Parameters
     ----------
     session
-    component: An instance of a subclass of cmp.Component
     id
     raw_name
     plant_id
     plant_name
 
     Returns
     -------
@@ -135,7 +143,25 @@
     Returns
     -------
     The updated object after commit to the database (this may have had modifications made by database side logic
     """
 
     session.delete(component)
     session.commit()
+
+
+def get_operational_events(session: Session, event_id=None, plant_id=None, search_start=None, search_end=None):
+    if search_start is None and search_end is None:
+        return get_components(session, cmp.OperationalEvent, id=event_id, plant_id=plant_id)
+
+    if search_end is None:
+        search_end = datetime.datetime(9999, 1, 1, 0, 0)
+    if search_start is None:
+        search_end = datetime.datetime(1900, 1, 1, 0, 0)
+
+    events = session.query(cmp.OperationalEvent).join(cmp.Plant).where(cmp.Plant.id == plant_id).where(
+        or_(
+            and_(cmp.OperationalEvent.event_start >= search_start, cmp.OperationalEvent.event_start <= search_end),
+            and_(cmp.OperationalEvent.event_end >= search_start, cmp.OperationalEvent.event_end <= search_end),
+            and_(cmp.OperationalEvent.event_start <= search_end, cmp.OperationalEvent.event_end >= search_start)
+        )).all()
+    return events
```

## sunpeek/db_utils/db_data_operations.py

```diff
@@ -1,409 +1,443 @@
-import asyncio
-from io import BytesIO
-import sys, os
-import psycopg2
-from psycopg2 import OperationalError, sql
-import psycopg2.extras as extras
-import pandas as pd
-import time
-import datetime
-from sqlalchemy import text, MetaData, Table, Column, Boolean, String, Float, DateTime, inspect
-
-from sunpeek.common.utils import hit_logger
-from sunpeek.db_utils import DATETIME_COL_NAME
-
-
-# default page size for database execute - this can be very large which should improve performance
-DEFAULT_PAGE_SIZE = 100000
-
-
-def show_psycopg2_exception(err):
-    """Prints errors ocurred during postgresql db interactions.
-
-    Parameters
-    ----------
-    err
-        Error catched in program execution regarding PostgreSQL operations.
-
-    Notes
-    -----
-    This code is part of the article by Learner CARES in 
-    https://medium.com/analytics-vidhya/part-4-pandas-dataframe-to-postgresql-using-python-8ffdb0323c09
-    Used for debugging and logging purposes.
-
-    """
-    # get details about the exception
-    err_type, err_obj, traceback = sys.exc_info()
-    # get the line number when exception occured
-    line_n = traceback.tb_lineno
-    hit_logger.error(f"\n[psycopg2_exception] ERROR: {err} on line number: {line_n}")
-    hit_logger.error(f"[psycopg2_exception] traceback: {traceback} -- type: {err_type}")
-    hit_logger.error(f"\n[psycopg2_exception] extensions.Diagnostics: {err.diag}")
-    hit_logger.error(f"[psycopg2_exception] pgerror: {err.pgerror}")
-    hit_logger.error(f"[psycopg2_exception] pgcode: {err.pgcode} \n")
-
-
-# connection methods
-
-
-def get_db_connection_dict():
-    try:
-        port = os.environ.get('HIT_DB_HOST', 'localhost:5432').split(':')[1]
-    except IndexError:
-        port = 5432
-
-    conn_params_dict = {
-        "host": os.environ.get('HIT_DB_HOST', 'localhost:5432').split(':')[0],
-        "port": port,
-        "database": os.environ.get('HIT_DB_NAME', 'harvestit'),
-        "user": os.environ.get('HIT_DB_USER'),
-        "password": os.environ.get('HIT_DB_PW')
-    }
-
-    return conn_params_dict
-
-
-def get_db_connection():
-    """Init db connections
-    """
-    db_connection = connect(get_db_connection_dict())
-    if db_connection is None:
-        raise ConnectionError('Failed to connect to to database')
-    return db_connection
-
-
-def connect(conn_params_dict):
-    """Connects to an specific database.
-
-    Parameters
-    ----------
-    conn_params_dict : `dict` 
-        A dictionary containing the user credentials for the conection,
-        the host and the name of the desired database.
-
-    Returns
-    -------
-    connection : `psycopg2_connection`
-        Established connection object to database.
-    """
-    # TODO del
-    connection = None
-    try:
-        hit_logger.info('[connect] Connecting to the PostgreSQL...........')
-        connection = psycopg2.connect(**conn_params_dict)
-        hit_logger.info("[connect] Connected !")
-
-    except OperationalError as err:
-        hit_logger.exception(err)
-        # passing exception to function
-        show_psycopg2_exception(err)
-        # set the connection to 'None' in case of error
-        connection = None
-    return connection
-
-
-def disconnect_db(connection):
-    """Closes the connection with database.
-
-    Parameters
-    ----------
-    connection : `psycopg2_connection`
-        Connection object to database.
-    """
-    connection.close()
-    hit_logger.info("[disconnect_db] HIT DB connection closed!")
-
-
-# util methods
-def db_table_exists(engine, table_name):
-    """
-    Checks the existence of the provided table in the database. Used for initialization of dynamic table creation.
-
-    Parameters
-    ----------
-    engine : `sqlalchemy engine object`
-        Connection object to database.
-
-    table_name : `str`
-        Table name to check for.
-
-    Returns
-    -------
-    True/False : `bool`
-        True if table exists in database, False otherwise.
-    """
-
-    insp = inspect(engine)
-    return insp.has_table(table_name)
-
-
-def get_sensor_data(connection, sensor_names, table_name, start_timestamp, end_timestamp=None):
-    """Retrieves the data from a sensor in the specified table. It can return both a single value or a range depending on the timestamps provided.
-    
-    Parameters
-    ----------
-    connection : `psycopg2_connection`
-        Connection object to database.
-    
-    sensor_names : `str`, `list`
-        Name of the sensor(s) to retrieve the data.
-    
-    table_name : `str`
-        Name of the table where the sensor data is stored.
-
-    start_timestamp,`datetime.datetime` or `str`
-        Timestamp of the data entry.
-    
-    end_timestamp, optional `datetime.datetime` or `str`, optional
-        Timestamp to retrieve a range of values if provided.
-    
-    """
-
-    hit_logger.info(
-        f"[get_sensor_data] Getting data for sensor \"{sensor_names}\" in \"{table_name}\" table")
-
-    # SQL query to execute
-    if isinstance(sensor_names, str):
-        sensor_names = [sensor_names]
-
-    fields = [sql.Identifier(col.lower()) for col in sensor_names]
-    fields = [sql.Identifier(DATETIME_COL_NAME)] + fields
-
-    if end_timestamp:
-        sql_object = sql.SQL(
-            """SELECT {fields} FROM {tb_name} WHERE {col_name} BETWEEN {start_tmstmp} AND {end_tmstmp} ORDER BY {order_col_name} ASC"""
-        ).format(
-            fields=sql.SQL(',').join(fields),
-            tb_name=sql.Identifier(table_name),
-            col_name=sql.Identifier(DATETIME_COL_NAME),
-            start_tmstmp=sql.Literal(start_timestamp),
-            end_tmstmp=sql.Literal(end_timestamp),
-            order_col_name=sql.Identifier(DATETIME_COL_NAME)
-        )
-    else:
-        # TODO Does not work because sensor_names are list -> TypeError
-        # query for queh just start timestamp is supplied
-        sql_object = sql.SQL(
-            """SELECT {fields} FROM {tb_name} WHERE {col_name} = {start_tmstmp} ORDER BY {order_col_name} ASC"""
-        ).format(
-            fields=sql.SQL(',').join([
-                sql.Identifier(DATETIME_COL_NAME),
-                sql.Identifier(sensor_names),
-            ]),
-            tb_name=sql.Identifier(table_name),
-            col_name=sql.Identifier(DATETIME_COL_NAME),
-            start_tmstmp=sql.Literal(start_timestamp),
-            order_col_name=sql.Identifier(DATETIME_COL_NAME)
-        )
-
-    cursor = connection.cursor()
-    try:
-        t_start = time.time()
-        cursor.execute(sql_object)
-        hit_logger.info(f"[get_sensor_data] Data retrieved in {time.time()-t_start}")
-
-        query_data = cursor.fetchall()
-        sensor_data = pd.DataFrame(list(query_data), columns=[DATETIME_COL_NAME]+sensor_names)
-        sensor_data = sensor_data.set_index(DATETIME_COL_NAME, drop=True)
-
-        # close the cursor object to prevent memory leaks
-        cursor.close()
-        return sensor_data
-
-    except (Exception, psycopg2.DatabaseError) as err:
-        hit_logger.error("[get_sensor_data] Error in get_sensor_data()")
-        # pass exception to function
-        if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
-            show_psycopg2_exception(err)
-        cursor.close()
-
-
-# TODO rename, align with execute batch, insert_series
-def update_virtual_sensor_data(connection,
-                               sensor_data: pd.Series,
-                               table,
-                               # plant_name: str,
-                               # sensor_raw_name: str,
-                               page_size=DEFAULT_PAGE_SIZE):
-
-    """Saves the re calculated data of a virtual sensor in the corresponsing raw_table.
-
-    Is different from execute_batch() in that it does not batch-erase overlapping data
-
-    """
-
-    hit_logger.info(f"[update_virtual_sensor_data] Inserting data into \"{table}\" table")
-
-    fld_name = sensor_data.name
-
-    df = sensor_data.to_frame()
-    df = df.rename_axis(DATETIME_COL_NAME).reset_index()
-    df = df.reindex(columns=df.columns[::-1])
-    tpls = df.to_records(index=False).tolist()
-    print(tpls[0])
-    hit_logger.info(f"[execute_batch] Tuple to save example:\n{tpls[0]}")
-
-
-    # TODO BUG use upsert operation instead: https://wiki.postgresql.org/wiki/UPSERT
-    # https://www.postgresqltutorial.com/postgresql-tutorial/postgresql-upsert/
-    # https://www.psycopg.org/docs/usage.html
-    # This code adds number of sensor_data rows to the database
-
-    # original
-    insert_str = sql.SQL("UPDATE {} SET {} = {} WHERE {} = {}").format(
-        sql.Identifier(table),
-        sql.Identifier(fld_name),
-        sql.Placeholder(),
-        sql.Identifier(DATETIME_COL_NAME),
-        sql.Placeholder()
-    )
-    # insert_str = sql.SQL("UPDATE {} SET {} = {} WHERE {} = {}").format(
-    #     sql.Identifier(table),
-    #     sql.Identifier(sensor_data.columns[1]),
-    #     sql.Placeholder(sensor_data.iloc[:,1]),
-    #     sql.Identifier("ds"),
-    #     sql.Placeholder(sensor_data.iloc[:,0])
-    # )
-    # https://stackoverflow.com/questions/60845779/psycopg2-how-to-insert-and-update-on-conflict-using-psycopg2-with-python
-    # insert_sql = '''
-    #     INSERT INTO tablename (col1, col2, col3, col4)
-    #     VALUES (%s, %s, %s, %s)
-    #     ON CONFLICT (col1) DO UPDATE SET
-    #     (col2, col3, col4) = (EXCLUDED.col2, EXCLUDED.col3, EXCLUDED.col4);
-    # '''
-
-    cursor = connection.cursor()
-
-    # cursor.rowcount
-    # cursor.execute("""
-    #     UPDATE table_name
-    #     SET z = codelist.z
-    #     FROM codelist
-    #     WHERE codelist.id = vehicle.id;
-    #     """)
-    # cursor.rowcount
-
-    try:
-        extras.execute_batch(cursor, insert_str, tpls, page_size=page_size)
-        # perhaps: cursor.execute(insert_str, tpls)
-        hit_logger.info("[save_virtual_sensor_data] Virtual sensor data inserted successfully!")
-        connection.commit()
-        return True
-    except (Exception, psycopg2.DatabaseError, OperationalError) as err:
-        hit_logger.error(f"[save_virtual_sensor_data] Error in save_virtual_sensor_data()")
-        hit_logger.exception(err)
-        # pass exception to function
-        if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
-            show_psycopg2_exception(err)
-        cursor.close()
-        connection.rollback()
-        return False
-
-
-def create_table_dynamic(engine, table_name, types_dict):
-    """
-    Creates a table dynamically based on the keys and datatypes from the provided dictionary
-
-    Params
-    ------
-    `sqlalchemy engine object` engine: Connection object to database.
-    `str` table_name: A string to name the db table.
-    `dict` data_dict: Dictionary containing all the data to save.
-    """
-
-    hit_logger.info(f"[create_table_dynamic] Creating table {table_name} dynamically...")
-
-    db_types = {bool: Boolean,
-                float: Float,
-                str: String,
-                datetime.datetime: DateTime(timezone=True)}
-
-    metadata_obj = MetaData()
-
-    table = Table(table_name, metadata_obj)
-    table.append_column(Column(DATETIME_COL_NAME, db_types[datetime.datetime]))
-
-    try:
-        for key, value in types_dict.items():
-            db_key = key.strip()
-            table.append_column(Column(db_key, db_types[value]))
-
-        table.create(engine)
-
-        mk_hypertable_query = text("SELECT create_hypertable(:tn, :ds, chunk_time_interval => INTERVAL '1 month');")
-        with engine.connect() as connection:
-            connection.execute(mk_hypertable_query, tn=table_name, ds=DATETIME_COL_NAME)
-
-        hit_logger.info(f"[CTD] Table {table_name} created!")
-
-    except OperationalError as err:
-        # pass exception to function
-        show_psycopg2_exception(err)
-
-
-def delete_overlapping_data(connection, table_name, overlapping_boundaries):
-    """
-    Deletes all the entries in the DB in case there is overlapping with the incoming data.
-    
-    Returns
-    -------
-    overlapping : Bool
-        Either overlapping entries were deleted in the db or not.
-    """
-
-    # overlaping handling
-    # 1. Run delete command on database for entries inside the overlapping range
-    # 2. This returns the number of rows affected, 0 if no entries are inside the range
-    # 3. Return a boolean value reporting if the overlapping delete was carried out.
-
-    overlapping = False
-    left_boundary, right_boundary = overlapping_boundaries
-
-    cursor = connection.cursor()
-    rows_deleted = 0
-    try:
-
-        delete_str = sql.SQL("DELETE FROM {} WHERE {} BETWEEN {} AND {}").format(
-            sql.Identifier(table_name),
-            sql.Identifier(DATETIME_COL_NAME),
-            sql.Literal(left_boundary),
-            sql.Literal(right_boundary)
-        )
-
-        cursor.execute(delete_str)
-        rows_deleted = cursor.rowcount
-
-        if rows_deleted > 0:
-            hit_logger.warning(
-                f"[delete_overlapping_data] Overlapping detected! Deleting data between the range [{left_boundary}, {right_boundary}] in the {table_name} table")
-            hit_logger.warning(f"[delete_overlapping_data] Deleted overlapping entries: {rows_deleted}")
-            overlapping = True
-            return overlapping
-        else:
-            hit_logger.info(f"[delete_overlapping_data] The incoming data does not overlap with records in the db.")
-            return overlapping
-
-    except (Exception, psycopg2.DatabaseError, OperationalError) as err:
-        hit_logger.exception(err)
-        # pass exception to function
-        if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
-            show_psycopg2_exception(err)
-        cursor.close()
-        connection.rollback()
-        return False
-
-
-def df_to_db(connection, datafrm, table):
-    cursor = connection.cursor()
-    try:
-        fio = BytesIO()
-        datafrm.to_csv(fio, sep=';', header=False)
-        fio.seek(0)
-        # Use psychopg2 cursor.copy_from method to send data from CSV buffer and perform copy database side.
-        cursor.copy_from(fio, table, sep=';', null='', columns=[datafrm.index.name]+[col.lower() for col in datafrm.columns])
-        cursor.close()
-        return True
-    except Exception as ex:
-        hit_logger.error(ex)
-        cursor.close()
-        return False
+# from io import BytesIO
+# import sys, os
+# import psycopg2
+# from psycopg2 import OperationalError, sql
+# import psycopg2.extras as extras
+# import pandas as pd
+# import time
+# import datetime
+# from sqlalchemy import text, MetaData, Table, Column, Boolean, String, Float, DateTime, inspect
+#
+# from sunpeek.common.utils import sp_logger
+# from sunpeek.db_utils import DATETIME_COL_NAME
+#
+#
+# # default page size for database execute - this can be very large which should improve performance
+# DEFAULT_PAGE_SIZE = 100000
+#
+#
+# def show_psycopg2_exception(err):
+#     """Prints errors ocurred during postgresql db interactions.
+#
+#     Parameters
+#     ----------
+#     err
+#         Error catched in program execution regarding PostgreSQL operations.
+#
+#     Notes
+#     -----
+#     This code is part of the article by Learner CARES in
+#     https://medium.com/analytics-vidhya/part-4-pandas-dataframe-to-postgresql-using-python-8ffdb0323c09
+#     Used for debugging and logging purposes.
+#
+#     """
+#     # get details about the exception
+#     err_type, err_obj, traceback = sys.exc_info()
+#     # get the line number when exception occured
+#     line_n = traceback.tb_lineno
+#     sp_logger.error(f"\n[psycopg2_exception] ERROR: {err} on line number: {line_n}")
+#     sp_logger.error(f"[psycopg2_exception] traceback: {traceback} -- type: {err_type}")
+#     sp_logger.error(f"\n[psycopg2_exception] extensions.Diagnostics: {err.diag}")
+#     sp_logger.error(f"[psycopg2_exception] pgerror: {err.pgerror}")
+#     sp_logger.error(f"[psycopg2_exception] pgcode: {err.pgcode} \n")
+#
+#
+# # connection methods
+#
+#
+# def get_db_connection_dict():
+#     try:
+#         port = os.environ.get('HIT_DB_HOST', 'localhost:5432').split(':')[1]
+#     except IndexError:
+#         port = 5432
+#
+#     conn_params_dict = {
+#         "host": os.environ.get('HIT_DB_HOST', 'localhost:5432').split(':')[0],
+#         "port": port,
+#         "database": os.environ.get('HIT_DB_NAME', 'harvestit'),
+#         "user": os.environ.get('HIT_DB_USER'),
+#         "password": os.environ.get('HIT_DB_PW')
+#     }
+#
+#     return conn_params_dict
+#
+#
+# def get_db_connection():
+#     """Init db connections
+#     """
+#     db_connection = connect(get_db_connection_dict())
+#     if db_connection is None:
+#         raise ConnectionError('Failed to connect to to database')
+#     return db_connection
+#
+#
+# def connect(conn_params_dict):
+#     """Connects to an specific database.
+#
+#     Parameters
+#     ----------
+#     conn_params_dict : `dict`
+#         A dictionary containing the user credentials for the conection,
+#         the host and the name of the desired database.
+#
+#     Returns
+#     -------
+#     connection : `psycopg2_connection`
+#         Established connection object to database.
+#     """
+#
+#     try:
+#         sp_logger.info('[connect] Connecting to the PostgreSQL...........')
+#         connection = psycopg2.connect(**conn_params_dict)
+#         sp_logger.info("[connect] Connected !")
+#
+#     except OperationalError as err:
+#         sp_logger.exception(err)
+#         # passing exception to function
+#         show_psycopg2_exception(err)
+#         # set the connection to 'None' in case of error
+#         connection = None
+#     return connection
+#
+#
+# def disconnect_db(connection):
+#     """Closes the connection with database.
+#
+#     Parameters
+#     ----------
+#     connection : `psycopg2_connection`
+#         Connection object to database.
+#     """
+#     connection.close()
+#     sp_logger.info("[disconnect_db] HIT DB connection closed!")
+#
+#
+# # util methods
+# def db_table_exists(engine, table_name):
+#     """
+#     Checks the existence of the provided table in the database. Used for initialization of dynamic table creation.
+#
+#     Parameters
+#     ----------
+#     engine : `sqlalchemy engine object`
+#         Connection object to database.
+#
+#     table_name : `str`
+#         Table name to check for.
+#
+#     Returns
+#     -------
+#     True/False : `bool`
+#         True if table exists in database, False otherwise.
+#     """
+#
+#     insp = inspect(engine)
+#     return insp.has_table(table_name)
+#
+#
+# def get_sensor_data(connection, sensor_names, table_name, start_timestamp, end_timestamp=None):
+#     """Retrieves the data from a sensor in the specified table. It can return both a single value or a range depending on the timestamps provided.
+#
+#     Parameters
+#     ----------
+#     connection : `psycopg2_connection`
+#         Connection object to database.
+#
+#     sensor_names : `str`, `list`
+#         Name of the sensor(s) to retrieve the data.
+#
+#     table_name : `str`
+#         Name of the table where the sensor data is stored.
+#
+#     start_timestamp,`datetime.datetime` or `str`
+#         Timestamp of the data entry.
+#
+#     end_timestamp, optional `datetime.datetime` or `str`, optional
+#         Timestamp to retrieve a range of values if provided.
+#
+#     """
+#
+#     sp_logger.debug(f"[get_sensor_data] Getting data for sensor \"{sensor_names}\" in \"{table_name}\" table")
+#
+#     # SQL query to execute
+#     if isinstance(sensor_names, str):
+#         sensor_names = [sensor_names]
+#
+#     fields = [sql.Identifier(col.lower()) for col in sensor_names]
+#     fields = [sql.Identifier(DATETIME_COL_NAME)] + fields
+#
+#     if end_timestamp:
+#         sql_object = sql.SQL(
+#             """SELECT {fields} FROM {tb_name} WHERE {col_name} BETWEEN {start_tmstmp} AND {end_tmstmp} ORDER BY {order_col_name} ASC"""
+#         ).format(
+#             fields=sql.SQL(',').join(fields),
+#             tb_name=sql.Identifier(table_name),
+#             col_name=sql.Identifier(DATETIME_COL_NAME),
+#             start_tmstmp=sql.Literal(start_timestamp),
+#             end_tmstmp=sql.Literal(end_timestamp),
+#             order_col_name=sql.Identifier(DATETIME_COL_NAME)
+#         )
+#     else:
+#         # query for queh just start timestamp is supplied
+#         sql_object = sql.SQL(
+#             """SELECT {fields} FROM {tb_name} WHERE {col_name} = {start_tmstmp} ORDER BY {order_col_name} ASC"""
+#         ).format(
+#             fields=sql.SQL(',').join([
+#                 sql.Identifier(DATETIME_COL_NAME),
+#                 sql.Identifier(sensor_names),
+#             ]),
+#             tb_name=sql.Identifier(table_name),
+#             col_name=sql.Identifier(DATETIME_COL_NAME),
+#             start_tmstmp=sql.Literal(start_timestamp),
+#             order_col_name=sql.Identifier(DATETIME_COL_NAME)
+#         )
+#
+#     cursor = connection.cursor()
+#     try:
+#         t_start = time.time()
+#         cursor.execute(sql_object)
+#         query_data = cursor.fetchall()
+#         sp_logger.debug(f"[get_sensor_data] Data retrieved in {time.time() - t_start}")
+#
+#         sensor_data = pd.DataFrame(list(query_data), columns=[DATETIME_COL_NAME]+sensor_names)
+#         sensor_data = sensor_data.set_index(DATETIME_COL_NAME, drop=True)
+#
+#         # close the cursor object to prevent memory leaks
+#         cursor.close()
+#         return sensor_data
+#
+#     except (Exception, psycopg2.DatabaseError) as err:
+#         sp_logger.error("[get_sensor_data] Error in get_sensor_data()")
+#         # pass exception to function
+#         if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
+#             show_psycopg2_exception(err)
+#         cursor.close()
+#
+#
+# def update_virtual_sensor_data(connection,
+#                                sensor_data: pd.Series,
+#                                table,
+#                                # plant_name: str,
+#                                # sensor_raw_name: str,
+#                                page_size=DEFAULT_PAGE_SIZE):
+#
+#     """Saves the re calculated data of a virtual sensor in the corresponsing raw_table.
+#
+#     Is different from execute_batch() in that it does not batch-erase overlapping data
+#
+#     """
+#
+#     sp_logger.debug(f"[update_virtual_sensor_data] Inserting data into \"{table}\" table")
+#
+#     fld_name = sensor_data.name
+#
+#     df = sensor_data.to_frame()
+#     df = df.rename_axis(DATETIME_COL_NAME).reset_index()
+#     df = df.reindex(columns=df.columns[::-1])
+#     tpls = df.to_records(index=False).tolist()
+#     print(tpls[0])
+#     sp_logger.debug(f"[execute_batch] Tuple to save example:\n{tpls[0]}")
+#
+#     # original
+#     insert_str = sql.SQL("UPDATE {} SET {} = {} WHERE {} = {}").format(
+#         sql.Identifier(table),
+#         sql.Identifier(fld_name),
+#         sql.Placeholder(),
+#         sql.Identifier(DATETIME_COL_NAME),
+#         sql.Placeholder()
+#     )
+#     # insert_str = sql.SQL("UPDATE {} SET {} = {} WHERE {} = {}").format(
+#     #     sql.Identifier(table),
+#     #     sql.Identifier(sensor_data.columns[1]),
+#     #     sql.Placeholder(sensor_data.iloc[:,1]),
+#     #     sql.Identifier("ds"),
+#     #     sql.Placeholder(sensor_data.iloc[:,0])
+#     # )
+#     # https://stackoverflow.com/questions/60845779/psycopg2-how-to-insert-and-update-on-conflict-using-psycopg2-with-python
+#     # insert_sql = '''
+#     #     INSERT INTO tablename (col1, col2, col3, col4)
+#     #     VALUES (%s, %s, %s, %s)
+#     #     ON CONFLICT (col1) DO UPDATE SET
+#     #     (col2, col3, col4) = (EXCLUDED.col2, EXCLUDED.col3, EXCLUDED.col4);
+#     # '''
+#
+#     cursor = connection.cursor()
+#
+#     # cursor.rowcount
+#     # cursor.execute("""
+#     #     UPDATE table_name
+#     #     SET z = codelist.z
+#     #     FROM codelist
+#     #     WHERE codelist.id = vehicle.id;
+#     #     """)
+#     # cursor.rowcount
+#
+#     try:
+#         extras.execute_batch(cursor, insert_str, tpls, page_size=page_size)
+#         # perhaps: cursor.execute(insert_str, tpls)
+#         sp_logger.debug("[save_virtual_sensor_data] Virtual sensor data inserted successfully!")
+#         connection.commit()
+#         return True
+#     except (Exception, psycopg2.DatabaseError, OperationalError) as err:
+#         sp_logger.error(f"[save_virtual_sensor_data] Error in save_virtual_sensor_data()")
+#         sp_logger.exception(err)
+#         # pass exception to function
+#         if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
+#             show_psycopg2_exception(err)
+#         cursor.close()
+#         connection.rollback()
+#         return False
+#
+#
+# def create_table_dynamic(session, table_name, types_dict):
+#     """
+#     Creates a table dynamically based on the keys and datatypes from the provided dictionary
+#
+#     Params
+#     ------
+#     `sqlalchemy engine object` engine: An sqlalchemy engine object used to connect to the database.
+#     `str` table_name: A string to name the db table.
+#     `dict` data_dict: Dictionary in the form {<name>: <python datatype>} for all columns to be created.
+#     """
+#
+#     sp_logger.info(f"[create_table_dynamic] Creating table {table_name} dynamically...")
+#
+#     db_types = {bool: Boolean,
+#                 float: Float,
+#                 str: String,
+#                 datetime.datetime: DateTime(timezone=True)}
+#
+#     metadata_obj = MetaData()
+#
+#     table = Table(table_name, metadata_obj)
+#     table.append_column(Column(DATETIME_COL_NAME, db_types[datetime.datetime]))
+#
+#     for key, value in types_dict.items():
+#         db_key = key.strip().lower()
+#         table.append_column(Column(db_key, db_types[value]))
+#
+#     try:
+#         table.create(session.get_bind())
+#
+#         # mk_hypertable_query = sql.SQL("SELECT create_hypertable({}, {}, chunk_time_interval => INTERVAL '1 month');"
+#         #                               "CREATE INDEX ix_time ON {tn} ({ds} DESC);")\
+#         #     .format(
+#         #         sql.Placeholder(),
+#         #         sql.Placeholder(),
+#         #         tn = sql.Identifier(table_name),
+#         #         ds = sql.Identifier(DATETIME_COL_NAME)
+#         #     )
+#
+#         mk_hypertable_query = sql.SQL("CREATE INDEX ix_time ON {tn} ({ds} DESC);").format(
+#                 tn = sql.Identifier(table_name),
+#                 ds = sql.Identifier(DATETIME_COL_NAME)
+#         )
+#
+#         con = session.get_bind().raw_connection()
+#         con.cursor().execute(mk_hypertable_query, (table_name, DATETIME_COL_NAME))
+#         con.commit()
+#         sp_logger.debug(f"[CTD] Table {table_name} created!")
+#
+#     except OperationalError as err:
+#         # pass exception to function
+#         session.rollback()
+#         show_psycopg2_exception(err)
+#         raise
+#
+#
+# def create_new_data_cols(engine, table_name, types_dict):
+#     """
+#     Compares a dictionary of column names against the columns already in the table called table_name, and creates any
+#     columns that are in the dictionary but not the table, using datatypes compatible with the python types provided.
+#     Parameters
+#     ----------
+#     `sqlalchemy engine object` engine:
+#         An sqlalchemy engine object used to connect to the database.
+#     `str` table_name: A string to name the db table.
+#     `dict` data_dict: Dictionary in the form {<name>: <python datatype>} for new columns to be created. Existing columns
+#       can be included, they will be ignored.
+#     """
+#     db_types = {bool: 'boolean',
+#                 float: 'double precision',
+#                 str: 'VARCHAR',
+#                 datetime.datetime: 'timestamp with time zone'}
+#
+#     metadata_obj = MetaData()
+#     raw_table = Table(table_name, metadata_obj, autoload_with=engine)
+#     new_cols = set([key.lower() for key in types_dict.keys()]) - set([col.name for col in raw_table.columns])
+#
+#     for key in new_cols:
+#         db_key = key.strip().lower()
+#         stmt = sql.SQL('ALTER TABLE {0} ADD COLUMN {1} {2}').format(sql.Identifier(raw_table.name),
+#                                                                     sql.Identifier(db_key),
+#                                                                     sql.SQL(db_types[types_dict[key]]))
+#         with engine.connect() as connection:
+#             connection.execute(stmt.as_string(engine.raw_connection().connection))
+#
+#
+# def delete_overlapping_data(connection, table_name, overlapping_boundaries):
+#     """
+#     Deletes all the entries in the DB in case there is overlapping with the incoming data.
+#
+#     Returns
+#     -------
+#     overlapping : Bool
+#         Either overlapping entries were deleted in the db or not.
+#     """
+#
+#     # overlaping handling
+#     # 1. Run delete command on database for entries inside the overlapping range
+#     # 2. This returns the number of rows affected, 0 if no entries are inside the range
+#     # 3. Return a boolean value reporting if the overlapping delete was carried out.
+#
+#     overlapping = False
+#     left_boundary, right_boundary = overlapping_boundaries
+#
+#     cursor = connection.cursor()
+#     rows_deleted = 0
+#     try:
+#
+#         delete_str = sql.SQL("DELETE FROM {} WHERE {} BETWEEN {} AND {}").format(
+#             sql.Identifier(table_name),
+#             sql.Identifier(DATETIME_COL_NAME),
+#             sql.Literal(left_boundary),
+#             sql.Literal(right_boundary)
+#         )
+#
+#         cursor.execute(delete_str)
+#         rows_deleted = cursor.rowcount
+#
+#         if rows_deleted > 0:
+#             sp_logger.warning(
+#                 f"[delete_overlapping_data] Overlapping detected! Deleting data between the range [{left_boundary}, {right_boundary}] in the {table_name} table")
+#             sp_logger.warning(f"[delete_overlapping_data] Deleted overlapping entries: {rows_deleted}")
+#             overlapping = True
+#             return overlapping
+#         else:
+#             sp_logger.debug(f"[delete_overlapping_data] The incoming data does not overlap with records in the db.")
+#             return overlapping
+#
+#     except (Exception, psycopg2.DatabaseError, OperationalError) as err:
+#         sp_logger.exception(err)
+#         # pass exception to function
+#         if isinstance(err, (psycopg2.DatabaseError, OperationalError)):
+#             show_psycopg2_exception(err)
+#         cursor.close()
+#         connection.rollback()
+#         return False
+#
+#
+# def df_to_db(connection, datafrm, table):
+#     cursor = connection.cursor()
+#     try:
+#         fio = BytesIO()
+#         datafrm.to_csv(fio, sep=';', header=False)
+#         fio.seek(0)
+#         # Use psychopg2 cursor.copy_from method to send data from CSV buffer and perform copy database side.
+#         cursor.copy_from(fio, table, sep=';', null='', columns=[datafrm.index.name]+[col.lower() for col in datafrm.columns])
+#         cursor.close()
+#         return True
+#     except Exception as ex:
+#         sp_logger.error(ex)
+#         cursor.close()
+#         return False
```

## sunpeek/db_utils/init_db.py

```diff
@@ -1,40 +1,55 @@
-import sqlalchemy
+import os
 from sqlalchemy_utils import database_exists, create_database
+from sqlalchemy import event
+from sqlalchemy.engine import Engine
+import alembic.config
 
 import sunpeek.components as cmp
 from sunpeek.common import utils
-import sunpeek.definitions
-
-db_url = utils.get_db_conection_string()
+from sunpeek.common.errors import DatabaseAlreadyExistsError
+import sunpeek.definitions.collector_types
+import sunpeek.definitions.fluid_definitions
 
 
 def init_db():
-    assert not database_exists(db_url), f"Database {db_url.split('/')[-1]} already exists, please set HIT_DB_NAME to a " \
-                                        f"database doesn't exist yet, it will be created for you"
-
-    utils.hit_logger.info(f'[init_db] Attempting to setup DB on {db_url}')
-    engine = sqlalchemy.create_engine('/'.join(utils.get_db_conection_string().split('/')[:-1]))
-    with engine.begin() as con:
-        le = len(list(con.execute(sqlalchemy.text("select extname from pg_extension where extname='timescaledb';"))))
-        assert le == 1, "Timescaledb extension must be installed and available"
-    engine.dispose()
+    db_url = utils.get_db_conection_string()
+    if database_exists(db_url):
+        raise DatabaseAlreadyExistsError(f"Database {db_url.split('/')[-1]} already exists, please set HIT_DB_NAME to "
+                                         f"a database doesn't exist yet, it will be created for you")
+
+    utils.sp_logger.info(f'[init_db] Attempting to setup DB {os.environ.get("HIT_DB_NAME", "harvestit")} on '
+                         f'{os.environ.get("HIT_DB_HOST", "localhost:5432")}')
+    # engine = sqlalchemy.create_engine('/'.join(utils.get_db_conection_string().split('/')[:-1]))
+    # engine.dispose()
 
     create_database(db_url)
 
     cmp.make_tables(utils.db_engine)
 
-    with utils.S() as session:
-        #Add collector types
+    with utils.S.begin() as session:
+        # Add collector types
         for item in sunpeek.definitions.collector_types.all_definitions:
             session.add(item)
 
-        #Add fluids
+        # Add fluids
         for item in sunpeek.definitions.fluid_definitions.all_definitions:
             session.add(item)
 
         session.commit()
         session.expunge_all()
 
+    os.chdir(os.path.join(os.path.dirname(os.path.realpath(__file__)), '../..'))
+    alembicArgs = ['--raiseerr', 'stamp', 'head']
+    alembic.config.main(argv=alembicArgs)
+
+
+@event.listens_for(Engine, "connect")
+def set_sqlite_pragma(dbapi_connection, connection_record):
+    if os.environ.get('HIT_DB_TYPE', 'postgresql') == 'sqlite':
+        cursor = dbapi_connection.cursor()
+        cursor.execute("PRAGMA foreign_keys=ON")
+        cursor.close()
+
 
 if __name__ == '__main__':
     init_db()
```

## sunpeek/definitions/__init__.py

```diff
@@ -1,8 +1,17 @@
 """
-This package contains definitions for the pre-defined components such as sensor types, fluids, collectors etc.
-These are used to pre-populate the application database, and should NOT be used directly in application code,
-other than tests
+This package contains definitions for the pre-defined components such as fluids or collectors.
+These are used to pre-populate the application database.
 """
+import enum
+from pathlib import Path
 
-from sunpeek.definitions import collector_types
-from sunpeek.definitions import fluid_definitions
+# from sunpeek.definitions import collector_types
+# from sunpeek.definitions import fluid_definitions
+
+
+class FluidProps(str, enum.Enum):
+    density = 'density'
+    heat_capacity = 'heat capacity'
+
+
+fluid_data_dir = Path(__file__).with_name('fluid_data')
```

## sunpeek/definitions/collector_types.py

```diff
@@ -22,15 +22,15 @@
                      a5=Q(7.313, "kJ m**-2 K**-1"),
                      kd=Q(0.93, ""),
                      eta0b=Q(0.745, ""),
                      f_prime=Q(0.95, ""),
                      iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
                                                      iam_reference=Q([1, 0.99, 0.97, 0.94, 0.9, 0.82, 0.65, 0.32, 0]))
                      ),
-    CollectorTypeQDT(name='Gasokol 55',
+    CollectorTypeQDT(name='powerSol 55',
                      manufacturer_name="Gasokol GmbH",
                      product_name="powerSol 55",
                      licence_number='011-7S2928 F',
                      test_report_id="21246087.001 (2019-05-24)",
                      certificate_date_issued=datetime(2019, 6, 4),
                      certificate_lab="TÜV Rheinland Energy GmbH, Germany",
                      test_reference_area='gross',
@@ -43,15 +43,15 @@
                      a2=Q(0.012, "W m**-2 K**-2"),
                      a5=Q(13.489, "kJ m**-2 K**-1"),
                      kd=Q(0.88, ""),
                      eta0b=Q(0.741, ""),
                      iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
                                                      iam_reference=Q([1, 0.99, 0.97, 0.94, 0.89, 0.8, 0.61, 0.3, 0]))
                      ),
-    CollectorTypeQDT(name='Gasokol 120',
+    CollectorTypeQDT(name='powerSol 120',
                      manufacturer_name="Gasokol GmbH",
                      product_name="powerSol 120",
                      licence_number='011-7S2928 F',
                      test_report_id="21246087.001 (2019-05-24)",
                      certificate_date_issued=datetime(2019, 6, 4),
                      certificate_lab="TÜV Rheinland Energy GmbH, Germany",
                      area_gr=Q(12.0, 'm**2'),
@@ -64,15 +64,15 @@
                      a2=Q(0.012, "W m**-2 K**-2"),
                      a5=Q(13.489, "kJ m**-2 K**-1"),
                      kd=Q(0.88, ""),
                      eta0b=Q(0.741, ""),
                      iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
                                                      iam_reference=Q([1, 0.99, 0.97, 0.94, 0.89, 0.8, 0.61, 0.3, 0]))
                      ),
-    CollectorTypeQDT(name='Gasokol 136',
+    CollectorTypeQDT(name='powerSol 136',
                      manufacturer_name="Gasokol GmbH",
                      product_name="powerSol 136",
                      licence_number='011-7S2928 F',
                      test_report_id="21246087.001 (2019-05-24)",
                      certificate_date_issued=datetime(2019, 6, 4),
                      test_reference_area='gross',
                      certificate_lab="TÜV Rheinland Energy GmbH, Germany",
@@ -92,16 +92,17 @@
     CollectorTypeQDT(name='Greenonetec 3803',
                      manufacturer_name="GREENoneTEC Solarindustrie GmbH",
                      product_name='GK 3803',
                      licence_number='011-7S2565 F',
                      test_report_id='15COL1247 (2015-08-28), 15COL1247Q (2015-08-28)',
                      certificate_date_issued=datetime(2015, 8, 28),
                      certificate_lab='TZS, ITW University Stuttgart, Germany',
-                     test_reference_area="gross",
+                     test_reference_area="aperture",
                      area_gr=Q(7.91, 'm**2'),
+                     area_ap=Q(7.41, 'm**2'),
                      gross_width=Q(3557, "mm"),
                      gross_length=Q(2224, "mm"),
                      gross_height=Q(135, "mm"),
                      a1=Q(2.102, "W m**-2 K**-1"),
                      a2=Q(0.016, "W m**-2 K**-2"),
                      a5=Q(9.664, "kJ m**-2 K**-1"),
                      kd=Q(0.931, ""),
@@ -112,15 +113,16 @@
     CollectorTypeQDT(name='Greenonetec 3803S',
                      manufacturer_name="GREENoneTEC Solarindustrie GmbH",
                      product_name='GK 3803S',
                      licence_number='011-7S2566 F',
                      test_report_id='15COL1257 (2015-08-28), 15COL1257Q (2015-08-28)',
                      certificate_date_issued=datetime(2015, 8, 28),
                      certificate_lab='TZS, ITW University Stuttgart, Germany',
-                     test_reference_area="gross",
+                     test_reference_area="aperture",
+                     area_ap=Q(7.41, 'm**2'),
                      area_gr=Q(7.91, 'm**2'),
                      gross_width=Q(3557, "mm"),
                      gross_length=Q(2224, "mm"),
                      gross_height=Q(135, "mm"),
                      a1=Q(3.083, "W m**-2 K**-1"),
                      a2=Q(0.013, "W m**-2 K**-2"),
                      a5=Q(9.985, "kJ m**-2 K**-1"),
@@ -132,16 +134,17 @@
     CollectorTypeQDT(name='Greenonetec 3133',
                      manufacturer_name="GREENoneTEC Solarindustrie GmbH",
                      product_name='GK 3133',
                      licence_number='011-7S2565 F',
                      test_report_id='15COL1247 (2015-08-28), 15COL1247Q (2015-08-28)',
                      certificate_date_issued=datetime(2015, 8, 28),
                      certificate_lab='TZS, ITW University Stuttgart, Germany',
-                     test_reference_area="gross",
+                     test_reference_area="aperture",
                      area_gr=Q(13.17, 'm**2'),
+                     area_ap=Q(12.35, 'm**2'),
                      gross_width=Q(5920, "mm"),
                      gross_length=Q(2224, "mm"),
                      gross_height=Q(135, "mm"),
                      a1=Q(2.102, "W m**-2 K**-1"),
                      a2=Q(0.016, "W m**-2 K**-2"),
                      a5=Q(9.664, "kJ m**-2 K**-1"),
                      kd=Q(0.931, ""),
@@ -152,16 +155,17 @@
     CollectorTypeQDT(name='Greenonetec 3133S',
                      manufacturer_name="GREENoneTEC Solarindustrie GmbH",
                      product_name='GK 3133S',
                      licence_number='011-7S2566 F',
                      test_report_id='15COL1257 (2015-08-28), 15COL1257Q (2015-08-28)',
                      certificate_date_issued=datetime(2015, 8, 28),
                      certificate_lab='TZS, ITW University Stuttgart, Germany',
-                     test_reference_area="gross",
+                     test_reference_area="aperture",
                      area_gr=Q(13.17, 'm**2'),
+                     area_ap=Q(12.35, 'm**2'),
                      gross_width=Q(5920, "mm"),
                      gross_length=Q(2224, "mm"),
                      gross_height=Q(135, "mm"),
                      a1=Q(3.083, "W m**-2 K**-1"),
                      a2=Q(0.013, "W m**-2 K**-2"),
                      a5=Q(9.985, "kJ m**-2 K**-1"),
                      kd=Q(0.918, ""),
@@ -225,17 +229,117 @@
                      a1=Q(2.416, 'W m**-2 K**-1'),
                      a2=Q(0.008, 'W m**-2 K**-2'),
                      a5=Q(8.3, "kJ m**-2 K**-1"),
                      kd=Q(0.964, ''),
                      iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
                                                      iam_reference=Q([1, 1, 0.99, 0.98, 0.94, 0.83, 0.56, 0.28, 0]))
                      ),
+    CollectorTypeQDT(name='ökoTech HT 16.7 Export',
+                     manufacturer_name="ökoTech Solarkollektoren GmbH",
+                     product_name='HT',
+                     licence_number='011-7S837 F',
+                     test_report_id='2.04.01120.1.0- QT, 2.04.01120.1.0- LT, 2.04.00667.1.0-2 - QT',
+                     certificate_date_issued=datetime(2017, 2, 7),
+                     certificate_lab='TÜV Rheinland Energy GmbH, Germany',
+                     test_reference_area="gross",
+                     area_gr=Q(16.7, 'm**2'),
+                     gross_width=Q(7170, "mm"),
+                     gross_length=Q(2330, "mm"),
+                     gross_height=Q(187, "mm"),
+                     eta0b=Q(0.701, ''),
+                     a1=Q(2.582, 'W m**-2 K**-1'),
+                     a2=Q(0.005, 'W m**-2 K**-2'),
+                     a5=Q(14.7, "kJ m**-2 K**-1"),
+                     kd=Q(0.983, ''),
+                     iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 90], 'deg'),
+                                                     iam_reference=Q([1, 0.99, 0.97, 0.93, 0.88, 0.78, 0.58, 0.0]))
+                     ),
+    CollectorTypeQDT(name='ökoTech HT 4.2 Export',
+                     manufacturer_name="ökoTech Solarkollektoren GmbH",
+                     product_name='HT',
+                     licence_number='011-7S837 F',
+                     test_report_id='2.04.01120.1.0- QT, 2.04.01120.1.0- LT, 2.04.00667.1.0-2 - QT',
+                     certificate_date_issued=datetime(2017, 2, 7),
+                     certificate_lab='TÜV Rheinland Energy GmbH, Germany',
+                     test_reference_area="gross",
+                     area_gr=Q(4.2, 'm**2'),
+                     gross_width=Q(2076, "mm"),
+                     gross_length=Q(2050, "mm"),
+                     gross_height=Q(187, "mm"),
+                     eta0b=Q(0.701, ''),
+                     a1=Q(2.582, 'W m**-2 K**-1'),
+                     a2=Q(0.005, 'W m**-2 K**-2'),
+                     a5=Q(14.7, "kJ m**-2 K**-1"),
+                     kd=Q(0.983, ''),
+                     iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 90], 'deg'),
+                                                     iam_reference=Q([1, 0.99, 0.97, 0.93, 0.88, 0.78, 0.58, 0.0]))
+                     ),
+    CollectorTypeQDT(name='ensol DIS 150',
+                     manufacturer_name="Energetyka Solarna ensol Sp. z.o.o.",
+                     product_name='DIS 150',
+                     licence_number='011-7S2978 F',
+                     test_report_id='21249150.001',
+                     certificate_date_issued=datetime(2020, 7, 20),
+                     certificate_lab='TÜV Rheinland Energy GmbH, Germany',
+                     test_reference_area="gross",
+                     area_gr=Q(15.5, 'm**2'),
+                     gross_width=Q(6606, "mm"),
+                     gross_length=Q(2350, "mm"),
+                     gross_height=Q(173, "mm"),
+                     eta0b=Q(0.765, ''),
+                     a1=Q(2.23, 'W m**-2 K**-1'),
+                     a2=Q(0.008, 'W m**-2 K**-2'),
+                     a5=Q(6.483, "kJ m**-2 K**-1"),
+                     kd=Q(0.91, ''),
+                     iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
+                                                     iam_reference=Q([1, 0.99, 0.98, 0.95, 0.91, 0.84, 0.70, 0.35, 0]))
+                     ),
+    CollectorTypeQDT(name='Sunrain FPC1500C',
+                     manufacturer_name="Jiangsu Sunrain Solar Energy Co., Ltd",
+                     product_name='FPC1500C',
+                     licence_number='011-7S3004 F',
+                     test_report_id='201203085GZU-001',
+                     certificate_date_issued=datetime(2020, 2, 25),
+                     certificate_lab='DIN CERTCO',
+                     test_reference_area="gross",
+                     area_gr=Q(15.02, 'm**2'),
+                     gross_width=Q(5960, "mm"),
+                     gross_length=Q(2520, "mm"),
+                     gross_height=Q(166, "mm"),
+                     eta0b=Q(0.852, ''),
+                     a1=Q(3.03, 'W m**-2 K**-1'),
+                     a2=Q(0.014, 'W m**-2 K**-2'),
+                     a5=Q(6.833, "kJ m**-2 K**-1"),
+                     kd=Q(0.92, ''),
+                     iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
+                                                     iam_reference=Q([1, 1, 1, 0.99, 0.96, 0.9, 0.78, 0.52, 0.0]))
+                     ),
+    CollectorTypeQDT(name='TVP MT-Power v4',
+                     manufacturer_name='TVP Solar SA',
+                     product_name='MT- Power v4',
+                     licence_number='011-7S1890F',
+                     test_report_id='16COL1343, 16COL1343Q',
+                     certificate_date_issued=datetime(2017,5,24),
+                     certificate_lab='DIN CERTCO',
+                     test_reference_area='gross',
+                     area_gr=Q(1.96, 'm**2'),
+                     gross_length=Q(975, 'mm'),
+                     gross_width=Q(2015, 'mm'),
+                     gross_height=Q(51, 'mm'),
+                     eta0b=Q(0.737, ''),
+                     a1=Q(0.504, 'W m**-2 K**-1'),
+                     a2=Q(0.006, 'W m**-2 K**-2'),
+                     a5=Q(15.32, "kJ m**-2 K**-1"),
+                     kd=Q(0.957, ''),
+                     iam_method=iam.IAM_Interpolated(aoi_reference=Q([10, 20, 30, 40, 50, 60, 70, 80, 90], 'deg'),
+                                                     iam_reference=Q([1, 1, 0.99, 0.98, 0.95, 0.88, 0.72, 0.36, 0.0]))
+                     ),
 
     # Collectors tested with static test ----------------------------------------------------------------------------
-    # Overwritten by CollectorType below, because CollectorTypeSST doesn not allow for an eta0b parameter.
+    # Overwritten by CollectorType below, because CollectorTypeSST does not allow for an eta0b parameter.
     # CollectorTypeSST(name='Greenonetec HT 13,6',
     #                  manufacturer_name="GREENoneTEC Solarindustrie GmbH",
     #                  product_name='GK HT 13,6',
     #                  licence_number='011-7S2819 F',
     #                  test_report_id='20COLC1735ISO (2020-11-10), 20COLC1735ISOQ (2010-11-10), C1735L, '
     #                                 'C1781L (2018-09-06)',
     #                  certificate_date_issued=datetime(2020, 11, 10),
```

## sunpeek/definitions/fluid_definitions.py

```diff
@@ -1,601 +1,65 @@
-import os
-from pathlib import Path
-from sunpeek.components import WPDFluidDefinition, CoolPropFluidDefinition
-from sunpeek.components.fluids import WPDModelPure
+import enum
+from collections import namedtuple
+
+from sunpeek.components.fluids import WPDFluidDefinition, CoolPropFluidDefinition
+
+WPDFluidInfo = namedtuple('WPDFluidInfo',
+                          ['name', 'is_pure', 'unit_density', 'unit_heat_capacity', 'manufacturer', 'description'])
+
+
+class WPDFluids(enum.Enum):
+    """This enum defines the basic information of all own / predefined fluids.
+    These are available within the SunPeek Python package and also in the database after init_db().
+
+    The "name" string of WPDFluidInfo is supposed to be the subfolder (of fluid_data_dir) where the fluid data csv
+    files are stored: density.csv and heat_capacity.csv
+    To add a new fluid, just simply add an entry in this class and put the csv files in the right subfolder.
+    """
+    # Pure fluids
+    fhw_pekasolar = WPDFluidInfo('Pekasolar_FHW',
+                                 is_pure=True,
+                                 unit_density={'te': 'degC', 'out': 'kg m**-3'},
+                                 unit_heat_capacity={'te': 'degC', 'out': 'J g**-1 K**-1'},
+                                 manufacturer="Pekasolar",
+                                 description="Pekasolar fluid used in plant FHW, Pekasolar. "
+                                             "Fixed concentration, as used in plant and lab-measured.")
+    corro_star = WPDFluidInfo('Gasokol, corroStar mixture',
+                              is_pure=True,
+                              unit_density={'te': 'degC', 'out': 'kg m**-3'},
+                              unit_heat_capacity={'te': 'degC', 'out': 'J kg**-1 K**-1'},
+                              manufacturer="Gasokol GmbH",
+                              description="Monopropylene glycol, fixed-concentration mixture, 36 vol-% of 'Thermum P'. "
+                                          "Fluid property datasheet 2023.")
+    # Mixed fluids
+    thermum_p = WPDFluidInfo('Wocklum Thermum P',
+                             is_pure=False,
+                             unit_density={'te': 'degC', 'c': 'percent', 'out': 'kg m**-3'},
+                             unit_heat_capacity={'te': 'degC', 'c': 'percent', 'out': 'kJ kg**-1 K**-1'},
+                             manufacturer="Wocklum GmbH",
+                             description="Wocklum / Thermum monopropylene glycol fluid 'Thermum P'. "
+                                         "Fluid property datasheet 2023.")
 
-raw_data_dir = Path(__file__).with_name('raw_data')
 
 wpd_fluids = [
-    WPDFluidDefinition('Pekasolar_FHW',
-                       WPDModelPure(unit={'te': 'degC', 'out': 'kg m**-3'}).train(
-                           os.path.join(raw_data_dir, 'FHW, Pekasolar', 'Pekasolar, pdf export, density.csv')),
-                       WPDModelPure(unit={'te': 'degC', 'out': 'J g**-1 K**-1'}).train(
-                           os.path.join(raw_data_dir, 'FHW, Pekasolar', 'Pekasolar, pdf export, heat capacity.csv')),
-                       manufacturer="Pekasolar",
-                       description="Fluid used in plant FHW, Pekasolar. Fixed concentration as used in plant."),
+    # Pure fluids
+    WPDFluidDefinition.from_fluid_info(WPDFluids.fhw_pekasolar.value),
+    WPDFluidDefinition.from_fluid_info(WPDFluids.corro_star.value),
+    # Mixed fluids
+    WPDFluidDefinition.from_fluid_info(WPDFluids.thermum_p.value),
 ]
 
 coolprop_fluids = [
     CoolPropFluidDefinition(model_type='CoolProp',
                             name='water',
                             manufacturer=None,
                             description='HEOS::water',
                             is_pure=True,
                             ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='AS10',
-                            manufacturer=None,
-                            description='Aspen Temper -10, Potassium acetate/formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='AS20',
-                            manufacturer=None,
-                            description='Aspen Temper -20, Potassium acetate/formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='AS30',
-                            manufacturer=None,
-                            description='Aspen Temper -30, Potassium acetate/formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='AS40',
-                            manufacturer=None,
-                            description='Aspen Temper -40, Potassium acetate/formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='AS55',
-                            manufacturer=None,
-                            description='Aspen Temper -55, Potassium acetate/formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DEB',
-                            manufacturer=None,
-                            description='Diethylbenzene mixture - Dowtherm J',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DSF',
-                            manufacturer=None,
-                            description='Dynalene SF',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DowJ',
-                            manufacturer=None,
-                            description='DowthermJ',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DowJ2',
-                            manufacturer=None,
-                            description='Dowtherm J, Diethylbenzene mixture',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DowQ',
-                            manufacturer=None,
-                            description='DowthermQ',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='DowQ2',
-                            manufacturer=None,
-                            description='Dowtherm Q, Diphenylethane/alkylated aromatics',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HC10',
-                            manufacturer=None,
-                            description='Dynalene HC10',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HC20',
-                            manufacturer=None,
-                            description='Dynalene HC20',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HC30',
-                            manufacturer=None,
-                            description='Dynalene HC30',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HC40',
-                            manufacturer=None,
-                            description='Dynalene HC40',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HC50',
-                            manufacturer=None,
-                            description='Dynalene HC50',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HCB',
-                            manufacturer=None,
-                            description='Hydrocarbon blend - Dynalene MV',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HCM',
-                            manufacturer=None,
-                            description='Hydrocarbon mixture - Gilotherm D12',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HFE',
-                            manufacturer=None,
-                            description='Hydrofluoroether - HFE-7100 3M Novec',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HFE2',
-                            manufacturer=None,
-                            description='HFE-7100, Hydrofluoroether',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HY20',
-                            manufacturer=None,
-                            description='HYCOOL 20, Potassium formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HY30',
-                            manufacturer=None,
-                            description='HyCool 30, Potassium formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HY40',
-                            manufacturer=None,
-                            description='HyCool 40, Potassium formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HY45',
-                            manufacturer=None,
-                            description='HyCool 45, Potassium formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='HY50',
-                            manufacturer=None,
-                            description='HyCool 50, Potassium formate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='NBS',
-                            manufacturer=None,
-                            description='NBS, Water',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='NaK',
-                            manufacturer=None,
-                            description='Nitrate salt, 0.6 NaNO3 and 0.4 KNO3',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PBB',
-                            manufacturer=None,
-                            description='Pirobloc HTF-BASIC',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PCL',
-                            manufacturer=None,
-                            description='Paracryol, Aliphatic Hydrocarbon',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PCR',
-                            manufacturer=None,
-                            description='Paratherm CR',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PGLT',
-                            manufacturer=None,
-                            description='Paratherm GLT',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PHE',
-                            manufacturer=None,
-                            description='Paratherm HE',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PHR',
-                            manufacturer=None,
-                            description='Paratherm HR',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PLR',
-                            manufacturer=None,
-                            description='Paratherm LR',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PMR',
-                            manufacturer=None,
-                            description='Paratherm MR',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PMS1',
-                            manufacturer=None,
-                            description='Polydimethylsiloxan 1 - Baysilone KT3',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PMS2',
-                            manufacturer=None,
-                            description='Polydimethylsiloxan 2 - Syltherm XLT',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PNF',
-                            manufacturer=None,
-                            description='Paratherm NF',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='PNF2',
-                            manufacturer=None,
-                            description='Paratherm NF, Hydrotreated mineral oil',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='S800',
-                            manufacturer=None,
-                            description='Syltherm 800',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='SAB',
-                            manufacturer=None,
-                            description='Synthetic alkyl benzene - Marlotherm X',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='T66',
-                            manufacturer=None,
-                            description='Therminol66',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='T72',
-                            manufacturer=None,
-                            description='Therminol72',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TCO',
-                            manufacturer=None,
-                            description='Citrus oil terpene - d-Limonene',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TD12',
-                            manufacturer=None,
-                            description='TherminolD12',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TVP1',
-                            manufacturer=None,
-                            description='TherminolVP1',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TVP1869',
-                            manufacturer=None,
-                            description='Thermogen VP 1869',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TX22',
-                            manufacturer=None,
-                            description='Texatherm22',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TY10',
-                            manufacturer=None,
-                            description='Tyfoxit 1.10, Potassium Acetate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TY15',
-                            manufacturer=None,
-                            description='Tyfoxit 1.15, Potassium Acetate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TY20',
-                            manufacturer=None,
-                            description='Tyfoxit 1.20, Potassium Acetate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='TY24',
-                            manufacturer=None,
-                            description='Tyfoxit 1.24, Potassium Acetate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='Water',
-                            manufacturer=None,
-                            description='Fit of EOS from 1 bar to 100 bar',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='XLT',
-                            manufacturer=None,
-                            description='SylthermXLT',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='XLT2',
-                            manufacturer=None,
-                            description='Syltherm XLT, Polydimethylsiloxan',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='ZS10',
-                            manufacturer=None,
-                            description='Zitrec S10, Potassium formate/Sodium propionate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='ZS25',
-                            manufacturer=None,
-                            description='Zitrec S25, Potassium formate/Sodium propionate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='ZS40',
-                            manufacturer=None,
-                            description='Zitrec S40, Potassium formate/Sodium propionate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='ZS45',
-                            manufacturer=None,
-                            description='Zitrec S45, Potassium formate/Sodium propionate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='ZS55',
-                            manufacturer=None,
-                            description='Zitrec S55, Potassium formate/Sodium propionate',
-                            is_pure=True,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='FRE',
-                            manufacturer=None,
-                            description='Freezium, Potassium Formate',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='IceEA',
-                            manufacturer=None,
-                            description='Ice slurry with Ethanol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='IceNA',
-                            manufacturer=None,
-                            description='Ice slurry with NaCl',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='IcePG',
-                            manufacturer=None,
-                            description='Ice slurry with Propylene Glycol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='LiBr',
-                            manufacturer=None,
-                            description='Lithium-bromide solution - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MAM',
-                            manufacturer=None,
-                            description='Ammonia (NH3) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MAM2',
-                            manufacturer=None,
-                            description='Melinder, Ammonia',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MCA',
-                            manufacturer=None,
-                            description='Calcium Chloride (CaCl2) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MCA2',
-                            manufacturer=None,
-                            description='Melinder, Calcium Chloride',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MEA',
-                            manufacturer=None,
-                            description='Ethyl Alcohol (Ethanol) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MEA2',
-                            manufacturer=None,
-                            description='Melinder, Ethanol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MEG',
-                            manufacturer=None,
-                            description='Ethylene Glycol - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MEG2',
-                            manufacturer=None,
-                            description='Melinder, Ethylene Glycol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MGL',
-                            manufacturer=None,
-                            description='Glycerol - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MGL2',
-                            manufacturer=None,
-                            description='Melinder, Glycerol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MITSW',
-                            manufacturer=None,
-                            description='MIT Seawater',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MKA',
-                            manufacturer=None,
-                            description='Potassium Acetate (CH3CO2K) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MKA2',
-                            manufacturer=None,
-                            description='Melinder, Potassium Acetate',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MKC',
-                            manufacturer=None,
-                            description='Potassium Carbonate (K2CO3) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MKC2',
-                            manufacturer=None,
-                            description='Melinder, Potassium Carbonate',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MKF',
-                            manufacturer=None,
-                            description='Potassium Formate (CHKO2) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MLI',
-                            manufacturer=None,
-                            description='Lithium Chloride (LiCl) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MMA',
-                            manufacturer=None,
-                            description='Methyl Alcohol (Methanol) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MMA2',
-                            manufacturer=None,
-                            description='Melinder, Methanol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MMG',
-                            manufacturer=None,
-                            description='MgCl2 - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MMG2',
-                            manufacturer=None,
-                            description='Melinder, Magnesium Chloride',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MNA',
-                            manufacturer=None,
-                            description='Sodium Chloride (NaCl) - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MNA2',
-                            manufacturer=None,
-                            description='Melinder, Sodium Chloride',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MPG',
-                            manufacturer=None,
-                            description='Propylene Glycol - aq',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='MPG2',
-                            manufacturer=None,
-                            description='Melinder, Propylene Glycol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='VCA',
-                            manufacturer=None,
-                            description='VDI, Calcium Cloride',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='VKC',
-                            manufacturer=None,
-                            description='VDI, Potassium Carbonate',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='VMA',
-                            manufacturer=None,
-                            description='VDI, Methanol',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='VMG',
-                            manufacturer=None,
-                            description='VDI, Magnesium Chloride',
-                            is_pure=False,
-                            ),
-    CoolPropFluidDefinition(model_type='CoolProp',
-                            name='VNA',
-                            manufacturer=None,
-                            description='VDI, Sodium Chloride',
-                            is_pure=False,
-                            ),
+
     CoolPropFluidDefinition(model_type='CoolProp',
                             name='AEG',
                             manufacturer=None,
                             description='ASHRAE, Ethylene Glycol',
                             is_pure=False,
                             ),
     CoolPropFluidDefinition(model_type='CoolProp',
@@ -672,10 +136,592 @@
                             ),
 ]
 
 all_definitions = coolprop_fluids + wpd_fluids
 
 
 def get_definition(name):
-    for fluid in all_definitions:
-        if fluid.name == name or name in fluid.description:
-            return fluid
+    for fluid_def in all_definitions:
+        if (fluid_def.name == name) or (name in fluid_def.description):
+            return fluid_def
+
+# Unused CoolProp fluids  --------------------------------------------------------
+
+# CoolProp incompressible pure fluids: Removed, these are mostly not relevant for solar thermal
+# http://www.coolprop.org/fluid_properties/Incompressibles.html#id122
+# See also: https://gitlab.com/sunpeek/web-ui/-/issues/110
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='AS10',
+#                         manufacturer=None,
+#                         description='Aspen Temper -10, Potassium acetate/formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='AS20',
+#                         manufacturer=None,
+#                         description='Aspen Temper -20, Potassium acetate/formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='AS30',
+#                         manufacturer=None,
+#                         description='Aspen Temper -30, Potassium acetate/formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='AS40',
+#                         manufacturer=None,
+#                         description='Aspen Temper -40, Potassium acetate/formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='AS55',
+#                         manufacturer=None,
+#                         description='Aspen Temper -55, Potassium acetate/formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DEB',
+#                         manufacturer=None,
+#                         description='Diethylbenzene mixture - Dowtherm J',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DSF',
+#                         manufacturer=None,
+#                         description='Dynalene SF',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DowJ',
+#                         manufacturer=None,
+#                         description='DowthermJ',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DowJ2',
+#                         manufacturer=None,
+#                         description='Dowtherm J, Diethylbenzene mixture',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DowQ',
+#                         manufacturer=None,
+#                         description='DowthermQ',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='DowQ2',
+#                         manufacturer=None,
+#                         description='Dowtherm Q, Diphenylethane/alkylated aromatics',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HC10',
+#                         manufacturer=None,
+#                         description='Dynalene HC10',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HC20',
+#                         manufacturer=None,
+#                         description='Dynalene HC20',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HC30',
+#                         manufacturer=None,
+#                         description='Dynalene HC30',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HC40',
+#                         manufacturer=None,
+#                         description='Dynalene HC40',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HC50',
+#                         manufacturer=None,
+#                         description='Dynalene HC50',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HCB',
+#                         manufacturer=None,
+#                         description='Hydrocarbon blend - Dynalene MV',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HCM',
+#                         manufacturer=None,
+#                         description='Hydrocarbon mixture - Gilotherm D12',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HFE',
+#                         manufacturer=None,
+#                         description='Hydrofluoroether - HFE-7100 3M Novec',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HFE2',
+#                         manufacturer=None,
+#                         description='HFE-7100, Hydrofluoroether',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HY20',
+#                         manufacturer=None,
+#                         description='HYCOOL 20, Potassium formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HY30',
+#                         manufacturer=None,
+#                         description='HyCool 30, Potassium formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HY40',
+#                         manufacturer=None,
+#                         description='HyCool 40, Potassium formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HY45',
+#                         manufacturer=None,
+#                         description='HyCool 45, Potassium formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='HY50',
+#                         manufacturer=None,
+#                         description='HyCool 50, Potassium formate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='NBS',
+#                         manufacturer=None,
+#                         description='NBS, Water',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='NaK',
+#                         manufacturer=None,
+#                         description='Nitrate salt, 0.6 NaNO3 and 0.4 KNO3',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PBB',
+#                         manufacturer=None,
+#                         description='Pirobloc HTF-BASIC',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PCL',
+#                         manufacturer=None,
+#                         description='Paracryol, Aliphatic Hydrocarbon',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PCR',
+#                         manufacturer=None,
+#                         description='Paratherm CR',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PGLT',
+#                         manufacturer=None,
+#                         description='Paratherm GLT',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PHE',
+#                         manufacturer=None,
+#                         description='Paratherm HE',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PHR',
+#                         manufacturer=None,
+#                         description='Paratherm HR',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PLR',
+#                         manufacturer=None,
+#                         description='Paratherm LR',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PMR',
+#                         manufacturer=None,
+#                         description='Paratherm MR',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PMS1',
+#                         manufacturer=None,
+#                         description='Polydimethylsiloxan 1 - Baysilone KT3',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PMS2',
+#                         manufacturer=None,
+#                         description='Polydimethylsiloxan 2 - Syltherm XLT',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PNF',
+#                         manufacturer=None,
+#                         description='Paratherm NF',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='PNF2',
+#                         manufacturer=None,
+#                         description='Paratherm NF, Hydrotreated mineral oil',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='S800',
+#                         manufacturer=None,
+#                         description='Syltherm 800',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='SAB',
+#                         manufacturer=None,
+#                         description='Synthetic alkyl benzene - Marlotherm X',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='T66',
+#                         manufacturer=None,
+#                         description='Therminol66',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='T72',
+#                         manufacturer=None,
+#                         description='Therminol72',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TCO',
+#                         manufacturer=None,
+#                         description='Citrus oil terpene - d-Limonene',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TD12',
+#                         manufacturer=None,
+#                         description='TherminolD12',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TVP1',
+#                         manufacturer=None,
+#                         description='TherminolVP1',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TVP1869',
+#                         manufacturer=None,
+#                         description='Thermogen VP 1869',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TX22',
+#                         manufacturer=None,
+#                         description='Texatherm22',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TY10',
+#                         manufacturer=None,
+#                         description='Tyfoxit 1.10, Potassium Acetate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TY15',
+#                         manufacturer=None,
+#                         description='Tyfoxit 1.15, Potassium Acetate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TY20',
+#                         manufacturer=None,
+#                         description='Tyfoxit 1.20, Potassium Acetate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='TY24',
+#                         manufacturer=None,
+#                         description='Tyfoxit 1.24, Potassium Acetate',
+#                         is_pure=True,
+#                         ),
+
+# Default and recommended for water is to use the "HEOS::water" definition
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='Water',
+#                         manufacturer=None,
+#                         description='Fit of EOS from 1 bar to 100 bar',
+#                         is_pure=True,
+#                         ),
+
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='XLT',
+#                         manufacturer=None,
+#                         description='SylthermXLT',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='XLT2',
+#                         manufacturer=None,
+#                         description='Syltherm XLT, Polydimethylsiloxan',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='ZS10',
+#                         manufacturer=None,
+#                         description='Zitrec S10, Potassium formate/Sodium propionate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='ZS25',
+#                         manufacturer=None,
+#                         description='Zitrec S25, Potassium formate/Sodium propionate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='ZS40',
+#                         manufacturer=None,
+#                         description='Zitrec S40, Potassium formate/Sodium propionate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='ZS45',
+#                         manufacturer=None,
+#                         description='Zitrec S45, Potassium formate/Sodium propionate',
+#                         is_pure=True,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='ZS55',
+#                         manufacturer=None,
+#                         description='Zitrec S55, Potassium formate/Sodium propionate',
+#                         is_pure=True,
+#                         ),
+
+# CoolProp incompressible mass-based binary fluids: Removed, these are mostly not relevant for solar thermal
+# http://www.coolprop.org/fluid_properties/Incompressibles.html#id123
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='FRE',
+#                         manufacturer=None,
+#                         description='Freezium, Potassium Formate',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='IceEA',
+#                         manufacturer=None,
+#                         description='Ice slurry with Ethanol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='IceNA',
+#                         manufacturer=None,
+#                         description='Ice slurry with NaCl',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='IcePG',
+#                         manufacturer=None,
+#                         description='Ice slurry with Propylene Glycol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='LiBr',
+#                         manufacturer=None,
+#                         description='Lithium-bromide solution - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MAM',
+#                         manufacturer=None,
+#                         description='Ammonia (NH3) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MAM2',
+#                         manufacturer=None,
+#                         description='Melinder, Ammonia',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MCA',
+#                         manufacturer=None,
+#                         description='Calcium Chloride (CaCl2) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MCA2',
+#                         manufacturer=None,
+#                         description='Melinder, Calcium Chloride',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MEA',
+#                         manufacturer=None,
+#                         description='Ethyl Alcohol (Ethanol) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MEA2',
+#                         manufacturer=None,
+#                         description='Melinder, Ethanol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MEG',
+#                         manufacturer=None,
+#                         description='Ethylene Glycol - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MEG2',
+#                         manufacturer=None,
+#                         description='Melinder, Ethylene Glycol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MGL',
+#                         manufacturer=None,
+#                         description='Glycerol - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MGL2',
+#                         manufacturer=None,
+#                         description='Melinder, Glycerol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MITSW',
+#                         manufacturer=None,
+#                         description='MIT Seawater',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MKA',
+#                         manufacturer=None,
+#                         description='Potassium Acetate (CH3CO2K) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MKA2',
+#                         manufacturer=None,
+#                         description='Melinder, Potassium Acetate',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MKC',
+#                         manufacturer=None,
+#                         description='Potassium Carbonate (K2CO3) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MKC2',
+#                         manufacturer=None,
+#                         description='Melinder, Potassium Carbonate',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MKF',
+#                         manufacturer=None,
+#                         description='Potassium Formate (CHKO2) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MLI',
+#                         manufacturer=None,
+#                         description='Lithium Chloride (LiCl) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MMA',
+#                         manufacturer=None,
+#                         description='Methyl Alcohol (Methanol) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MMA2',
+#                         manufacturer=None,
+#                         description='Melinder, Methanol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MMG',
+#                         manufacturer=None,
+#                         description='MgCl2 - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MMG2',
+#                         manufacturer=None,
+#                         description='Melinder, Magnesium Chloride',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MNA',
+#                         manufacturer=None,
+#                         description='Sodium Chloride (NaCl) - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MNA2',
+#                         manufacturer=None,
+#                         description='Melinder, Sodium Chloride',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MPG',
+#                         manufacturer=None,
+#                         description='Propylene Glycol - aq',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='MPG2',
+#                         manufacturer=None,
+#                         description='Melinder, Propylene Glycol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='VCA',
+#                         manufacturer=None,
+#                         description='VDI, Calcium Cloride',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='VKC',
+#                         manufacturer=None,
+#                         description='VDI, Potassium Carbonate',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='VMA',
+#                         manufacturer=None,
+#                         description='VDI, Methanol',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='VMG',
+#                         manufacturer=None,
+#                         description='VDI, Magnesium Chloride',
+#                         is_pure=False,
+#                         ),
+# CoolPropFluidDefinition(model_type='CoolProp',
+#                         name='VNA',
+#                         manufacturer=None,
+#                         description='VDI, Sodium Chloride',
+#                         is_pure=False,
+#                         ),
```

## sunpeek/demo/demo_plant.py

```diff
@@ -1,39 +1,54 @@
 import json
+from datetime import datetime
 from sqlalchemy.orm import Session
 
-from sunpeek.common import config_parser, data_uploader
+import sunpeek.demo
+from sunpeek.common import config_parser
+from sunpeek.data_handling import data_uploader
+from sunpeek.data_handling.wrapper import use_csv
 from sunpeek.db_utils import crud
 import sunpeek.components as cmp
-import sunpeek.demo
+import sunpeek.core_methods.virtuals as virtuals
 
 
 def requires_demo_data(func):
     if not sunpeek.demo.DEMO_DATA_AVAILABLE:
         raise ModuleNotFoundError(
             "This function requires optional dependency sunpeek-demo. Install it with `pip install sunpeek[demo]`")
     return func
 
 
 @requires_demo_data
 def create_demoplant(session: Session, name: str = None):
     with open(sunpeek.demo.DEMO_CONFIG_PATH, 'r') as f:
         conf = json.load(f)
 
-    if name is not None:
-        conf['plant']['name'] = name
+    # Plant name must be unique in database => create unique
+    unique_plant_name = f'demoplant_{datetime.now().strftime("%Y%m%d_%H%M%S")}'
+    name = unique_plant_name if (name is None) else name
+    conf['plant']['name'] = name
 
     config_parser.make_and_store_plant(conf, session)
 
-    return crud.get_plants(session, plant_name=conf['plant']['name'])
+    plant = crud.get_plants(session, plant_name=conf['plant']['name'])
+    virtuals.config_virtuals(plant)
+    session.commit()
+    return plant
 
 
 @requires_demo_data
-def add_demo_data(plant: cmp.Plant, session: Session = None, tz: str = 'UTC'):
+def add_demo_data(plant: cmp.Plant, session: Session = None):
+    files = [sunpeek.demo.DEMO_DATA_PATH_1MONTH]
+    timezone = 'UTC'
+    datetime_template = data_uploader.DatetimeTemplates.year_month_day
+
     if session is not None:
-        up = data_uploader.DataUploader_db(plant=plant,
-                                           files=[sunpeek.demo.DEMO_DATA_PATH_1MONTH],
-                                           timezone=tz,
-                                           session=session)
-        up.do_upload()   # includes virtual sensor calculation
+        up = data_uploader.DataUploader_pq(plant=plant,
+                                           timezone=timezone,
+                                           datetime_template=datetime_template,
+                                           )
+        up.do_upload(files=files)  # includes virtual sensor calculation
     else:
-        plant.use_csv(csv_files=[sunpeek.demo.DEMO_DATA_PATH_1MONTH], timezone=tz)  # includes virtual sensor calculation
+        use_csv(plant, csv_files=files,
+                timezone=timezone,
+                datetime_template=datetime_template)
```

## sunpeek/demo/demo_plant_script.py

```diff
@@ -1,53 +1,53 @@
 """
 This module holds an example to show the functionality of the SunPeek package and the Performance Check method.
 
 The Python code shows how to configure the plant / collector array, call the Performance Check method (ISO 24194) and
 produce some plots. 
 This script is based on the FHW / Fernheizwerk plant in Graz, Austria.
-# TODO Add reference to Zenodo / data-in-brief, once available
+The data used here (together with a detailed description) is available at https://zenodo.org/record/7741084
 
 .. codeauthor:: Philip Ohnewein <p.ohnewein@aee.at>
 .. codeauthor:: Marnoch Hamilton-Jones <m.hamilton-jones@aee.at>
 .. codeauthor:: Daniel Tschopp <d.tschopp@aee.at>
 """
 
 import json
 import warnings
 from datetime import datetime
 import webbrowser
 
 import sunpeek.demo
+from sunpeek.data_handling.wrapper import use_csv
 from sunpeek.demo.demo_plant import requires_demo_data
-import sunpeek.core_methods.pc_method as pc
+from sunpeek.core_methods.pc_method.wrapper import run_performance_check
+from sunpeek.core_methods.pc_method import plot_all
 from sunpeek.common.unit_uncertainty import Q
 from sunpeek.common import config_parser
-from sunpeek.components import CollectorTypeQDT, iam_methods
-from sunpeek.components import FluidFactory, WPDFluidDefinition, ModelFactory, CoolPropFluid
-from sunpeek.definitions.fluid_definitions import get_definition
+from sunpeek.common.utils import DatetimeTemplates
+from sunpeek.components import CollectorTypeQDT, iam_methods, FluidFactory, CoolPropFluid
+from sunpeek.definitions.fluid_definitions import get_definition, WPDFluids
 
 
-def get_fluid(fluid_str='FHW'):
-    """Return heat transfer fluid: 'FHW' for FHW fluid, other options to see how other fluids would behave.
+def get_fluid(fluid_str: str = WPDFluids.fhw_pekasolar.value.name):
+    """Return heat transfer fluid: Default is fluid of FHW plant. Choose other fluid to see how they would behave.
     """
-    if fluid_str == 'FHW':
+    if fluid_str == WPDFluids.fhw_pekasolar.value.name:
         # FHW laboratory-tested fluid, with property models trained from csv files
-        rho_model = ModelFactory(unit={'te': 'degC', 'out': 'kg m**-3'}).train(sunpeek.demo.DEMO_FLUID_RHO_PATH)
-        cp_model = ModelFactory(unit={'te': 'degC', 'out': 'J g**-1 K**-1'}).train(sunpeek.demo.DEMO_FLUID_CP_PATH)
-        return FluidFactory(fluid=WPDFluidDefinition('FHW, Pekasolar', rho_model, cp_model))
+        return FluidFactory(fluid=get_definition(fluid_str))
+
     # Examples of CoolProp fluids
-    elif fluid_str.lower() == 'water':
-        return CoolPropFluid(get_definition('water'))
-    else:
-        fluid = CoolPropFluid(get_definition(fluid_str), concentration=Q(40, 'percent'))
+    if fluid_str.lower() == 'water':
+        return FluidFactory(fluid=get_definition('water'))
+
+    fluid = CoolPropFluid(get_definition(fluid_str), concentration=Q(40, 'percent'))
 
     if fluid is not None:
         return fluid
-    else:
-        raise ValueError(f'Unknown CoolProp fluid string "{fluid_str}".')
+    raise ValueError(f'Unknown fluid string "{fluid_str}".')
 
 
 def get_collector():
     """Return collector definition of flat plate collector used in collector array
     """
     return CollectorTypeQDT(name="Arcon 3510",
                             manufacturer_name="Arcon-Sunmark A/S",
@@ -86,20 +86,28 @@
     plant.fluid_solar = get_fluid()
     # This is just to showcase how other fluids would be used:
     # plant.fluid_solar = get_fluid('water')
     # plant.fluid_solar = get_fluid('ASHRAE, Propylene Glycol')
     # plant.fluid_solar = get_fluid('Antifrogen L')
 
     # STEP 2: Submit measurement data
-    # data_output = plant.use_csv(sunpeek.demo.DEMO_DATA_PATH_2DAYS, timezone='UTC')
-    data_output = plant.use_csv(sunpeek.demo.DEMO_DATA_PATH_1MONTH, timezone='UTC')
+    # data = sunpeek.demo.DEMO_DATA_PATH_2DAYS
+    data = sunpeek.demo.DEMO_DATA_PATH_1MONTH
+    # data = sunpeek.demo.DEMO_DATA_PATH_1YEAR
+    data_output = use_csv(plant, csv_files=[data], timezone='UTC', datetime_template=DatetimeTemplates.year_month_day)
 
     # STEP 3: Run Performance Check method & create plots
-    pc_output = pc.PCMethod.create_improved(plant=plant, equation_id=2).run()
-    # pc_output = pc.PCMethod.create_iso(plant=plant, equation_id=2).run()
+    # Use default settings:
+    pc_output = run_performance_check(plant).output
+    # or try specific settings:
+    # pc_output = run_performance_check(plant,
+    #                                   method=['extended'],
+    #                                   equation=[2],
+    #                                   safety_uncertainty=0.9,
+    #                                   ).output
 
     try:
-        pc.plot_all(pc_output)
+        plot_all(pc_output)
     except webbrowser.Error:
         warnings.warn('Cannot plot results, no runnable browser detected')
     except ModuleNotFoundError:
         warnings.warn('Cannot plot results, module plotly not installed')
```

## sunpeek/exporter.py

```diff
@@ -1,16 +1,23 @@
+import json
 import tarfile, tempfile, io, time, os
 import pandas as pd
 import sqlalchemy
 import sqlalchemy.orm
+from typing import Union
+import platform
+import parquet_datastore_utils as pu
 
+import sunpeek
 import sunpeek.components as cmp
+import sunpeek.common
 from sunpeek.components.helpers import ResultStatus
 import sunpeek.serializable_models as smodels
 from sunpeek.db_utils import db_data_operations, crud
+# from sunpeek.db_utils import DATETIME_COL_NAME
 
 
 def create_export_config(plant):
 
     collectors = [array.collector_type for array in plant.arrays]
     sensor_types = [sensor.sensor_type for sensor in plant.raw_sensors if sensor.sensor_type is not None]
     fluid_definitions = [plant.fluid_solar.fluid]
@@ -30,16 +37,19 @@
         info.mtime = time.time()
         conf_file.seek(0)
         tf.addfile(tarinfo=info, fileobj=conf_file)
 
         for year in years:
             start = index[str(year)][0]
             end = index[str(year)][-1]
-            df = db_data_operations.get_sensor_data(session.bind.raw_connection(), sensors, plant.raw_table_name,
-                                                   start_timestamp=start, end_timestamp=end)
+            df_raw = pu.read(uri=plant.raw_data_path,
+                             columns=[sensor.raw_name for sensor in sensors if not sensor.is_virtual])
+            df_calc = pu.read(uri=plant.calc_data_path,
+                              columns=[sensor.raw_name for sensor in sensors if sensor.is_virtual])
+            df = pd.concat([df_raw, df_calc], axis=1)
             f = io.BytesIO()
             df.to_csv(f, sep=';')
             info = tarfile.TarInfo(name=f"rawdata_{plant.name}_{year}.csv")
             info.size = len(f.getbuffer())
             info.mtime = time.time()
             f.seek(0)
             tf.addfile(tarinfo=info, fileobj=f)
@@ -52,17 +62,17 @@
     if job:
         setattr(job, attr, value)
     return job
 
 
 def create_export_package(plant: cmp.Plant, include_virtuals: bool, job: cmp.Job=None):
     if include_virtuals:
-        sensors = [sensor.raw_name.lower() for sensor in plant.raw_sensors if not sensor.is_virtual]
+        sensors = [sensor for sensor in plant.raw_sensors if not sensor.is_virtual]
     else:
-        sensors = [sensor.raw_name.lower() for sensor in plant.raw_sensors]
+        sensors = [sensor for sensor in plant.raw_sensors]
 
     session = sqlalchemy.orm.object_session(plant)
 
     job = _update_job(job, 'status', ResultStatus.running)
     crud.update_component(session, job)
 
     try:
@@ -72,7 +82,81 @@
         job = _update_job(job, 'status', ResultStatus.done)
         job = _update_job(job, 'result_path', temp_path)
         crud.update_component(session, job)
         return temp_path
     except:
         _update_job(job, 'status', ResultStatus.failed)
         raise
+
+
+def _get_plants_config(plants):
+    confs = []
+    for plant in plants:
+        confs.append(json.loads(smodels.Plant.from_orm(plant).json())) #Ensure we can convert to json later if needed
+    return confs
+
+
+def dump_debug_info(include_plants: Union[bool, list] = True, include_db_structure: bool = True, file_path: str = None,
+                    session: sqlalchemy.orm.Session = None):
+    """
+    Creates a file in memory containing various information that is useful for reproducing issues for debugging purposes.
+    Can optionally write this to disk or return the file object.
+
+    Parameters
+    ----------
+    include_plants : bool or list of plant names
+        True to include all plants, False for none or specify the names of specific plants to include
+    include_db_structure : bool
+        Whether to include a list of database tables and their columns. If include_plants is a list, only raw data
+        tables for plants listed will be included
+    file_path : str
+       An optional path to write the output to. If this is given, the absolute path to the output file will be returned.
+    session : sqlalchemy.orm.Session
+       An optional database session object, required if include_plants or include_db_structure is True
+
+    Returns
+    -------
+    out : dict or absolute output file path as str
+    """
+
+    out = {}
+    out['version'] = sunpeek.__version__
+    out['platform'] = platform.platform()
+    out['architecture'] = platform.architecture()
+    out['in_docker'] = os.path.exists('/.dockerenv')
+
+    if session is None and (include_db_structure or include_plants):
+        raise TypeError('include_db_structure or include_plants was True with session set to None. '
+                        'Need a valid database session to get plant or database structure information.')
+    elif session is None:
+        return out
+
+    include_plants_is_list = False
+    if include_plants:
+        plants = session.query(cmp.Plant).all()
+        out['plant_configurations'] = _get_plants_config(plants)
+    else:
+        try:
+            plants = [session.query(cmp.Plant).where(cmp.Plant.name == name).one() for name in include_plants]
+            out['plant_configurations'] = _get_plants_config(plants)
+            include_plants_is_list = True
+        except TypeError:
+            pass
+
+    if include_db_structure:
+        db_tables = {}
+        metadata = sqlalchemy.MetaData()
+        metadata.reflect(sunpeek.common.utils.db_engine)
+        for table in metadata.tables.values():
+            if include_plants_is_list and 'raw_data' in table.name and any([plant_name in table.name for plant_name in include_plants]):
+                continue
+            if not include_plants and 'raw_data' in table.name:
+                continue
+            db_tables[table.name] = {'columns': [col.name for col in table.columns]}
+        out['database_tables'] = db_tables
+
+    if file_path is None:
+        return out
+    else:
+        with open(file_path, 'w') as f:
+            json.dump(out, f)
+    return os.path.abspath(file_path)
```

## sunpeek/serializable_models.py

```diff
@@ -1,35 +1,37 @@
 import datetime
 import uuid
+import enum
+from dataclasses import field
+from pydantic.dataclasses import dataclass
 import numpy as np
 from pydantic import validator, constr
-from typing import Union, Dict, List
+from typing import Union, Any, Dict, List
 import pint.errors
 
 import sunpeek.components as cmp
-import sunpeek.components.helpers
+from sunpeek.common.unit_uncertainty import Q
 from sunpeek.components.base import IsVirtual
-from sunpeek.components.helpers import SensorMap
+from sunpeek.components.helpers import SensorMap, DatetimeTemplates, AccuracyClass, InstallCondition
+from sunpeek.components.fluids import UninitialisedFluid
 from sunpeek.base_model import BaseModel
-from sunpeek.common.unit_uncertainty import Q
 
-#Needed to allow con
-from sunpeek.components.types import SensorType
-from sunpeek.components.base import SensorSlot
-from sunpeek.common.data_uploader import DataUploadResponse, DataUploadResponseFile
 
 class ComponentBase(BaseModel):
     sensor_map: Union[Dict[str, Union[str, None]], None]
 
     @validator('sensor_map', pre=True)
     def get_raw_name(cls, v):
         out = {}
         for key, item in v.items():
             if isinstance(item, SensorMap):
-                out[key] = item.sensor.raw_name
+                try:
+                    out[key] = item.sensor.raw_name
+                except AttributeError:
+                    pass
             else:
                 out[key] = item
         return out
 
 
 def np_to_list(val):
     if isinstance(val, np.ndarray) and val.ndim == 1:
@@ -155,54 +157,53 @@
 
 class CollectorTypeSST(CollectorTypeBase):
     ceff: Quantity
 
 
 class SensorBase(BaseModel):
     description: Union[str, None]
-    accuracy_class: Union[sunpeek.components.helpers.AccuracyClass, None]
-    installation_condition: Union[sunpeek.components.helpers.InstallCondition, None]
+    accuracy_class: Union[AccuracyClass, None]
+    installation_condition: Union[InstallCondition, None]
     info: Union[dict, None] = {}
     raw_name: Union[str, None]
     native_unit: Union[str, None]
 
     @validator('info', pre=True)
     def convert_info(cls, v):
         if isinstance(v, cmp.SensorInfo):
             return v._info
         return v
 
-    @validator('raw_name', pre=True)
-    def sanitize_name(cls, v):
-        if isinstance(v, str):
-            return v.strip()
-        return v
-
     @validator('native_unit', pre=True)
     def check_unit(cls, v):
         if isinstance(v, str):
             Q(1, v)
 
         return v
 
 
+
 class Sensor(SensorBase):
     id: Union[int, None]
     plant_id: Union[int, None]
     raw_name: Union[str, None]
     sensor_type: Union[str, None]
     native_unit: Union[str, None]
+    formatted_unit: Union[str, None]
     is_virtual: Union[bool, None]
+    can_calculate: Union[bool, None]
+    is_mapped: Union[bool, None]
 
     @validator('sensor_type', pre=True)
     def convert_sensor_type(cls, v):
         if isinstance(v, cmp.SensorType):
             return v.name
         return v
 
+
 class NewSensor(SensorBase):
     raw_name: str
     native_unit: str = None
 
 
 class BulkUpdateSensor(Sensor):
     id: int
@@ -219,23 +220,23 @@
     hc_model_sha1: Union[str, None]
     heat_capacity_unit_te: Union[str, None]
     heat_capacity_unit_out: Union[str, None]
     heat_capacity_unit_c: Union[str, None]
     density_unit_te: Union[str, None]
     density_unit_out: Union[str, None]
     density_unit_c: Union[str, None]
-    heat_capacity_onnx: Union[str, None]
-    density_onnx: Union[str, None]
+    # heat_capacity_onnx: Union[str, None]
+    # density_onnx: Union[str, None]
 
-    @validator('heat_capacity_onnx', 'density_onnx', pre=True)
-    def onnx_to_str(cls, v):
-        try:
-            return v.hex()
-        except AttributeError:
-            return v
+    # @validator('heat_capacity_onnx', 'density_onnx', pre=True)
+    # def onnx_to_str(cls, v):
+    #     try:
+    #         return v.hex()
+    #     except AttributeError:
+    #         return v
 
 
 class Fluid(BaseModel):
     id: Union[int, None]
     name: Union[str, None]
     manufacturer_name: Union[str, None]
     product_name: Union[str, None]
@@ -287,38 +288,53 @@
 class NewArray(Array):
     name: str
     collector_type: str
     sensors: Union[Dict[str, NewSensor], None]
     sensor_map: Union[dict, None]
 
 
+class DataUploadDefaults(BaseModel):
+    id: Union[int, None]
+    datetime_template: Union[DatetimeTemplates, None]
+    datetime_format: Union[str, None]
+    timezone: Union[str, None]
+    csv_separator: Union[str, None]
+    csv_decimal: Union[str, None]
+    csv_encoding: Union[str, None]
+    index_col: Union[int, None]
+
+
 class PlantBase(ComponentBase):
     owner: Union[str, None]
     operator: Union[str, None]
     description: Union[str, None]
     location_name: Union[str, None]
     altitude: Union[Quantity, None]
     fluid_solar: Union[FluidSummary, str, None]
     arrays: Union[List[Array], None]
     fluid_vol: Union[Quantity, None]
     raw_sensors: Union[List[Sensor], None]
 
     @validator('fluid_solar', pre=True)
     def convert_fluid(cls, v):
         if isinstance(v, cmp.Fluid):
+            if isinstance(v, UninitialisedFluid):
+                return FluidSummary(name=v.fluid_def_name, fluid=v.fluid_def_name, concentration=None)
             return FluidSummary(name=v.name, fluid=v.fluid.name, concentration=getattr(v, 'concentration', None))
         return v
 
 
 class Plant(PlantBase):
     name: Union[str, None]
     id: Union[int, None]
     latitude: Union[Quantity, None]
     longitude: Union[Quantity, None]
     fluid_solar: Union[FluidSummary, str, None]
+    local_tz_string_with_DST: Union[str, None]
+    data_upload_defaults: Union[DataUploadDefaults, None]
 
 
 class UpdatePlant(Plant):
     sensors: Union[Dict[str, NewSensor], None]
     fluid_solar: Union[FluidSummary, None]
 
 
@@ -413,72 +429,85 @@
     #              descriptive_name: str,
     #              virtual: Union[IsVirtual, str],
     #              description: str = None):
     #     super().__init__(name=name, sensor_type=sensor_type, descriptive_name=descriptive_name, virtual=virtual,
     #                      description=description)
 
 
+class PCMethodOutputPlant(BaseModel):
+    id: Union[int, None]
+    plant: Plant
+
+    n_intervals: Union[int, None]
+    datetime_intervals_start: Union[List[datetime.datetime], None]
+    datetime_intervals_end: Union[List[datetime.datetime], None]
+
+    tp_measured: Union[Quantity, None]
+    tp_sp_measured: Union[Quantity, None]
+    tp_sp_estimated: Union[Quantity, None]
+    tp_sp_estimated_safety: Union[Quantity, None]
+    mean_tp_sp_measured: Union[Quantity, None]
+    mean_tp_sp_estimated: Union[Quantity, None]
+    mean_tp_sp_estimated_safety: Union[Quantity, None]
+
+    target_actual_slope: Union[Quantity, None]
+    target_actual_slope_safety: Union[Quantity, None]
+
+    fluid_solar: Union[FluidSummary, None]
+    mean_temperature: Union[Quantity, None]
+    mean_fluid_density: Union[Quantity, None]
+    mean_fluid_heat_capacity: Union[Quantity, None]
+
+    @validator('datetime_intervals_start', 'datetime_intervals_end', pre=True)
+    def array_to_list(cls, val):
+        if isinstance(val, np.ndarray):
+            return list(val)
+
+
 class PCMethodOutputArray(BaseModel):
     id: Union[int, None]
     array: Array
+
     tp_sp_measured: Union[Quantity, None]
-    tp_sp_expected: Union[Quantity, None]
-    tp_sp_expected_safety: Union[Quantity, None]
+    tp_sp_estimated: Union[Quantity, None]
+    tp_sp_estimated_safety: Union[Quantity, None]
+    mean_tp_sp_measured: Union[Quantity, None]
+    mean_tp_sp_estimated: Union[Quantity, None]
+    mean_tp_sp_estimated_safety: Union[Quantity, None]
 
 
 class PCMethodOutput(BaseModel):
     id: Union[int, None]
     plant: PlantSummary
 
     datetime_eval_start: datetime.datetime
     datetime_eval_end: datetime.datetime
 
     # Algorithm settings
     pc_method_name: str
     evaluation_mode: str
     equation: int
-    check_accuracy_level: int
-
-    interval_length: Union[datetime.timedelta, None]
-    safety_combined: Union[float, None]
     wind_used: bool
 
-    max_nan_density: Union[float, None]
-    min_data_in_interval: Union[int, None]
-    max_gap_in_interval: Union[datetime.timedelta, None]
-
     # Results
-    n_intervals: Union[int, None]
-
-    datetime_intervals_start: Union[List[datetime.datetime], None]
-    datetime_intervals_end: Union[List[datetime.datetime], None]
-
-    # Plant results
-    tp_measured: Union[Quantity,None]
-    tp_sp_measured: Union[Quantity, None]
-    tp_sp_expected: Union[Quantity,None]
-    tp_sp_expected_safety: Union[Quantity, None]
+    settings: Dict[str, Any]  # Type checking done in PCSettings
+    plant_output: PCMethodOutputPlant
+    array_output: List[PCMethodOutputArray]
 
-    target_actual_slope: Union[Quantity, None]
-    target_actual_slope_safety: Union[Quantity, None]
 
-    # Array results
-    array_results: List[PCMethodOutputArray]
+class OperationalEvent(BaseModel):
+    id: Union[int, None]
+    plant: Union[str, PlantSummary]
+    event_start: datetime.datetime
+    event_end: Union[datetime.datetime, None]
+    ignored_range: bool = False
+    description: Union[str, None]
+    original_timezone: Union[str, None]
 
-    fluid_solar: Union[FluidSummary, None]
-    mean_temperature: Union[Quantity, None]
-    mean_fluid_density: Union[Quantity, None]
-    mean_fluid_heat_capacity: Union[Quantity, None]
 
-    @validator('datetime_intervals_start', 'datetime_intervals_end', pre=True)
-    def array_to_list(cls, val):
-        if isinstance(val, np.ndarray):
-            return list(val)
-            
-            
 # def dataclass_to_pydantic(cls: dataclasses.dataclass, name: str) -> BaseModel:
 #     # get attribute names and types from dataclass into pydantic format
 #     pydantic_field_kwargs = dict()
 #     for _field in dataclasses.fields(cls):
 #         # check is field has default value
 #         if isinstance(_field.default, dataclasses._MISSING_TYPE):
 #             # no default
@@ -491,7 +520,153 @@
 #
 #         except AttributeError:
 #             pass
 #
 #         pydantic_field_kwargs[ _field.name] = (_field.type, default)
 #
 #     return pydantic.create_model(name, **pydantic_field_kwargs, __base__=BaseModel)
+
+
+class ProblemType(str, enum.Enum):
+    component_slot = 'Component slot'
+    component_attrib = 'Component attribute'
+    sensor_info = 'Sensor info'
+    component_missing = 'Component missing'
+    other_problem = 'Unspecified problem'
+    unexpected_in_calc = 'Unexpected calculation error'
+    unexpected_getting_problems = 'Unexpected error getting problem report'
+
+
+@dataclass
+class AlgoProblem:
+    """A pydantic class used to hold information on a problem / missing info for a calculation / CoreStrategy.
+    Can be used to track problems / missing information back to the root cause.
+
+    Parameters
+    ----------
+    problem_type : ProblemType enum
+    affected_component : ComponentBase, optional
+        The component where some problem occurs / information is missing.
+    affected_item_name : str, optional
+        Typically the name of the affected sensor slot or attribute of the affected component.
+    description : str, optional
+    """
+    problem_type: ProblemType
+    affected_component: Union[Plant, Array, None] = None
+    affected_item_name: Union[str, None] = None
+    description: Union[str, None] = None
+
+
+@dataclass
+class ProblemReport:
+    """Standardized reporting of problems / missing information required to perform some calculation.
+
+    This applies to all calculations in SunPeek, i.e. both virtual sensors and other calculations e.g. PC method.
+    Any CoreStrategy and CoreAlgorithm holds / can return a ProblemReport which holds structured information as to
+    what problems / missing information there is that prevents the strategy / algo to complete.
+
+    ProblemReport implements an n-level tree, where each node (ProblemReport) has n leaves (own_problems) and points
+    at m other nodes (sub_problems). sub_problems are implemented as dict with key == strategy name.
+
+    Parameters
+    ----------
+    success : bool, optional, default True
+        True if the algo or strategy holding / producing the problem report is successful, meaning that at least
+        parts of its results can be calculated and / or only optional information is missing.
+    own_problems : List[AlgoProblem], optional
+        List of reported problems that affect the algo / strategy itself (as opposed to problems coming from called /
+        sub algorithms). Example: Strategy needs some component attribute, but that attribute is None.
+    sub_reports : Dict[str, ProblemReport], optional
+        Problems that are not directly associated to the algo / strategy holding this ProblemReport, but rather stem
+        from a previous calculation / strategy. Example: Strategy needs some virtual sensor, but that had its own
+        problems, reported as a ProblemReport.
+    problem_slots : List[str], optional
+        Set by virtual sensor strategies, problem_slots can be used to report partial success, i.e.:
+        If a strategy is successful for some but not all virtual sensors, the success flag can be set to True,
+        and the ProblemReport applies only to the virtual sensor slot names which cannot be calculated,
+        i.e. the problem_slots.
+    """
+    success: Union[bool, None] = True
+    own_problems: Union[List[AlgoProblem], None] = None
+    sub_reports: Union[Dict[str, 'ProblemReport'], None] = None
+    problem_slots: Union[List[str], None] = field(default_factory=list)  # Used if some virtual sensors / slots fail
+
+    @property
+    def successful_strategy_str(self) -> Union[str, None]:
+        """Loop through strategies, return name of first successful strategy, or None if no strategy was successful.
+        """
+        if not self.success:
+            return None
+        for strategy_name, problem in self.sub_reports.items():
+            if problem.success:
+                return strategy_name
+        return None
+
+    def add_own(self, algo_problem: AlgoProblem):
+        lst = [] if self.own_problems is None else self.own_problems
+        lst.append(algo_problem)
+        self.own_problems = lst
+        self.success = False
+
+    def add_sub(self, strategy_name: str, problem_report: 'ProblemReport'):
+        dct = {} if self.sub_reports is None else self.sub_reports
+        dct.update({strategy_name: problem_report})
+        self.sub_reports = dct
+        self.success = False
+
+    def parse(self, include_successful_strategies: bool = False, include_problem_slots: bool = True) -> str:
+        def parse_problem(algo_problem: AlgoProblem) -> str:
+            result = f'- {algo_problem.problem_type.value}: '
+            if algo_problem.affected_item_name is not None:
+                # result += f'item "{algo_problem.affected_item_name}" '
+                result += f'"{algo_problem.affected_item_name}" '
+            if algo_problem.affected_component is not None:
+                result += f'in {algo_problem.affected_component.__class__.__name__} "{algo_problem.affected_component.name}"'
+                # result += f'in component "{algo_problem.affected_component.name}"'
+            if algo_problem.description is not None:
+                result += f': {algo_problem.description}'
+            else:
+                result += '.'
+            result = '\n' + result if result else ''
+            return result
+
+        def parse_sub_reports(reports: Dict[str, 'ProblemReport']) -> str:
+            # Recursive walk through the problem reports of all strategies (strategy name is dict key).
+            result = ''
+            for strategy_name, problem_report in reports.items():
+                include_slots = self.problem_slots and include_problem_slots
+                skip = problem_report.success and not include_successful_strategies and not include_slots
+                # if problem_report.success and include_successful_strategies:
+                if skip:
+                    continue
+                if not problem_report.success:
+                    sub = problem_report.parse(include_successful_strategies, include_problem_slots)
+                else:
+                    if not self.problem_slots:
+                        sub = ' No problems found.'
+                    else:  # partial success, some virtual sensors missing
+                        sub = f'Some virtual sensors could not be calculated: {", ".join(self.problem_slots)}. '
+                        # if not problem_report.no_problems:
+                        sub += problem_report.parse(include_successful_strategies, include_problem_slots)
+                result += '\n' if result else ''
+                result += f'Strategy "{strategy_name}":{sub}'
+            return result
+
+        result = ''
+        if self.own_problems is not None:
+            for algo_problem in self.own_problems:
+                result += parse_problem(algo_problem)
+
+        if self.sub_reports is not None:
+            result += parse_sub_reports(self.sub_reports)
+
+        return result
+
+
+# Goal = Report success / problems of a specific PC method strategy.
+@dataclass
+class PCMethodProblem:
+    evaluation_mode: str
+    equation: int
+    wind_used: bool
+    success: bool
+    problem_str: str
```

## Comparing `sunpeek/components/fluid_helpers.py` & `sunpeek/components/fluids_wpd_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,370 +1,338 @@
+from typing import Union
 import warnings
-
-import numpy as np
+from pathlib import Path
 from abc import ABC, abstractmethod
+import numpy as np
+import pandas as pd
+import numbers
+
 from sklearn.preprocessing import PolynomialFeatures, StandardScaler
 from sklearn.linear_model import Ridge
 from sklearn.pipeline import make_pipeline
 from sklearn.model_selection import GridSearchCV, ShuffleSplit
-from skl2onnx import convert_sklearn
-from skl2onnx.common.data_types import FloatTensorType
-import onnxruntime as rt
-import pandas as pd
-import os
+from sunpeek.definitions import FluidProps, fluid_data_dir
+
+
+class ModelFactory:
 
+    @classmethod
+    def from_info_and_property(cls, fluid_info: 'sunpeek.definitions.fluid_definitions.WPDFluidInfo', prop: FluidProps):
+        fn = fluid_data_dir / fluid_info.name / prop.value
+        csv_file = fn.with_suffix('.csv')
+
+        unit = fluid_info.unit_density if prop == FluidProps.density else fluid_info.unit_heat_capacity
+
+        return ModelFactory(unit=unit,
+                            is_pure=fluid_info.is_pure,
+                            csv_file=csv_file)
+
+    def __new__(cls, unit: dict = None,
+                is_pure: bool = None,
+                csv_file: Union[str, Path] = None,
+                df: pd.DataFrame = None):
+        """Returns an instance of a trained WPDModel.
+
+        Returns a pure fluid model (WPDModelPure) if unit has only 2 entries (output, temperature),
+        otherwise if unit has 3 entries (output, temperature, concentration) a mixed fluid model (WPDFluidMixed).
+        This method also trains the model (= fits a sklearn model), based on the given df or csv_file.
 
-class ModelFactory():
-    def __new__(cls, unit=None, onnx_file=None, onnx_model=None, onnx_model_bytes=None, is_pure=None):
-        """Returns an instance of WPDModel, WPDModelPure or WPDModelMixed, depending on provided units.
         Parameters
         ----------
         unit : dict
             Units for inputs and outputs of the fluid model.
             Must have keys 'te' and 'out', optionally 'c' (then a WPDModelMixed is returned).
             Values must be valid pint unit strings.
-        onnx_file : str
-            Path to stored, trained ONNX file.
+        is_pure : bool
+            True if unit
+        csv_file : str, Path
+            Data file used to train the model. Usually, this is a WebPlotDigitizer export csv file.
+            Is expected to have multiple datasets, one for each concentration level.
+        df: pd.DataFrame
+            Is used to train the model.
 
         Raises
         ------
         TypeError
             If unit is not a dict.
         KeyError
             If required keys 'te' and 'out' are not found, or dictionary has extra keys not 'te', 'c' or 'out'.
         """
-        if not isinstance(unit, dict):
-            raise TypeError('Parameter unit expected to be dictionary.')
-        if len(unit) == 2:
-            if set(unit.keys()) != {'te', 'out'}:
-                raise KeyError('Keys "te" and "out" not in unit dict.')
-        elif len(unit) == 3:
-            if set(unit.keys()) != {'te', 'c', 'out'}:
-                raise KeyError('Keys "te", "c" and "out" not in unit dict.')
-        else:
-            raise KeyError('Mismatched unit dict. Must have keys "te" and "out" and optionally "c" (for mixed fluids).')
 
-        if len(unit) == 2 or is_pure:
-            model = WPDModelPure(unit)
-        else:
-            model = WPDModelMixed(unit)
+        model = WPDModelPure(unit) if is_pure else WPDModelMixed(unit)
+
+        # Make sure either df or csv_file is given
+        has_df = df is not None
+        has_file = csv_file is not None
+        if not (has_df ^ has_file):
+            raise ValueError(
+                'Model training accepts either a raw data file or a DataFrame. None or both of them were given.')
+
+        # Train model
+        model.df = df if has_df else model.csv2df(csv_file)
+        model.sk_model = model.train()
 
-        if onnx_file is not None:
-            model._onnx_file = onnx_file
-        if onnx_model is not None:
-            model.onnx_model = onnx_model.SerializeToString()
-        if onnx_model_bytes is not None:
-            model.onnx_model = onnx_model_bytes
         return model
 
 
 class WPDModel(ABC):
     """
     Model for a particular property of a fluid, e.g. for density or for heat capacity.
-    Has an ONNX filename and the units for all inputs (temperature, optionally concentration) and the calculated output.
+    # Has an ONNX filename and the units for all inputs (temperature, optionally concentration) and the calculated output.
+    Has the units for all inputs (temperature, optionally concentration) and the calculated output.
     Can read WebPlotDigitizer csv files, train sklearn fit, save trained model as ONNX file and make predictions.
     Attributes
     ----------
     unit : dict
         Units for temperature ['te'], optionally concentration ['c'] and (mandatory) output property ['out'].
         Must be valid pint unit strings. These units are sent to the trained model if a prediction is required,
         and the prediction output is interpreted in unit['out'].
-    _onnx_file : str
-        Filename where trained sklearn is stored as an ONNX model.
     """
 
-    _INPUT_NAME = 'wpd_input'
+    n_inputs = None
+    predictor_cols_in = []
+    predictor_col_out = 'out'
 
     def __init__(self, unit):
-        self.unit = unit
-        self._csv_file = None
-        self._onnx_file = None
-        self._df = None
-        self.onnx_model = None
-
-    @property
-    def csv_file(self):
-        if self._csv_file is None:
-            raise TypeError('self._csv_file is None. You have to call train(csv_file).')
-        return self._csv_file
-
-    @property
-    def onnx_file(self):
-        if self._onnx_file is None:
-            raise TypeError('self._onnx_file is None. You have to call train() before predict().')
-        return self._onnx_file
-
-    def train(self, csv_file, **kwargs):
-        """
-        Fits polynomial interpolation from WebPlotDigitizer exported csv data, returns fitted ONNX model.
-        ONNX model is stored in same folder as csv_file and has same filename, but extension ".onnx"
-
-        Parameters
-        ----------
-        csv_file : str
-            WebPlotDigitizer export csv file. is expected to have multiple datasets, one for each concentration level.
-        kwargs :
-            Keyword arguments that will be passed to self.fit().
+        if len(unit) != 1 + self.n_inputs:
+            raise ValueError(f'Unit dictionary of fluid definition must have length {self.n_inputs}, '
+                             f'the units for output (e.g. density), temperature, and concentration (for mixed fluids).')
+
+        expected_cols = set(['out'] + self.predictor_cols_in)
+        if set(unit.keys()) != expected_cols:
+            raise KeyError(f'Missing or mismatched keys in unit dictionary. Required keys: {", ".join(expected_cols)}.')
 
-        Returns
-        -------
-        Filename where ONNX model was stored.
-        """
-        self._csv_file = csv_file
-        self.csv2df()
-        sk_model = self.fit(**kwargs)
-        # self._onnx_file = self.sk2onnx(sk_model)
-        onnx = convert_sklearn(sk_model, initial_types=self.sk_initial_type())
-        self.onnx_model = onnx.SerializeToString()
-        return self
+        self.unit = unit
+        self.df = None
+        self.sk_model = None
 
-    def fit(self, degree_range=None):
-        """
-        Polynomial interpolation with grid-search cross-validation of interpolation coefficients.
-        Inspired by https://stackoverflow.com/questions/47442102/how-to-find-the-best-degree-of-polynomials
+    def train(self, fit_type: str = 'polynomial'):
+        """Fits polynomial interpolation model to fluid raw data in df.
 
         Parameters
         ----------
-        degree_range : int
-            Miniumum and maximum polynomial degrees.
+        fit_type : str
+            Type of sklearn fit. Currently, only 'polynomial' implemented, works good enough.
 
         Returns
         -------
         Trained sklearn model.
         """
-        if degree_range is None:
-            degree_range = np.arange(2, 4)  # default: quadratic or cubic polynomials
-        # pipe = make_pipeline(PolynomialFeatures(), LinearRegression())
+        if fit_type == 'polynomial':
+            # Polynomial interpolation with grid-search cross-validation of interpolation coefficients.
+            # Inspired by https://stackoverflow.com/questions/47442102/how-to-find-the-best-degree-of-polynomials
+            degree_range = np.arange(2, 4)  # quadratic or cubic polynomials
+            pipe = make_pipeline(StandardScaler(), PolynomialFeatures(), Ridge(alpha=1e-3))
+            param_grid = {'polynomialfeatures__degree': degree_range}
+            # grid = GridSearchCV(pipe, param_grid, cv=20)
+            # grid = GridSearchCV(pipe, param_grid, cv=20, scoring='neg_mean_absolute_error')
+            # grid = GridSearchCV(pipe, param_grid, cv=LeaveOneOut(), scoring='neg_mean_absolute_error')
+            grid = GridSearchCV(pipe, param_grid, cv=ShuffleSplit(n_splits=10), scoring='neg_mean_absolute_error')
 
+        # elif fit_type == 'spline':
+        # # SplineTransformer not supported in ONNX conversion
         # Spline & ridge regression: Would be an interesting option, but currently not convertible to onnx.
         # https://scikit-learn.org/stable/auto_examples/linear_model/plot_polynomial_interpolation.html#sphx-glr-auto-examples-linear-model-plot-polynomial-interpolation-py
         # pipeline example: https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.SplineTransformer.html#sklearn.preprocessing.SplineTransformer
-
-        # pipe = make_pipeline(StandardScaler(), PolynomialFeatures(), LinearRegression())
-        # param_grid = {'polynomialfeatures__degree': degree_range}
-        # # grid = GridSearchCV(pipe, param_grid, cv=20)
-        # # grid = GridSearchCV(pipe, param_grid, cv=20, scoring='neg_mean_absolute_error')
-        # # grid = GridSearchCV(pipe, param_grid, cv=LeaveOneOut(), scoring='neg_mean_absolute_error')
-        # grid = GridSearchCV(pipe, param_grid, cv=ShuffleSplit(n_splits=10), scoring='neg_mean_absolute_error')
-
-        pipe = make_pipeline(StandardScaler(), PolynomialFeatures(), Ridge(alpha=1e-3))
-        param_grid = {'polynomialfeatures__degree': degree_range}
-        # grid = GridSearchCV(pipe, param_grid, cv=20)
-        # grid = GridSearchCV(pipe, param_grid, cv=20, scoring='neg_mean_absolute_error')
-        # grid = GridSearchCV(pipe, param_grid, cv=LeaveOneOut(), scoring='neg_mean_absolute_error')
-        grid = GridSearchCV(pipe, param_grid, cv=ShuffleSplit(n_splits=10), scoring='neg_mean_absolute_error')
-
-        # # SplineTransformer not supported in ONNX conversion
         # pipe = make_pipeline(SplineTransformer(degree=3), Ridge(alpha=1e-3))
         # param_grid = {'splinetransformer__n_knots': np.arange(4,10)}
         # # grid = GridSearchCV(pipe, param_grid, cv=20)
         # # grid = GridSearchCV(pipe, param_grid, cv=20, scoring='neg_mean_absolute_error')
         # # grid = GridSearchCV(pipe, param_grid, cv=LeaveOneOut(), scoring='neg_mean_absolute_error')
         # grid = GridSearchCV(pipe, param_grid, cv=ShuffleSplit(n_splits=10), scoring='neg_mean_absolute_error')
 
+        else:
+            raise ValueError(f'Unknown "fit_type": {fit_type}.')
+
         # X = self.df[['te', 'c']].to_numpy()
-        X = self.get_X_df().to_numpy()
-        y = self._df['out'].to_numpy()
+        # X = self.get_predictors_in().to_numpy()
+        # y = self.df['out'].to_numpy()
+        # grid.fit(X, y)
+        # grid.fit(self.get_predictors_in, self.get_predictors_out)
+
+        X = self.df[self.predictor_cols_in]
+        y = self.df[self.predictor_col_out]
         grid.fit(X, y)
         model = grid.best_estimator_
+
         return model
 
         # reg = model.named_steps['linearregression']
         # reg.get_params()
         # coefs = reg.coef_
         # intercept = reg.intercept_
 
-    def sk2onnx(self, model):
-        """
-        Saves trained sklearn model as ONNX, with same filename as csv_file but .onnx extension.
-
-        Note
-        ----
-        Not all sklearn models are supported. For a reference of supported models, see
-        https://onnx.ai/sklearn-onnx/supported.html
-
-        Parameters
-        ----------
-        model :
-        Trained sklearn model.
+    @staticmethod
+    def _preprocess_prediction_inputs(*args):
+        """Args can be a) only temperature, or b) temperature and concentration.
+        If concentration is given as a scalar -> gracefully expand to match temperature dimension.
+        Returns temperature or tuple temperature, concentration.
+        """
+
+        if len(args) == 1:
+            # only temperature given (pure fluid)
+            return args,
+
+        # Temperature and concentration given (mixed fluid)
+        temperature = args[0]
+        concentration_ = args[1]
+        if concentration_ is None:
+            return temperature
+
+        scalar_concentration = isinstance(concentration_, numbers.Number)
+        if scalar_concentration:
+            concentration = np.full_like(temperature, concentration_)
+        else:
+            concentration = concentration_
+            if len(temperature) != len(concentration):
+                raise ValueError('Dimension mismatch among the given inputs "temperature" and "concentration".')
 
-        Returns
-        -------
-        Filename where ONNX model was stored.
-        """
-        pre, ext = os.path.splitext(self.csv_file)
-        onnx_file = pre + ".onnx"
-        # Convert model into ONNX format
-        onnx = convert_sklearn(model, initial_types=self.sk_initial_type())
-        self.onnx_model = onnx.SerializeToString()
-        with open(onnx_file, "wb") as f:
-            f.write(onnx.SerializeToString())
-        return onnx_file
-
-    def sk_initial_type(self):
-        initial_type = [(self._INPUT_NAME, FloatTensorType([None, self.n_inputs]))]
-        return initial_type
+        return temperature, concentration
 
     def predict(self, *args):
-        """
-        Compute model prediction with ONNX Runtime, based on self.onnx_file
+        """Compute model prediction (fluid density, heat capacity) based on trained sklearn model, self.sk_model.
+
         Parameters
         ----------
         args : pint Quantity
-            Inputs required for prediciton: temperature and (optionally) concentration.
-            Fluid temperature in unit self.unit['te']
-            Fluid concentration in unit self.unit['c']
+            Inputs required for prediciton: temperature and (for mixed fluids) concentration.
+            Fluid temperature in unit self.unit['te'], typically 'degC'
+            Fluid concentration in unit self.unit['c'], typically 'percent'
 
         Returns
         -------
-        pint Quantity
-        Calculated fluid property in unit self.unit['out']
+        pint Quantity : Calculated fluid property (density or heat capacity) in unit self.unit['out']
         """
-        # sess = rt.InferenceSession(self.onnx_file)
-        sess = rt.InferenceSession(self.onnx_model)
-        X = np.array(list(args)).transpose().reshape(-1, self.n_inputs).astype(np.float32)
-        pred_onx = sess.run(['variable'], {self._INPUT_NAME: X})[0]
-        return pred_onx.flatten()
+        inputs = self._preprocess_prediction_inputs(*args)
+        X = np.array(inputs).transpose().reshape(-1, self.n_inputs)
+        nan_inputs = np.isnan(X).any(axis=1)
 
-    def is_trained(self):
-        return self.onnx_model is not None
+        out = np.full(nan_inputs.shape, np.nan)
+        out[~nan_inputs] = self.sk_model.predict(X[~nan_inputs].reshape(-1, self.n_inputs))
 
-    @property
-    @abstractmethod
-    def n_inputs(self):
-        pass
+        return out.flatten()
 
     @abstractmethod
-    def get_X_df(self):
-        pass
-
-    @abstractmethod
-    def csv2df(self):
-        pass
+    def csv2df(self, csv_file):
+        raise NotImplementedError()
 
 
 class WPDModelPure(WPDModel):
+    n_inputs = 1
+    predictor_cols_in = ['te']
 
-    def csv2df(self):
+    def csv2df(self, csv_file):
         """Read WebPlotDigitizer csv with single dataset into dataframe.
         """
-        df_csv = pd.read_csv(self.csv_file, header=0, sep=',')
-        df_csv.rename(columns={'X': 'te', 'Y': 'out'}, inplace=True)
-        self._df = df_csv
-
-    @property
-    def n_inputs(self):
-        return 1
+        df = pd.read_csv(csv_file, header=0, sep=',')
+        df = df.rename(columns={'X': 'te', 'Y': 'out'})
 
-    def get_X_df(self):
-        return self._df[['te']]
+        return df
 
-    def _plot_fit(self, type=None):   # pragma: no cover
+    def _plot_fit(self, plot_type: FluidProps = None):  # pragma: no cover
         """Check quality of model fit, after calling self.train().
         Plots model fit and original / ground truth data from WebPlotDigitizer csv dataset.
         """
         try:
             import plotly.graph_objects as go
         except ModuleNotFoundError:
-            warnings.warn('This function requires the plotly package, which is not installed. Install it with `pip install plotly`')
+            warnings.warn(
+                'This function requires the plotly package, which is not installed. Install it with `pip install plotly`')
+            return
+
         N_POINTS = 50
         fig = go.Figure()
-        te = np.linspace(self._df['te'].min() - 20, self._df['te'].max() + 20, N_POINTS)
+        te = np.linspace(self.df['te'].min() - 20, self.df['te'].max() + 20, N_POINTS)
         out = self.predict(te)
         fig.add_trace(go.Scatter(x=te, y=out,
                                  mode='lines',
                                  name='Model prediction'))
         # Measured values as scatter
-        fig.add_trace(go.Scatter(x=self._df['te'], y=self._df['out'],
+        fig.add_trace(go.Scatter(x=self.df['te'], y=self.df['out'],
                                  mode='markers',
                                  marker=dict(
                                      color='Black',
                                      size=10,
                                      opacity=0.4,
                                      line=dict(
                                          color='Black',
                                          width=1
                                      )),
                                  name='WPD measurements'))
 
-        if type == 'density':
+        if plot_type == FluidProps.density:
             fig.update_layout(title='Density', width=1600, height=1200,
                               xaxis_title="Temperature [degC]", yaxis_title="Density [{self.unit['out']}]",
                               legend_traceorder="reversed")
-        elif type == 'heat_capacity':
+        elif plot_type == FluidProps.heat_capacity:
             fig.update_layout(title='Heat capacity', width=1600, height=1200,
                               xaxis_title="Temperature [degC]", yaxis_title=f"Heat capacity [{self.unit['out']}]",
                               legend_traceorder="reversed")
-        else:
-            raise ('type must be "density" or "heat_capacity"')
         fig.show()
 
 
 class WPDModelMixed(WPDModel):
+    n_inputs = 2
+    predictor_cols_in = ['te', 'c']
 
-    def csv2df(self):
+    def csv2df(self, csv_file):
         """
         Read WebPlotDigitizer csv with multiple datasets, combine into single dataframe with added dataset level column.
         """
-        df_csv = pd.read_csv(self.csv_file, header=[0, 1], sep=',')
+        df_csv = pd.read_csv(csv_file, header=[0, 1], sep=',')
         dataset_names = [c for c in df_csv.columns.get_level_values(0) if not c.startswith('Unnamed')]
         df = pd.DataFrame()
         for n in dataset_names:
             i = df_csv.columns.get_loc((n, 'X'))
             x = df_csv.iloc[:, i].dropna()
             y = df_csv.iloc[:, i + 1].dropna()
             c = pd.Series(float(n), index=x.index)
             df2 = pd.concat([x.rename('te'), y.rename('out'), c.rename('c')], axis=1)
             df = pd.concat([df, df2], ignore_index=True)
-        self._df = df
-
-    @property
-    def n_inputs(self):
-        return 2
 
-    def get_X_df(self):
-        return self._df[['te', 'c']]
+        return df
 
-    def _plot_fit(self, type=None):   # pragma: no cover
+    def _plot_fit(self, plot_type: FluidProps = None):  # pragma: no cover
         """Check quality of model fit, after calling self.train().
         Plots model fit and original / ground truth data from WebPlotDigitizer csv dataset.
         """
         try:
             import plotly.graph_objects as go
         except ModuleNotFoundError:
-            warnings.warn('This function requires the plotly package, which is not installed. Install it with `pip install plotly`')
+            warnings.warn(
+                'This function requires the plotly package, which is not installed. Install it with `pip install plotly`')
+            return
+
         N_POINTS = 50
         # For all concentration levels, create output curves within measured temperature limits
-        df = self._df.groupby('c').te.agg(['min', 'max'])
+        df = self.df.groupby('c').te.agg(['min', 'max'])
         fig = go.Figure()
         for i in np.arange(df.shape[0]):
             te = np.linspace(df.iloc[i, 0], df.iloc[i, 1], N_POINTS)
             c = df.index[i]
-            c = np.full(te.shape, c)
             out = self.predict(te, c)
             fig.add_trace(go.Scatter(x=te, y=out,
                                      mode='lines',
                                      name=f"Model prediction, c={df.index[i]}%"))
         # Measured values as scatter
-        fig.add_trace(go.Scatter(x=self._df['te'], y=self._df['out'],
+        fig.add_trace(go.Scatter(x=self.df['te'], y=self.df['out'],
                                  mode='markers',
                                  marker=dict(
                                      color='Black',
                                      size=10,
                                      opacity=0.4,
                                      line=dict(
                                          color='Black',
                                          width=1
                                      )),
                                  name='WPD measurements'))
 
-        if type == 'density':
+        if plot_type == FluidProps.density:
             fig.update_layout(title='Density', width=1600, height=1200,
                               xaxis_title="Temperature [degC]", yaxis_title="Density [{self.unit['out']}]",
                               legend_traceorder="reversed")
-        elif type == 'heat_capacity':
+        elif plot_type == FluidProps.heat_capacity:
             fig.update_layout(title='Heat capacity', width=1600, height=1200,
                               xaxis_title="Temperature [degC]", yaxis_title=f"Heat capacity [{self.unit['out']}]",
                               legend_traceorder="reversed")
-        else:
-            raise ('type must be "density" or "heat_capacity"')
+
         fig.show()
```

## Comparing `sunpeek-0.2.9.dist-info/COPYING.LESSER` & `sunpeek-0.3.0.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `sunpeek-0.2.9.dist-info/METADATA` & `sunpeek-0.3.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpeek
-Version: 0.2.9
+Version: 0.3.0
 Summary: Large Solar Thermal Monitoring Tool. Implements the Performance Check Method of ISO 24194
 Home-page: https://gitlab.com/sunpeek/sunpeek
 License: LGPL-3.0-only
 Keywords: solarthermal,solar,energy,monitoring
 Author: Philip Ohnewein, Daniel Tschopp, Lukas Feierl, Marnoch Hamilton-Jones, Jonathan Cazco
 Maintainer: Marnoch Hamilton-Jones
 Maintainer-email: m.hamilton-jones@aee.at
@@ -15,45 +15,48 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: all
 Provides-Extra: api
 Provides-Extra: db
 Provides-Extra: demo
+Requires-Dist: alembic ; extra == "db" or extra == "all"
 Requires-Dist: coolprop (>=6.4,<6.5)
 Requires-Dist: fastapi (>=0.92) ; extra == "api" or extra == "all"
 Requires-Dist: httpx ; extra == "api" or extra == "all"
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: lxml
 Requires-Dist: metpy
 Requires-Dist: numpy
-Requires-Dist: onnxruntime
-Requires-Dist: pandas
-Requires-Dist: pint (==0.19.2)
-Requires-Dist: pint-pandas (==0.2)
+Requires-Dist: orjson
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: parquet-datastore-utils
+Requires-Dist: pint (>=0.19.2,<0.21)
+Requires-Dist: pint-pandas (>=0.2)
 Requires-Dist: protobuf (<4)
 Requires-Dist: psycopg2-binary ; extra == "db" or extra == "api" or extra == "all"
 Requires-Dist: pvlib
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pyephem
+Requires-Dist: pyproj (<3.5.0)
 Requires-Dist: python-dotenv
 Requires-Dist: python-multipart ; extra == "api" or extra == "all"
-Requires-Dist: scikit-learn (<1.2)
+Requires-Dist: scikit-learn
 Requires-Dist: scipy (>=1.10)
-Requires-Dist: skl2onnx (==1.13)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlalchemy-utils
 Requires-Dist: statsmodels
 Requires-Dist: sunpeek-exampledata (>=0.1.0) ; extra == "demo" or extra == "all"
 Requires-Dist: times
 Requires-Dist: timezonefinder
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: trio
 Requires-Dist: uvicorn[standard] (<0.18) ; extra == "api" or extra == "all"
 Requires-Dist: yamlloader
+Project-URL: Documentation, https://docs.sunpeek.org
 Project-URL: Repository, https://gitlab.com/sunpeek/sunpeek
 Description-Content-Type: text/markdown
 
 ![Logo_Transparent_wide.svg](https://gitlab.com/sunpeek/sunpeek/-/raw/main/static_assets/Logo_Transparent_wide.svg?inline=false)
 
 **Core:**
 
@@ -71,111 +74,135 @@
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/sunpeek/web-ui?label=image&logo=docker)](https://hub.docker.com/r/sunpeek/sunpeek)
 ![GitLab contributors](https://img.shields.io/gitlab/contributors/sunpeek/web-ui)
 ![Open Issues](https://img.shields.io/gitlab/issues/open-raw/sunpeek/web-ui?gitlab_url=https%3A%2F%2Fgitlab.com) 
 
 # About SunPeek
 SunPeek implements a dynamic, in situ test methodology for large solar thermal plants, packaged as an open source software 
 application and python library. It also includes the first open source implementation of the ISO 24194 procedure 
-for checking the yield of solar thermal collector fields
+for checking the performance of solar thermal collector fields.
 
-SunPeek was originally developed as part of the HarvestIT research project, see https://www.collector-array-test.org
+Full documentation is at [https://docs.sunpeek.org](https://docs.sunpeek.org)
+
+SunPeek was originally developed as part of the HarvestIT research project, see [https://www.collector-array-test.org](https://www.collector-array-test.org)
 
 ## A Web Application and a Python Library
 SunPeek is available as both a complete, containerised web application - intended to make the ongoing monitoring of one or
 several solar thermal plants simple and intuitive - and as a python library, for use by researchers and for building into 
 other tools. To install the python library, simply run `pip install sunpeek`. To set up the web application, see below.
 
 ## License
 Except where specifically noted otherwise, SunPeek is made available under the GNU Lesser General Public License. This means
 that you can use the software, copy it, redistribute it and include it in other software, including commercial, proprietary 
 software, for free, as long as you abide by the terms of the GNU GPL, with the exceptions provided by the LGPL. In particular, 
 if you redistribute a modified version of the software, you must make the source code of your modifications available, and
 if you include the software in another piece of software or physical product, you must give users notice that SunPeek is 
 used, and inform them where to obtain a copy of the SunPeek source code and license.
 
-Note that the SunPeek WebUI (https://gitlab.com/sunpeek/web-ui), is covered by a seperate licence, the BSD-3-Clause, see:
-https://opensource.org/licenses/BSD-3-Clause
+Note that the [SunPeek WebUI](https://gitlab.com/sunpeek/web-ui), is covered by a separate licence, the BSD-3-Clause, see:
+[https://opensource.org/licenses/BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
 
 Copyright (c) 2020-2022, AEE - Institut für Nachhaltige Technologien, SOLID Solar Energy Systems GmbH, GASOKOL GmbH, Schneid Gesellschaft m.b.H.  
 Copyright (c) 2023, SunPeek Open Source Contributors
 
 SunPeek is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 
-# Run
-## Linux
-The preferred way to run the SunPeek application is with docker on a Linux host. Running on Docker on Windows ([see below](#windows)) 
-or installing directly on the host (not recommended) is also possible. 
-
-## Deploy Full Application with Docker Compose
-The full application can be run with docker compose. This requires docker engine 19.03+, supporting the `docker compose`
-command (instead of the older separate `docker-compose` tool). Use `docker version` to check. To install docker go to
-https://docs.docker.com/engine/install/ select the relevant platform and follow the instructions.
+# Running SunPeek
+## Prerequisites
+* Ideally, a modern linux environment, although running on Windows and MacOS is also possible, with _at least_:
+  * 5GB free disk space (this is needed for unpacking the application, after installation it will use around 2 GB)
+  * A 7th Gen i5 or better processor.
+  * 8GB RAM
+* Docker and Docker compose (v2) installed ([see below](#get-docker))
+
+## Get Docker
+In order to provide a consistent environment and allow SunPeek to work across a wide range of install environments, 
+it is provided as a set of Docker images (essentially, very lightweight virtual machines). A docker compose 
+configuration is also provided, if you are installing sunpeek on a single machine, this is probably what you want to 
+use, follow the links below for instructions depending on your environment.
+
+### Linux   
+To install docker on Linux go to https://docs.docker.com/engine/install/ select the relevant platform and follow the 
+instructions.  
+### Windows 10 and 11  
+On desktop windows, the easiest way to get Docker is to install [docker desktop](https://www.docker.com/products/docker-desktop/).  
+### Windows server   
+To install the Docker Engine on Windows Server, see [this guide from Microsoft](https://learn.microsoft.com/en-us/virtualization/windowscontainers/quick-start/set-up-environment?tabs=dockerce)
+
+## Using the easy setup GUI or scripts
+For convenience, a bash script for Linux or a simple graphical utility for use on Windows is provided. These will do 
+some basic configuration for running SunPeek on a single machine, optionally accessible over a local network.
+Docker is still required.   
+```{note}
+If you have previously set up SunPeek using the default configuration, you must first 
+remove all stored data by running the command `docker volume rm harvestit_hit_postgres_data` in a terminal/command 
+prompt, _this will also remove uploaded data._ You do not need to do this to update the software, see 
+[Upgrading to a new version of SunPeek](#upgrading-to-a-new-version-of-sunpeek)
+```
 
+#### On Linux
 1. Use https://gitlab.com/api/v4/projects/43333900/repository/archive?path=deploy to download an archive of the 
 deployment files and unzip it to the location you want to run it from.
-2. Open `api.env.template` and set `HIT_DB_PW` to a strong random password
-3. Open `db.env.template` and set `POSTGRES_PASSWORD` to _the same_ strong random password.
-4. If you want to access the application from anywhere except the local machine, open `ui.env.template` and replace `localhost`
-in `HIT_API_BASE_URL` with a URL which can be used to access the machine on which the application is running. **IMORTANT:
-it is strongly recommended that you don't make SunPeek accessible from the public internet. At present there are NO built
-in access controls**
-5. In a terminal in the unzipped folder, run `docker compose up -d`
-6. After at most 2 minutes (usually a few seconds), the web UI should be accessible at http://localhost, or the url set 
-in step 4.
-
-## Windows
-### Get Docker
-#### Windows 10 and 11
-On desktop windows, the easiest way to get Docker is to install [docker desktop](https://www.docker.com/products/docker-desktop/).
-#### Windows server 
-To install the Docker Engine on Windows Server, see [this guide from Microsoft](https://learn.microsoft.com/en-us/virtualization/windowscontainers/quick-start/set-up-environment?tabs=dockerce)
+2. Run `quick-setup.sh` and answer the prompts, this will create a database password and default configuration files from templates.
+3. In a terminal in the unzipped folder, run `docker compose up -d`
+4. After at most 2 minutes (usually a few seconds), the web UI should be accessible at http://localhost, or the url set 
+in step 2.
 
-### Set up SunPeek
-1. [Download](https://gitlab.com/api/v4/projects/43333900/repository/archive?path=deploy) the archive of the deployment files
-2. Open a powershell terminal (or e.g. the Terminal window in PyCharm) in the deployment folder, and run `.\quick-setup.ps1`
-3. Run `docker-compose up -d` to start the application in "detached" mode (i.e. in the background). If you want to run
-it attached to the terminal to see console output from the containers, run `docker-compose up`.
-4. After at most 2 minutes (usually a few seconds), the web UI should be accessible at `<external.url>` 
-(`localhost` by default), and the api at `<external.url>/api/v1`. See `<external.url>/api/v1/docs` for API documentation.
-5. To update the application to use newer images, run `docker compose pull` then `docker compose restart`
-
-##### Using the Easy Installer
-For convenience, if you wish to avoid using powershell, a simple graphical utility is provided for use on Windows. 
-Docker is still required. **NOTE: If you have previously set up SunPeek using the default configuration, you must first 
-remove all stored data by running the command `docker volume rm harvestit_hit_postgres_data`, _this will also remove 
-uploaded data._ You do not need to do this to update the software, simply open a command prompt in the folder where you 
-stored the SunPeek configuration and run `docker compose pull`, then `docker compose up -d`**
+#### On Windows
 1. Download [this file](https://gitlab.com/sunpeek/sunpeek/-/raw/main/sunpeek_easy_installer.zip?inline=false), and unzip
 it to a temporary location.
 2. Run `sunpeek_easy_installer.exe`
 3. You should then get a small window with 2 fields. You must select a location to store the configuration files for the
 application, if you are running the application only for access from the local machine, leave the default in the url field. 
 4. Click setup. 
 5. Once the window closes open the directory you specified, and double-click the start.bat file. A command prompt will 
 open to display the startup process.
 6. Docker compose will download the required application components, this may take several minutes, once you see all 
 components listed as 'started' or 'healthy' you can close the command prompt.
 7. Open a browser and go to the url specified in the setup tool, probably http://localhost to see the web-UI for the tool.
 8. To stop the application, assuming no other processes are running under docker on your machine, simply shut down the 
-docker engine. If you are using Docker Desktop, this can be done by right clicking the Docker icon the the system try and 
+docker engine. If you are using Docker Desktop, this can be done by right-clicking the Docker icon the system try and 
 selecting Quit
 
-#### Configuration
+## Advanced Configuration
+```{danger}
+It is strongly recommended that you don't make SunPeek accessible from the public internet. At present there are NO 
+ built-in access controls
+```
 Configuration is via environment variables, which can be set by any configuration management system you use, however the
-default setup uses `.env` files. To deploy the application on a single host, only the database password and external URL
-need to be set. The `.\quick-setup.ps1` or easy installer does this for you, or you can manually set the value of 
-`HIT_DB_PW` and `POSTGRES_PASSWORD` in the `api.env` and `db.env` files to *the same* random, unique password string, 
-and the value of `HIT_API_BASE_URL` in the `ui.env` file to <external.url>/api/v1.  
-_*NOTE*_: This setup is designed to deploy all containers on a single machine where docker compose is running. 
+default setup uses `.env` files. To deploy the application on a single host, only the external URL needs to be set. The 
+easy installer does this for you, or you can set the value of `HIT_API_BASE_URL` in the `ui.env` file to 
+<external.url>/api/v1. Other configuration variables are documented at 
+[docs.sunpeek.org/configuration-variables.html](https://docs.sunpeek.org/configuration-variables.html)
+```{note}
+This setup is designed to deploy all containers on a single machine where docker compose is running. 
 The configuration for the Traefik reverse proxy is stored in a directory which is *bind mounted* to the container. For 
-other deployment approaches (e.g. using Kubernetes), a different a more appropriate Traefik dynamic 
+other deployment approaches (e.g. using Kubernetes), a more appropriate Traefik dynamic 
 [configuration provider](https://doc.traefik.io/traefik/providers/overview/) should be selected.
+```
 
-#### Technical Details - What does compose do?
+### Database Backends
+SunPeek supports SQLite and PostgreSQL as backend databases for storing plant configurations, collector and fluid types 
+etc. For single host installs with small number of plants, SQLite should be sufficient and this is therefore the default
+configuration. To use the PostgreSQL backend you can add `HIT_DB_TYPE=postgresql` to `api.env`, and set the values of
+the `HIT_DB_PW` and `POSTGRES_PASSWORD` variables in the `api.env` and `db.env` files to *the same* random, unique 
+password string. The docker compose setup includes an optional postgres service, which can be started along with the 
+other containers with `docker compose --profile postgres up` 
+
+## Upgrading to a new version of SunPeek
+Updates to SunPeek are accomplished by pulling newer versions of the docker images used to run the application. These 
+are used to create new containers in place of the old ones. If you used the default configuration, a persistent docker 
+volume called `sunpeek_postgres_data` will have been created, this _should_ avoid data loss, however keeping backups is 
+always recommended. The update process is as follows, and is the same on all operating systems:
+1. Open a terminal/command prompt in the configuration folder selected during setup.
+2. Run `docker compose pull` to download the latest images
+3. Run `docker compose up -d` to recreate any containers which have updated images.  
+
+
+## Technical Details - What does compose do?
 [Docker Compose](https://docs.docker.com/compose/) is a tool for *orchestrating* docker containers, to create 
 applications made up of several docker containers. When the HarvestIT application is started with the default docker-compose 
 file, the following things happen:
 1. Compose checks if each of the images defined in the compose file, is available with the correct tag locally, if not it
 pulls them from the relevant registry
 2. A virtual network is created, for the containers to communicate with each other. This is segregated from the host machine's
 main network interfaces.
@@ -189,56 +216,17 @@
 URL. It can also [be configured](https://doc.traefik.io/traefik/https/overview/) to terminate TLS (HTTPS) encrypted 
 connections and obtain certificates automatically, to secure connections to the application.
 5. Compose waits until the database container reports a "healthy" status, then starts the api container (using image 
 `sunpeek:latest)`, this is the main HarvestIT application.
 6. The `harvestit` container runs a database initialization scripts to get the database ready. 
 7. Once the api container has started, the webui container is started. 
 
-# Development
-## Development Environment
-SunPeek uses [Poetry](https://python-poetry.org/) as a virtual environment and dependency manager and build system. To 
-get started:
-1. [install poetry](https://python-poetry.org/docs/#installation)
-2. You may need to allow powershell to run scripts (for example to use the built-in terminal in PyCharm on Windows). 
-To do this, go to the start menu, search powershell, right click and select run as administrator. In the terminal that 
-opens run `set-executionpolicy remotesigned`
-3. Clone this repository (or a fork of it, see [CONTRIBUTING](https://gitlab.com/sunpeek/sunpeek/-/blob/main/CONTRIBUTING.md)).
-4. Open a terminal in the repository root and run `poetry install --with dev`. This will get you a python virtual environment 
-with all the required dependencies. If you get errors from poetry, try running `poetry lock`, then `poetry install --with dev` again.
-
-If you are using PyCharm as your IDE, make sure you have version 2022.3 or newer, then follow [these instructions](https://www.jetbrains.com/help/pycharm/poetry.html)
-to set up PyCharm to work with the Poetry virtual env. You may need to restart PyCharm after installing poetry.
-
-## Getting a local development database
-The application can work with any postgresql database, provided it has the timescaledb extension installed. The `init_db`
-module in HarvestIT will create a new database according to your settings (see the [config variables](https://docs.sunpeek.org/configuration-variables.html),
-and add our "preinstalled data" (fluid definitions, sensor types etc...), to it.   
-The easiest way to get a local database is to run the [TimescaleDB docker image](https://hub.docker.com/r/timescale/timescaledb/), 
-this is what the test fixtures described in [Test Database] do automatically. There is a script called `setup_dev_db.py´ 
-provided as a convenience. The description below assumes you will use this method.
-
-If you need to write integration tests, there are test fixtures that deal with the steps below automatically. 
-To create the container and set up the database with a test plant, run the following in a terminal, starting in the root project folder:
-```
-cd ./tests
-docker-compose up -d
-cd ..
-python -m setup_dev_db
-```
-
-## Running the application in the development environment
-### Run directly in a local terminal
-In a terminal window with the correct virtual environment active, run: `uvicorn sunpeek.api.main:app --reload`
-
-### Run standalone in Docker 
-Pull and run the latest image from the Docker Hub image registry: `docker run -p 8000:8000 --name sunpeek sunpeek/sunpeek:latest`
-
-#### Prerequisits:
-* You need to have docker desktop installed https://www.docker.com/products/docker-desktop/, on windows enabling WSL2 is recommended, but docker desktop should work without it https://docs.microsoft.com/en-us/windows/wsl/install
-  * You need to have [docker-compose](https://docs.docker.com/compose/) available, this is usually installed automatically with Docker desktop.
+# Developing
+For information on contributing to sunpeek, see CONTRIBUTING.md, for developer documentation see 
+[https://docs.sunpeek.org/developing.html](https://docs.sunpeek.org/developing.html)
 
 # Maintainers and Steering Committee
 SunPeek is developed as an open source project, with contributions gladly accepted from interested members of the community.
 The overall direction of the project is managed by a **steering committee**, which currently consists of: 
 * Daniel Tschopp <d.tschopp@aee.at>
 * Philip Ohnewein <p.ohnewein@aee.at>
 * Marnoch Hamilton-Jones <m.hamilton-jones@aee.at>
```

## Comparing `sunpeek-0.2.9.dist-info/COPYING` & `sunpeek-0.3.0.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `sunpeek-0.2.9.dist-info/RECORD` & `sunpeek-0.3.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 sunpeek/__init__.py,sha256=3OVGGe7fF52quxTfpeGZ9WLlVZ9wc3BK7sWngF73KpM,1035
 sunpeek/api/__init__.py,sha256=6D8BHGZVV1B9mw90ii9DPj8aqgk7T2uGcMSJgpcVgrY,264
 sunpeek/api/dependencies.py,sha256=_JRAjCRDF3hV8Bfyq6E2MD8gYhojSekgJRMTka_-Qp8,581
-sunpeek/api/main.py,sha256=EZbruVpkTsB1yF0VYCAagFp8Cp8hl-Jn0WIhUPrMXXg,4170
+sunpeek/api/main.py,sha256=zWgF3GCSuCHD8XlWDcKETEk35sXfqx0xJcIz6sqereM,5737
 sunpeek/api/routers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunpeek/api/routers/api_jobs.py,sha256=WUAYTISuGg2gkufuZSblaL9NDXnjQVXd64TxixX2z1U,1713
+sunpeek/api/routers/api_jobs.py,sha256=ow_AdoC04SyibS7enKsD4Cq3aNRfJIY6tLdLEgxEuU4,1718
 sunpeek/api/routers/config.py,sha256=MONE455TkLterNKUBAYCT5ikdUJKErKNHJZg7u1UGoI,5692
-sunpeek/api/routers/evaluations.py,sha256=46kZv5TVH13Vhy0JrqEx-1joEdBHMAk0o_L94vM9sMQ,3403
-sunpeek/api/routers/files.py,sha256=kPrPUvQQRFG-aXu8oTYRvmK3yDwOHNGhQ3j19xv8yTQ,2782
-sunpeek/api/routers/plant.py,sha256=wxBPCgfcl4xfll61Ky12aXBec8vShubHGe5O83lbmXw,13410
+sunpeek/api/routers/evaluations.py,sha256=9N5SnEhykB69m2LNr4auNeFbIgUydXIIGRMG7wPcc1o,5513
+sunpeek/api/routers/files.py,sha256=ZViDGFt1FqX7h_bm7_fK44oaM4AIo8ZXk6V28mPqKAg,6582
+sunpeek/api/routers/plant.py,sha256=TpRVi8QMnFjmyf0y3WfWyHxxUMwAHbP1LZniX2hXMA0,19436
 sunpeek/base_model.py,sha256=v3tIRStkycYr5uYReaQ7VDztTRFw0Js6j9hNtUDGUyc,780
-sunpeek/common/__init__.py,sha256=F-tVAK0f825j6YF2s2VymVDW37QVf1l_YwfGuD4AbgA,150
+sunpeek/common/__init__.py,sha256=WVUQ1PQnwc5lHNsQm0dnkXsUfmgfC8qC9UEgpUKnE_E,100
 sunpeek/common/common_units.py,sha256=DPykzkJEX8oGql7iw6ZK6kiI5rsoIHrR3KCXydqPbRc,1248
-sunpeek/common/config_parser.py,sha256=K333ki5NsweVTEn3M3n8iA1887tHSVzQxABgBjy4KNk,1446
-sunpeek/common/context.py,sha256=FEMY6BRd2NOKIS98-t_PcY406jy4UL7Tm9nteKoKrAs,19464
-sunpeek/common/data_uploader.py,sha256=th9sHn89N5PJo5plYUOfWjkWa1t67sAlNNVg_m-_mhM,17482
-sunpeek/common/errors.py,sha256=USCDD1EINZebhx-5n_dEK_JVzNl9GlgrjiHLv0CQFYA,1056
-sunpeek/common/unit_uncertainty.py,sha256=dSJUBRm8eQ2cC_KsL8e8OreDctiZiHfizQBXHRyywX4,17621
-sunpeek/common/utils.py,sha256=fYtfHvZqK9kxLCaBbMaQzFtg4cFj4IwxB51366hiTmg,6119
-sunpeek/components/__init__.py,sha256=_Jjf_EKQviEy0pwQQHLwdsf2jM07RdOEEls1rDWDK9A,960
-sunpeek/components/base.py,sha256=TBuDGzaemZuoOeG0ayHpd4-VwFjbD61SCYMPI03FiIM,12272
-sunpeek/components/components_factories.py,sha256=eyJJPYt-W7VdWuOtx1Ii11JZWnempLuFY1gKsrzD97c,2763
-sunpeek/components/fluid_helpers.py,sha256=sr2qkk-vv4xsxIPuQhxAku7aJcOOoqlinNAVV3X87ok,15276
-sunpeek/components/fluids.py,sha256=y6TUyezuoq5zF70y9x50vcaAaaj78Lw0bvhvNksuFS4,26357
-sunpeek/components/helpers.py,sha256=kXZCGhN1oeB_myCdrUWSnIQut7EHN8Q6TzRvZSzEsR8,14915
-sunpeek/components/iam_methods.py,sha256=WBUSnZwVMh1LphW4v7kCTvZwt6w7qw_yfc1Um89953U,15711
+sunpeek/common/config_parser.py,sha256=NfKIR2a9abhPxQI52UFLm_R1o9s_IDu1-mc39PI86no,1968
+sunpeek/common/errors.py,sha256=lASviLRJhtDEdro41Lj__Br4sYp5EG89u2iNVoRaXuk,1802
+sunpeek/common/time_zone.py,sha256=q73QtB4gBxuCDqnO6yxtWYUNXE2nm6ydFpmyL6Gy7iM,6639
+sunpeek/common/unit_uncertainty.py,sha256=355iPUVFtlFDASsezyT_58GUWXD8dIJ5PZPne1HJ20s,17863
+sunpeek/common/utils.py,sha256=nJzOZhtgm95C1DA3H53pjKm6OU-9Bx9LX2Dsy96m3Tw,5134
+sunpeek/components/__init__.py,sha256=ffw2cp0QyLk9YEzjPPI2igVO-YU7SzkbfOv0WsUGtD4,986
+sunpeek/components/base.py,sha256=ftMIv1luBZMoNgrRxDaG3M1PpagPQE6A9esPpId49Pk,13435
+sunpeek/components/components_factories.py,sha256=nDQSyiCUw-3PQqm4T0ItRf6h9p25Q52XUCtooitQnK0,2800
+sunpeek/components/fluids.py,sha256=FpYwEOauBJJhrnxBnIVAQ4QGs8jvs8c9Jyjr3Tx56ig,26948
+sunpeek/components/fluids_wpd_models.py,sha256=dU685R5VBey42l1tlPqb82xiIEQwi4MbvSsxXL-TqFg,14800
+sunpeek/components/helpers.py,sha256=hKgEg1Uhn4tmM9ZOwlcQ9RqETWNNSPdy850LwogHCkw,14886
+sunpeek/components/iam_methods.py,sha256=DTkFR4FmMyoxhPq4_j177MCqSDrvG54VZGKSjd9L7xw,15752
 sunpeek/components/jobs.py,sha256=iYU2KpDCFZJVcJkMISPctC8c5yAzECKleoqK5Pn0o9U,674
-sunpeek/components/operational_events.py,sha256=a82dyo32zE2VltSiy8bs2FNFXaxRijO8jk2DcVOnorw,2031
-sunpeek/components/physical.py,sha256=SbrAGVVnN2PXvEU7XypHWWpirOxoZTH8_P6D73TkG10,57176
-sunpeek/components/results.py,sha256=VYRJYL4HzeJ3NSCDQLV1oiydizpNW0jQoEBUn_bYSRw,2874
-sunpeek/components/sensor.py,sha256=ptq5ST8TbvZ1xiP_25ZiHe6NtcAq8pAlzUE1sKSxU_s,18114
-sunpeek/components/sensor_types.py,sha256=CcOSh6y_tzt7Ol4FJHmSm7qdReqV2tCYllPK4MRSEmg,10512
-sunpeek/components/types.py,sha256=VRk-lK_dNmB-PXE9nb3eG2_DAVtgNRXaA73J4RP8juo,21647
-sunpeek/core_methods/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunpeek/core_methods/pc_method/__init__.py,sha256=2EWBwo0TxC4i0-7YUBugibJ9zkORCfUkY41Eub3yxMU,3203
-sunpeek/core_methods/pc_method/equation.py,sha256=HvAQHr6OWp6eafKpZSVhcV2T4GCydU2nv65YuF0PAGQ,13949
-sunpeek/core_methods/pc_method/main.py,sha256=NHSkv3PP2Hg8W_Dah1M9AvWQiMVPRdGxTV0p29kSd0s,27733
-sunpeek/core_methods/pc_method/plotting.py,sha256=KbU-ST3MRMHPs5csDfQa8pyA82PAVpqBR6VLBAqfO8c,12817
-sunpeek/core_methods/pc_method/verify_validate.py,sha256=RYSbBNZX7IhQFMzR0wgjBLAe3TEgJ-ckHstkSXgq1k4,3664
-sunpeek/core_methods/virtuals/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunpeek/core_methods/virtuals/main.py,sha256=ikQ6iW2_pZ0P8iIR9xoCKmtCI_RPp_wM5POJkeKxe7o,30187
-sunpeek/core_methods/virtuals/radiation.py,sha256=Rc5ocqKOn4TSUzNIT0jKvrsr9PcnCDf1xyuoDVkWrVM,33627
+sunpeek/components/operational_events.py,sha256=mKT8QamEfXYLIclwGJeXUqG44zozruGg560XHvM8rfU,3804
+sunpeek/components/physical.py,sha256=sFLuxpxxhtrSEGxdefFho0qpyv05HH92QcxAwjZeIDM,49882
+sunpeek/components/results.py,sha256=_sNDJbwHgTl-f7f-tP7Rr9NgjGde_EwXgL-kTUSTo-g,3075
+sunpeek/components/sensor.py,sha256=7enxAzMgWxlBCbJLntZeflYyk6lIi_uwIM-t4m3DXlU,23359
+sunpeek/components/sensor_types.py,sha256=cgj-J4kO31VXjNY8w1k8mBT6OPFEG0prZMd4AgvqWlU,11412
+sunpeek/components/types.py,sha256=7ajsuRqSxf3rYC0sW4vSKdQyW59GsHXZjKHPPaw-uMo,21504
+sunpeek/core_methods/__init__.py,sha256=Js-UR8fqFyHIkPCX_2XQX-rGLPRb-AzkElBEK57nz2w,87
+sunpeek/core_methods/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sunpeek/core_methods/common/main.py,sha256=QgYX34ZGWiOniEpaIGB7bA0pHO_WYLJvDwsdAtxExLs,13669
+sunpeek/core_methods/pc_method/__init__.py,sha256=ay7JztMWmxBEb2U-cuKdL7-UKcX6Xat3slqhpS27mGA,4570
+sunpeek/core_methods/pc_method/equation.py,sha256=3MvA4_plpzxkGO6P8PmeSMnV6VX07AqE8FT4RE7C358,15126
+sunpeek/core_methods/pc_method/main.py,sha256=S6XRoKVWZp95L9lMGWvzKROiq1s8tBDxadxd5Hk9bCw,31604
+sunpeek/core_methods/pc_method/plotting.py,sha256=hln6QFu7ShcsK___zIwczjdPPoO3X7MmawlJHhmjqos,22617
+sunpeek/core_methods/pc_method/wrapper.py,sha256=f8s1ezFJlRuOpGfuM9RQZQV4y7oLmrTyuT5QYixUZ2s,10781
+sunpeek/core_methods/virtuals/__init__.py,sha256=Mabq_yA70c9I63nDY8A63jyw8PMShe3f6X4QzqRDoGg,83
+sunpeek/core_methods/virtuals/algorithms.py,sha256=yLyBZv5HYRplmjmMIbeWeZY6U4kpm5-IE9C-gpYyPuA,41535
+sunpeek/core_methods/virtuals/main.py,sha256=S0H_ZqV_-FnfQapvxJeK830h8urixmQePwYs3EgyaaE,4224
+sunpeek/core_methods/virtuals/radiation.py,sha256=rzDZaA8pldmxuF1oZJ6N_eUtYud52XjglnENH2mA5jQ,35090
+sunpeek/core_methods/virtuals/virtuals_array.py,sha256=FAepbbwe8gnAN706f4SW58hAfmP4qUzyY-pfLVwry0A,3449
+sunpeek/core_methods/virtuals/virtuals_plant.py,sha256=h2XEqneBqVM6iyFBHd0B8XL0QUsfI7EmzCwDge5_T4M,3868
+sunpeek/data_handling/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sunpeek/data_handling/context.py,sha256=T5lV98XGw3xnIY_QQF6rqK1ST_TpLKfVkaF0NiTR2O8,23508
+sunpeek/data_handling/data_uploader.py,sha256=4qcdfI9yVVYVAnbohe-_kDVqL8m0mlMLepVXuEls0oc,24335
+sunpeek/data_handling/wrapper.py,sha256=DqTzGs5afZZuSng6azWTOD2qMzXbsOIsD4jTTKCobVo,1849
 sunpeek/db_utils/__init__.py,sha256=btLFbporMPPB8l8OvHVb7D4ZwQHd0nj0Tfgj0eOGqfg,25
-sunpeek/db_utils/crud.py,sha256=pOsVNiEAkD8h8zzfhRcVpn5USpDT4yVOnNN0we2U_h8,4139
-sunpeek/db_utils/db_data_operations.py,sha256=9PY3bc9iZmEJda-O7q2SVzmrgi_YUgTfWd0vrrkO9oY,14093
-sunpeek/db_utils/init_db.py,sha256=jJoffGvFXV1fFWnZfkGDqaxIBVpg05kmvNUmGRJ15NM,1334
-sunpeek/definitions/__init__.py,sha256=8rDML0L55eo1aRiEdAW4cFvtVjezpC6CjAyRRPVNx1U,345
-sunpeek/definitions/collector_types.py,sha256=V6qfb1Tl8InkF_l1KcyNxYQzHciDs5Qz1nA-5S8KWN4,18422
-sunpeek/definitions/fluid_definitions.py,sha256=JuvCnpwwigYyCIEamC8DoFHpw-1DTVEUvORrTGop6Ac,31721
-"sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.csv",sha256=ZYl0nS6erP8Gn2GlsmOjaA3l_3xo3nvt7WVU0Nk2leI,88
-"sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, density.onnxbytes",sha256=NMZtifJo0Dt1nRvDeo57ydl8G0UQOEpSIYekEkNrxVI,993
-"sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.csv",sha256=uVb9p15EsbH1Ule1VAoQfT_C1du8NP0q1YhmOMGB-lM,241
-"sunpeek/definitions/raw_data/FHW, Pekasolar/Pekasolar, pdf export, heat capacity.onnxbytes",sha256=YS5luTplfWulcE8PtHtodKcKBwjPtKCIPM16jRDydHs,993
+sunpeek/db_utils/crud.py,sha256=xhY0jRRGtinnVwYzdwKuBYVifXjF_M_Fdj6NgOEJEvo,5593
+sunpeek/db_utils/db_data_operations.py,sha256=kyqkWnCGLQETmhj_PPY-ahzCgJZAErYq2fb87PSirXc,16575
+sunpeek/db_utils/init_db.py,sha256=m07Es2bbc1B9YUDE0TbSGUVXobl5B9_7ZyBs4isXEHs,1921
+sunpeek/definitions/__init__.py,sha256=KEbtAAapQNPxxfKYp_HpCIZQ7Ugj4wM0BCaZW6K7G8A,454
+sunpeek/definitions/collector_types.py,sha256=Ffyz1MI4C3PsbgZh8vp4SmVBXoGEnCncEAAiU4vZ1b4,24370
+"sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/density.csv",sha256=6R3gcJJiKOuiy2ebwzMrvZ1vodzfP4Eh0ONztBzsAFk,334
+"sunpeek/definitions/fluid_data/Gasokol, corroStar mixture/heat capacity.csv",sha256=clSvcbd6ar_FPqw-eWn_qMFNZSmiGGD67tBDCKxT0ps,337
+sunpeek/definitions/fluid_data/Pekasolar_FHW/density.csv,sha256=ZYl0nS6erP8Gn2GlsmOjaA3l_3xo3nvt7WVU0Nk2leI,88
+sunpeek/definitions/fluid_data/Pekasolar_FHW/heat capacity.csv,sha256=uVb9p15EsbH1Ule1VAoQfT_C1du8NP0q1YhmOMGB-lM,241
+sunpeek/definitions/fluid_data/Wocklum Thermum P/density.csv,sha256=rb1uk1d9bj3MdDQfWb1-YcxhC_RZ7mjhNAdSoHn7XZ8,3450
+sunpeek/definitions/fluid_data/Wocklum Thermum P/heat capacity.csv,sha256=F-IZeYyL2U3rww2tTP1qRWH0bCY3FhGY7f9-FtlvZ_w,2532
+sunpeek/definitions/fluid_definitions.py,sha256=Qry_kWr-cHKEnEbKl9WolUiAJ9g2NzO-rnmIVNpJ2lI,33003
 sunpeek/demo/__init__.py,sha256=djMLgvrYODa5bcBr2KnbPZ37s1yO_3igMAEYNXp_iPQ,528
-sunpeek/demo/demo_plant.py,sha256=DZCVSzFBOL1M3Zu6S6P0vnaTt4HvvTZgbj83MUpcaTo,1371
-sunpeek/demo/demo_plant_script.py,sha256=VIqwhCMpeFLG_VUpqVpFdSsSyuNsSww8ZsoP0ve6Lo4,4894
-sunpeek/exporter.py,sha256=z0_-ZylxNcWi-ZYYu1xByp9fDEHbJ7I6zcaAF5oYpy4,2836
-sunpeek/serializable_models.py,sha256=uKRIa6i7wLMWb9pf1svG6dJMWE4VX_PQiMnvvklEnwc,14227
-sunpeek-0.2.9.dist-info/COPYING.LESSER,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-sunpeek-0.2.9.dist-info/METADATA,sha256=HOII11VzvpOuBSQk939Wa7RoQprU6etD4wGH_q1SluI,16989
-sunpeek-0.2.9.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-sunpeek-0.2.9.dist-info/COPYING,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-sunpeek-0.2.9.dist-info/RECORD,,
+sunpeek/demo/demo_plant.py,sha256=tVfvaM7wa2bWLIeZxwpykS0HHxPsoxXthU9zfwJV6Gs,1902
+sunpeek/demo/demo_plant_script.py,sha256=ifWIWRvLTA-IYaTfM-BGZc6mnh15A3-SOwFTs2ehKuE,5168
+sunpeek/exporter.py,sha256=okT1A2hiRjtu-usUAnl5Oq84bIMrkvMuSvTYCitlhGs,6191
+sunpeek/serializable_models.py,sha256=xpUo3zcj9v2irOaqXzg9JbeLpT-RHEtzNQPhpGBLC7I,22264
+sunpeek-0.3.0.dist-info/COPYING.LESSER,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+sunpeek-0.3.0.dist-info/METADATA,sha256=sAN5Hi0B4DaiR12IKpTQmCEuujQpVO4xlBpkOQDPKd4,15233
+sunpeek-0.3.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+sunpeek-0.3.0.dist-info/COPYING,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+sunpeek-0.3.0.dist-info/RECORD,,
```

