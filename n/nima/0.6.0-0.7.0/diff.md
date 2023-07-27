# Comparing `tmp/nima-0.6.0.tar.gz` & `tmp/nima-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nima-0.6.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nima-0.6.0.tar` & `nima-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,56 @@
--rw-r--r--   0        0        0     1476 2022-06-24 09:49:50.652137 nima-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1334 2022-07-15 13:19:49.796613 nima-0.6.0/docs/README.md
--rw-r--r--   0        0        0     3290 2022-07-15 13:19:49.840615 nima-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       43 2022-06-24 09:49:50.680139 nima-0.6.0/src/nima/__init__.py
--rw-r--r--   0        0        0    15351 2022-07-15 12:50:04.621413 nima-0.6.0/src/nima/__main__.py
--rwxr-xr-x   0        0        0    33232 2022-07-15 12:50:04.622413 nima-0.6.0/src/nima/nima.py
--rw-r--r--   0        0        0        0 2022-06-24 09:49:50.680139 nima-0.6.0/src/nima/py.typed
--rw-r--r--   0        0        0     2427 2022-07-15 13:20:28.219680 nima-0.6.0/setup.py
--rw-r--r--   0        0        0     2619 2022-07-15 13:20:28.220048 nima-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nima-0.7.0/.codespellrc
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nima-0.7.0/.darglint
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 nima-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nima-0.7.0/.python-version
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nima-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 nima-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nima-0.7.0/bandit.yml
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nima-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nima-0.7.0/docs/AUTHORS.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.7.0/docs/CHANGELOG.md -> ../CHANGELOG.md
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nima-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 nima-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima-0.7.0/docs/license.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nima-0.7.0/docs/reference.rst
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nima-0.7.0/docs/_static/.gitignore
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nima-0.7.0/docs/_static/custom.css
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nima-0.7.0/examples/holoview.ipynb.REMOVED.git-id
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/__init__.py
+-rw-r--r--   0        0        0    15527 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/__main__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/generat.py
+-rw-r--r--   0        0        0    32310 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/nima.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.7.0/src/nima/py.typed
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nima-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nima-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_generat.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_nima.py
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 nima-0.7.0/tests/test_scripts.py
+-rw-r--r--   0        0        0  6538791 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/1b_c16_15.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat0.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat1.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/test_flat2.tif
+-rw-r--r--   0        0        0   746328 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15_dim.png
+-rw-r--r--   0        0        0   101490 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15_meas.png
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/test_flat.tif
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/test_flat_gaussnorm.tif
+-rw-r--r--   0        0        0   616620 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf
+-rw-r--r--   0        0        0   469663 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf
+-rw-r--r--   0        0        0   626676 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/bg.csv
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1.csv
+-rw-r--r--   0        0        0   179299 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1_rcl.tif
+-rw-r--r--   0        0        0   186357 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label1_rpH.tif
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2.csv
+-rw-r--r--   0        0        0    96791 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2_rcl.tif
+-rw-r--r--   0        0        0   114272 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label2_rpH.tif
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3.csv
+-rw-r--r--   0        0        0    54510 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3_rcl.tif
+-rw-r--r--   0        0        0    50655 2020-02-02 00:00:00.000000 nima-0.7.0/tests/data/output/1b_c16_15/label3_rpH.tif
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 nima-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nima-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 nima-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nima-0.7.0/docs/README.md
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 nima-0.7.0/PKG-INFO
```

### Comparing `nima-0.6.0/LICENSE.txt` & `nima-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima-0.6.0/src/nima/__main__.py` & `nima-0.7.0/src/nima/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 from pathlib import Path
 
 import click
 import dask.array as da
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
+import sigfig  # type: ignore
 import tifffile  # type: ignore
 from dask.diagnostics.progress import ProgressBar
-from dask.distributed import Client
-from dask.distributed import progress
+from dask.distributed import Client, progress
 from matplotlib.backends import backend_pdf  # type: ignore
 from scipy import ndimage  # type: ignore
-from scipy import stats
 
 from nima import nima
 from nima.nima import ImArray
 
 
 @click.command()
 @click.version_option()
