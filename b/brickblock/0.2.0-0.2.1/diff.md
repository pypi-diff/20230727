# Comparing `tmp/brickblock-0.2.0.tar.gz` & `tmp/brickblock-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickblock-0.2.0.tar", max compression
+gzip compressed data, was "brickblock-0.2.1.tar", max compression
```

## Comparing `brickblock-0.2.0.tar` & `brickblock-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35823 2023-07-15 07:40:33.964780 brickblock-0.2.0/LICENSE
--rw-r--r--   0        0        0     1470 2023-07-24 19:18:19.551792 brickblock-0.2.0/README.md
--rw-r--r--   0        0        0       31 2023-07-15 12:28:30.690454 brickblock-0.2.0/brickblock/__init__.py
--rw-r--r--   0        0        0    22917 2023-07-21 09:08:13.965513 brickblock-0.2.0/brickblock/objects.py
--rw-r--r--   0        0        0    19290 2023-07-24 18:54:24.796383 brickblock-0.2.0/brickblock/space.py
--rw-r--r--   0        0        0      535 2023-07-24 19:12:15.039393 brickblock-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 brickblock-0.2.0/setup.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 brickblock-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-15 07:40:33.964780 brickblock-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1470 2023-07-24 19:18:19.551792 brickblock-0.2.1/README.md
+-rw-r--r--   0        0        0       31 2023-07-15 12:28:30.690454 brickblock-0.2.1/brickblock/__init__.py
+-rw-r--r--   0        0        0    23303 2023-07-26 23:33:41.959270 brickblock-0.2.1/brickblock/objects.py
+-rw-r--r--   0        0        0    26636 2023-07-27 19:03:22.294981 brickblock-0.2.1/brickblock/space.py
+-rw-r--r--   0        0        0      535 2023-07-27 19:17:18.470614 brickblock-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 brickblock-0.2.1/setup.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 brickblock-0.2.1/PKG-INFO
```

### Comparing `brickblock-0.2.0/LICENSE` & `brickblock-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brickblock-0.2.0/README.md` & `brickblock-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `brickblock-0.2.0/brickblock/objects.py` & `brickblock-0.2.1/brickblock/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -410,37 +410,41 @@
         facecolor: The color for each of the faces in every cube. The default is
             None, i.e. transparent cubes. If this is set, then by default alpha
             will be 1.
         linewidth: The width for each of the lines in every cube.
         edgecolor: The color for each of the lines in every cube.
         alpha: The transparency for each of the faces in every cube. The default
             is 0, i.e. transparent cubes.
+        style: The visual style of the entire object. Other field values will
+            take precedence over this style should they conflict.
         name: A name for this entire object, used for querying within a Space.
     """
 
     h: int
     w: int
     d: int
     faces: np.ndarray
     facecolor: tuple[float, float, float] | None = None
     linewidth: float = 0.1
     edgecolor: str = "black"
     alpha: float = 0.0
+    style: str = "default"
     name: str | None = None
 
     def __init__(
         self,
         base_vector: np.ndarray,
         w: int,
         h: int,
         d: int,
         facecolor: tuple[float, float, float] | None = None,
         linewidth: float = 0.1,
         edgecolor: str = "black",
         alpha: float | None = None,
+        style: str = "default",
         name: str | None = None,
     ) -> None:
         # Users will not expect setting the facecolor only to have the object be
         # invisible by default, so if the facecolor is set but not the alpha,
         # have the object be fully opaque.
         if alpha is None and facecolor is not None:
             alpha = 1.0
@@ -459,14 +463,18 @@
             )
 
         if w <= 0 or h <= 0 or d <= 0:
             raise ValueError(
                 "Composite object must have positively-sized dimensions."
             )
 
+        style = style.lower()
+        if style not in ["default", "classic"]:
+            raise ValueError("Composite object was given an invalid style.")
+
         # Explain this in docs - but essentially this is for navigating around
         # limitation in matplotlib where the Z axis is the vertical one. You
         # cannot just use the camera to fix the problem (I think). Or at least,
         # not with 3D objects and the notion of left/right etc. You need to
         # transpose or flip the actual data (or the axes), and this is the
         # simplest way to achieve this. Of course, the flip-side is that now you
         # are saying the z-axis corresponds to height in Brickblock, which is
@@ -496,14 +504,15 @@
         self.h = h
         self.d = d
         self.faces = self._construct_faces(full_points)
         self.facecolor = facecolor
         self.linewidth = linewidth
         self.edgecolor = edgecolor
         self.alpha = alpha
+        self.style = style
         self.name = name
 
     def points(self) -> np.ndarray:
         """
         Get the set of unique points that define this object.
         """
         # TODO: Figure out the relevant points that define the bounds of the
```

