# Comparing `tmp/plateauutils-0.0.2.tar.gz` & `tmp/plateauutils-0.0.3.tar.gz`

## Comparing `plateauutils-0.0.2.tar` & `plateauutils-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 plateauutils-0.0.2/dev-requirements.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 plateauutils-0.0.2/requirements.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/Makefile
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/conf.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/make.bat
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/modules.rst
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.mesh_geocorder.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.parser.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.tile_list.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/__init__.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/plateau_parser.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/polygon_to_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/__init__.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/geo_to_mesh.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/__init__.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/__init__.py
--rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/city_gml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/tests/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/tests/test_city_gml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tests/__init__.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tests/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/__init__.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/geo_to_tile.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/polygon_to_tile_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/test_geo_to_tile.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.2/LICENSE
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 plateauutils-0.0.2/README.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 plateauutils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 plateauutils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 plateauutils-0.0.3/dev-requirements.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 plateauutils-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/Makefile
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/conf.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/make.bat
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/modules.rst
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.mesh_geocorder.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.parser.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.3/doc/plateauutils.tile_list.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/__init__.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/plateau_parser.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/abc/polygon_to_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/__init__.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/geo_to_mesh.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/__init__.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/__init__.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/tests/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/parser/tests/test_city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tests/__init__.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/geo_to_tile.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/polygon_to_tile_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/test_geo_to_tile.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.3/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 plateauutils-0.0.3/README.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 plateauutils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 plateauutils-0.0.3/PKG-INFO
```

### Comparing `plateauutils-0.0.2/dev-requirements.txt` & `plateauutils-0.0.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/.github/workflows/ci.yml` & `plateauutils-0.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/.github/workflows/documentation.yml` & `plateauutils-0.0.3/.github/workflows/documentation.yml`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install sphinx
+          if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Sphinx build
         run: |
           rm -fr _build
           sphinx-build doc _build
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
```

### Comparing `plateauutils-0.0.2/doc/Makefile` & `plateauutils-0.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/doc/conf.py` & `plateauutils-0.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/doc/index.rst` & `plateauutils-0.0.3/doc/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     >>> from shapely import from_wkt
     >>> from plateauutils.parser.city_gml_parser import CityGMLParser
     >>> target_polygon = from_wkt("POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))")
     >>> parser = CityGMLParser(target_polygon)
     >>> result = parser.download_and_parse("https://assets.cms.plateau.reearth.io/assets/d6/70821e-7f58-4f69-bc34-341875704e78/40203_kurume-shi_2020_citygml_3_op.zip", "/tmp")
     >>> result
-    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '610'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '610'},...]
+    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '非木造'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '非木造'},...]
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    modules
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plateauutils-0.0.2/doc/make.bat` & `plateauutils-0.0.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/doc/plateauutils.mesh_geocorder.rst` & `plateauutils-0.0.3/doc/plateauutils.mesh_geocorder.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/doc/plateauutils.tile_list.rst` & `plateauutils-0.0.3/doc/plateauutils.tile_list.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/cli.py` & `plateauutils-0.0.3/plateauutils/cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/abc/plateau_parser.py` & `plateauutils-0.0.3/plateauutils/abc/plateau_parser.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/abc/polygon_to_list.py` & `plateauutils-0.0.3/plateauutils/abc/polygon_to_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/mesh_geocorder/geo_to_mesh.py` & `plateauutils-0.0.3/plateauutils/mesh_geocorder/geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py` & `plateauutils-0.0.3/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class PolygonToMeshCodeList(PolygonToList):
     """Polygonからメッシュコードのリストを返すクラス
 
     Parameters
     ----------
-    polygon : shapely.geometry.Point
+    polygon : shapely.geometry.Polygon
         対象となるポリゴン
     mesh : str
         メッシュコードの粒度
     """
 
     def __init__(self, polygon, mesh="2"):
         super().__init__(polygon)
```

### Comparing `plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py` & `plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py` & `plateauutils-0.0.3/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/parser/city_gml_parser.py` & `plateauutils-0.0.3/plateauutils/parser/city_gml_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             )
             # ファイルが二つ以上ある場合に対応させる
             for file_path in glob.glob(target_file_path):
                 # XMLのオブジェクトとして読み込む
                 tree = ET.parse(file_path)
                 root = tree.getroot()
                 # パース処理を実施する