@@ -249,17 +248,21 @@
         ]
         df[column_order].to_csv(bname / Path("label" + str(k)).with_suffix(".csv"))
     # ##
     # labelX_{rcl,rpH}.tif ### require r_cl and r_pH present in d_im
     objs = ndimage.find_objects(d_im_bg["labels"])
     for n, o in enumerate(objs):
         name = bname / Path("label" + str(n + 1) + "_rcl").with_suffix(".tif")
-        tifffile.imwrite(name, d_im_bg["r_cl"][o], compression="lzma")
+        tifffile.imwrite(
+            name, d_im_bg["r_cl"][o], compression="lzma", photometric="minisblack"
+        )
         name = bname / Path("label" + str(n + 1) + "_rpH").with_suffix(".tif")
-        tifffile.imwrite(name, d_im_bg["r_pH"][o], compression="lzma")
+        tifffile.imwrite(
+            name, d_im_bg["r_pH"][o], compression="lzma", photometric="minisblack"
+        )
 
 
 #######################################################################################
 @click.group()
 @click.pass_context
 @click.version_option()
 @click.option(
@@ -307,24 +310,25 @@
     else:
         output = fpath.with_suffix(".png")
     if not hpix.empty:
         hpix.to_csv(output.with_suffix(".csv"), index=False)
         # FIXME hpix.y is a pd.Series[int]; it could be cast into NDArray[int]
         # TODO: if any of x y is out of the border ignore them
         nima.correct_hotpixel(err, hpix.y, hpix.x)  # type: ignore
-    shapiro = stats.shapiro(err)
-    click.secho("Shapiro-Wilk normality test p-value: " + f"{shapiro[1]:7.3g}")
+    p25, p50, p75 = np.percentile(err.ravel(), [25, 50, 75])
+    err_str = sigfig.round(p50, p75 - p25)
+    click.secho("Estimated read noise: " + err_str)
     tifffile.imwrite(output.with_suffix(".tiff"), bias)
     # Output summary graphics.
     title = os.fspath(output.with_suffix("").name)
     if bias.ndim == 2:
         plt_img_profiles(bias, title, output, hpix)
         plt_img_profiles(
             err,
-            title[:7] + f"{shapiro[1]:7.3g}",
+            "".join(("[", title[:9], "] $\\sigma_{read} = $", err_str)),
             output.with_suffix(".err.png"),
         )
     else:
         for i in range(bias.shape[0]):
             plt_img_profiles(bias[i], title, output.with_suffix(f".{i}.png"), hpix)
 
 
@@ -364,18 +368,18 @@
 @click.argument("globpath", type=str)
 def mflat(ctx: click.Context, globpath: str, bias: Path) -> None:
     """Flat from a collection of (.tif) files."""
     image_sequence = tifffile.TiffSequence(globpath)
     axes_n_shape = " ".join((str(image_sequence.axes), str(image_sequence.shape)))
     click.secho(axes_n_shape, fg="green")
     store = image_sequence.aszarr()
-    Client()
+    Client()  # type: ignore
     f = da.mean(da.from_zarr(store).rechunk(), axis=0)  # type: ignore
     fp = f.persist()
-    progress(fp)
+    progress(fp)  # type: ignore
     tprojection = fp.compute()
     if ctx.obj["output"]:
         output = ctx.obj["output"]
     else:
         output = Path(globpath).name.replace("*", "").replace("?", "")
         output = Path(output).with_suffix(".tiff")
     if bias is not None:
```

### Comparing `nima-0.6.0/src/nima/nima.py` & `nima-0.7.0/src/nima/nima.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,37 +6,33 @@
 channels.
 """
 from __future__ import annotations
 
 from collections import defaultdict
 from itertools import chain
 from pathlib import Path
-from typing import Any
-from typing import Sequence
-from typing import TypeVar
+from typing import Any, Sequence, TypeVar
 
 import matplotlib as mpl
 import matplotlib.cm
 import matplotlib.colors  # type: ignore
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import skimage  # type: ignore
 import skimage.feature  # type: ignore
 import skimage.segmentation  # type: ignore
 import skimage.transform  # type: ignore
 import tifffile  # type: ignore
 from numpy.typing import NDArray
-from scipy import ndimage  # type: ignore
-from scipy import signal
+from scipy import ndimage, signal  # type: ignore
 from skimage import filters
 from skimage.morphology import disk  # type: ignore
 
-
-ImArray = TypeVar("ImArray", NDArray[np.float_], NDArray[np.int_])
+ImArray = TypeVar("ImArray", NDArray[np.int_], NDArray[np.float_], NDArray[np.bool_])
 
 # TODO: https://towardsdatascience.com/creating-custom-plotting-functions-with-matplotlib-1f4b8eba6aa1
 
 
 def myhist(
     im: ImArray,
     bins: int = 60,
@@ -53,55 +49,14 @@
     if nf:
         plt.figure()
     plt.plot(bin_centers, hist, lw=2)
     if log:
         plt.yscale("log")  # type: ignore
 
 
-def plot_im_series(
-    im: ImArray,
-    cmap: matplotlib.colors.Colormap = matplotlib.colors.BASE_COLORS,
-    horizontal: bool = True,
-    **kw: Any,
-) -> None:
-    """Plot a image series with a maximum of 9 elements.
-
-    ..note:: Consider deprecation. Use d_show() instead.
-
-    """
-    if horizontal:
-        fig = plt.figure(figsize=(12, 5.6))
-        s = 100 + len(im) * 10 + 1
-    else:
-        fig = plt.figure(figsize=(5.6, 12))
-        s = len(im) * 100 + 10 + 1
-    for i, img in enumerate(im):
-        ax = fig.add_subplot(s + i)
-        # Switched from plt.cmd to ax.cmd
-        ax.imshow(img, cmap=cmap, **kw)
-        plt.axis("off")  # type: ignore
-    plt.subplots_adjust(wspace=0.02, hspace=0.02, top=1, bottom=0, left=0, right=1)
-
-
-def plot_otsu(
-    im: ImArray, cmap: mpl.colors.Colormap | None = None
-) -> NDArray[np.bool_]:
-    """Otsu threshold and plot im_series.
-
-    .. note:: Consider deprecation.
-
-    """
-    if not cmap:
-        cmap = plt.cm.gray  # type: ignore
-    val = filters.threshold_otsu(im)
-    mask = im > val
-    plot_im_series(im * mask, cmap=cmap)
-    return np.array(mask)
-
-
 def read_tiff(fp: Path, channels: Sequence[str]) -> tuple[dict[str, ImArray], int, int]:
     """Read multichannel tif timelapse image.
 
     Parameters
     ----------
     fp : Path
         File (TIF format) to be opened.
@@ -132,15 +87,15 @@
         axes = tif.series[0].axes
     idx = axes.rfind("T")
     if idx >= 0:
         n_times = im.shape[idx]
     else:
         n_times = 1
     if im.shape[axes.rfind("C")] % n_channels:
-        raise Exception("n_channel mismatch total lenght of tif sequence")
+        raise Exception("n_channel mismatch total length of tif sequence")
     else:
         d_im = {}
         for i, ch in enumerate(channels):
             # FIXME: must be 'TCYX' or 'ZCYX'
             if len(axes) == 4:
                 d_im[ch] = im[:, i]  # im[i::n_channels]
             elif len(axes) == 3:
@@ -168,14 +123,15 @@
         for i, r in enumerate(rng):
             ax = f.add_subplot(n_rows, n_channels, i * n_channels + n + 1)
             img0 = ax.imshow(d_im[ch][r], **kws)
             plt.colorbar(  # type: ignore
                 img0, ax=ax, orientation="vertical", pad=0.02, shrink=0.85
             )
             plt.xticks([])
+
             plt.yticks([])
             plt.ylabel(ch + " @ t = " + str(r))
     plt.subplots_adjust(wspace=0.2, hspace=0.02, top=0.9, bottom=0.1, left=0, right=1)
     return f
 
 
 def d_median(d_im: dict[str, ImArray]) -> dict[str, ImArray]:
@@ -215,15 +171,15 @@
 ) -> dict[str, ImArray]:
     """Shading correction on d_im.
 
     Subtract dark; then divide by flat.
 
     Works either with flat or d_flat
     Need also dark for each channel because it can be different when using
-    different acquisiton times.
+    different acquisition times.
 
     Parameters
     ----------
     d_im
         Dictionary of images.
     dark : 2D image or (2D) d_im
         Dark image.
@@ -272,25 +228,26 @@
     Return median, whole vector, figures (in a [list])
 
     Parameters
     ----------
     im
         An image stack.
     kind : str
-        Method {'arcsinh', 'entropy', 'adaptive', 'li_adaptive', 'li_li'} used for the segmentation.
+        Method {'arcsinh', 'entropy', 'adaptive', 'li_adaptive', 'li_li'} used for the
+        segmentation.
     perc : float
         Perc % of max-min (default=10) for thresholding *entropy* and *arcsinh*
         methods.
     radius : int, optional
         Radius (default=10) used in *entropy* and *arcsinh* (percentile_filter)
         methods.
     adaptive_radius : int, optional
         Size for the adaptive filter of skimage (default is im.shape[1]/2).
     arcsinh_perc : int, optional
-        Perc (default=80) used in the percentile_filter (scipy) whithin
+        Perc (default=80) used in the percentile_filter (scipy) within
         *arcsinh* method.
 
     Returns
     -------
     median : float
         Median of the bg masked pixels.
     pixel_values : list ?
@@ -303,14 +260,16 @@
         adaptive_radius = int(im.shape[1] / 2)
         if adaptive_radius % 2 == 0:  # sk >0.12.0 check for even value
             adaptive_radius += 1
     if (perc < 0.0) or (perc > 100.0):
         raise Exception("perc must be in [0, 100] range")
     else:
         perc /= 100
+    lim_ = False
+    m = None
     if kind == "arcsinh":
         lim = np.arcsinh(im)
         lim = ndimage.percentile_filter(lim, arcsinh_perc, size=radius)
         lim_ = True
         title: Any = radius, perc
         thr = (1 - perc) * lim.min() + perc * lim.max()
         m = lim < thr
@@ -354,15 +313,15 @@
 
     def plot() -> plt.Figure:
         f = plt.figure(figsize=(9, 5))
         ax1 = f.add_subplot(121)
         masked = im * m
         cmap = plt.cm.inferno  # type: ignore
         img0 = ax1.imshow(masked, cmap=cmap)
-        plt.colorbar(img0, ax=ax1, orientation="horizontal")  # type:ignore
+        plt.colorbar(img0, ax=ax1, orientation="horizontal")  # type: ignore
         plt.title(kind + " " + str(title) + "\n" + str(iqr))
         f.add_subplot(122)
         myhist(im[m], log=True)
         f.tight_layout()
         return f
 
     f1 = plot()
@@ -562,36 +521,36 @@
         )
         max_diameter = pr[0].equivalent_diameter
         size = max_diameter * 2.20
         for p in pr[1:]:
             max_diameter = max(max_diameter, p.equivalent_diameter)
         print(max_diameter)
         # for time, (d, l) in enumerate(zip(ga_wiener, labels)):
-        for time, (d, l) in enumerate(zip(distance, labels)):
+        for time, (d, lbl) in enumerate(zip(distance, labels)):
             local_maxi = skimage.feature.peak_local_max(
                 d,
-                labels=l,
+                labels=lbl,
                 footprint=np.ones((size, size)),
                 min_distance=size,
                 indices=False,
                 exclude_border=False,
             )
             markers = skimage.measure.label(local_maxi)
             print(np.unique(markers))
             if randomwalk:
                 markers[~mask[time]] = -1
                 labels_ws = skimage.segmentation.random_walker(mask[time], markers)
             else:
-                labels_ws = skimage.morphology.watershed(-d, markers, mask=l)
+                labels_ws = skimage.morphology.watershed(-d, markers, mask=lbl)
             labels[time] = labels_ws
     d_im["labels"] = labels
 
 
 def d_ratio(
-    d_im: dict[str, NDArray[Any]],
+    d_im: dict[str, ImArray],
     name: str = "r_cl",
     channels: tuple[str, str] = ("C", "R"),
     radii: tuple[int, int] = (7, 3),
 ) -> None:
     """Ratio image between 2 channels in d_im.
 
     Add masked (bg=0; fg=ratio) median-filtered ratio for 2 channels. So, d_im
