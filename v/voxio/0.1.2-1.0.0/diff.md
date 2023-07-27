# Comparing `tmp/voxio-0.1.2.tar.gz` & `tmp/voxio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxio-0.1.2.tar", max compression
+gzip compressed data, was "voxio-1.0.0.tar", max compression
```

## Comparing `voxio-0.1.2.tar` & `voxio-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1658 2023-02-23 18:11:12.531986 voxio-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      893 2023-03-25 07:20:06.435288 voxio-0.1.2/README.md
--rw-r--r--   0        0        0     1335 2023-03-25 07:27:17.197523 voxio-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 18:02:41.603087 voxio-0.1.2/voxio/__init__.py
--rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-0.1.2/voxio/augment/__init__.py
--rw-r--r--   0        0        0     9043 2023-03-25 07:20:06.432288 voxio-0.1.2/voxio/augment/label_binary_image.py
--rw-r--r--   0        0        0      953 2023-03-25 07:20:06.426288 voxio-0.1.2/voxio/caching.py
--rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-0.1.2/voxio/clean/__init__.py
--rwxr-xr-x   0        0        0     1606 2023-03-25 07:20:06.436288 voxio-0.1.2/voxio/clean/single_big_obj_artifact_purge.py
--rw-r--r--   0        0        0     1600 2023-03-25 07:20:06.402289 voxio-0.1.2/voxio/cli/__init__.py
--rw-r--r--   0        0        0      144 2023-03-25 07:20:06.402289 voxio-0.1.2/voxio/cli/settings.py
--rw-r--r--   0        0        0      893 2023-03-25 07:20:06.396289 voxio-0.1.2/voxio/crop.py
--rw-r--r--   0        0        0     2270 2023-03-25 07:20:06.426288 voxio-0.1.2/voxio/read.py
--rw-r--r--   0        0        0        0 2023-03-19 15:27:51.685539 voxio-0.1.2/voxio/utils/__init__.py
--rw-r--r--   0        0        0     1597 2023-03-25 07:20:06.402289 voxio-0.1.2/voxio/utils/distance.py
--rw-r--r--   0        0        0     1448 2023-03-25 07:20:06.402289 voxio-0.1.2/voxio/utils/interpolate.py
--rw-r--r--   0        0        0     1327 2023-03-25 07:20:06.426288 voxio-0.1.2/voxio/utils/io.py
--rw-r--r--   0        0        0     1622 2023-03-25 07:20:06.426288 voxio-0.1.2/voxio/utils/misc.py
--rw-r--r--   0        0        0       29 2023-03-19 15:27:51.685539 voxio-0.1.2/voxio/utils/typings.py
--rw-r--r--   0        0        0      336 2023-03-25 07:20:06.417288 voxio-0.1.2/voxio/volume_info/__init__.py
--rw-r--r--   0        0        0     6097 2023-03-25 07:20:06.427288 voxio-0.1.2/voxio/volume_info/read.py
--rw-r--r--   0        0        0     7805 2023-03-25 07:20:06.427288 voxio-0.1.2/voxio/volume_info/volume_info.py
--rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 voxio-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1658 2023-03-25 07:28:26.601121 voxio-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0      893 2023-03-25 07:20:06.435288 voxio-1.0.0/README.md
+-rw-r--r--   0        0        0     1327 2023-07-27 04:49:24.462098 voxio-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 18:02:41.603087 voxio-1.0.0/voxio/__init__.py
+-rw-r--r--   0        0        0      953 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/caching.py
+-rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-1.0.0/voxio/clean/__init__.py
+-rwxr-xr-x   0        0        0     1596 2023-07-27 04:35:37.202047 voxio-1.0.0/voxio/clean/single_big_obj_artifact_purge.py
+-rw-r--r--   0        0        0     1592 2023-07-27 08:01:39.157450 voxio-1.0.0/voxio/cli/__init__.py
+-rw-r--r--   0        0        0      144 2023-03-25 07:20:06.402289 voxio-1.0.0/voxio/cli/settings.py
+-rw-r--r--   0        0        0      899 2023-07-27 04:47:18.387395 voxio-1.0.0/voxio/crop.py
+-rw-r--r--   0        0        0     2248 2023-07-27 04:40:04.303418 voxio-1.0.0/voxio/read.py
+-rw-r--r--   0        0        0        0 2023-03-19 15:27:51.685539 voxio-1.0.0/voxio/utils/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-27 04:47:18.397395 voxio-1.0.0/voxio/utils/distance.py
+-rw-r--r--   0        0        0     1466 2023-07-27 04:47:18.377395 voxio-1.0.0/voxio/utils/interpolate.py
+-rw-r--r--   0        0        0     1370 2023-07-27 04:47:41.670340 voxio-1.0.0/voxio/utils/io.py
+-rw-r--r--   0        0        0     1603 2023-07-27 04:51:53.495746 voxio-1.0.0/voxio/utils/misc.py
+-rw-r--r--   0        0        0       29 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/utils/typings.py
+-rw-r--r--   0        0        0      336 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/volume_info/__init__.py
+-rw-r--r--   0        0        0     6101 2023-07-27 04:47:18.414395 voxio-1.0.0/voxio/volume_info/read.py
+-rw-r--r--   0        0        0     7788 2023-07-27 04:51:53.615746 voxio-1.0.0/voxio/volume_info/volume_info.py
+-rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-1.0.0/voxio/workflows/__init__.py
+-rw-r--r--   0        0        0     9044 2023-07-27 04:53:54.110462 voxio-1.0.0/voxio/workflows/label_binary_image.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 voxio-1.0.0/PKG-INFO
```

### Comparing `voxio-0.1.2/LICENSE.md` & `voxio-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voxio-0.1.2/README.md` & `voxio-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `voxio-0.1.2/pyproject.toml` & `voxio-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "voxio"
-version = "0.1.2"
+version = "1.0.0"
 description = "Library for ingesting and processing voxel (3D imaging) data"
 authors = ["caniko <canhtart@gmail.com>"]
 license = "BSD-4"
 repository = "https://github.com/caniko/voxio"
 readme = "README.md"
 
-keywords = ["3D", "voxel", "processing", "fix", "mesh"]
+keywords = ["voxel", "processing", "fix", "mesh"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Multimedia :: Graphics :: 3D Modeling",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Visualization",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.scripts]
 voxio = "voxio.cli:voxio_cli"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-pydantic = "^1.10.6"
+python = ">=3.10,<3.11"
+pydantic = "^2.0"
 psutil = "^5.9.4"
 
 # Maintained by project author
-pydantic-numpy = ">=2.0"
+pydantic-numpy = ">=3.0"
 
-numpy = ">=1.17"
+numpy = ">=1.23"
 scipy = "*"
 scikit-image = "^0.20.0"
 itk-morphologicalcontourinterpolation = "^1.1.0"
 opencv-python = "^4.7.0.72"
 imagesize = "^1.4.1"
 click = "^8.1.3"
 numba = "^0.56.4"
```