### Comparing `brickblock-0.2.0/brickblock/space.py` & `brickblock-0.2.1/brickblock/space.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,14 +36,44 @@
 
 @dataclass
 class Deletion(SpaceStateChange):
     timestep_id: int
     name: str | None
 
 
+"""
+Doc of how the index works
+
+The index is a hierarchial index comprised of dictionaries. At the top-level, we
+have scenes as the keys. Each scene points to its timesteps. Each timestep
+points to an entry representing each of the objects inserted at that timestep.
+
+This entry is currently a list of pids. While this is simple, it has issues:
+
+* Even a moderately-sized composite is comprised of many primitives, so these
+lists can become very large.
+* If multiple objects with unique pids get added in a single timestep, there is
+no distinction between this case and having a single composite object.
+
+One solution is to store ranges for composites. This works because their
+primitives are contiguous in memory anyway. A major advantage is memory usage.
+Another advantage is that if the entry is a list of ints and ranges, we can now
+assume each item in that list is its own object, and so the length of the list
+is equal to the number of objects. The number of primitives could also
+potentially be calculated and stored on creating an entry.
+
+The issue with storing ranges is how that would be done currently. Since
+_add_cuboid_primitive does not distinguish between individual cubes or cubes
+that are part of composites, the index entry needs to add a single primitive ID
+to the list. This either means that you reduce the list at the end of creating
+the composite to a range, that you move that logic out of _add_cuboid_primitive,
+or that you implement composite addition properly.
+"""
+
+
 class Space:
     """
     Representation of a 3D coordinate space, which tracks its state over time.
 
     Any added objects are stored in a variety of formats, such as by coordinate
     data, by name, and various IDs. This facilitates multiple ways of querying
     them within a space.
@@ -109,24 +139,26 @@
         Add a Cube primitive to the space.
         """
         primitive_id = self._add_cuboid_primitive(cube)
         self._add_name(cube.name, [primitive_id])
         self.num_objs += 1
         self.changelog.append(Addition(self.time_step, None))
         self.time_step += 1
+        self._update_bounds([primitive_id])
 
     def add_cuboid(self, cuboid: Cuboid) -> None:
         """
         Add a Cuboid primitive to the space.
         """
         primitive_id = self._add_cuboid_primitive(cuboid)
         self._add_name(cuboid.name, [primitive_id])
         self.num_objs += 1
         self.changelog.append(Addition(self.time_step, None))
         self.time_step += 1
+        self._update_bounds([primitive_id])
 
     # TODO: Rather than adding individual cubes, this should be a single call
     # and leverage the provided data better by direct insertion.
     def add_composite(self, composite: CompositeCube) -> None:
         """
         Add a CompositeCube object to the space.
         """
@@ -146,83 +178,108 @@
                 facecolor=composite.facecolor,
                 linewidth=composite.linewidth,
                 edgecolor=composite.edgecolor,
                 alpha=composite.alpha,
             )
             primitive_ids.append(self._add_cuboid_primitive(cube))
 
