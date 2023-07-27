# Comparing `tmp/streetlevel-0.3.1.tar.gz` & `tmp/streetlevel-0.4.0.tar.gz`

## Comparing `streetlevel-0.3.1.tar` & `streetlevel-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,58 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 streetlevel-0.3.1/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streetlevel-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 streetlevel-0.3.1/doc/mapy.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 streetlevel-0.3.1/doc/streetside.md
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 streetlevel-0.3.1/doc/streetview.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/dataclasses.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/geo.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/mapy/__init__.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/mapy/mapy.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/mapy/panorama.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetside/__init__.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetside/panorama.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetside/streetside.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetview/__init__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetview/depth.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetview/panorama.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetview/protobuf.py
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 streetlevel-0.3.1/streetlevel/streetview/streetview.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetside/streetside_test.py
--rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetside/data/find_object.json
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetview/streetview_test.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetview/data/coverage_tile_object.json
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetview/data/find_object.json
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 streetlevel-0.3.1/tests/streetview/data/lookup_object.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 streetlevel-0.3.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 streetlevel-0.3.1/LICENSE
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 streetlevel-0.3.1/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 streetlevel-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 streetlevel-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 streetlevel-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 streetlevel-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streetlevel-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/streetlevel.lookaround.rst
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/streetlevel.mapy.rst
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/streetlevel.streetside.rst
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/streetlevel.streetview.rst
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 streetlevel-0.4.0/docs/_static/css/additional.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/dataclasses.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/geo.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/util.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/__init__.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/api.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/auth.py
+-rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/lookaround.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/panorama.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/proto/MapTile.proto
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/proto/MapTile_pb2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/lookaround/proto/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/mapy/__init__.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/mapy/api.py
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/mapy/mapy.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/mapy/panorama.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetside/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetside/api.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetside/panorama.py
+-rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetside/streetside.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetside/util.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/__init__.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/api.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/depth.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/panorama.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/protobuf.py
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/streetview.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 streetlevel-0.4.0/streetlevel/streetview/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/mapy/__init__.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/mapy/mapy_test.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/mapy/data/getbest.pkl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetside/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetside/streetside_test.py
+-rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetside/data/find_object.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetview/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetview/streetview_test.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetview/data/coverage_tile_object.json
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetview/data/find_object.json
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 streetlevel-0.4.0/tests/streetview/data/lookup_object.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 streetlevel-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 streetlevel-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 streetlevel-0.4.0/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 streetlevel-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 streetlevel-0.4.0/PKG-INFO
```

### Comparing `streetlevel-0.3.1/.github/workflows/python-publish.yml` & `streetlevel-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/streetlevel/geo.py` & `streetlevel-0.4.0/streetlevel/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def tile_coord_to_wgs84(x, y, zoom):
     scale = 1 << zoom
     pixel_coord = (x * TILE_SIZE, y * TILE_SIZE)
     world_coord = (pixel_coord[0] / scale, pixel_coord[1] / scale)
     lat_lon = mercator_to_wgs84(world_coord[0], world_coord[1])
-    return lat_lon[1], lat_lon[0]
+    return lat_lon
     
 
 def wgs84_to_tile_coord(lat, lon, zoom):
     scale = 1 << zoom
     world_coord = wgs84_to_mercator(lat, lon)
     pixel_coord = (math.floor(world_coord[0] * scale), math.floor(world_coord[1] * scale))
     tile_coord = (math.floor((world_coord[0] * scale) / TILE_SIZE), math.floor((world_coord[1] * scale) / TILE_SIZE))
```

### Comparing `streetlevel-0.3.1/streetlevel/streetside/streetside.py` & `streetlevel-0.4.0/streetlevel/lookaround/lookaround.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,207 @@
-import asyncio
+import math
 from datetime import datetime
-from io import BytesIO
-from pathlib import Path
-from typing import List, Union
+from enum import IntEnum
+from typing import List, Union, Tuple
 
-import numpy as np
-from PIL import Image
 import requests
+from aiohttp import ClientSession
 from requests import Session
 
-from .panorama import StreetsidePanorama
-from streetlevel.geo import *
-from ..util import download_files_async
+from . import api
+from .auth import Authenticator
+import streetlevel.geo as geo
+from .panorama import LookaroundPanorama, CoverageType
 
-TILE_SIZE = 256
+FACE_ENDPOINT = "https://gspe72-ssl.ls.apple.com/mnn_us/"
 
 
-def to_base4(n: int) -> str:
-    return np.base_repr(n, 4)
-
-
-def from_base4(n: str) -> int:
-    return int(n, 4)
-
-
-def find_panoramas_in_bbox(north: float, west: float, south: float, east: float,
-                           limit: int = 50, session: Session = None) -> List[StreetsidePanorama]:
+class Face(IntEnum):
     """
-    Retrieves panoramas within a bounding box.
+    Face indices of a Look Around panorama.
     """
-    response = _find_panoramas_raw(north, west, south, east, limit, session)
+    FRONT = 0,  #:
+    RIGHT = 1,  #:
+    BACK = 2,  #:
+    LEFT = 3,  #:
+    TOP = 4,  #:
+    BOTTOM = 5  #:
 
-    panos = []
-    for pano in response[1:]:  # first object is elapsed time
-        # TODO: parse bl, ml, nbn, pbn, ad fields
-
-        # as it turns out, months/days without leading zeros
-        # don't have a cross-platform format code in strptime.
-        # wanna guess what kind of dates bing returns?
-        datestr = pano["cd"]
-        datestr = datestr.split("/")
-        datestr[0] = datestr[0].rjust(2, "0")
-        datestr[1] = datestr[1].rjust(2, "0")
-        datestr = "/".join(datestr)
-        date = datetime.strptime(datestr, "%m/%d/%Y %I:%M:%S %p")
-
-        pano_obj = StreetsidePanorama(
-            id=pano["id"],
-            lat=pano["la"],
-            lon=pano["lo"],
-            date=date,
-            next=pano["ne"] if "ne" in pano else None,
-            previous=pano["pr"] if "pr" in pano else None,
-            elevation=pano["al"] if "al" in pano else None,
-            heading=math.radians(pano["he"]) if "he" in pano else None,
-            pitch=math.radians(pano["pi"]) if "pi" in pano else None,
-            roll=math.radians(pano["ro"]) if "ro" in pano else None,
-        )
-        panos.append(pano_obj)
-    return panos
 
