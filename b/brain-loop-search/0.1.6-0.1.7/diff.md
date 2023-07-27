# Comparing `tmp/brain-loop-search-0.1.6.tar.gz` & `tmp/brain-loop-search-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-loop-search-0.1.6.tar", last modified: Tue May 16 15:10:41 2023, max compression
+gzip compressed data, was "brain-loop-search-0.1.7.tar", last modified: Thu Jul 27 11:02:11 2023, max compression
```

## Comparing `brain-loop-search-0.1.6.tar` & `brain-loop-search-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.178825 brain-loop-search-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.040970 brain-loop-search-0.1.6/.github/
--rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.6/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.042915 brain-loop-search-0.1.6/.github/workflows/
--rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.6/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.6/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4968 2023-05-16 15:10:41.177589 brain-loop-search-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.080484 brain-loop-search-0.1.6/brain_loop_search/
--rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.6/brain_loop_search/__init__.py
--rw-rw-rw-   0        0        0    11716 2023-05-16 15:06:38.000000 brain-loop-search-0.1.6/brain_loop_search/brain_utils.py
--rw-rw-rw-   0        0        0    13783 2023-05-16 05:43:01.000000 brain-loop-search-0.1.6/brain_loop_search/packing.py
--rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.6/brain_loop_search/search.py
--rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.6/brain_loop_search/structures.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.088723 brain-loop-search-0.1.6/brain_loop_search.egg-info/
--rw-rw-rw-   0        0        0     4968 2023-05-16 15:10:40.000000 brain-loop-search-0.1.6/brain_loop_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-16 15:10:41.000000 brain-loop-search-0.1.6/brain_loop_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:10:40.000000 brain-loop-search-0.1.6/brain_loop_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-16 15:10:40.000000 brain-loop-search-0.1.6/brain_loop_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-16 15:10:40.000000 brain-loop-search-0.1.6/brain_loop_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 15:10:41.178825 brain-loop-search-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 15:10:41.176581 brain-loop-search-0.1.6/test/
--rw-rw-rw-   0        0        0   149419 2023-05-16 15:07:06.000000 brain-loop-search-0.1.6/test/test.png
--rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.6/test/test2.png
--rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.6/test/test_flow.py
--rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.6/test/test_graph_packing.py
--rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.6/test/test_ontology.py
--rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.6/test/test_sssp.py
--rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.6/test/test_vertex_packing.py
--rw-rw-rw-   0        0        0     1137 2023-05-16 15:08:16.000000 brain-loop-search-0.1.6/test/test_vis.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.524175 brain-loop-search-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.259768 brain-loop-search-0.1.7/.github/
+-rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.7/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.262272 brain-loop-search-0.1.7/.github/workflows/
+-rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.7/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.7/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4968 2023-07-27 11:02:11.523177 brain-loop-search-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.304824 brain-loop-search-0.1.7/brain_loop_search/
+-rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.7/brain_loop_search/__init__.py
+-rw-rw-rw-   0        0        0    12282 2023-07-27 10:52:14.000000 brain-loop-search-0.1.7/brain_loop_search/brain_utils.py
+-rw-rw-rw-   0        0        0    13783 2023-05-16 05:43:01.000000 brain-loop-search-0.1.7/brain_loop_search/packing.py
+-rw-rw-rw-   0        0        0    19897 2023-07-27 11:00:15.000000 brain-loop-search-0.1.7/brain_loop_search/search.py
+-rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.7/brain_loop_search/structures.csv
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.313773 brain-loop-search-0.1.7/brain_loop_search.egg-info/
+-rw-rw-rw-   0        0        0     4968 2023-07-27 11:02:11.000000 brain-loop-search-0.1.7/brain_loop_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-07-27 11:02:11.000000 brain-loop-search-0.1.7/brain_loop_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:02:11.000000 brain-loop-search-0.1.7/brain_loop_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-27 11:02:11.000000 brain-loop-search-0.1.7/brain_loop_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-27 11:02:11.000000 brain-loop-search-0.1.7/brain_loop_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:02:11.524175 brain-loop-search-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 11:02:11.495451 brain-loop-search-0.1.7/test/
+-rw-rw-rw-   0        0        0   149419 2023-05-16 15:07:06.000000 brain-loop-search-0.1.7/test/test.png
+-rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.7/test/test2.png
+-rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.7/test/test_flow.py
+-rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.7/test/test_graph_packing.py
+-rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.7/test/test_ontology.py
+-rw-rw-rw-   0        0        0     3600 2023-07-27 11:00:42.000000 brain-loop-search-0.1.7/test/test_sssp.py
+-rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.7/test/test_vertex_packing.py
+-rw-rw-rw-   0        0        0     1137 2023-05-16 15:08:16.000000 brain-loop-search-0.1.7/test/test_vis.py
```

### Comparing `brain-loop-search-0.1.6/.github/workflows/static.yml` & `brain-loop-search-0.1.7/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/.gitignore` & `brain-loop-search-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/LICENSE` & `brain-loop-search-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/PKG-INFO` & `brain-loop-search-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.6
+Version: 0.1.7
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.6/README.md` & `brain-loop-search-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/brain_loop_search/brain_utils.py` & `brain-loop-search-0.1.7/brain_loop_search/brain_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 the brain ontology.
 
 The `CCFv3Ontology` is an example of how to derive an ontology.
 
 `draw_loop_in_ccf` is a visualization based on the brainrender project, also a good example.
 What is tricky is that this lib needs internet connection to download the atlas, and used some deprecated functions
 by other libs, so it may not work well for first-time. You might need to modify the lib's code.