+        if composite.style == "classic":
+            cube_base_point_idx = (0, 0, 0)
+            # Swap the axes around here - otherwise you will get double-swapping
+            # of the dimensions.
+            base_vector = composite.faces[cube_base_point_idx]
+            w, d, h = base_vector
+            cuboid = Cuboid(
+                np.array([w, h, d]),
+                w=composite.w,
+                h=composite.h,
+                d=composite.d,
+                facecolor=None,
+                linewidth=1.0,
+                edgecolor="black",
+                alpha=0.0,
+            )
+            primitive_ids.append(self._add_cuboid_primitive(cuboid))
+
         self._add_name(composite.name, primitive_ids)
 
         self.changelog.append(Addition(self.time_step, None))
         self.num_objs += 1
         self.time_step += 1
+        self._update_bounds(primitive_ids)
 
     def _add_cuboid_primitive(self, cuboid: Cube | Cuboid) -> int:
         """
         Add a primitive to the space by updating the various indices and data
         structures, and return its ID.
 
         # Args
             cuboid: Primitive Cube/Cuboid to add to the space's various data
             structures.
         """
         cuboid_bounding_box = cuboid.get_bounding_box()
         cuboid_mean = np.mean(cuboid.points(), axis=0).reshape((3, 1))
 
+        # Update the bounding box - via total, mean, and dims.
         self.total += cuboid_mean
 
         self.mean = self.total / (self.primitive_counter + 1)
 
         if self.primitive_counter == 0:
             dim = cuboid_bounding_box
         else:
             # Since there are multiple objects, ensure the resulting dimensions
-            # of the surrounding box are centred around the mean.
+            # of the surrounding box are the extrema of the objects within.
             dim = np.array(
                 [
                     [
                         min(self.dims[i][0], cuboid_bounding_box[i][0]),
                         max(self.dims[i][1], cuboid_bounding_box[i][1]),
                     ]
                     for i in range(len(cuboid_bounding_box))
                 ]
             ).reshape((3, 2))
 
         self.dims = dim
 
+        # Update the coordinate data, resizing if necessary.
         current_no_of_entries = self.cuboid_coordinates.shape[0]
         if self.primitive_counter >= current_no_of_entries:
             # refcheck set to False since this avoids issues with the debugger
             # referencing the array!
             self.cuboid_coordinates.resize(
                 (2 * current_no_of_entries, *self.cuboid_coordinates.shape[1:]),
                 refcheck=False,
             )
 
         self.cuboid_coordinates[self.primitive_counter] = cuboid.faces
+
+        # Update the visual metadata store.
         for key, value in cuboid.get_visual_metadata().items():
             if key in self.cuboid_visual_metadata.keys():
                 self.cuboid_visual_metadata[key].append(value)
             else:
                 self.cuboid_visual_metadata[key] = [value]
 
+        # Update the index, adding entries if necessary.
         def add_key_to_nested_dict(d, keys):
             for key in keys[:-1]:
                 if key not in d:
                     d[key] = {}
                 d = d[key]
             if keys[-1] not in d:
                 d[keys[-1]] = []
 
         keys = [self.scene_counter, self.time_step]
         add_key_to_nested_dict(self.cuboid_index, keys)
         self.cuboid_index[self.scene_counter][self.time_step].append(
             self.primitive_counter
         )
 
