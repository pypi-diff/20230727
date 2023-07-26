# Comparing `tmp/tipg-0.2.0.tar.gz` & `tmp/tipg-0.3.0.tar.gz`

## Comparing `tipg-0.2.0.tar` & `tipg-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/__init__.py
--rw-r--r--   0        0        0    32494 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/collections.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/database.py
--rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/errors.py
--rw-r--r--   0        0        0    73270 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/logger.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/main.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/middleware.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/model.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/enums.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/resources/response.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/collection.html
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/collections.html
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/header.html
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/item.html
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/items.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/landing.html
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/map.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tileset.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.2.0/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.2.0/LICENSE
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.2.0/README.md
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 tipg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 tipg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/__init__.py
+-rw-r--r--   0        0        0    32496 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/collections.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/database.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/errors.py
+-rw-r--r--   0        0        0    73592 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/logger.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/main.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/middleware.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/model.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/enums.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/response.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/collections.html
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/header.html
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/item.html
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/items.html
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/landing.html
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/map.html
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.3.0/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tipg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 tipg-0.3.0/PKG-INFO
```

### Comparing `tipg-0.2.0/tipg/collections.py` & `tipg-0.3.0/tipg/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,15 +976,15 @@
                 table=table["name"],
                 schema=table["schema"],
                 description=table.get("description", None),
                 id_column=id_column,
                 properties=properties,
                 datetime_column=datetime_column,
                 geometry_column=geometry_column,
-                parameters=table.get("parameters", []),
+                parameters=table.get("parameters") or [],
             )
 
         return Catalog(collections=catalog, last_updated=datetime.datetime.now())
 
 
 async def register_collection_catalog(app: FastAPI, **kwargs: Any) -> None:
     """Register Table catalog."""
```

### Comparing `tipg-0.2.0/tipg/database.py` & `tipg-0.3.0/tipg/database.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/dependencies.py` & `tipg-0.3.0/tipg/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,23 @@
         return collection_catalog["collections"][collectionId]
 
     raise HTTPException(
         status_code=404, detail=f"Table/Function '{collectionId}' not found."
     )
 
 