-                ret = self._parse(root)
+                ret = self._parse(root, file_path)
                 # 返り値に追加
                 return_list.extend(ret)
         # 返り値を返却
         return return_list
 
     def download_and_parse(self, url: str = "", target_dir: str = "") -> list:
         """CityGMLファイルをダウンロードして、情報を返すメソッド
@@ -114,15 +114,15 @@
             polygon_to_mesh_code = PolygonToMeshCodeList(polygon, mesh)
             # 返り値に追加
             for j in polygon_to_mesh_code.output():
                 return_list.append(j)
         # 返り値を返す
         return return_list
 
-    def _parse(self, root: ET.Element) -> list:
+    def _parse(self, root: ET.Element, file_path: str) -> list:
         # 返り値を作成
         return_list = []
         # core:cityObjectMemberの一覧を取得
         city_object_members = root.findall(
             ".//{http://www.opengis.net/citygml/2.0}cityObjectMember"
         )
         # core:cityObjectMemberごとに処理
@@ -142,26 +142,47 @@
             # uro:buildingDetailAttributeを取得
             building_detail_attribute = city_object_member.find(
                 ".//{https://www.geospatial.jp/iur/uro/2.0}buildingDetailAttribute"
             )
             # uro:buildingStructureTypeを取得
             building_structure_type = building_detail_attribute.find(
                 ".//{https://www.geospatial.jp/iur/uro/2.0}buildingStructureType"
-            ).text
+            )
+            # uro:codeSpaceを取得
+            code_space = building_structure_type.get("codeSpace")
+            # codeSpaceから値を取得
+            code_space_root = ET.parse(
+                os.path.abspath(os.path.join(file_path, "..", code_space))
+            )
+            code_space_root_root = code_space_root.getroot()
+            building_structure_type_text = None
+            for code_space_root_root_child in code_space_root_root.findall(
+                ".//{http://www.opengis.net/gml}dictionaryEntry"
+            ):
+                gml_name = code_space_root_root_child.find(
+                    ".//{http://www.opengis.net/gml}name"
+                )
+                if str(gml_name.text) == str(building_structure_type.text):
+                    building_structure_type_text = str(
+                        code_space_root_root_child.find(
+                            ".//{http://www.opengis.net/gml}description"
+                        ).text
+                    )
+                    break
             # bldg:lod1Solidを取得
             lod1_solid = city_object_member.find(
                 ".//{http://www.opengis.net/citygml/building/2.0}lod1Solid"
             )
             # 返り値に入る値を作成
             return_value = {
                 "gid": gid,
                 "center": None,
                 "min_height": 10000,
                 "measured_height": measured_height,
-                "building_structure_type": building_structure_type,
+                "building_structure_type": building_structure_type_text,
             }
             # gml:posListを取得
             pos_lists = lod1_solid.findall(".//{http://www.opengis.net/gml}posList")
             for poi_list in pos_lists:
                 # posListをパース
                 polygon, max_height = self._parse_poi_list(poi_list.text)
                 if max_height < return_value["min_height"]:
```

### Comparing `plateauutils-0.0.2/plateauutils/parser/tests/test_city_gml_parser.py` & `plateauutils-0.0.3/plateauutils/parser/tests/test_city_gml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
             "https://file.smellman.org/test_citygml.zip", tmpdir
         )
         assert len(result) == 3
         assert result[0]["gid"] == "bldg_383f1804-aa34-4634-949f-f769e09fa92d"
         assert result[0]["center"] == [130.41263587199947, 33.22489181671553]
         assert result[0]["min_height"] == 3.805999994277954
         assert result[0]["measured_height"] == 9.3
-        assert result[0]["building_structure_type"] == "610"
+        assert result[0]["building_structure_type"] == "非木造"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plateauutils-0.0.2/plateauutils/tests/test_cli.py` & `plateauutils-0.0.3/plateauutils/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/tile_list/geo_to_tile.py` & `plateauutils-0.0.3/plateauutils/tile_list/geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/tile_list/polygon_to_tile_list.py` & `plateauutils-0.0.3/plateauutils/tile_list/polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/tile_list/tests/test_geo_to_tile.py` & `plateauutils-0.0.3/plateauutils/tile_list/tests/test_geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/plateauutils/tile_list/tests/test_polygon_to_tile_list.py` & `plateauutils-0.0.3/plateauutils/tile_list/tests/test_polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/.gitignore` & `plateauutils-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/LICENSE` & `plateauutils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.2/README.rst` & `plateauutils-0.0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     '533945471'
     >>> from shapely import from_wkt
     >>> from plateauutils.parser.city_gml_parser import CityGMLParser
     >>> target_polygon = from_wkt("POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))")
     >>> parser = CityGMLParser(target_polygon)
     >>> result = parser.download_and_parse("https://assets.cms.plateau.reearth.io/assets/d6/70821e-7f58-4f69-bc34-341875704e78/40203_kurume-shi_2020_citygml_3_op.zip", "/tmp")
     >>> result
-    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '610'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '610'},...]
+    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '非木造'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '非木造'},...]
 
 How to develop
 --------------
 
 .. code:: bash
 
     python3.9 -m venv venv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plateauutils-0.0.2/pyproject.toml` & `plateauutils-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "A collection of utilities for the Plateau project"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
 ]
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "click",
     "numpy",
     "requests",
     "shapely",
     "tqdm",
 ]
```

### Comparing `plateauutils-0.0.2/PKG-INFO` & `plateauutils-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateauutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of utilities for the Plateau project
 Project-URL: Homepage, https://eukarya-inc.github.io/plateauutils/
 Project-URL: Bug Reports, https://github.com/eukarya-inc/plateauutils/issues
 Project-URL: Source, https://github.com/eukarya-inc/plateauutils
 Author: Eukarya Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -234,15 +234,15 @@
     '533945471'
     >>> from shapely import from_wkt
     >>> from plateauutils.parser.city_gml_parser import CityGMLParser
     >>> target_polygon = from_wkt("POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))")
     >>> parser = CityGMLParser(target_polygon)
     >>> result = parser.download_and_parse("https://assets.cms.plateau.reearth.io/assets/d6/70821e-7f58-4f69-bc34-341875704e78/40203_kurume-shi_2020_citygml_3_op.zip", "/tmp")
     >>> result
-    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '610'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '610'},...]
+    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '非木造'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '非木造'},...]
 
 How to develop
 --------------
 
 .. code:: bash
 
     python3.9 -m venv venv
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