+        # Update the primitive_counter.
         primitive_id = self.primitive_counter
         self.primitive_counter += 1
 
         return primitive_id
 
     def _add_name(self, name: str | None, primitive_ids: list[int]) -> None:
         """
@@ -236,23 +293,48 @@
         if name is not None:
             if name in self.cuboid_names.keys():
                 raise Exception(
                     f"There already exists an object with name {name}."
                 )
             self.cuboid_names[name] = primitive_ids
 
+    def _update_bounds(self, primitive_ids: list[int]) -> None:
+        """
+        Update the bounding box of the space, based on the primitives given by
+        `primitive_ids`.
+
+        Whether one or more primitives are given, the space will update its
+        bounds over the extrema in both cases.
+
+        The bounds of the space are updated regardless of whether or not the
+        provided primitives are visible.
+
+        # Args
+            primitive_ids: The primitives for which coordinate data is used to
+                update the bounding box of this space.
+        """
+        N = len(primitive_ids)
+        primitives = self.cuboid_coordinates[primitive_ids].reshape(
+            (N * 6 * 4, 3)
+        )
+        given_mins = np.min(primitives, axis=0)
+        given_maxes = np.max(primitives, axis=0)
+
+        self.dims[:, 0] = np.minimum(self.dims[:, 0], given_mins.T)
+        self.dims[:, 1] = np.maximum(self.dims[:, 1], given_maxes.T)
+
     # TODO: Decide how deletion should be implemented. Masking columns seem the
     # most logical, but this could be an issue for memory consumption. On the
     # other hand, 'actual deletion' would involve potentially expensive memory
     # shuffling.
     # Moreover, should you even be worrying about deletion? Masking is what you
     # really want in virtually all cases. Deletion should actually be quite rare
     # unless a user does something dumb or adds crazy numbers of objects.
 
-    def mutate_by_coordinate(self, coordinate: np.array, **kwargs) -> None:
+    def mutate_by_coordinate(self, coordinate: np.ndarray, **kwargs) -> None:
         """
         Mutate the visual metadata of all objects - composite or primitive, with
         base vectors equal to `coordinate` - with the named arguments in
         `kwargs`.
 
         Primitives that are part of composites are not included - that is, if
         `coordinate` intersects with a composite on any point other than its
@@ -263,52 +345,15 @@
 
         # Args
             coordinate: The coordinate which is compared to the base vector of
                 all objects in the space.
             kwargs: Sequence of named arguments that contain updated visual
                 property values.
         """
-        if coordinate.shape != (3,):
-            raise ValueError(
-                "Coordinates are three-dimensional, the input vector should be "
-                "3D."
-            )
-
-        # Map the coordinate to the correct representation.
-        # TODO: Decouple the user from a fixed basis.
-        w, h, d = coordinate
-        coordinate = np.array([w, d, h])
-
-        # First gather the IDs of primitive entries that match the coordinate.
-        matching_base_vectors = []
-        primitives_to_update = []
-        current_idx = 0
-
-        for idx in range(self.primitive_counter):
-            primitive = self.cuboid_coordinates[idx]
-            if np.array_equal(primitive[0, 0], coordinate):
-                matching_base_vectors.append(idx)
-
-        # Find all objects (primitive or composite) corresponding to those IDs.
-        for scene_id in sorted(self.cuboid_index.keys()):
-            for timestep_id in sorted(self.cuboid_index[scene_id].keys()):
-                primitive_ids = self.cuboid_index[scene_id][timestep_id]
-                # Because we gathered matching_base_vectors in order, and the
-                # bottom-left-front point of all objects is the first point, we
-                # can check just the first primitive_id of the list for both
-                # primitives and composites.
-
-                # Skip forward if you caught intermediate primitives.
-                while matching_base_vectors[current_idx] < primitive_ids[0]:
-                    current_idx += 1
-
-                if primitive_ids[0] == matching_base_vectors[current_idx]:
-                    primitives_to_update.extend(primitive_ids)
-                    current_idx += 1
-
+        primitives_to_update = self._select_by_coordinate(coordinate)
         self._mutate_by_primitive_ids(primitives_to_update, **kwargs)
 
     def mutate_by_name(self, name: str, **kwargs) -> None:
         """
         Mutate the visual metadata of the object - composite or primitive, that
         has its name equal to `name` - with the named arguments in `kwargs`.
 
@@ -384,14 +429,122 @@
             if key not in self.cuboid_visual_metadata.keys():
                 raise KeyError(
                     "The provided key doesn't match any valid visual property."
                 )
             for primitive_id in primitive_ids:
                 self.cuboid_visual_metadata[key][primitive_id] = kwargs[key]
 