+def get_coverage_tile(tile_x: int, tile_y: int, session: Session = None) -> List[LookaroundPanorama]:
+    """
+    Fetches Look Around coverage on a specific map tile. Coordinates are in Slippy Map aka XYZ format
+    at zoom level 17.
 
-def _find_panoramas_raw(north, west, south, east, limit=50, session=None):
-    url = f"https://t.ssl.ak.tiles.virtualearth.net/tiles/cmd/StreetSideBubbleMetaData?" \
-          f"count={limit}&north={north}&south={south}&east={east}&west={west}"
-    if session is None:
-        response = requests.get(url)
-    else:
-        response = session.get(url)
-    panos = response.json()
-    return panos
+    :param tile_x: X coordinate of the tile.
+    :param tile_y: Y coordinate of the tile.
+    :param session: *(optional)* A requests session.
+    :return: A list of LookaroundPanoramas. If no coverage was returned by the API, the list is empty.
+    """
+    tile = api.get_coverage_tile_raw(tile_x, tile_y, session=session)
+    return _parse_panos(tile, tile_x, tile_y)
 
 
-def find_panoramas(lat: float, lon: float, radius: float = 25,
-                   limit: int = 50, session: Session = None) -> List[StreetsidePanorama]:
-    """
-    Retrieves panoramas within a square around a point.
-    """
-    top_left, bottom_right = create_bounding_box_around_point(lat, lon, radius)
-    return find_panoramas_in_bbox(
-        top_left[1], top_left[0],
-        bottom_right[1], bottom_right[0],
-        limit=limit, session=session)
+async def get_coverage_tile_async(tile_x: int, tile_y: int, session: ClientSession) -> List[LookaroundPanorama]:
+    tile = await api.get_coverage_tile_raw_async(tile_x, tile_y, session)
+    return _parse_panos(tile, tile_x, tile_y)
 
 
-def download_panorama(panoid: int, path: str, zoom: int = 3, single_image: bool = True, pil_args: dict = None) -> None:
+def get_coverage_tile_by_latlon(lat: float, lon: float, session: Session = None) -> List[LookaroundPanorama]:
     """
-    Downloads a panorama to a file.
+    Same as :func:`get_coverage_tile <get_coverage_tile>`, but for fetching the tile on which a point is located.
+
+    :param lat: Latitude of the point.
+    :param lon: Longitude of the point.
+    :param session: *(optional)* A requests session.
+    :return: A list of LookaroundPanoramas. If no coverage was returned by the API, the list is empty.
     """
-    if pil_args is None:
-        pil_args = {}
+    x, y = geo.wgs84_to_tile_coord(lat, lon, 17)
+    return get_coverage_tile(x, y, session=session)
 
-    if single_image:
-        pano = get_panorama(panoid, zoom=zoom, single_image=single_image)
-        pano.save(path, **pil_args)
-    else:
-        faces = get_panorama(panoid, zoom=zoom, single_image=single_image)
-        path = Path(path)
-        for idx, face in enumerate(faces):
-            face_path = path.parent / f"{path.stem}_{idx}{path.suffix}"
-            face.save(face_path, **pil_args)
 
+async def get_coverage_tile_by_latlon_async(lat: float, lon: float, session: ClientSession) -> List[LookaroundPanorama]:
+    x, y = geo.wgs84_to_tile_coord(lat, lon, 17)
+    return await get_coverage_tile_async(x, y, session)
 
-def get_panorama(panoid: int, zoom: int = 3, single_image: bool = True) -> Union[List[Image.Image], Image.Image]:
-    """
-    Downloads a panorama as PIL image.
+
+def get_panorama_face(pano: Union[LookaroundPanorama, Tuple[int, int]],
+                      face: Face, zoom: int,
+                      auth: Authenticator, session: Session = None) -> bytes:
     """
-    faces = _generate_tile_list(panoid, zoom)
-    _download_tiles(faces)
-    return _stitch_panorama(faces, single_image=single_image)
+    Downloads one face of a panorama and returns it as ``bytes``.
 
+    Images are in HEIC format. Since HEIC is a poorly supported format across the board,
+    decoding the image is left to the user of the library.
 
-def _generate_tile_list(panoid, zoom):
-    """
-    Generates a list of a panorama's tiles.
-    Returns a list of faces and its tiles.
+    :param pano: The panorama, or its ID.
+    :param face: The face.
+    :param zoom: The zoom level. 0 is highest, 7 is lowest.
+    :param auth: An Authenticator object.
+    :param session: *(optional)* A requests session.
+    :return: The HEIC file containing the face.
     """
-    if zoom > 3:
-        raise ValueError("Zoom can't be greater than 3")
-    panoid_base4 = to_base4(panoid).rjust(16, "0")
-    subdivs = pow(4, zoom)
-    faces = {}
-    for face_id in range(0, 6):
-        face_id_base4 = to_base4(face_id + 1).rjust(2, "0")
-        face_tiles = []
-        for subdiv in range(0, subdivs):
-            if zoom < 1:
-                subdiv_base4 = ""
-            else:
-                subdiv_base4 = to_base4(subdiv).rjust(zoom, "0")
-            tile_key = f"{face_id_base4}{subdiv_base4}"
-            url = f"https://t.ssl.ak.tiles.virtualearth.net/tiles/hs{panoid_base4}{tile_key}.jpg?g=0"
-            face_tiles.append({"face": face_id_base4, "subdiv": subdiv, "url": url})
-        faces[face_id] = face_tiles
-    return faces
+    panoid, region_id = _panoid_to_string(pano)
+    url = _build_panorama_face_url(panoid, region_id, int(face), zoom, auth)
+    requester = session if session else requests
+    response = requester.get(url)
 
+    if response.ok:
+        return response.content
+    else:
+        raise Exception(str(response))
 
-def _download_tiles(faces):
-    """
-    Downloads the tiles of a panorama.
-    """
-    for face_id, face in faces.items():
-        tiles = asyncio.run(download_files_async([tile["url"] for tile in face]))
-        for idx, tile in enumerate(face):
-            tile["image"] = tiles[idx]
 
+def download_panorama_face(pano: Union[LookaroundPanorama, Tuple[int, int]],
+                           path: str, face: Face, zoom: int,
+                           auth: Authenticator, session: Session = None) -> None:
+    """
+    Downloads one face of a panorama to a file.
+
+    :param pano: The panorama, or its ID.
+    :param path: Output path.
+    :param face: The face.
+    :param zoom: The zoom level. 0 is highest, 7 is lowest.
+    :param auth: An Authenticator object.
+    :param session: *(optional)* A requests session.
+    """
+    face_bytes = get_panorama_face(pano, face, zoom, auth, session)
+    with open(path, "wb") as f:
+        f.write(face_bytes)
+
+
+"""
+# TODO make this work. as it is, it 403s every time
+
+async def get_panorama_face_async(pano: Union[LookaroundPanorama, Tuple[int, int]],
+                                  face: Face, zoom: int,
+                                  auth: Authenticator, session: ClientSession) -> bytes:
+    panoid, region_id = _panoid_to_string(pano)
+    url = _build_panorama_face_url(panoid, region_id, int(face), zoom, auth)
+    async with session.get(url) as response:
+        if response.ok:
+            return await response.read()
+        else:
+            raise Exception(str(response))
+
+async def download_panorama_face_async(pano: Union[LookaroundPanorama, Tuple[int, int]],
+                                       path: str, face: Face, zoom: int,
+                                       auth: Authenticator, session: ClientSession) -> None:
+    face_bytes = await get_panorama_face_async(pano, face, zoom, auth, session)
+    with open(path, "wb") as f:
+        f.write(face_bytes) 
+"""
+
+
+def _panoid_to_string(pano):
+    if isinstance(pano, LookaroundPanorama):
+        panoid, region_id = str(pano.id), str(pano.region_id)
+    else:
+        panoid, region_id = str(pano[0]), str(pano[1])
 
-def _stitch_four(face):
-    """
-    Stitches four consecutive individual tiles.
-    """
-    sub_tile = Image.new('RGB', (TILE_SIZE * 2, TILE_SIZE * 2))
-    for idx, tile in enumerate(face[0:4]):
-        tile_img = Image.open(BytesIO(tile["image"]))
-        x = idx % 2
-        y = idx // 2
-        sub_tile.paste(im=tile_img, box=(x * TILE_SIZE, y * TILE_SIZE))
-    return sub_tile
+    if len(panoid) > 20:
+        raise ValueError("panoid must not be longer than 20 digits.")
+    if len(region_id) > 10:
+        raise ValueError("region_id must not be longer than 10 digits.")
 