@@ -617,15 +576,15 @@
     Notes
     -----
     Add a key named "name" and containing the calculated ratio to d_im.
 
     """
     with np.errstate(divide="ignore", invalid="ignore"):
         # 0/0 and num/0 can both happen.
-        ratio = d_im[channels[0]] / d_im[channels[1]]
+        ratio = np.array(d_im[channels[0]] / d_im[channels[1]], dtype=(float))
     for i, r in enumerate(ratio):
         np.nan_to_num(r, copy=False, posinf=0, neginf=0)
         for radius in radii:
             r = ndimage.median_filter(r, radius)
         ratio[i] = r * d_im["mask"][i]
     d_im[name] = ratio
 
@@ -643,17 +602,19 @@
     Parameters
     ----------
     d_im : d_im
         desc
     channels : list of string
         All d_im channels (default=['C', 'G', 'R']).
     channels_cl : tuple of string
-        Names (default=('C', 'R')) of the numerator and denominator channels for cl ratio.
+        Names (default=('C', 'R')) of the numerator and denominator channels for cl
+        ratio.
     channels_ph : tuple of string
-        Names (default=('G', 'C')) of the numerator and denominator channels for pH ratio.
+        Names (default=('G', 'C')) of the numerator and denominator channels for pH
+        ratio.
     ratios_from_image : bool, optional
         Boolean (default=True) for executing d_ratio i.e. compute ratio images.
     radii : (int, int), Optional
         Radii of the optional median average performed on ratio images.
 
     Returns
     -------
@@ -712,15 +673,15 @@
             df = pd.DataFrame(
                 {
                     "r_pH_median": ratios_ph[:, label - 1],
                     "r_cl_median": ratios_cl[:, label - 1],
                 }
             )
             # concat only on index that are present in both
-            meas[label] = pd.concat([meas[label], df], axis=1, join="inner")  # type: ignore
+            meas[label] = pd.concat([meas[label], df], axis=1, join="inner")
     return meas, pr
 
 
 def d_plot_meas(
     bgs: pd.DataFrame, meas: dict[np.int32, pd.DataFrame], channels: Sequence[str]
 ) -> plt.Figure:
     """Plot meas object.