+def CatalogParams(request: Request) -> Catalog:
+    """Return Collections Catalog."""
+    collection_catalog: Catalog = getattr(request.app.state, "collection_catalog", None)
+    if not collection_catalog:
+        raise MissingCollectionCatalog("Could not find collections catalog.")
+
+    return collection_catalog
+
+
 def accept_media_type(
     accept: str, mediatypes: List[enums.MediaType]
 ) -> Optional[enums.MediaType]:
     """Return MediaType based on accept header and available mediatype.
 
     Links:
     - https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html
```

### Comparing `tipg-0.2.0/tipg/errors.py` & `tipg-0.3.0/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/factory.py` & `tipg-0.3.0/tipg/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,33 +25,29 @@
 from morecantile import tms as default_tms
 from morecantile.defaults import TileMatrixSets
 from pygeofilter.ast import AstType
 
 from tipg import model
 from tipg.collections import Catalog, Collection
 from tipg.dependencies import (
+    CatalogParams,
     CollectionParams,
     ItemsOutputType,
     OutputType,
     TileParams,
     bbox_query,
     datetime_query,
     filter_query,
     function_parameters_query,
     ids_query,
     properties_filter_query,
     properties_query,
     sortby_query,
 )
-from tipg.errors import (
-    MissingCollectionCatalog,
-    MissingGeometryColumn,
-    NoPrimaryKey,
-    NotFound,
-)
+from tipg.errors import MissingGeometryColumn, NoPrimaryKey, NotFound
 from tipg.resources.enums import MediaType
 from tipg.resources.response import GeoJSONResponse, SchemaJSONResponse
 from tipg.settings import FeaturesSettings, MVTSettings, TMSSettings
 
 from fastapi import APIRouter, Depends, Path, Query
 from fastapi.responses import ORJSONResponse
 
@@ -189,14 +185,15 @@
 class EndpointsFactory(metaclass=abc.ABCMeta):
     """Endpoints Factory."""
 
     # FastAPI router
     router: APIRouter = field(default_factory=APIRouter)
 
     # collection dependency
+    catalog_dependency: Callable[..., Catalog] = CatalogParams
     collection_dependency: Callable[..., Collection] = CollectionParams
 
     # Router Prefix is needed to find the path for routes when prefixed
     # e.g if you mount the route with `/foo` prefix, set router_prefix to foo
     router_prefix: str = ""
 
     templates: Jinja2Templates = DEFAULT_TEMPLATES
@@ -435,18 +432,22 @@
                     "content": {
                         MediaType.json.value: {},
                         MediaType.html.value: {},
                     }
                 },
             },
         )
-        def collections(
+        def collections(  # noqa: C901
             request: Request,
             bbox_filter: Annotated[Optional[List[float]], Depends(bbox_query)],
             datetime_filter: Annotated[Optional[List[str]], Depends(datetime_query)],
+            type_filter: Annotated[
+                Optional[Literal["Function", "Table"]],
+                Query(alias="type", description="Filter based on Collection type."),
+            ] = None,
             limit: Annotated[
                 Optional[int],
                 Query(
                     ge=0,
                     le=1000,
                     description="Limits the number of collection in the response.",
                 ),
@@ -455,27 +456,30 @@
                 Optional[int],
                 Query(
                     ge=0,
                     description="Starts the response at an offset.",
                 ),
             ] = None,
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
+            collection_catalog=Depends(self.catalog_dependency),
         ):
             """List of collections."""
-            collection_catalog: Catalog = getattr(
-                request.app.state, "collection_catalog", None
-            )
-            if not collection_catalog:
-                raise MissingCollectionCatalog("Could not find collections catalog.")
-
             collections_list = list(collection_catalog["collections"].values())
 
             limit = limit or 0
             offset = offset or 0
 
+            # type filter
+            if type_filter is not None:
+                collections_list = [
+                    collection
+                    for collection in collections_list
+                    if collection.type == type_filter
+                ]
+
             # bbox filter
             if bbox_filter is not None:
                 collections_list = [
                     collection
                     for collection in collections_list
                     if collection.bounds is not None
                     and s_intersects(bbox_filter, collection.bounds)
```

### Comparing `tipg-0.2.0/tipg/main.py` & `tipg-0.3.0/tipg/main.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/middleware.py` & `tipg-0.3.0/tipg/middleware.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/model.py` & `tipg-0.3.0/tipg/model.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/settings.py` & `tipg-0.3.0/tipg/settings.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/filter/evaluate.py` & `tipg-0.3.0/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/filter/filters.py` & `tipg-0.3.0/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/resources/enums.py` & `tipg-0.3.0/tipg/resources/enums.py`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/sql/dbcatalog.sql` & `tipg-0.3.0/tipg/sql/dbcatalog.sql`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             ELSE
                 EXECUTE format('SELECT ST_SetSRID(ST_Extent(%I), %L) FROM %s', attname, srid, att.attrelid::regclass::text) INTO bounds_geom;
             END IF;
         END IF;
 
         IF bounds_geom IS NOT NULL THEN
             IF srid != 4326 THEN
-                bounds_geom := st_transform(bounds_geom, srid);
+                bounds_geom := st_transform(bounds_geom, 4326);
             END IF;
             bounds = ARRAY[ st_xmin(bounds_geom), st_ymin(bounds_geom), st_xmax(bounds_geom), st_ymax(bounds_geom) ];
         END IF;
     END IF;
 
     RETURN jsonb_strip_nulls(jsonb_build_object(
         'name', attname,
```

### Comparing `tipg-0.2.0/tipg/templates/collection.html` & `tipg-0.3.0/tipg/templates/collection.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/collections.html` & `tipg-0.3.0/tipg/templates/collections.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/conformance.html` & `tipg-0.3.0/tipg/templates/conformance.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/header.html` & `tipg-0.3.0/tipg/templates/header.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/items.html` & `tipg-0.3.0/tipg/templates/items.html`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 {% endfor %}
   </tbody>
 </table>
 {% endif %}
 </div>
 
 <script>
+  var currentURL = "{{ template.api_root }}/collections/{{ response.id }}/items"
 function changePageSize() {
   var url = "{{ template.api_root }}/collections/{{ response.id }}/items?";
   url += "limit=" + $("#limit").val();
   window.location.href = url;
 }
 $(function() {
 
@@ -91,15 +92,27 @@
   var map = L.map('map').setView([0, 0], 1);
   map.addLayer(new L.TileLayer(
     'https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
       maxZoom: 18,
       attribution: 'Map data &copy; <a href="https://openstreetmap.org/copyright">OpenStreetMap contributors</a>'
     }
   ));
-  var features = L.geoJSON(geojson).addTo(map);
+
+  function addPopup(feature, layer) {
+    var aElm = document.createElement('a');
+    aElm.setAttribute('href', `${currentURL}/${feature.id}`);
+    aElm.setAttribute('target', '_blank');
+    aElm.innerText = feature.id;
+    layer.bindPopup(aElm);
+  }
+
+  var features = L.geoJSON(geojson, {
+    onEachFeature: addPopup
+  }).addTo(map);
+
   map.fitBounds(features.getBounds());
 
   //
   // paging
   //
   var offset = 0; // defaults
   var limit = 10;
```

### Comparing `tipg-0.2.0/tipg/templates/landing.html` & `tipg-0.3.0/tipg/templates/landing.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/map.html` & `tipg-0.3.0/tipg/templates/map.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/queryables.html` & `tipg-0.3.0/tipg/templates/queryables.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/tilematrixset.html` & `tipg-0.3.0/tipg/templates/tilematrixset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/tilematrixsets.html` & `tipg-0.3.0/tipg/templates/tilematrixsets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/tileset.html` & `tipg-0.3.0/tipg/templates/tileset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/tipg/templates/tilesets.html` & `tipg-0.3.0/tipg/templates/tilesets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/.gitignore` & `tipg-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/LICENSE` & `tipg-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/README.md` & `tipg-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.2.0/pyproject.toml` & `tipg-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 dependencies = [
     "orjson",
     "asyncpg>=0.23.0",
     "buildpg>=0.3",
     "fastapi>=0.95.1",
     "jinja2>=2.11.2,<4.0.0",
     "morecantile>=4.2,<5.0",
-    "geojson-pydantic>=0.4.3",
+    "pydantic[dotenv]~=1.0",
+    "geojson-pydantic>=0.4.3,<1.0",
     "pygeofilter>=0.2.0,<0.3.0",
     "ciso8601~=2.3",
     "starlette-cramjam>=0.3,<0.4",
     "importlib_resources>=1.1.0; python_version < '3.9'",
     "typing_extensions; python_version < '3.9'",
 ]
```

### Comparing `tipg-0.2.0/PKG-INFO` & `tipg-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipg
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
         
@@ -38,19 +38,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: asyncpg>=0.23.0
 Requires-Dist: buildpg>=0.3
 Requires-Dist: ciso8601~=2.3
 Requires-Dist: fastapi>=0.95.1
-Requires-Dist: geojson-pydantic>=0.4.3
+Requires-Dist: geojson-pydantic<1.0,>=0.4.3
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
 Requires-Dist: jinja2<4.0.0,>=2.11.2
 Requires-Dist: morecantile<5.0,>=4.2
 Requires-Dist: orjson
+Requires-Dist: pydantic[dotenv]~=1.0
 Requires-Dist: pygeofilter<0.3.0,>=0.2.0
 Requires-Dist: starlette-cramjam<0.4,>=0.3
 Requires-Dist: typing-extensions; python_version < '3.9'
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tipg Version: 0.2.0 Summary: Simple and Fast
+Metadata-Version: 2.1 Name: tipg Version: 0.3.0 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -23,31 +23,31 @@
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS Requires-
 Python: >=3.8 Requires-Dist: asyncpg>=0.23.0 Requires-Dist: buildpg>=0.3
 Requires-Dist: ciso8601~=2.3 Requires-Dist: fastapi>=0.95.1 Requires-Dist:
-geojson-pydantic>=0.4.3 Requires-Dist: importlib-resources>=1.1.0;
+geojson-pydantic<1.0,>=0.4.3 Requires-Dist: importlib-resources>=1.1.0;
 python_version < '3.9' Requires-Dist: jinja2<4.0.0,>=2.11.2 Requires-Dist:
-morecantile<5.0,>=4.2 Requires-Dist: orjson Requires-Dist:
-pygeofilter<0.3.0,>=0.2.0 Requires-Dist: starlette-cramjam<0.4,>=0.3 Requires-
-Dist: typing-extensions; python_version < '3.9' Provides-Extra: dev Requires-
-Dist: pre-commit; extra == 'dev' Provides-Extra: docs Requires-Dist: mkdocs;
-extra == 'docs' Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist:
-pdocs; extra == 'docs' Requires-Dist: pygments; extra == 'docs' Provides-Extra:
-server Requires-Dist: uvicorn[standard]<0.19.0,>=0.12.0; extra == 'server'
-Provides-Extra: test Requires-Dist: httpx; extra == 'test' Requires-Dist:
-mapbox-vector-tile; extra == 'test' Requires-Dist: numpy; extra == 'test'
-Requires-Dist: protobuf<4.0,>=3.0; extra == 'test' Requires-Dist: psycopg2;
-extra == 'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-
-asyncio; extra == 'test' Requires-Dist: pytest-benchmark; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test' Requires-Dist: pytest-pgsql; extra
-== 'test' Requires-Dist: sqlalchemy<1.4,>=1.1; extra == 'test' Description-
-Content-Type: text/markdown
+morecantile<5.0,>=4.2 Requires-Dist: orjson Requires-Dist: pydantic
+[dotenv]~=1.0 Requires-Dist: pygeofilter<0.3.0,>=0.2.0 Requires-Dist:
+starlette-cramjam<0.4,>=0.3 Requires-Dist: typing-extensions; python_version <
+'3.9' Provides-Extra: dev Requires-Dist: pre-commit; extra == 'dev' Provides-
+Extra: docs Requires-Dist: mkdocs; extra == 'docs' Requires-Dist: mkdocs-
+material; extra == 'docs' Requires-Dist: pdocs; extra == 'docs' Requires-Dist:
+pygments; extra == 'docs' Provides-Extra: server Requires-Dist: uvicorn
+[standard]<0.19.0,>=0.12.0; extra == 'server' Provides-Extra: test Requires-
+Dist: httpx; extra == 'test' Requires-Dist: mapbox-vector-tile; extra == 'test'
+Requires-Dist: numpy; extra == 'test' Requires-Dist: protobuf<4.0,>=3.0; extra
+== 'test' Requires-Dist: psycopg2; extra == 'test' Requires-Dist: pytest; extra
+== 'test' Requires-Dist: pytest-asyncio; extra == 'test' Requires-Dist: pytest-
+benchmark; extra == 'test' Requires-Dist: pytest-cov; extra == 'test' Requires-
+Dist: pytest-pgsql; extra == 'test' Requires-Dist: sqlalchemy<1.4,>=1.1; extra
+== 'test' Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/10407788/204477834-2533241a-5927-
                           4f56-959e-4e8494027bc0.png]
       Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
                  [Test] [Coverage] [Package_version] [License]
 --- **Documentation**: https://developmentseed.org/tipg/ **Source Code**:
 https://github.com/developmentseed/tipg --- `tipg`, pronounced *T[ee]pg*, is a
 **python** package which helps creating lightweight OGC **Features** and
```