+    def create_by_offset(
+        self,
+        offset: np.ndarray,
+        coordinate: np.ndarray | None = None,
+        name: str | None = None,
+        timestep: int | None = None,
+        scene: int | None = None,
+        **kwargs,
+    ) -> None:
+        """
+        Create a duplicate of an object (or objects) selected by any one of
+        `coordinate`, `name`, `timestep`, or `scene`, shifted by `offset`.
+
+        The offset is done with respect to the base vectors of the objects.
+
+        Exactly one of `coordinate`, `name`, `timestep`, or `scene` must be set.
+        The selection can refer to multiple objects - in this case, a duplicate
+        is made for each object in the selection.
+
+        Note that all objects created will be treated as having been created at
+        the same timestep.
+
+        The remaining args are used to override the inherited visual properties
+        of the created objects. These will apply to all created objects - if a
+        single value is given, then this is broadcast to all objects. Otherwise
+        a list with the same number of created objects is given and will be
+        applied in order of insertion.
+
+        # Args
+            offset: Offset by base vector, in XYZ coordinate form.
+            coordinate: Optional selection, where all objects with equal base
+                vectors will be selected.
+            name: Optional selection, where the object with that name will be
+                selected.
+            timestep: Optional selection, where all objects created in that
+                timestep will be selected.
+            scene: Optional selection, where all objects created in that scene
+                will be selected.
+            kwargs: Optional visual property arguments - can be a dict with
+                scalar or list of values.
+        """
+        exactly_one_set = (
+            sum([a is not None for a in [coordinate, name, timestep, scene]])
+            == 1
+        )
+        if not exactly_one_set:
+            raise ValueError(
+                "Exactly one selection argument can be set when creating "
+                "objects."
+            )
+
+        if coordinate is not None:
+            primitive_ids = self._select_by_coordinate(coordinate)
+        if name is not None:
+            primitive_ids = self._select_by_name(name)
+        if timestep is not None:
+            primitive_ids = self._select_by_timestep(timestep)
+        if scene is not None:
+            primitive_ids = self._select_by_scene(scene)
+
+        # TODO: You ideally want an index of which primitives correspond to
+        # composites, if any.
+        print(primitive_ids)
+
+    def _select_by_coordinate(self, coordinate: np.ndarray) -> list[int]:
+        if coordinate.shape != (3,):
+            raise ValueError(
+                "Coordinates are three-dimensional, the input vector should be "
+                "3D."
+            )
+
+        # Map the coordinate to the correct representation.
+        # TODO: Decouple the user from a fixed basis.
+        w, h, d = coordinate
+        coordinate = np.array([w, d, h])
+
+        # First gather the IDs of primitive entries that match the coordinate.
+        matching_base_vectors = []
+        primitives_to_update = []
+        objects_to_update = []
+        current_idx = 0
+
+        for idx in range(self.primitive_counter):
+            primitive = self.cuboid_coordinates[idx]
+            if np.array_equal(primitive[0, 0], coordinate):
+                matching_base_vectors.append(idx)
+
+        # Find all objects (primitive or composite) corresponding to those IDs.
+        for scene_id in sorted(self.cuboid_index.keys()):
+            for timestep_id in sorted(self.cuboid_index[scene_id].keys()):
+                primitive_ids = self.cuboid_index[scene_id][timestep_id]
+                # Because we gathered matching_base_vectors in order, and the
+                # bottom-left-front point of all objects is the first point, we
+                # can check just the first primitive_id of the list for both
+                # primitives and composites.
+
+                # Skip forward if you caught intermediate primitives.
+                while matching_base_vectors[current_idx] < primitive_ids[0]:
+                    current_idx += 1
+
+                if primitive_ids[0] == matching_base_vectors[current_idx]:
+                    if len(primitive_ids) > 1:
+                        objects_to_update.append()
+                    primitives_to_update.extend(primitive_ids)
+                    current_idx += 1
+
+        return primitives_to_update
+
     def snapshot(self) -> None:
         """
         Store the current state of the space as a scene, used for rendering.
 
         Note that valid scenes must have 1+ transforms - i.e. adding,
         deleting, or mutating an object, must be present in a scene.
         """