-running.
+running. (The usage of brainrender will block other processes from using the package, so it's dumped.)
 
 """
-import itertools
-import os
+# import itertools
+# import os
 import typing
-import networkx as nx
+# import networkx as nx
 
 import pandas as pd
 import numpy as np
 from importlib_resources import files, as_file
 from .packing import Ontology
-from brainrender import Scene, settings
-from myterial import grey, white, grey_dark
-from vedo.shapes import Spline, Arrow, Tube, Line
+# from brainrender import Scene, settings
+# from myterial import grey, white, grey_dark
+# from vedo.shapes import Spline, Arrow, Tube, Line
 
 import colorsys
 import random
-from brainrender._colors import map_color
+# from brainrender._colors import map_color
 
 
 with as_file(files('brain_loop_search') / 'structures.csv') as path:
     ccfv3 = pd.read_csv(path, index_col=1)
 
 
 class CCFv3Ontology(Ontology):
@@ -76,204 +76,205 @@
     def ancestors_of(self, vert: typing.Iterable) -> pd.Series:
         return self._tree.loc[vert, 'parents']
 
     def immediate_children_of(self, vert: typing.Iterable) -> pd.Series:
         return self._tree.loc[vert, 'children']
 
 
-def draw_brain_graph(graph: nx.DiGraph, path: str | os.PathLike, thr: float = 0, render_ops: dict = None, cmap='jet'):
-    """
-    Plot a directed graph among ccfv3 brain structures.
-
-    Note: It will reset some of the brainrender global settings.
-
-    Using brainrender can cause some problem, as it
-    will attempt downloading the brain atlas from the internet and ping google.com beforehand.
-
-    If you are not connected, it will fail.
-
-    One solution to do this is to remove the ping in the package source. If the downloading is too slow,
-    you can manually download it from their website and decompress it into the package's storage directory, usually set
-    in `$HOME/.brainglobe`. Anyway, you can hack into their code to see it for yourself.
-
-    Another problem I found with brainrender is that it uses numpy's deprecated features, you might need to
-    refactor the lib source until it passes.
-
-    :param graph: a list of shortest paths consisting of brain structure IDs. Each sublist will be assigned a different
-    random color. You need to make sure the heads and tails are repeated in adjacent lists.
-    :param path: screenshot save path.
-    :param thr: only edge weights over this will be plotted.
-    :param render_ops: render options. Default is None to use the default options, see the code.
-    :param cmap: matplotlib colormap.
-    """
-    if render_ops is None:
-        render_ops = {
-            'interactive': False,
-            'camera': {
-                'pos': (4811, 3225, -42167),
-                'viewup': (0, -1, 0),
-                'clippingRange': (24770, 51413),
-                'focalPoint': (7252, 4096, -5657),
-                'distance': 36602
-            },
-            'zoom': 2
-        }
-    settings.SHOW_AXES = False
-    settings.SHADER_STYLE = "cartoon"
-    settings.ROOT_ALPHA = .05
-    settings.ROOT_COLOR = grey
-    settings.BACKGROUND_COLOR = white
-
-    scene = Scene(atlas_name='allen_mouse_100um')
-
-    regions = list(graph.nodes)
-    regions = ccfv3.loc[regions, 'acronym']
-    scene.add_brain_region(*list(regions), alpha=.02, hemisphere='left', silhouette=True)
-    e = graph.edges(data=True)
-    data = [d['weight'] for u, v, d in e if u != v]
-    vmax, vmin = max(data), min(data)
-
-    # change silhouette
-    for i in scene.get_actors(br_class="brain region"):
-        i._silhouette_kwargs['lw'] = 1
-        i._silhouette_kwargs['color'] = grey_dark
-
-    rt = scene.get_actors(br_class="brain region", name="root")[0]
-    rt._silhouette_kwargs['lw'] = 1
-    rt._silhouette_kwargs['color'] = grey
-
-    for u, v, d in e:
-        if u == v or d['weight'] < thr:
-            continue
-        # tube
-        # get a proper center of each region (this is difficult, for brain structures can be very twisted)
-        # then connect them to make a spline for a tube, which will envelop arrows
-        run = list(regions.loc[[u, v]])
-        actors = scene.get_actors(br_class="brain region", name=run)
-        sorted_actors = [None] * len(actors)
-        run_map = dict(zip(run, range(len(run))))
-        for a in actors:
-            sorted_actors[run_map[a.name]] = a
-        z_mean = [np.mean(m.points()[:, 2]) for m in sorted_actors]
-        centers = [np.mean(m.points()[m.points()[:, 2] - z < 10], axis=0) * (1, 1, -1) for m, z in zip(sorted_actors, z_mean)]
-        spl = Line(*centers, res=3)
-        pts = spl.points()
-        c = map_color(d['weight'], cmap, vmin, vmax)
-        feint = list(colorsys.rgb_to_hsv(*c))
-        feint[1] /= 2
-        feint = colorsys.hsv_to_rgb(*feint)
-
-        rr = 1 + (d['weight'] - vmin) / (vmax - vmin)
-        radius = [(np.linalg.norm(i - centers[0]) + np.linalg.norm(i - centers[-1])) / 20 * rr for i in pts]
-        scene.add(Tube(pts, radius, c=feint, alpha=0.2))
-
-        # arrows
-        scene.add(*[Arrow(*i, c=c, s=rr*3) for i in itertools.pairwise(pts)])
-
-    scene.render(**render_ops)
-    scene.screenshot(str(path))
-    scene.close()
-
-
-def draw_single_loop(loop: list[list], path: str | os.PathLike, render_ops: dict = None):
-    """
-    Plot one loop in the ccfv3 atlas using brainrender.
-
-    Note: It will reset some of the brainrender global settings.
-    Do not use this in interactive mode like jupyter, where some render options may not work.
-
-    Using brainrender can cause some problem, as it
-    will attempt downloading the brain atlas from the internet and ping google.com beforehand.
-
-    If you are not connected, it will fail.
-
-    One solution to do this is to remove the ping in the package source. If the downloading is too slow,
-    you can manually download it from their website and decompress it into the package's storage directory, usually set
-    in `$HOME/.brainglobe`. Anyway, you can hack into their code to see it for yourself.
-
-    Another problem I found with brainrender is that it uses numpy's deprecated features, you might need to
-    refactor the lib source until it passes.
-
-    :param loop: a list of shortest paths consisting of brain structure IDs. Each sublist will be assigned a different
-    random color. You need to make sure the heads and tails are repeated in adjacent lists.
-    :param path: screenshot save path.
-    :param render_ops: render options. Default is None to use the default options, see the code.
-    """
-    if render_ops is None:
-        render_ops = {
-            'interactive': False,
-            'camera': {
-                'pos': (4811, 3225, -42167),
-                'viewup': (0, -1, 0),
-                'clippingRange': (24770, 51413),
-                'focalPoint': (7252, 4096, -5657),
-                'distance': 36602
-            },
-            'zoom': 2
-        }
-    settings.SHOW_AXES = False
-    settings.SHADER_STYLE = "cartoon"
-    settings.ROOT_ALPHA = .05
-    settings.ROOT_COLOR = grey
-    settings.BACKGROUND_COLOR = white
-
-    scene = Scene(atlas_name='allen_mouse_100um')
-
-    # the root brain (usually this is just a background and not used to plot loops)
-    rt = scene.get_actors(br_class="brain region", name="root")[0]
-    rt._silhouette_kwargs['lw'] = 1
-    rt._silhouette_kwargs['color'] = grey
-
-    text_map = {}
-    count = 0
-    for run in loop:
-        run = list(ccfv3.loc[run, 'acronym'])
-        for i in run[:-1]:
-            if i not in text_map:
-                text_map[i] = []
-            count += 1
-            text_map[i].append(str(count))
-
-    for run in loop:    # each run in a loop is one sssp, will be marked by different colors
-        # map to ccf acronym
-        run = list(ccfv3.loc[run, 'acronym'])
-
-        # all traversed brain structures but the first and last one (axes)
-        scene.add_brain_region(*run[1:-1], alpha=.2, hemisphere='left', silhouette=False)
-
-        # axis regions will add silhouette, and bigger alpha
-        scene.add_brain_region(run[0], run[-1], alpha=.5, hemisphere='left', silhouette=False)
-        scene.add_silhouette(*scene.get_actors(br_class="brain region", name=[run[0], run[-1]]), lw=2)
-
-        # random hue
-        hue = random.random()
-
-        # tube
-        # get a proper center of each region (this is difficult, for brain structures can be very twisted)
-        # then connect them to make a spline for a tube, which will envelop arrows
-        actors = scene.get_actors(br_class="brain region", name=run)
-        sorted_actors = [None] * len(actors)
-        run_map = dict(zip(run, range(len(run))))
-        for a in actors:
-            sorted_actors[run_map[a.name]] = a
-        z_mean = [np.mean(m.points()[:, 2]) for m in sorted_actors]
-        centers = [np.mean(m.points()[m.points()[:, 2] - z < 10], axis=0) * (1, 1, -1) for m, z in zip(sorted_actors, z_mean)]
-        if len(centers) < 3:
-            spl = Line(*centers, res=20)
-        else:
-            spl = Spline(centers)
-        pts = spl.points()
-        radius = [(np.linalg.norm(i - centers[0]) + np.linalg.norm(i - centers[-1])) / 100 for i in pts]
-        scene.add(Tube(pts, radius, c=colorsys.hsv_to_rgb(hue, .5, .9), alpha=0.2))
-
-        # arrows
-        scene.add(*[Arrow(*i, c=colorsys.hsv_to_rgb(hue, .9, .9)) for i in itertools.pairwise(pts)])
-
-        # text
-        for i in range(len(run) - 1):
-            if run[i] in text_map:
-                sorted_actors[i].caption(f'{"/".join(text_map.pop(run[i]))}. {run[i]}',
-                                         centers[i] * (1, 1, -1), (.04, .04))
-
-    scene.render(**render_ops)
-    scene.screenshot(str(path))
-    scene.close()
+# def draw_brain_graph(graph: nx.DiGraph, path: str | os.PathLike, thr: float = 0, render_ops: dict = None, cmap='jet'):
+#     """
+#     Plot a directed graph among ccfv3 brain structures.
+#
+#     Note: It will reset some of the brainrender global settings.
+#     Do not use this in interactive mode like jupyter, where some render options may not work.
+#
+#     Using brainrender can cause some problem, as it
+#     will attempt downloading the brain atlas from the internet and ping google.com beforehand.
+#
+#     If you are not connected, it will fail.
+#
+#     One solution to do this is to remove the ping in the package source. If the downloading is too slow,
+#     you can manually download it from their website and decompress it into the package's storage directory, usually set
+#     in `$HOME/.brainglobe`. Anyway, you can hack into their code to see it for yourself.
+#
+#     Another problem I found with brainrender is that it uses numpy's deprecated features, you might need to
+#     refactor the lib source until it passes.
+#
+#     :param graph: a list of shortest paths consisting of brain structure IDs. Each sublist will be assigned a different
+#     random color. You need to make sure the heads and tails are repeated in adjacent lists.
+#     :param path: screenshot save path.
+#     :param thr: only edge weights over this will be plotted.
+#     :param render_ops: render options. Default is None to use the default options, see the code.
+#     :param cmap: matplotlib colormap.
+#     """
+#     if render_ops is None:
+#         render_ops = {
+#             'interactive': False,
+#             'camera': {
+#                 'pos': (4811, 3225, -42167),
+#                 'viewup': (0, -1, 0),
+#                 'clippingRange': (24770, 51413),
+#                 'focalPoint': (7252, 4096, -5657),
+#                 'distance': 36602
+#             },
+#             'zoom': 2
+#         }
+#     settings.SHOW_AXES = False
+#     settings.SHADER_STYLE = "cartoon"
+#     settings.ROOT_ALPHA = .05
+#     settings.ROOT_COLOR = grey
+#     settings.BACKGROUND_COLOR = white
+#
+#     scene = Scene(atlas_name='allen_mouse_100um')
+#
+#     regions = list(graph.nodes)
+#     regions = ccfv3.loc[regions, 'acronym']
+#     scene.add_brain_region(*list(regions), alpha=.02, hemisphere='left', silhouette=True)
+#     e = graph.edges(data=True)
+#     data = [d['weight'] for u, v, d in e if u != v]
+#     vmax, vmin = max(data), min(data)
+#
+#     # change silhouette
+#     for i in scene.get_actors(br_class="brain region"):
+#         i._silhouette_kwargs['lw'] = 1
+#         i._silhouette_kwargs['color'] = grey_dark
+#
+#     rt = scene.get_actors(br_class="brain region", name="root")[0]
+#     rt._silhouette_kwargs['lw'] = 1
+#     rt._silhouette_kwargs['color'] = grey
+#
+#     for u, v, d in e:
+#         if u == v or d['weight'] < thr:
+#             continue
+#         # tube
+#         # get a proper center of each region (this is difficult, for brain structures can be very twisted)
+#         # then connect them to make a spline for a tube, which will envelop arrows
+#         run = list(regions.loc[[u, v]])
+#         actors = scene.get_actors(br_class="brain region", name=run)
+#         sorted_actors = [None] * len(actors)
+#         run_map = dict(zip(run, range(len(run))))
+#         for a in actors:
+#             sorted_actors[run_map[a.name]] = a
+#         z_mean = [np.mean(m.points()[:, 2]) for m in sorted_actors]
+#         centers = [np.mean(m.points()[m.points()[:, 2] - z < 10], axis=0) * (1, 1, -1) for m, z in zip(sorted_actors, z_mean)]
+#         spl = Line(*centers, res=3)
+#         pts = spl.points()
+#         c = map_color(d['weight'], cmap, vmin, vmax)
+#         feint = list(colorsys.rgb_to_hsv(*c))
+#         feint[1] /= 2
+#         feint = colorsys.hsv_to_rgb(*feint)
+#
+#         rr = 1 + (d['weight'] - vmin) / (vmax - vmin)
+#         radius = [(np.linalg.norm(i - centers[0]) + np.linalg.norm(i - centers[-1])) / 20 * rr for i in pts]
+#         scene.add(Tube(pts, radius, c=feint, alpha=0.2))
+#
+#         # arrows
+#         scene.add(*[Arrow(*i, c=c, s=rr*3) for i in itertools.pairwise(pts)])
+#
+#     scene.render(**render_ops)
+#     scene.screenshot(str(path))
+#     scene.close()
+#
+#
+# def draw_single_loop(loop: list[list], path: str | os.PathLike, render_ops: dict = None):
+#     """
+#     Plot one loop in the ccfv3 atlas using brainrender.
+#
+#     Note: It will reset some of the brainrender global settings.
+#     Do not use this in interactive mode like jupyter, where some render options may not work.
+#
+#     Using brainrender can cause some problem, as it
+#     will attempt downloading the brain atlas from the internet and ping google.com beforehand.
+#
+#     If you are not connected, it will fail.
+#
+#     One solution to do this is to remove the ping in the package source. If the downloading is too slow,
+#     you can manually download it from their website and decompress it into the package's storage directory, usually set
+#     in `$HOME/.brainglobe`. Anyway, you can hack into their code to see it for yourself.
+#
+#     Another problem I found with brainrender is that it uses numpy's deprecated features, you might need to
+#     refactor the lib source until it passes.
+#
+#     :param loop: a list of shortest paths consisting of brain structure IDs. Each sublist will be assigned a different
+#     random color. You need to make sure the heads and tails are repeated in adjacent lists.
+#     :param path: screenshot save path.
+#     :param render_ops: render options. Default is None to use the default options, see the code.
+#     """
+#     if render_ops is None:
+#         render_ops = {
+#             'interactive': False,
+#             'camera': {
+#                 'pos': (4811, 3225, -42167),
+#                 'viewup': (0, -1, 0),
+#                 'clippingRange': (24770, 51413),
+#                 'focalPoint': (7252, 4096, -5657),
+#                 'distance': 36602
+#             },
+#             'zoom': 2
+#         }
+#     settings.SHOW_AXES = False
+#     settings.SHADER_STYLE = "cartoon"
+#     settings.ROOT_ALPHA = .05
+#     settings.ROOT_COLOR = grey
+#     settings.BACKGROUND_COLOR = white
+#
+#     scene = Scene(atlas_name='allen_mouse_100um')
+#
+#     # the root brain (usually this is just a background and not used to plot loops)
+#     rt = scene.get_actors(br_class="brain region", name="root")[0]
+#     rt._silhouette_kwargs['lw'] = 1
+#     rt._silhouette_kwargs['color'] = grey
+#
+#     text_map = {}
+#     count = 0
+#     for run in loop:
+#         run = list(ccfv3.loc[run, 'acronym'])
+#         for i in run[:-1]:
+#             if i not in text_map:
+#                 text_map[i] = []
+#             count += 1
+#             text_map[i].append(str(count))
+#
+#     for run in loop:    # each run in a loop is one sssp, will be marked by different colors
+#         # map to ccf acronym
+#         run = list(ccfv3.loc[run, 'acronym'])
+#
+#         # all traversed brain structures but the first and last one (axes)
+#         scene.add_brain_region(*run[1:-1], alpha=.2, hemisphere='left', silhouette=False)
+#
+#         # axis regions will add silhouette, and bigger alpha
+#         scene.add_brain_region(run[0], run[-1], alpha=.5, hemisphere='left', silhouette=False)
+#         scene.add_silhouette(*scene.get_actors(br_class="brain region", name=[run[0], run[-1]]), lw=2)
+#
+#         # random hue
+#         hue = random.random()
+#
+#         # tube
+#         # get a proper center of each region (this is difficult, for brain structures can be very twisted)
+#         # then connect them to make a spline for a tube, which will envelop arrows
+#         actors = scene.get_actors(br_class="brain region", name=run)
+#         sorted_actors = [None] * len(actors)
+#         run_map = dict(zip(run, range(len(run))))
+#         for a in actors:
+#             sorted_actors[run_map[a.name]] = a
+#         z_mean = [np.mean(m.points()[:, 2]) for m in sorted_actors]
+#         centers = [np.mean(m.points()[m.points()[:, 2] - z < 10], axis=0) * (1, 1, -1) for m, z in zip(sorted_actors, z_mean)]
+#         if len(centers) < 3:
+#             spl = Line(*centers, res=20)
+#         else:
+#             spl = Spline(centers)
+#         pts = spl.points()
+#         radius = [(np.linalg.norm(i - centers[0]) + np.linalg.norm(i - centers[-1])) / 100 for i in pts]
+#         scene.add(Tube(pts, radius, c=colorsys.hsv_to_rgb(hue, .5, .9), alpha=0.2))
+#
+#         # arrows
+#         scene.add(*[Arrow(*i, c=colorsys.hsv_to_rgb(hue, .9, .9)) for i in itertools.pairwise(pts)])
+#
+#         # text
+#         for i in range(len(run) - 1):
+#             if run[i] in text_map:
+#                 sorted_actors[i].caption(f'{"/".join(text_map.pop(run[i]))}. {run[i]}',
+#                                          centers[i] * (1, 1, -1), (.04, .04))
+#
+#     scene.render(**render_ops)
+#     scene.screenshot(str(path))
+#     scene.close()
```

### Comparing `brain-loop-search-0.1.6/brain_loop_search/packing.py` & `brain-loop-search-0.1.7/brain_loop_search/packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/brain_loop_search/search.py` & `brain-loop-search-0.1.7/brain_loop_search/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
 import typing
 
 import networkx as nx
 import pandas as pd
 import numpy as np
 import itertools
-from copy import deepcopy
 from collections import OrderedDict
+from tqdm import tqdm
 
 
 class GraphMaintainer:
 
     def __init__(self):
         self.graph = nx.DiGraph()
 
@@ -190,14 +190,24 @@
     summation is also meaningful.
 
     With this class, you can get loops in forms of exact lists of nodes along the loop.
 
     The shortest path algorithm uses the 'weight' attribute in the networkx graph.
     """
 
+    def __init__(self):
+        super().__init__()
+        self.sssp = None
+
+    def init(self):
+        # bellman ford
+        self.sssp = {}
+        for k, v in tqdm(nx.all_pairs_bellman_ford_path(self.graph), total=self.graph.number_of_nodes()):
+            self.sssp[k] = v
+
     def chain_screen(self, n_axis=2, top: int = None, must_include: typing.Iterable = None, allow_knots=False,
                      axis_pool: typing.Iterable = None, axis_must_include: typing.Iterable = None, priority=np.sum):
         """
         Using connected single source shortest paths to find loops. You should ensure that in your graph smaller edge
         weights means stronger connection for this method.
 
         First, use Bellman Ford to find the shortest paths between all regions. Then loops can be found by
@@ -242,21 +252,21 @@
             assert len(axis_must_include) <= n_axis, "number of must included axis is more than specified"
         if axis_pool is not None:
             axis_pool = set(axis_pool)
             assert len(axis_pool) >= n_axis, "size of axis pool is smaller than specified"
             if axis_must_include is not None:
                 assert axis_must_include.issubset(axis_pool), "must included axis should be subset of axis pool"
 
-        # bellman ford
-        sssp = dict(nx.all_pairs_bellman_ford_path(self.graph))
+        if self.sssp is None:
+            self.init()
 
         # do an edge sorting beforehand, ascending
         # vertices not in axis pool (if not None) will be omitted
         connection = []
-        for k1, v1 in sssp.items():
+        for k1, v1 in self.sssp.items():
             if axis_pool is not None and k1 not in axis_pool:
                 continue
             for k2, v2 in v1.items():
                 if axis_pool is not None and k2 not in axis_pool:
                     continue
                 if k1 == k2:
                     continue
@@ -267,15 +277,15 @@
         connection.sort(key=lambda x: x[2])
         sorted_sssp = OrderedDict()
         # sorted_sssp[k1][k2] -> (length, list of vertices)
         # and k2 mapping is ordered
         for i, (k1, k2, w) in enumerate(connection):
             if k1 not in sorted_sssp:
                 sorted_sssp[k1] = OrderedDict()
-            sorted_sssp[k1][k2] = (w, sssp[k1][k2])
+            sorted_sssp[k1][k2] = (w, self.sssp[k1][k2])
 
         max_iter = [0 if top is None else top]
         loops = {}
 
         def dfs_loop_search(loop: list, visited: set, length: float):
             # finishing, the last part of the cycle,
             if len(loop) == n_axis - 1:
@@ -332,15 +342,15 @@
                 gen = next(gen)
             else:
                 stk.pop()
                 if not stk:
                     break
                 gen = stk[-1].send(gen)
 
-        return loops, deepcopy(sssp)
+        return loops
 
     def pair_complement(self, axis_pool: typing.Iterable = None):
         """
         Given a pair of vertices, the loop is defined as the direct connection between them plus the inverted shortest path.
         For example, with A and B, the loop can be either edge AB + the shortest path from B to A
         or edge BA + the shortest path from A to B. This comes in handy when shortest paths from A to B and B to A have
         intersection, leading to knots in a loop.
@@ -349,15 +359,16 @@
 
         :param axis_pool: a list of vertices for axes to choose from, which can largely narrow down the search space.
             Default as None to turn off, and it will try every pair of vertices as long as there's a direct edge.
         :return: a dict of loops, keys are the direct edges and values are the corresponding inverse shortest path.
         """
         if axis_pool is not None:
             axis_pool = set(axis_pool)
-        sssp = dict(nx.all_pairs_bellman_ford_path(self.graph))
+        if self.sssp is None:
+            self.init()
         out = {}
         for fro, to in self.graph.edges:
             if axis_pool is not None and (fro not in axis_pool or to not in axis_pool) or to == fro:
                 continue
-            if to in sssp and fro in sssp[to]:
-                out[(fro, to)] = sssp[to][fro]
+            if to in self.sssp and fro in self.sssp[to]:
+                out[(fro, to)] = self.sssp[to][fro]
         return out
```

### Comparing `brain-loop-search-0.1.6/brain_loop_search/structures.csv` & `brain-loop-search-0.1.7/brain_loop_search/structures.csv`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/brain_loop_search.egg-info/PKG-INFO` & `brain-loop-search-0.1.7/brain_loop_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.6
+Version: 0.1.7
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brain-loop-search-0.1.6/brain_loop_search.egg-info/SOURCES.txt` & `brain-loop-search-0.1.7/brain_loop_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/pyproject.toml` & `brain-loop-search-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test.png` & `brain-loop-search-0.1.7/test/test.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test2.png` & `brain-loop-search-0.1.7/test/test2.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test_flow.py` & `brain-loop-search-0.1.7/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test_graph_packing.py` & `brain-loop-search-0.1.7/test/test_graph_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test_ontology.py` & `brain-loop-search-0.1.7/test/test_ontology.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test_sssp.py` & `brain-loop-search-0.1.7/test/test_sssp.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
             ("c", "d", {"weight": 3}),
             ("e", "d", {"weight": 2})
         ])
 
     def test_find_loop_sssp(self):
         g = ShortestPathLoopSearch()
         g.add_subgraph(self.edges)
-        loops, sssp = g.chain_screen(n_axis=2)
+        g.init()
+        loops = g.chain_screen(n_axis=2)
         self.assertCountEqual(list(loops.keys()), [("a", "b"), ("a", "c"), ("b", "d"), ("c", "d"), ("b", "c")])
         self.assertCountEqual(["".join(s) for s in loops[("a", "b")]['loop']], ["ab", "ba"])
         self.assertCountEqual(["".join(s) for s in loops[("a", "c")]['loop']], ["ac", 'ca'])
         self.assertCountEqual(["".join(s) for s in loops[("b", "d")]['loop']], ["bd", "db"])
         self.assertCountEqual(["".join(s) for s in loops[("c", "d")]['loop']], ["cd", 'dbc'])
         self.assertCountEqual(["".join(s) for s in loops[("b", "c")]['loop']], ["bc", 'cdb'])
         print(loops)
```

### Comparing `brain-loop-search-0.1.6/test/test_vertex_packing.py` & `brain-loop-search-0.1.7/test/test_vertex_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.6/test/test_vis.py` & `brain-loop-search-0.1.7/test/test_vis.py`

 * *Files identical despite different names*