@@ -775,44 +736,47 @@
         for df in meas.values():
             axes[i, j].plot(df[ch], marker="o", color=ch_colors[ch])
         axes[i, j].set_title(ch)
         axes[i, j].grid()
     if n_axes == nrows * ncols:
         axes.flat[-2].set_xlabel("time")
         axes.flat[-1].set_xlabel("time")
-        bgs.plot(ax=axes[nrows - 1, ncols - 1], grid=True, color=ch_colors)  # type: ignore
+        bgs.plot(ax=axes[nrows - 1, ncols - 1], grid=True, color=ch_colors)
     else:
         axes.flat[-3].set_xlabel("time")
         axes.flat[-2].set_xlabel("time")
-        bgs.plot(ax=axes[nrows - 1, ncols - 2], grid=True, color=ch_colors)  # type: ignore
+        bgs.plot(ax=axes[nrows - 1, ncols - 2], grid=True, color=ch_colors)
         ax = list(chain(*axes))[-1]
         ax.remove()
 
     fig.tight_layout()
     return fig
 
 
 def plt_img_profile(
     img: ImArray,
     title: str | None = None,
     hpix: pd.DataFrame | None = None,
-    **kwargs: dict[str, Any],
+    vmin: float | None = None,
+    vmax: float | None = None,
 ) -> plt.Figure:
     """Summary graphics for Flat-Bias images.
 
     Parameters
     ----------
     img : ImArray
         Image of Flat or Bias.
     title : Optional[str]
         Title of the figure.
     hpix : pd.DataFrame, optional
         Identified hot pixels (as empty or not empty df).
-    kwargs : dict
-        Keywords passed to bg() function.
+    vmin : float, optional
+        Minimum value.
+    vmax : float, optional
+        Maximum value.
 
     Returns
     -------
     plt.Figure
 
     """
     # definitions for the axes