### Comparing `voxio-0.1.2/voxio/augment/label_binary_image.py` & `voxio-1.0.0/voxio/workflows/label_binary_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 from functools import partial
 from pathlib import Path
 from typing import Generator, Iterable
 
 import compress_pickle
 import numpy as np
 from numpy import ScalarType
-from pydantic import BaseModel, DirectoryPath, Field, FilePath, validate_arguments
-from pydantic_numpy import NDArray
+from pydantic import BaseModel, DirectoryPath, Field, FilePath, validate_call
+from pydantic_numpy import NpNDArray
 from scipy import ndimage
 from yaspin import yaspin
 
 from voxio.caching import CachingInfo
 from voxio.read import chunk_read_stack_images
 from voxio.utils.io import cv2_read_any_depth, write_indexed_images_to_directory
 from voxio.utils.misc import get_image_dimensions, number_of_planes_loadable_to_memory
 
 defaultdict_set = partial(defaultdict, set)
 
 
 class StateOfLabel(BaseModel):
     chunk_size: int
-    volume_index: int | None
+    volume_index: int | None = None
+
     bad_object_locations: list[tuple[int, int, int]] = Field(default_factory=list)
 
-    chunk_depths: list[int, ...] = Field(default_factory=list)
+    chunk_depths: list[int] = Field(default_factory=list)
     object_id_to_locs: dict[int, set[int]] = Field(default_factory=defaultdict_set)
 
     volume_index_to_must_map_later: dict[int, set[tuple[int, int]]] = Field(
         default_factory=defaultdict_set, description="tuple[old, new]"
     )
 
     def add_loc_to_ids(self, ids: Iterable[int], loc: int) -> None:
@@ -40,15 +41,15 @@
         return sum(self.chunk_depths[:volume_index])
 
     def plane_image_id_range(self, volume_index: int) -> Iterable[int]:
         start = self.current_chunk_depth(volume_index)
         return iter(range(start, start + self.chunk_depths[volume_index]))
 
 
-def remove_objects_that_contain_other_objects_from_labeled(labeled: NDArray) -> tuple[NDArray, NDArray]:
+def remove_objects_that_contain_other_objects_from_labeled(labeled: NpNDArray) -> tuple[NpNDArray, NpNDArray]:
     """
     Caused by improper annotation. In VAST, most likely because of
     annotating at a high mip-level, which leads to gaps in the lower mips,
     which translates to extracted values.
     """
     bad_object_locations = []
     for object_slice in ndimage.find_objects(labeled):
@@ -64,15 +65,15 @@
         for label in unique_labels:
             if label:  # != 0
                 labeled[labeled == label] = 0
 
     return ndimage.label(labeled)[0], np.array(bad_object_locations)
 
 
-@validate_arguments
+@validate_call
 def label_binary_image(
     image_paths: tuple[FilePath, ...],
     output_directory: DirectoryPath,
     less_than_or_eq_254: bool = False,
 ):
     caching_info = CachingInfo(data_directory=output_directory)
     state = (
```

### Comparing `voxio-0.1.2/voxio/caching.py` & `voxio-1.0.0/voxio/caching.py`

 * *Files identical despite different names*

### Comparing `voxio-0.1.2/voxio/clean/single_big_obj_artifact_purge.py` & `voxio-1.0.0/voxio/clean/single_big_obj_artifact_purge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import count
 from logging import getLogger
 
 import imagesize
 import numpy as np
-from pydantic import DirectoryPath, FilePath, validate_arguments
+from pydantic import DirectoryPath, FilePath, validate_call
 from scipy import ndimage
 from scipy.ndimage import find_objects
 
 from voxio.read import chunk_read_stack_images
 from voxio.utils.io import cv2_read_any_depth, write_indexed_images_to_directory
 from voxio.utils.misc import number_of_planes_loadable_to_memory
 
@@ -27,15 +27,15 @@
         _volume_from_slices(*slices): label
         for label, slices in zip(range(1, num_features + 1), find_objects(labeled))
         if slices
     }
     return labeled == size_to_label[max(size_to_label)]
 
 