@@ -410,17 +563,17 @@
     # the last one (though it shows the last one first). Can this be fixed?
     # (Yes - you are being an idiot).
     def render(self) -> tuple[plt.Figure, plt.Axes]:
         """
         Render every scene in the space with a matplotlib Axes, and return the
         figure-axes pair.
         """
-        fig = plt.figure(figsize=(10, 8))
+        fig = plt.figure(figsize=(10, 7))
         fig.subplots_adjust(
-            left=0, bottom=0, right=1, top=1, wspace=None, hspace=None
+            left=0, bottom=0, right=1, top=1, wspace=0.0, hspace=0.0
         )
         ax = fig.add_subplot(111, projection="3d")
         # Remove everything except the objects to display.
         ax.set_axis_off()
 
         # TODO: This logic really belongs in a `stream()` function. The render
         # method should just get all primitive_ids and then render everything
@@ -432,14 +585,29 @@
                 primitive_ids = self.cuboid_index[scene_id][timestep_id]
 
                 if len(primitive_ids) == 1:
                     ax = self._populate_ax_with_primitive(ax, primitive_ids[0])
                 else:
                     ax = self._populate_ax_with_composite(ax, primitive_ids)
 
+        # Use the space's bounds to update the camera and view.
+        # This is very janky but at least ensures everything is in view.
+        # One way this could be fixed would be to reorient everything so that
+        # aiming at the origin actually works. Essentially you take the
+        # difference between the center of the bounding box of the space, and
+        # the origin, and shift everything by the negative difference.
+        # The problem with this solution is a) it involves a transform over
+        # everything and b) would mean the user cannot turn on the axes to debug
+        # things as effectively. Potentially this could be explained in some
+        # docs though.
+        max_val = max(list(self.dims.flatten()))
+        ax.set_xlim(-max_val, max_val)
+        ax.set_ylim(-max_val, max_val)
+        ax.set_zlim(-max_val, max_val)
+
         return fig, ax
 
     def _populate_ax_with_primitive(
         self,
         ax: plt.Axes,
         primitive_id: int,
     ) -> plt.Axes:
```

### Comparing `brickblock-0.2.0/pyproject.toml` & `brickblock-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brickblock"
-version = "0.2.0"
+version = "0.2.1"
 description = "A fun visualisation library for those that like boxes"
 authors = ["Daniel Soutar <danielsoutar144@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/danielsoutar/brickblock"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `brickblock-0.2.0/setup.py` & `brickblock-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.7.2,<4.0.0', 'numpy>=1.25.1,<2.0.0', 'pytest>=7.4.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'brickblock',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A fun visualisation library for those that like boxes',
     'long_description': "# Brickblock: A fun visualisation library for those that like boxes\n\nThis is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.\n\n## Core abstractions\n\nAt the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.\n\nThere are objects used for composing visualisations in Brickblock, such as the `Cube`. Objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths. They can also be mutated - and can be selected by name, base vector, or various IDs.\n\nHaving these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.\n\n## Contributing\n\nContributions are more than welcome! There is a very rough TODO in [todo.md](todo.md) that outlines both short- and long-term goals for the library. However, there are some rules:\n\n* Always follow the [code of conduct](CODE_OF_CONDUCT.md)\n* All the tests should be passing with your change\n* Explain your change (PR template coming soon)\n* Add relevant tests and docstrings\n* Format your changes with `black`\n",
     'author': 'Daniel Soutar',
     'author_email': 'danielsoutar144@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/danielsoutar/brickblock',
```

### Comparing `brickblock-0.2.0/PKG-INFO` & `brickblock-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brickblock
-Version: 0.2.0
+Version: 0.2.1
 Summary: A fun visualisation library for those that like boxes
 Home-page: https://github.com/danielsoutar/brickblock
 Author: Daniel Soutar
 Author-email: danielsoutar144@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