@@ -851,15 +815,17 @@
         ax_px: plt.Axes,
         ax_py: plt.Axes,
         axh: plt.Axes,
         axc: plt.Axes,
         vmin: float | None = None,
         vmax: float | None = None,
     ) -> mpl.image.AxesImage:
-        ax_px.tick_params(axis="x", labelbottom=False, labeltop=True, top=True)  # type: ignore
+        ax_px.tick_params(  # type: ignore
+            axis="x", labelbottom=False, labeltop=True, top=True
+        )
         ax_py.tick_params(  # type: ignore
             axis="y", right=True, labelright=True, left=False, labelleft=False
         )
         ax.tick_params(axis="y", labelleft=False, right=True)  # type: ignore
         ax.tick_params(axis="x", top=True, labelbottom=False)  # type: ignore
         if vmin is None or vmax is None:  # both must be provided
             vmi, vma = np.percentile(im, [18.4, 81.6])  # 1/e (66.6 %)
@@ -877,23 +843,32 @@
         ax.axvline(xmin, c="k")  # type: ignore
         ax.axvline(xmax, c="k")  # type: ignore
         ax.axhline(ymin, c="k")  # type: ignore
         ax.axhline(ymax, c="k")  # type: ignore
         ax.yaxis.set_label_position("left")  # type: ignore
         ax.set_ylabel("Y")
         ax_py.plot(im.mean(axis=1), range(im.shape[0]), lw=4, alpha=0.5)  # type: ignore