+    return panoid, region_id
 
-split_list = lambda lst, sz: [lst[i:i+sz] for i in range(0, len(lst), sz)]
+
+def _parse_panos(tile, tile_x, tile_y):
+    panos = []
+    for raw_pano in tile.pano:
+        lat, lon = _protobuf_tile_offset_to_wgs84(
+            raw_pano.location.longitude_offset,
+            raw_pano.location.latitude_offset,
+            tile_x,
+            tile_y)
+        heading = _convert_heading(lat, lon, raw_pano.location.heading)
+        pano = LookaroundPanorama(
+            raw_pano.panoid,
+            tile.unknown13[raw_pano.region_id_idx].region_id,
+            lat,
+            lon,
+            heading,
+            CoverageType(tile.unknown13[raw_pano.region_id_idx].coverage_type),
+            datetime.utcfromtimestamp(raw_pano.timestamp / 1000.0)
+        )
+        panos.append(pano)
+    return panos
 
 
-def _stitch_face(face):
+def _convert_heading(lat: float, lon: float, raw_heading: int) -> float:
     """
-    Stitches one face of a panorama.
+    Converts the raw heading value to radians.
     """
-    if len(face) <= 4:
-        return _stitch_four(face)
-    else:
-        grid_size = int(math.sqrt(len(face)))
-        stitched_tile_size = (grid_size // 2) * TILE_SIZE
-        tile = Image.new('RGB', (stitched_tile_size * 2, stitched_tile_size * 2))
-        split = split_list(face, len(face) // 4)
-        tile.paste(im=_stitch_face(split[0]), box=(0, 0))
-        tile.paste(im=_stitch_face(split[1]), box=(stitched_tile_size, 0))
-        tile.paste(im=_stitch_face(split[2]), box=(0, stitched_tile_size))
-        tile.paste(im=_stitch_face(split[3]), box=(stitched_tile_size, stitched_tile_size))
-        return tile
-
-
-def _stitch_panorama(faces, single_image: bool = True) -> Union[List[Image.Image], Image.Image]:
-    """
-    Stitches downloaded tiles into full faces or one full image.
-    """
-    full_tile_size = int(math.sqrt(len(faces[1]))) * TILE_SIZE
-
-    stitched_faces = []
-    if len(faces[1]) == 1:
-        for i in range(0, 6):
-            stitched_faces.append(Image.open(BytesIO(faces[i][0]["image"])))
-    else:
-        for i in range(0, 6):
-            stitched_faces.append(_stitch_face(faces[i]))
-
-    if not single_image:
-        return stitched_faces
-    else:
-        pano_width = 4 * full_tile_size
-        pano_height = 3 * full_tile_size
-        image = Image.new('RGB', (pano_width, pano_height))
-
-        image.paste(im=stitched_faces[0], box=(1 * full_tile_size, 1 * full_tile_size))
-        image.paste(im=stitched_faces[1], box=(2 * full_tile_size, 1 * full_tile_size))
-        image.paste(im=stitched_faces[2], box=(3 * full_tile_size, 1 * full_tile_size))
-        image.paste(im=stitched_faces[3], box=(0,                  1 * full_tile_size))
-        image.paste(im=stitched_faces[4], box=(1 * full_tile_size, 0))
-        image.paste(im=stitched_faces[5], box=(1 * full_tile_size, 2 * full_tile_size))
-        return image
+    offset_factor = 1 / (16384 / 360)
+    heading = (offset_factor * raw_heading) - lon
+    # in the southern hemisphere, the heading also needs to be mirrored across the 90°/270° line
+    if lat < 0:
+        heading = -(heading - 90) + 90
+    return math.radians(heading)
+
+
+def _protobuf_tile_offset_to_wgs84(x_offset: int, y_offset: int, tile_x: int, tile_y: int) -> Tuple[float, float]:
+    """
+    Calculates the absolute position of a pano from the tile offsets returned by the API.
+    :param x_offset: The X coordinate of the raw tile offset returned by the API.
+    :param y_offset: The Y coordinate of the raw tile offset returned by the API.
+    :param tile_x: X coordinate of the tile this pano is on, at z=17.
+    :param tile_y: Y coordinate of the tile this pano is on, at z=17.
+    :return: The WGS84 lat/lon of the pano.
+    """
+    TILE_SIZE = 256
+    pano_x = tile_x + (x_offset / 64.0) / (TILE_SIZE - 1)
+    pano_y = tile_y + (255 - (y_offset / 64.0)) / (TILE_SIZE - 1)
+    lat, lon = geo.tile_coord_to_wgs84(pano_x, pano_y, 17)
+    return lat, lon
+
+
+def _build_panorama_face_url(panoid: str, region_id: str, face: int, zoom: int, auth: Authenticator) -> str:
+    zoom = min(7, zoom)
+    panoid_padded = panoid.zfill(20)
+    panoid_split = [panoid_padded[i:i + 4] for i in range(0, len(panoid_padded), 4)]
+    panoid_url = "/".join(panoid_split)
+    region_id_padded = region_id.zfill(10)
+    url = FACE_ENDPOINT + f"{panoid_url}/{region_id_padded}/t/{face}/{zoom}"
+    url = auth.authenticate_url(url)
+    return url
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `streetlevel-0.3.1/streetlevel/streetview/depth.py` & `streetlevel-0.4.0/streetlevel/streetview/depth.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/streetlevel/streetview/protobuf.py` & `streetlevel-0.4.0/streetlevel/streetview/protobuf.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/streetlevel/streetview/streetview.py` & `streetlevel-0.4.0/streetlevel/streetview/streetview.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,223 +1,252 @@
-import asyncio
-from io import BytesIO
 import itertools
-import json
-from typing import List, Union
-
+from typing import List, Optional
 from PIL import Image
-import requests
+from aiohttp import ClientSession
 from requests import Session
 
 from streetlevel.geo import *
-from .panorama import StreetViewPanorama, LocalizedString
-from .protobuf import *
+from .panorama import StreetViewPanorama, LocalizedString, CaptureDate
 from .depth import parse as parse_depth
-from ..dataclasses import Size
-from ..util import try_get, download_files_async
-
-
-def is_third_party_panoid(panoid: str) -> bool:
-    """
-    Returns whether a panoid refers to a third-party panorama.
-    """
-    return len(panoid) > 22
-
-
-def _split_ietf(tag: str) -> (str, str):
-    """
-    Splits an IETF language tag into its language part and country part.
-    """
-    tag = tag.split("-")
-    lang = tag[0]
-    country = tag[1] if len(tag) > 1 else tag[0]
-    return lang, country
-
-
-def _find_panorama_raw(lat, lon, radius=50, download_depth=False, locale="en", session=None):
-    radius = float(radius)
-    toggles = []
-    search_third_party = False
-    include_resolution_info = True
-    include_street_name_and_date = True
-    include_copyright_information = True
-    include_neighbors_and_historical = True
-    ietf_lang, ietf_country = _split_ietf(locale)
-
-    if search_third_party:
-        image_type = 10
-    else:
-        image_type = 2
-
-    if download_depth:
-        depth1 = {1: ProtobufEnum(0)}
-        depth2 = {1: ProtobufEnum(2)}
-    else:
-        depth1 = {}
-        depth2 = {}
-
-    if include_resolution_info:
-        toggles.append(ProtobufEnum(1))
-    if include_street_name_and_date:
-        toggles.append(ProtobufEnum(2))
-    if include_copyright_information:
-        toggles.append(ProtobufEnum(3))
-    toggles.append(ProtobufEnum(4))
-    if include_neighbors_and_historical:
-        toggles.append(ProtobufEnum(6))
-    toggles.append(ProtobufEnum(8))
-
-    search_message = {
-        1: {
-            1: 'apiv3',
-            5: 'US',
-            11: {1: {1: False}}
-        },
-        2: {1: {3: lat, 4: lon}, 2: radius},
-        3: {
-            2: {1: ietf_lang, 2: ietf_country},
-            9: {1: ProtobufEnum(2)},
-            11: {
-                1: {1: ProtobufEnum(image_type), 2: True, 3: ProtobufEnum(2)}
-            },
-        },
-        4: {
-            1: toggles,
-            5: depth1,
-            6: depth2,
-        }
-    }
-
-    url = "https://maps.googleapis.com/maps/api/js/GeoPhotoService.SingleImageSearch?pb=" \
-          + to_protobuf_url(search_message) + "&callback=_xdc_._v2mub5"
-
-    if session is None:
-        response = requests.get(url).text
-    else:
-        response = session.get(url).text
-    first_paren = response.index("(")
-    last_paren = response.rindex(")")
-    pano_data_json = "[" + response[first_paren + 1:last_paren] + "]"
-    pano_data = json.loads(pano_data_json)
-    return pano_data
+from . import api
+from ..dataclasses import Size, Tile
+from ..util import try_get, download_tiles, download_tiles_async, stitch_tiles
+from .util import is_third_party_panoid
 
 
-def find_panorama(lat: float, lon: float, radius: int = 50,
-                  locale: str = "en", session: Session = None) -> Union[StreetViewPanorama, None]:
+def find_panorama(lat: float, lon: float, radius: int = 50, locale: str = "en",
+                  search_third_party: bool = False, session: Session = None) -> Optional[StreetViewPanorama]:
     """
     Searches for a panorama within a radius around a point.
+
+    :param lat: Latitude of the center point.
+    :param lon: Longitude of the center point.
+    :param radius: *(optional)* Search radius in meters. Defaults to 50.
+    :param locale: *(optional)* Desired language of the location's address as IETF code.
+      Defaults to ``en``.
+    :param search_third_party: *(optional)* Whether to search for third-party panoramas
+      rather than official ones. Defaults to false.
+    :param session: *(optional)* A requests session.
+    :return: A StreetViewPanorama object if a panorama was found, or None.
     """
+
     # TODO
     # the `SingleImageSearch` call returns a different kind of depth data
     # than `photometa`; need to deal with that at some point
-    resp = _find_panorama_raw(lat, lon, radius=radius, download_depth=False,
-                              locale=locale, session=session)
+
+    resp = api.find_panorama_raw(lat, lon, radius=radius, download_depth=False,
+                                 locale=locale, search_third_party=search_third_party, session=session)
 
     response_code = resp[0][0][0]
     # 0: OK
     # 5: search returned no images
     # don't know if there are others
     if response_code != 0:
         return None
 
     pano = _parse_pano_message(resp[0][1])
     return pano
 
 
-def _lookup_panoid_raw(panoid, download_depth=False, locale="en", session=None):
-    pano_type = 10 if is_third_party_panoid(panoid) else 2
-    toggles = []
-    include_resolution_info = True
-    include_street_name_and_date = True
-    include_copyright_information = True
-    include_neighbors_and_historical = True
-    ietf_lang, ietf_country = _split_ietf(locale)
-
-    if include_resolution_info:
-        toggles.append(ProtobufEnum(1))
-    if include_street_name_and_date:
-        toggles.append(ProtobufEnum(2))
-    if include_copyright_information:
-        toggles.append(ProtobufEnum(3))
-    toggles.append(ProtobufEnum(4))  # does nothing?
-    toggles.append(ProtobufEnum(5))  # does nothing?
-    if include_neighbors_and_historical:
-        toggles.append(ProtobufEnum(6))
-
-    # these change stuff, but idk what exactly:
-    toggles.append(ProtobufEnum(8))
-    # toggles.append(ProtobufEnum(11))
-    toggles.append(ProtobufEnum(12))
-    # toggles.append(ProtobufEnum(13))
-
-    if download_depth:
-        depth1 = [{1: ProtobufEnum(1)}, {1: ProtobufEnum(2)}]
-        depth2 = [{1: ProtobufEnum(1)}, {1: ProtobufEnum(2)}]
-    else:
-        depth1 = [{}]
-        depth2 = [{}]
-
-    # this is the protobuf message in the request URL written out as a dict
-    pano_request_message = {
-        1: {1: 'maps_sv.tactile', 11: {2: {1: True}}},
-        2: {1: ietf_lang, 2: ietf_country},
-        3: {1: {1: ProtobufEnum(pano_type), 2: panoid}},
-        4: {
-            1: toggles,
-            2: {1: ProtobufEnum(1)},  # changing this to any other value causes huge changes;
-            # haven't looked into it any further though
-            4: {1: 48},  # all this does is change the size param in an icon URL
-            5: depth1,
-            6: depth2,
-            9: {  # none of these seem to do anything
-                1: [
-                    {1: ProtobufEnum(2), 2: True, 3: ProtobufEnum(2)},
-                    {1: ProtobufEnum(2), 2: False, 3: ProtobufEnum(3)},
-                    {1: ProtobufEnum(3), 2: True, 3: ProtobufEnum(2)},
-                    {1: ProtobufEnum(3), 2: False, 3: ProtobufEnum(3)},
-                    {1: ProtobufEnum(8), 2: False, 3: ProtobufEnum(3)},
-                    {1: ProtobufEnum(1), 2: False, 3: ProtobufEnum(3)},
-                    {1: ProtobufEnum(4), 2: False, 3: ProtobufEnum(3)},
-                    {1: ProtobufEnum(10), 2: True, 3: ProtobufEnum(2)},
-                    {1: ProtobufEnum(10), 2: False, 3: ProtobufEnum(3)}
-                ]
-            }
-        }
-    }
-    url = f"https://www.google.com/maps/photometa/v1?authuser=0&hl={ietf_lang}&gl={ietf_country}&pb=" \
-          + to_protobuf_url(pano_request_message)
-
-    if session is None:
-        response = requests.get(url).text
-    else:
-        response = session.get(url).text
-    pano_data_json = response[4:]  # skip that junk at the start
-    pano_data = json.loads(pano_data_json)
-    return pano_data
+async def find_panorama_async(lat: float, lon: float, session: ClientSession, radius: int = 50,
+                              locale: str = "en", search_third_party: bool = False) -> Optional[StreetViewPanorama]:
+    # TODO
+    # the `SingleImageSearch` call returns a different kind of depth data
+    # than `photometa`; need to deal with that at some point
+    resp = await api.find_panorama_raw_async(lat, lon, session, radius=radius, download_depth=False,
+                                             locale=locale, search_third_party=search_third_party)
+
+    response_code = resp[0][0][0]
+    # 0: OK
+    # 5: search returned no images
+    # don't know if there are others
+    if response_code != 0:
+        return None
 
+    pano = _parse_pano_message(resp[0][1])
+    return pano
 
-def lookup_panoid(panoid: str, download_depth: bool = False,
-                  locale: str = "en", session: Session = None) -> Union[StreetViewPanorama, None]:
+
+def find_panorama_by_id(panoid: str, download_depth: bool = False, locale: str = "en",
+                        session: Session = None) -> Optional[StreetViewPanorama]:
     """
-    Fetches metadata for a specific panorama.
+    Fetches metadata of a specific panorama.
+
+    Unfortunately, `as mentioned on this page
+    <https://developers.google.com/maps/documentation/tile/streetview#panoid_response>`_,
+    pano IDs are not stable, so a request that works today may return nothing a few months into the future.
+
+    :param panoid: The pano ID.
+    :param download_depth: Whether to download and parse the depth map.
+    :param locale: Desired language of the location's address as IETF code.
+    :param session: *(optional)* A requests session.
+    :return: A StreetViewPanorama object if a panorama with this ID exists, or None.
     """
-    resp = _lookup_panoid_raw(panoid, download_depth=download_depth,
-                              locale=locale, session=session)
+    resp = api.lookup_panoid_raw(panoid, download_depth=download_depth,
+                                 locale=locale, session=session)
 
     response_code = resp[1][0][0][0]
     # 1: OK
     # 2: Not found
     # don't know if there are others
     if response_code != 1:
         return None
 
     pano = _parse_pano_message(resp[1][0])
     return pano
 
 
+lookup_panoid = find_panorama_by_id
+
+
+async def find_panorama_by_id_async(panoid: str, session: ClientSession, download_depth: bool = False,
+                                    locale: str = "en") -> Optional[StreetViewPanorama]:
+    resp = await api.lookup_panoid_raw_async(panoid, session, download_depth=download_depth, locale=locale)
+
+    response_code = resp[1][0][0][0]
+    # 1: OK
+    # 2: Not found
+    # don't know if there are others
+    if response_code != 1:
+        return None
+
+    pano = _parse_pano_message(resp[1][0])
+    return pano
+
+
+def get_coverage_tile(tile_x: int, tile_y: int, session: Session = None) -> List[StreetViewPanorama]:
+    """
+    Fetches Street View coverage on a specific map tile. Coordinates are in Slippy Map aka XYZ format
+    at zoom level 17.
+
+    When viewing Google Maps with satellite imagery in globe view and zooming into a spot,
+    it makes this API call. This is useful because 1) it allows for fetching coverage for a whole area, and
+    2) there are various hidden/removed locations which cannot be found by any other method
+    (unless you access them by pano ID directly).
+
+    Note, however, that only ID, latitude and longitude of the most recent coverage are returned.
+    The rest of the metadata, as well as historical panoramas, must be fetched manually one by one.
+
+    :param tile_x: X coordinate of the tile.
+    :param tile_y: Y coordinate of the tile.
+    :param session: *(optional)* A requests session.
+    :return: A list of StreetViewPanoramas. If no coverage was returned by the API, the list is empty.
+    """
+    resp = api.get_coverage_tile_raw(tile_x, tile_y, session)
+
+    if resp is None:
+        return []
+
+    return _parse_coverage_tile_response(resp)
+
+
+async def get_coverage_tile_async(tile_x: int, tile_y: int, session: ClientSession) -> List[StreetViewPanorama]:
+    resp = await api.get_coverage_tile_raw_async(tile_x, tile_y, session)
+
+    if resp is None:
+        return []
+
+    return _parse_coverage_tile_response(resp)
+
+
+def get_coverage_tile_by_latlon(lat: float, lon: float, session: Session = None) -> List[StreetViewPanorama]:
+    """
+    Same as :func:`get_coverage_tile <get_coverage_tile>`, but for fetching the tile on which a point is located.
+
+    :param lat: Latitude of the point.
+    :param lon: Longitude of the point.
+    :param session: *(optional)* A requests session.
+    :return: A list of StreetViewPanoramas. If no coverage was returned by the API, the list is empty.
+    """
+    tile_coord = wgs84_to_tile_coord(lat, lon, 17)
+    return get_coverage_tile(tile_coord[0], tile_coord[1], session=session)
+
+
+async def get_coverage_tile_by_latlon_async(lat: float, lon: float, session: ClientSession) \
+        -> List[StreetViewPanorama]:
+    tile_coord = wgs84_to_tile_coord(lat, lon, 17)
+    return await get_coverage_tile_async(tile_coord[0], tile_coord[1], session)
+
+
+def download_panorama(pano: StreetViewPanorama, path: str, zoom: int = 5, pil_args: dict = None) -> None:
+    """
+    Downloads a panorama to a file.
+
+    :param pano: The panorama to download.
+    :param path: Output path.
+    :param zoom: *(optional)* Image size; 0 is lowest, 5 is highest. The dimensions of a zoom level of a
+        specific panorama depend on the camera used. If the requested zoom level does not exist,
+        the highest available level will be downloaded. Defaults to 5.
+    :param pil_args: *(optional)* Additional arguments for PIL's
+        `Image.save <https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.save>`_
+        method, e.g. ``{"quality":100}``. Defaults to ``{}``.
+    """
+    if pil_args is None:
+        pil_args = {}
+    image = get_panorama(pano, zoom=zoom)
+    image.save(path, **pil_args)
+
+
+async def download_panorama_async(pano: StreetViewPanorama, path: str, session: ClientSession,
+                                  zoom: int = 5, pil_args: dict = None) -> None:
+    if pil_args is None:
+        pil_args = {}
+    image = await get_panorama_async(pano, session, zoom=zoom)
+    image.save(path, **pil_args)
+
+
+def get_panorama(pano: StreetViewPanorama, zoom: int = 5) -> Image.Image:
+    """
+    Downloads a panorama and returns it as PIL image.
+
+    :param pano: The panorama to download.
+    :param zoom: *(optional)* Image size; 0 is lowest, 5 is highest. The dimensions of a zoom level of a
+        specific panorama depend on the camera used. If the requested zoom level does not exist,
+        the highest available level will be downloaded. Defaults to 5.
+    :return: A PIL image containing the panorama.
+    """
+    zoom = _validate_get_panorama_params(pano, zoom)
+    tile_list = _generate_tile_list(pano, zoom)
+    tile_images = download_tiles(tile_list)
+    stitched = stitch_tiles(tile_images,
+                            pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
+                            pano.tile_size.x, pano.tile_size.y)
+    return stitched
+
+
+async def get_panorama_async(pano: StreetViewPanorama, session: ClientSession, zoom: int = 5) -> Image.Image:
+    zoom = _validate_get_panorama_params(pano, zoom)
+    tile_list = _generate_tile_list(pano, zoom)
+    tile_images = await download_tiles_async(tile_list, session)
+    stitched = stitch_tiles(tile_images,
+                            pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
+                            pano.tile_size.x, pano.tile_size.y)
+    return stitched
+
+
+def _validate_get_panorama_params(pano, zoom):
+    if not pano.image_sizes:
+        raise ValueError("pano.image_sizes is None.")
+    zoom = max(0, min(zoom, len(pano.image_sizes) - 1))
+    return zoom
+
+
+def _parse_coverage_tile_response(tile):
+    panos = []
+    if tile[1] is not None and len(tile[1]) > 0:
+        for pano in tile[1][1]:
+            if pano[0][0] == 1:
+                continue
+            panoid = pano[0][0][1]
+            lat = pano[0][2][0][2]
+            lon = pano[0][2][0][3]
+            panos.append(StreetViewPanorama(panoid, lat, lon))
+    return panos
+
+
 def _parse_pano_message(msg):
     img_sizes = msg[2][3][0]
     img_sizes = list(map(lambda x: Size(x[0][1], x[0][0]), img_sizes))
     panoid = msg[1][1]
     lat = msg[5][0][1][0][2]
     lon = msg[5][0][1][0][3]
     others = try_get(lambda: msg[5][0][3][0])
@@ -242,17 +271,17 @@
     pano = StreetViewPanorama(
         id=panoid,
         lat=lat,
         lon=lon,
         heading=try_get(lambda: math.radians(msg[5][0][1][2][0])),
         pitch=try_get(lambda: math.radians(90 - msg[5][0][1][2][1])),
         roll=try_get(lambda: math.radians(msg[5][0][1][2][2])),
-        year=date[0],
-        month=date[1],
-        day=date[2] if len(date) > 2 else None,
+        date=CaptureDate(date[0],
+                         date[1],
+                         date[2] if len(date) > 2 else None),
         tile_size=Size(msg[2][3][1][0], msg[2][3][1][1]),
         image_sizes=img_sizes,
         source=source,
         country_code=try_get(lambda: msg[5][0][1][4]),
         street_name=street_name,
         address=address,
         copyright_message=try_get(lambda: msg[4][0][0][0][0]),
@@ -284,128 +313,25 @@
 
             connected.street_name = try_get(lambda: other[3][2][0])
     pano.historical = sorted(pano.historical, key=lambda x: (x.year, x.month), reverse=True)
 
     return pano
 
 
-def download_panorama(pano: StreetViewPanorama, path: str, zoom: int = 5, pil_args: dict = None) -> None:
-    """
-    Downloads and stitches a panorama and saves it to a file.
-    """
-    if pil_args is None:
-        pil_args = {}
-    pano = get_panorama(pano, zoom=zoom)
-    pano.save(path, **pil_args)
-
-
-def get_panorama(pano: StreetViewPanorama, zoom: int = 5) -> Image:
+def _generate_tile_list(pano: StreetViewPanorama, zoom: int) -> List[Tile]:
     """