-@validate_arguments
+@validate_call
 def clear_everything_but_largest_object(image_paths: tuple[FilePath, ...], output_directory: DirectoryPath) -> None:
     counter = count()
     for cleaned_image_stack in chunk_read_stack_images(
         image_paths,
         number_of_planes_loadable_to_memory(
             imagesize.get(image_paths[0]),
             memory_tolerance=0.33,
```

### Comparing `voxio-0.1.2/voxio/cli/__init__.py` & `voxio-1.0.0/voxio/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from pathlib import Path
 from typing import Iterable, Optional
 
 import click
-from pydantic import DirectoryPath, FilePath, validate_arguments
+from pydantic import DirectoryPath, FilePath, validate_call
 
-from voxio.augment.label_binary_image import label_binary_image
+from voxio.workflows.label_binary_image import label_binary_image
 from voxio.cli.settings import settings
 
 global_options = click.option("-i", "--input-dir", type=Path, help="The directory storing the images")(
     click.option("-o", "--output-dir", type=Path, help="The path to the directory to output the images")
 )(click.option("-f", "--image-format", help="The format of the images"))(
     click.option(
         "-d",
@@ -39,15 +39,15 @@
 @click.group
 def voxio_cli():
     pass
 
 
 @voxio_cli.command
 @global_options
-@validate_arguments
+@validate_call
 def label_binary(image_dir: DirectoryPath, output_dir: Path, index_regex: str, image_format: Optional[str]) -> None:
     _output_dir_workflow(output_dir)
     label_binary_image(
         find_and_sort_images(
             image_dir,
         )
     )
```

### Comparing `voxio-0.1.2/voxio/crop.py` & `voxio-1.0.0/voxio/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-from pydantic_numpy import NDArray
+from pydantic_numpy import NpNDArray
 
 
 def crop_3d_image_to_content(
-    image: NDArray, z_should_be_on_edges: bool = False
-) -> tuple[NDArray, tuple[int, int, int]]:
+    image: NpNDArray, z_should_be_on_edges: bool = False
+) -> tuple[NpNDArray, tuple[int, int, int]]:
     # Find the boundary of the object array, and crop the array accordingly
     zyx_defined_idxs = np.where(image)
     z_offset, y_offset, x_offset = np.min(zyx_defined_idxs, axis=1)
     z_bound, y_bound, x_bound = np.max(zyx_defined_idxs, axis=1)
 
     assert z_should_be_on_edges or (z_offset == 0 and z_bound == len(image) - 1), (
         f"Got z-  offset: {z_offset}; bound: {z_bound}. image length {len(image) - 1}. "
```

### Comparing `voxio-0.1.2/voxio/read.py` & `voxio-1.0.0/voxio/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from concurrent.futures import ThreadPoolExecutor
 from logging import getLogger
 from pathlib import Path
 from typing import Callable, Generator, Iterable, Sequence
 
 import numpy as np
-from pydantic import DirectoryPath, FilePath, validate_arguments
+from pydantic import DirectoryPath, FilePath, validate_call
 
 from voxio.utils.io import cv2_read_any_depth
 from voxio.utils.misc import break_into_chunks, get_number_indexed_image_paths
 
 logger = getLogger(__name__)
 
 
 def read_stack_images(
     image_paths: Sequence[FilePath],
-    image_reader: Callable[[Path | str], np.ndarray],
+    image_reader: Callable[[Path], np.ndarray],
     parallel: bool = True,
 ) -> np.ndarray:
     return (
         parallel_read_stack_images(image_paths, image_reader)
         if parallel
         else np.array([image_reader(img_path) for img_path in image_paths])
     )
 
 
 def simple_read_images(image_paths: Sequence[FilePath], parallel: bool = True) -> np.ndarray:
     return read_stack_images(image_paths, cv2_read_any_depth, parallel)
 
 
-@validate_arguments
+@validate_call
 def simple_find_read_images(image_directory: DirectoryPath, *finder_args, parallel: bool = True) -> np.ndarray:
     return read_stack_images(
         get_number_indexed_image_paths(image_directory, *finder_args), cv2_read_any_depth, parallel
     )
 
 
 def chunk_read_stack_images(
     image_paths: Sequence[FilePath],
     chunk_size: int,
-    image_reader: Callable[[Path | str], np.ndarray],
+    image_reader: Callable[[Path], np.ndarray],
     offset: int = 0,
     parallel: bool = True,
 ) -> Generator[np.ndarray, None, None]:
     for idx, image_paths_chunk in enumerate(break_into_chunks(image_paths, chunk_size)):
         if idx < offset:
             continue
         yield (
```

### Comparing `voxio-0.1.2/voxio/utils/distance.py` & `voxio-1.0.0/voxio/utils/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from logging import getLogger
 from math import sqrt
 from time import sleep
 from typing import Optional
 
 import numpy as np
 import psutil
-from pydantic_numpy import NDArray
+from pydantic_numpy import NpNDArray
 from scipy.spatial.distance import cdist
 from skimage.segmentation import find_boundaries
 
 logger = getLogger(__name__)
 
 
 def image_feature_distance(
-    labeled_array: NDArray, memory_headroom: Optional[float] = None
+    labeled_array: NpNDArray, memory_headroom: Optional[float] = None
 ) -> dict[frozenset[int], float]:
     """
     Takes a labeled array as returned by scipy.ndimage.label and
     returns an intra-feature distance matrix.
 
     https://stackoverflow.com/a/37230147
     """
```

### Comparing `voxio-0.1.2/voxio/utils/interpolate.py` & `voxio-1.0.0/voxio/utils/interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from functools import lru_cache
 
 import itk
 import numpy as np
 from numpy import ScalarType
-from pydantic_numpy import NDArray
+from pydantic_numpy import NpNDArray
 
 from voxio.utils.typings import TupleSlice
 
 
 def compute_new_z_resolution(number_of_planes: int, spacing: int) -> int:
     return (
         # The image planes
         number_of_planes
         # Number of spacers
         + (number_of_planes - 1) * spacing
     )
 
 
 @lru_cache
-def generate_spacing_array(yx_shape: TupleSlice, spacing: int, data_type: ScalarType) -> NDArray:
+def generate_spacing_array(yx_shape: TupleSlice, spacing: int, data_type: ScalarType) -> NpNDArray:
     return np.zeros((spacing, *yx_shape), dtype=data_type)
 
 
-def add_inter_spacing(stack: NDArray, spacing_array: NDArray) -> NDArray:
+def add_inter_spacing(stack: NpNDArray, spacing_array: NpNDArray) -> NpNDArray:
     spaced_stack = []
     for plane in stack:
         spaced_stack.append(np.expand_dims(plane, axis=0))
         spaced_stack.append(spacing_array)
     spaced_stack.pop()
     return np.concatenate(spaced_stack)
 
 
 def morphological_interpolation_max_resolution_spacing(
-    labeled_stack: NDArray, ceiled_inter_stack_voxel_distance: int
-) -> NDArray:
+    labeled_stack: NpNDArray, ceiled_inter_stack_voxel_distance: int
+) -> NpNDArray:
     return interpolate_spaced_array(
         add_inter_spacing(
             labeled_stack,
             generate_spacing_array(
                 labeled_stack.shape[1:],
                 ceiled_inter_stack_voxel_distance,
                 labeled_stack.dtype,
             ),
         )
     )
 
 
-def interpolate_spaced_array(spaced_array: NDArray) -> NDArray:
+def interpolate_spaced_array(spaced_array: NpNDArray) -> NpNDArray:
     return itk.GetArrayFromImage(itk.morphological_contour_interpolator(itk.GetImageFromArray(spaced_array)))
```

### Comparing `voxio-0.1.2/voxio/utils/io.py` & `voxio-1.0.0/voxio/utils/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 from pathlib import Path
 from typing import Iterable
 
 import cv2
 import numpy as np
 from PIL import Image
 from pydantic import DirectoryPath, FilePath
-from pydantic_numpy import NDArray, NDArrayBool
+from pydantic_numpy import NpNDArray
+from pydantic_numpy.typing import NpNDArrayBool
 
 
 def cv2_read_any_depth(image_path: FilePath) -> np.ndarray:
     return cv2.imread(str(image_path), cv2.IMREAD_ANYDEPTH)
 
 
 def read_binarize_rgb(image_path: FilePath) -> np.ndarray[bool, bool]:
     return np.any(cv2_read_any_depth(image_path), axis=-1)
 
 
-def compressed_png_save(image: NDArray, out_path: Path) -> None:
+def compressed_png_save(image: NpNDArray, out_path: Path) -> None:
     # https://stackoverflow.com/a/60552336
     assert out_path.suffix == ".png"
     cv2.imwrite(str(out_path), image, [cv2.IMWRITE_PNG_COMPRESSION, 9])
 
 
-def one_bit_save(image: NDArrayBool, out_path: Path) -> None:
+def one_bit_save(image: NpNDArrayBool, out_path: Path) -> None:
     Image.fromarray(image).save(out_path, bits=1, optimize=True)
 
 
 def write_indexed_images_to_directory(
-    images: Iterable[NDArray],
+    images: Iterable[NpNDArray],
     index_iterator: Iterable[int],
     output_directory: DirectoryPath,
     one_bit_image: bool = False,
 ) -> None:
     with ThreadPoolExecutor() as executor:
         for image_plane in images:
             executor.submit(
```

### Comparing `voxio-0.1.2/voxio/utils/misc.py` & `voxio-1.0.0/voxio/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import re
 from math import floor
 from typing import Any, Callable, Sequence
 
 import imagesize
 import numpy as np
 import psutil
-from pydantic import DirectoryPath, FilePath, validate_arguments
+from pydantic import DirectoryPath, FilePath, validate_call
 
 
-@validate_arguments
+@validate_call
 def get_image_paths(image_directory: DirectoryPath, image_format: str, sorting_key: Callable) -> tuple[FilePath, ...]:
     assert image_directory.is_dir()
 
     file_filter = f"*.{image_format}" if image_format else "*.*"
     return tuple(sorted(image_directory.glob(file_filter), key=sorting_key))
 
 
 def get_number_indexed_image_paths(image_directory: DirectoryPath, image_format: str = "png") -> tuple[FilePath, ...]:
     finder = re.compile(r"\d+")
     return tuple(sorted(image_directory.glob(f"*.{image_format}"), key=lambda p: finder.findall(p.stem)[0]))
 
 
-@validate_arguments
+@validate_call
 def number_of_planes_loadable_to_memory(
     plane_shape: Sequence[int], memory_tolerance: float = 1.0, byte_mul: int = 1
 ) -> int:
     return floor(psutil.virtual_memory().available * memory_tolerance / (np.multiply.reduce(plane_shape) * byte_mul))
 
 
-def break_into_chunks(source: Sequence, chunk_size: int) -> list[Sequence, ...]:
+def break_into_chunks(source: Sequence, chunk_size: int) -> list[Sequence,]:
     chunks = []
     start, stop = 0, chunk_size
     while stop < len(source):
         chunks.append(source[start:stop])
         start = stop
         stop += chunk_size
     chunks.append(source[start:])
```

### Comparing `voxio-0.1.2/voxio/volume_info/read.py` & `voxio-1.0.0/voxio/volume_info/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from typing import Sequence
 
 import compress_pickle
 import numpy as np
 import psutil
 from imagesize import imagesize
 from pydantic import FilePath
-from pydantic_numpy import NDArray
+from pydantic_numpy import NpNDArray
 from scipy.ndimage import find_objects
 
 from voxio.read import cv2_read_any_depth, parallel_scan_stack_images
 from voxio.utils.distance import image_feature_distance
 from voxio.utils.misc import sort_indexed_dict_keys_to_value_list
 from voxio.volume_info.volume_info import VolumeInfo
 
-IndexAndImage = tuple[int, NDArray]
+IndexAndImage = tuple[int, NpNDArray]
 
 logger = logging.getLogger(__file__)
 
 
 def _biggest_tuple_slice_from_two(slice_a: slice, slice_b: slice) -> slice:
     return slice(min(slice_a.start, slice_b.start), max(slice_a.stop, slice_b.stop))
```

### Comparing `voxio-0.1.2/voxio/volume_info/volume_info.py` & `voxio-1.0.0/voxio/volume_info/volume_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from voxio.volume_info import MAX_NUMBER_OF_UNITS_UINT8
 
 logger = logging.getLogger(__file__)
 
 
 class VolumeInfo(BaseModel):
     plane_dimension: tuple[int, int]
-    unit_id_to_size_stack_sequence: list[dict[int, int], ...]
+    unit_id_to_size_stack_sequence: list[dict[int, int]]
     unit_pair_to_min_distance: dict[frozenset[int], float] = Field(default_factory=dict)
     unit_id_to_yx_slices: dict[int, list[slice, slice]] = Field(default_factory=dict)
 
     # We use this default_factory when serializing from YAML, empty sets confuse Pydantic
     unit_ids_on_stack_edge: set[int] = Field(default_factory=set)
 
     minimum_z_depth: ClassVar[int] = 4
@@ -114,19 +114,19 @@
         return whole, partially, uint8_compatible
 
     @cached_property
     def number_of_image_planes_loadable_to_memory(self) -> int:
         return number_of_planes_loadable_to_memory(self.plane_dimension)
 
     @property
-    def unit_id_stack_sequence(self) -> list[set[int], ...]:
+    def unit_id_stack_sequence(self) -> list[set[int],]:
         return [set(stack_dict.keys()) for stack_dict in self.unit_id_to_size_stack_sequence]
 
     @cached_property
-    def unit_id_to_stack_locations(self) -> dict[int, list[int, ...]]:
+    def unit_id_to_stack_locations(self) -> dict[int, list[int,]]:
         result = defaultdict(list)
         for plane_index, unit_id_to_size_on_plane in enumerate(self.unit_id_to_size_stack_sequence):
             for unit_id in unit_id_to_size_on_plane:
                 result[unit_id].append(plane_index)
         return result
 
     @cached_property
@@ -134,15 +134,15 @@
         result = defaultdict(lambda: 0)
         for unit_id_to_size_on_plane in self.unit_id_to_size_stack_sequence:
             for unit_id, object_size_on_plane in unit_id_to_size_on_plane.items():
                 result[unit_id] += int(object_size_on_plane)
         return dict(sorted(result.items(), key=lambda kv: kv[1], reverse=True))
 
     @cached_property
-    def unit_id_to_gaps(self) -> dict[int, list[int, ...]]:
+    def unit_id_to_gaps(self) -> dict[int, list[int,]]:
         result = {}
         for unit_id, locations in self.unit_id_to_stack_locations.items():
             if gaps := set(range(locations[0], locations[-1] + 1)).difference(locations):
                 result[unit_id] = list(gaps)
         return result
 
     @cached_property
```

### Comparing `voxio-0.1.2/PKG-INFO` & `voxio-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: voxio
-Version: 0.1.2
+Version: 1.0.0
 Summary: Library for ingesting and processing voxel (3D imaging) data
 Home-page: https://github.com/caniko/voxio
 License: BSD-4
-Keywords: 3D,voxel,processing,fix,mesh
+Keywords: voxel,processing,fix,mesh
 Author: caniko
 Author-email: canhtart@gmail.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: imagesize (>=1.4.1,<2.0.0)
 Requires-Dist: itk-morphologicalcontourinterpolation (>=1.1.0,<2.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
-Requires-Dist: numpy (>=1.17)
+Requires-Dist: numpy (>=1.23)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: pydantic-numpy (>=2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-numpy (>=3.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Repository, https://github.com/caniko/voxio
 Description-Content-Type: text/markdown
 
 # Voxio: I/O package for 3D images
```