-        ax_py.plot(im[:, xmin:xmax].mean(axis=1), range(im.shape[0]), alpha=0.7, c="k")  # type: ignore
-        axh.hist(im.ravel(), bins=max(int(im.max() - im.min()), 25), log=True, alpha=0.6, lw=4, histtype="bar")  # type: ignore
+        ax_py.plot(
+            im[:, xmin:xmax].mean(axis=1), range(im.shape[0]), alpha=0.7, c="k"
+        )  # type: ignore
+        axh.hist(  # type: ignore
+            im.ravel(),
+            bins=max(int(im.max() - im.min()), 25),
+            log=True,
+            alpha=0.6,
+            lw=4,
+            histtype="bar",
+        )
         return img
 
     if hpix is not None:
         if not hpix.empty:
             ax.plot(hpix["x"], hpix["y"], "+", mfc="gray", mew=2, ms=14)
 
-    im2c = img_hist(img, ax, ax_px, ax_py, ax_hist, ax_cm, **kwargs)  # type: ignore
+    im2c = img_hist(img, ax, ax_px, ax_py, ax_hist, ax_cm, vmin, vmax)
     ax_cm.axis("off")
     fig.colorbar(  # type: ignore
         im2c, ax=ax_cm, fraction=0.99, shrink=0.99, aspect=4, orientation="horizontal"
     )
     return fig
 
 
@@ -930,15 +905,17 @@
     ax1.plot(img[ymin:ymax, :].mean(axis=0), alpha=0.2, lw=2, c="k")  # type: ignore
     ax2 = fig.add_subplot(gs[0:2, 2])
     ax2.plot(  # type: ignore
         img[:, xmin:xmax].mean(axis=1), range(img.shape[0]), alpha=0.2, lw=2, c="k"
     )
     ax2.plot(img.mean(axis=1), range(img.shape[0]))
     axh = fig.add_subplot(gs[2, 2])
-    axh.hist(img.ravel(), bins=max(int(img.max() - img.min()), 25), log=True)  # type: ignore
+    axh.hist(
+        img.ravel(), bins=max(int(img.max() - img.min()), 25), log=True
+    )  # type: ignore
     if title:
         kw = {"weight": "bold", "ha": "left"}
         fig.suptitle(title, fontsize=12, **kw)  # type: ignore
     return fig
 
 
 def hotpixels(bias: ImArray, n_sd: int = 20) -> pd.DataFrame:
```