-    Downloads and stitches a panorama and returns it as PIL image.
-    """
-    zoom = max(0, min(zoom, len(pano.image_sizes) - 1))
-    tile_list = _generate_tile_list(pano, zoom)
-    tiles = _download_tiles(tile_list)
-    stitched = _stitch_tiles(pano, tile_list, tiles, zoom)
-    return stitched
-
-
-def _generate_tile_list(pano, zoom):
-    """
-    Generates a list of a panorama's tiles.
-    Returns a list of (x, y, tile_url) tuples.
+    Generates a list of a panorama's tiles and the URLs pointing to them.
     """
     img_size = pano.image_sizes[zoom]
     tile_width = pano.tile_size.x
     tile_height = pano.tile_size.y
     cols = math.ceil(img_size.x / tile_width)
     rows = math.ceil(img_size.y / tile_height)
 
-    image_url = "https://cbk0.google.com/cbk?output=tile&panoid={0:}&zoom={3:}&x={1:}&y={2:}"
-    third_party_image_url = "https://lh3.ggpht.com/p/{0:}=x{1:}-y{2:}-z{3:}"
+    IMAGE_URL = "https://cbk0.google.com/cbk?output=tile&panoid={0:}&zoom={3:}&x={1:}&y={2:}"
+    THIRD_PARTY_IMAGE_URL = "https://lh3.ggpht.com/p/{0:}=x{1:}-y{2:}-z{3:}"
 
-    url_to_use = third_party_image_url if is_third_party_panoid(pano.id) else image_url
+    url_to_use = THIRD_PARTY_IMAGE_URL if is_third_party_panoid(pano.id) else IMAGE_URL
 
-    coord = list(itertools.product(range(cols), range(rows)))
-    tiles = [(x, y, url_to_use.format(pano.id, x, y, zoom)) for x, y in coord]
+    coords = list(itertools.product(range(cols), range(rows)))
+    tiles = [Tile(x, y, url_to_use.format(pano.id, x, y, zoom)) for x, y in coords]
     return tiles
-
-
-def _download_tiles(tile_list):
-    """
-    Downloads tiles from a tile list generated by _generate_tile_list().
-    """
-    tiles = asyncio.run(download_files_async([t[2] for t in tile_list]))
-
-    tile_data = {}
-    for i, (x, y, url) in enumerate(tile_list):
-        tile_data[(x, y)] = tiles[i]
-
-    return tile_data
-
-
-def _stitch_tiles(pano, tile_list, tile_data, zoom):
-    """
-    Stitches downloaded tiles to a full image.
-    """
-    img_size = pano.image_sizes[zoom]
-    tile_width = pano.tile_size.x
-    tile_height = pano.tile_size.y
-
-    panorama = Image.new('RGB', (img_size.x, img_size.y))
-
-    for x, y, url in tile_list:
-        tile = Image.open(BytesIO(tile_data[(x, y)]))
-        panorama.paste(im=tile, box=(x * tile_width, y * tile_height))
-        del tile
-
-    return panorama
-
-
-def get_coverage_tile(tile_x: int, tile_y: int, session: Session = None) -> List[StreetViewPanorama]:
-    """
-    Gets all panoramas on a Google Maps tile (at zoom level 17 specifically, for some reason).
-    Returns panoid, lat, lon only.
-    This function uses the API call which is triggered when zooming into a tile in globe view on Google Maps,
-    so it can be used to find hidden coverage.
-    This call only returns the most recent coverage for a location.
-    """
-    resp = _get_coverage_tile_raw(tile_x, tile_y, session)
-
-    if resp is None:
-        return []
-
-    panos = []
-    if resp[1] is not None and len(resp[1]) > 0:
-        for pano in resp[1][1]:
-            if pano[0][0] == 1:
-                continue
-            panoid = pano[0][0][1]
-            lat = pano[0][2][0][2]
-            lon = pano[0][2][0][3]
-            panos.append(StreetViewPanorama(panoid, lat, lon))
-
-    return panos
-
-
-def _get_coverage_tile_raw(tile_x, tile_y, session=None):
-    url = "https://www.google.com/maps/photometa/ac/v1?pb=!1m1!1smaps_sv.tactile!6m3!1i{0}!2i{1}!3i17!8b1"
-    url = url.format(tile_x, tile_y)
-    if session is None:
-        response = requests.get(url).text
-    else:
-        response = session.get(url).text
-    data_json = response[4:]
-    data = json.loads(data_json)
-    return data
-
-
-def get_coverage_tile_by_latlon(lat: float, lon: float, session: Session = None) -> List[StreetViewPanorama]:
-    """
-    Gets all panoramas on a Google Maps tile (at zoom level 17 specifically, for some reason).
-    Returns panoid, lat, lon only.
-    This function uses the API call which is triggered when zooming into a tile in globe view on Google Maps,
-    so it can be used to find hidden coverage.
-    This call only returns the most recent coverage for a location.
-    """
-    tile_coord = wgs84_to_tile_coord(lat, lon, 17)
-    return get_coverage_tile(tile_coord[0], tile_coord[1], session=session)
```

### Comparing `streetlevel-0.3.1/tests/streetside/streetside_test.py` & `streetlevel-0.4.0/tests/streetside/streetside_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import pytest
 from pytest import approx
 import json
 from streetlevel import streetside
-from streetlevel.dataclasses import Size
 
 
 def mocked_find_panoramas_raw(north, west, south, east, limit=50, session=None):
     with open("streetside/data/find_object.json", "r") as f:
         return json.load(f)
 
 
-streetside.streetside._find_panoramas_raw = mocked_find_panoramas_raw
+streetside.api.find_panoramas_raw = mocked_find_panoramas_raw
 
 
 def test_find_panoramas_in_bbox():
     panos = streetside.find_panoramas_in_bbox(-23.860792, 35.343169, -23.863089, 35.347470)
     assert len(panos) != 0
     assert panos[0].id == 362530254
     assert panos[0].lat == approx(-23.862083, 0.001)
```

### Comparing `streetlevel-0.3.1/tests/streetside/data/find_object.json` & `streetlevel-0.4.0/tests/streetside/data/find_object.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/tests/streetview/streetview_test.py` & `streetlevel-0.4.0/tests/streetview/streetview_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-import pytest
 from pytest import approx
 import json
 from streetlevel import streetview
 from streetlevel.dataclasses import Size
 
 
 def mocked_lookup_panoid_raw(panoid, download_depth=False, locale="en", session=None):
     with open("streetview/data/lookup_object.json", "r") as f:
         return json.load(f)
 
 
-def mocked_find_panorama_raw(lat, lon, radius=50, download_depth=False, locale="en", session=None):
+def mocked_find_panorama_raw(lat, lon, radius=50, download_depth=False, locale="en",
+                             search_third_party=False, session=None):
     with open("streetview/data/find_object.json", "r") as f:
         return json.load(f)
 
 
 def mocked_get_coverage_tile_raw(tile_x, tile_y, session=None):
     with open("streetview/data/coverage_tile_object.json", "r") as f:
         return json.load(f)
 
 
-streetview.streetview._lookup_panoid_raw = mocked_lookup_panoid_raw
-streetview.streetview._find_panorama_raw = mocked_find_panorama_raw
-streetview.streetview._get_coverage_tile_raw = mocked_get_coverage_tile_raw
+streetview.api.lookup_panoid_raw = mocked_lookup_panoid_raw
+streetview.api.find_panorama_raw = mocked_find_panorama_raw
+streetview.api.get_coverage_tile_raw = mocked_get_coverage_tile_raw
 
 
-def test_is_third_party_panoid():
+def test_is_third_party_panoid(request):
     assert not streetview.is_third_party_panoid("n-Zd6bDDL_XOc_jkNgFsGg")
     assert streetview.is_third_party_panoid("AF1QipN3bwjvnpTUbfCZ18wsUMrpZ6Ul2mhVfNKl71_X")
 
 
-def test_lookup_panoid():
+def test_find_panorama_by_id():
     panoid = "n-Zd6bDDL_XOc_jkNgFsGg"
-    pano = streetview.lookup_panoid(panoid, download_depth=False, locale="en", session=None)
+    pano = streetview.find_panorama_by_id(panoid, download_depth=False, locale="en", session=None)
     assert pano.id == panoid
     assert pano.lat == approx(47.15048822721601, 0.001)
     assert pano.lon == approx(11.13385612403307, 0.001)
-    assert pano.month == 3
-    assert pano.year == 2021
+    assert pano.date.month == 3
+    assert pano.date.year == 2021
     assert pano.country_code == "AT"
     assert pano.tile_size == Size(512, 512)
     assert len(pano.image_sizes) == 6
     assert pano.image_sizes[-1] == Size(16384, 8192)
 
 
-# todo mock image requests
-#def test_download_panorama():
-#    panoid = "n-Zd6bDDL_XOc_jkNgFsGg"
-#    pano = streetview.lookup_panoid(panoid, download_depth=False, locale="en", session=None)
-#    image = streetview.get_panorama(pano, zoom=1)
-#    assert image.width == pano.image_sizes[1][1]
-#    assert image.height == pano.image_sizes[1][0]
-
-
 def test_find_panorama():
     pano = streetview.find_panorama(47.15048822721601, 11.13385612403307,
                                     radius=100, locale="en", session=None)
     assert pano.id == "n-Zd6bDDL_XOc_jkNgFsGg"
     assert pano.lat == approx(47.15048822721601, 0.001)
     assert pano.lon == approx(11.13385612403307, 0.001)
```

### Comparing `streetlevel-0.3.1/tests/streetview/data/coverage_tile_object.json` & `streetlevel-0.4.0/tests/streetview/data/coverage_tile_object.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/tests/streetview/data/find_object.json` & `streetlevel-0.4.0/tests/streetview/data/find_object.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/tests/streetview/data/lookup_object.json` & `streetlevel-0.4.0/tests/streetview/data/lookup_object.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/.gitignore` & `streetlevel-0.4.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -126,8 +126,9 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 .idea/
 *.ipynb
-*.jpg
+*.jpg
+*.heic
```

### Comparing `streetlevel-0.3.1/LICENSE` & `streetlevel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streetlevel-0.3.1/README.md` & `streetlevel-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # streetlevel
-**streetlevel** is a module for downloading panoramas and metadata from Google Street View, Bing Streetside and Mapy.cz Panorama.
+**streetlevel** is a module for downloading panoramas and metadata from street-level imagery services including Google Street View and Apple Look Around.
 
-Since it relies on internal / inofficial API calls, it may break unexpectedly.
+Since it relies on calls to internal APIs, it may break unexpectedly.
 
 ## Installation
 ```sh
 pip install streetlevel
 ```
 
 ## Example
@@ -14,132 +14,149 @@
 ```python
 from streetlevel import streetview
 
 pano = streetview.find_panorama(46.8839586, 12.169002)
 streetview.download_panorama(pano, f"{pano.id}.jpg")
 ```
 
+## Documentation
+Documentation is available at [streetlevel.readthedocs.io](https://streetlevel.readthedocs.io/).
+
 ## Functionality overview
 ✔ implemented / available; 🟡 partially implemented / available; ❌ not implemented; ⚫ not available / not applicable
 
 <table>
   <thead>
     <th></th>
     <th align="center">Street View</th>
+    <th align="center">Look Around</th>
     <th align="center">Streetside</th>
     <th align="center">Mapy.cz Panorama</th>
   </thead>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Finding panoramas</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Finding panoramas</b><br>
       How panoramas can be retrieved through the API.
     </td>
   </thead>
   <tr>
     <td align="right">Find panoramas around a point</td>
     <td align="center">✔<br>
       (returns closest only)
     </td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
     <td align="center">✔<br>
       (returns closest only)
     </td>
   </tr>
   <tr>
     <td align="right">Find panoramas by slippy map tile or bounding box</td>
     <td align="center">✔<br>
       (tile, z=17)
     </td>
     <td align="center">✔<br>
+      (tile, z=17)
+    </td>
+    <td align="center">✔<br>
       (bounding box)
     </td>
     <td align="center">⚫</td>
   </tr>
   <tr>
     <td align="right">Get specific panorama by ID</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">✔</td>
     <td align="center">⚫</td>
   </tr>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Imagery</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Imagery</b><br>
       The type of imagery returned by the service.
     </td>
   </thead>
   <tr>
     <td align="right">Download panoramas</td>
     <td align="center">✔</td>
+    <td align="center">✔<br>(unstitched)</td>
     <td align="center">✔</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Download depth information</td>
-    <td align="center">✔</td>
+    <td align="center">✔<br>(simplified)</td>
+    <td align="center">❌</td>
     <td align="center">⚫</td>
     <td align="center">⚫<br>(?)</td>
   </tr>
   <tr>
     <td align="right">Image projection</td>
     <td align="center">Equirectangular</td>
+    <td align="center">???</td>
     <td align="center">Cubemap</td>
     <td align="center">Equirectangular</td>
   </tr>
   <tr>
     <td align="right">Image format</td>
     <td align="center">JPEG</td>
+    <td align="center">HEIC</td>
     <td align="center">JPEG</td>
     <td align="center">JPEG</td>
   </tr>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Available metadata</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Available metadata</b><br>
       Metadata returned by the API of the service alongside ID and location.
     </td>
   </thead>
   <tr>
     <td align="right">Capture date</td>
     <td align="center">✔<br>
       (month and year only for official coverage; full date for inofficial coverage)
     </td>
     <td align="center">✔</td>
     <td align="center">✔</td>
+    <td align="center">✔</td>
   </tr>
   <tr>
-    <td align="right">Yaw/heading, pitch, roll</td>
-    <td align="center">✔<br>
+    <td align="right">Heading, pitch, roll</td>
+    <td align="center">✔</td>
+    <td align="center">🟡<br>(only heading is implemented; inaccurate in some locations)</td>
     <td align="center">✔</td>
     <td align="center">✔<br></td>
   </tr>
   <tr>
     <td align="right">Elevation</td>
     <td align="center">⚫</td>
+    <td align="center">❌</td>
     <td align="center">✔</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Nearby / linked panoramas</td>
     <td align="center">✔</td>
+    <td align="center">⚫</td>
     <td align="center">✔<br>
       (previous and next image in sequence)
     </td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Historical panoramas</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Address</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
   </tr>
   <tr>
     <td align="right">Creator</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
   </tr>
 </table>
-
-## Documentation
-Documentation of all available functionality can be found in the `doc` folder.
```

### Comparing `streetlevel-0.3.1/pyproject.toml` & `streetlevel-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "streetlevel"
-version = "0.3.1"
+version = "0.4.0"
 license = "MIT"
 authors = [
   { name="sk-zk", email="sk-zk@users.noreply.github.com" },
 ]
 description = "Download panoramas and metadata from Street View and others"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `streetlevel-0.3.1/PKG-INFO` & `streetlevel-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetlevel
-Version: 0.3.1
+Version: 0.4.0
 Summary: Download panoramas and metadata from Street View and others
 Project-URL: Homepage, https://github.com/sk-zk/streetlevel
 Project-URL: Bug Tracker, https://github.com/sk-zk/streetlevel/issues
 Author-email: sk-zk <sk-zk@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # streetlevel
-**streetlevel** is a module for downloading panoramas and metadata from Google Street View, Bing Streetside and Mapy.cz Panorama.
+**streetlevel** is a module for downloading panoramas and metadata from street-level imagery services including Google Street View and Apple Look Around.
 
-Since it relies on internal / inofficial API calls, it may break unexpectedly.
+Since it relies on calls to internal APIs, it may break unexpectedly.
 
 ## Installation
 ```sh
 pip install streetlevel
 ```
 
 ## Example
@@ -31,132 +31,149 @@
 ```python
 from streetlevel import streetview
 
 pano = streetview.find_panorama(46.8839586, 12.169002)
 streetview.download_panorama(pano, f"{pano.id}.jpg")
 ```
 
+## Documentation
+Documentation is available at [streetlevel.readthedocs.io](https://streetlevel.readthedocs.io/).
+
 ## Functionality overview
 ✔ implemented / available; 🟡 partially implemented / available; ❌ not implemented; ⚫ not available / not applicable
 
 <table>
   <thead>
     <th></th>
     <th align="center">Street View</th>
+    <th align="center">Look Around</th>
     <th align="center">Streetside</th>
     <th align="center">Mapy.cz Panorama</th>
   </thead>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Finding panoramas</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Finding panoramas</b><br>
       How panoramas can be retrieved through the API.
     </td>
   </thead>
   <tr>
     <td align="right">Find panoramas around a point</td>
     <td align="center">✔<br>
       (returns closest only)
     </td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
     <td align="center">✔<br>
       (returns closest only)
     </td>
   </tr>
   <tr>
     <td align="right">Find panoramas by slippy map tile or bounding box</td>
     <td align="center">✔<br>
       (tile, z=17)
     </td>
     <td align="center">✔<br>
+      (tile, z=17)
+    </td>
+    <td align="center">✔<br>
       (bounding box)
     </td>
     <td align="center">⚫</td>
   </tr>
   <tr>
     <td align="right">Get specific panorama by ID</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">✔</td>
     <td align="center">⚫</td>
   </tr>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Imagery</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Imagery</b><br>
       The type of imagery returned by the service.
     </td>
   </thead>
   <tr>
     <td align="right">Download panoramas</td>
     <td align="center">✔</td>
+    <td align="center">✔<br>(unstitched)</td>
     <td align="center">✔</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Download depth information</td>
-    <td align="center">✔</td>
+    <td align="center">✔<br>(simplified)</td>
+    <td align="center">❌</td>
     <td align="center">⚫</td>
     <td align="center">⚫<br>(?)</td>
   </tr>
   <tr>
     <td align="right">Image projection</td>
     <td align="center">Equirectangular</td>
+    <td align="center">???</td>
     <td align="center">Cubemap</td>
     <td align="center">Equirectangular</td>
   </tr>
   <tr>
     <td align="right">Image format</td>
     <td align="center">JPEG</td>
+    <td align="center">HEIC</td>
     <td align="center">JPEG</td>
     <td align="center">JPEG</td>
   </tr>
   <thead>
-    <td colspan="4" style="padding-top:20px"><b>Available metadata</b><br>
+    <td colspan="5" style="padding-top:20px"><b>Available metadata</b><br>
       Metadata returned by the API of the service alongside ID and location.
     </td>
   </thead>
   <tr>
     <td align="right">Capture date</td>
     <td align="center">✔<br>
       (month and year only for official coverage; full date for inofficial coverage)
     </td>
     <td align="center">✔</td>
     <td align="center">✔</td>
+    <td align="center">✔</td>
   </tr>
   <tr>
-    <td align="right">Yaw/heading, pitch, roll</td>
-    <td align="center">✔<br>
+    <td align="right">Heading, pitch, roll</td>
+    <td align="center">✔</td>
+    <td align="center">🟡<br>(only heading is implemented; inaccurate in some locations)</td>
     <td align="center">✔</td>
     <td align="center">✔<br></td>
   </tr>
   <tr>
     <td align="right">Elevation</td>
     <td align="center">⚫</td>
+    <td align="center">❌</td>
     <td align="center">✔</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Nearby / linked panoramas</td>
     <td align="center">✔</td>
+    <td align="center">⚫</td>
     <td align="center">✔<br>
       (previous and next image in sequence)
     </td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Historical panoramas</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
   </tr>
   <tr>
     <td align="right">Address</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
   </tr>
   <tr>
     <td align="right">Creator</td>
     <td align="center">✔</td>
     <td align="center">⚫</td>
+    <td align="center">⚫</td>
     <td align="center">✔</td>
   </tr>
 </table>
-
-## Documentation
-Documentation of all available functionality can be found in the `doc` folder.
```

