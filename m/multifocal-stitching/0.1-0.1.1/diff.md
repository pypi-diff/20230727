# Comparing `tmp/multifocal-stitching-0.1.tar.gz` & `tmp/multifocal-stitching-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multifocal-stitching-0.1.tar", last modified: Thu Jul 27 05:20:38 2023, max compression
+gzip compressed data, was "multifocal-stitching-0.1.1.tar", last modified: Thu Jul 27 05:30:19 2023, max compression
```

## Comparing `multifocal-stitching-0.1.tar` & `multifocal-stitching-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.1/LICENSE
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2719 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      699 2023-07-27 05:20:17.000000 multifocal-stitching-0.1/README.md
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1564 2023-07-27 05:19:57.000000 multifocal-stitching-0.1/pyproject.toml
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/setup.cfg
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/src/
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/src/multifocal_stitching/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       41 2023-07-27 04:00:42.000000 multifocal-stitching-0.1/src/multifocal_stitching/__init__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1816 2023-07-27 04:19:13.000000 multifocal-stitching-0.1/src/multifocal_stitching/merge_imgs.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     6063 2023-07-27 04:31:32.000000 multifocal-stitching-0.1/src/multifocal_stitching/stitching.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1185 2023-07-27 04:26:53.000000 multifocal-stitching-0.1/src/multifocal_stitching/utils.py
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2719 2023-07-27 05:20:38.000000 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      443 2023-07-27 05:20:38.000000 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/SOURCES.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-27 05:20:38.000000 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/dependency_links.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       91 2023-07-27 05:20:38.000000 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/requires.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-27 05:20:38.000000 multifocal-stitching-0.1/src/multifocal_stitching.egg-info/top_level.txt
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:20:38.835842 multifocal-stitching-0.1/tests/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1906 2023-07-27 05:07:49.000000 multifocal-stitching-0.1/tests/test_stitching.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.1.1/LICENSE
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5037 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3015 2023-07-27 05:28:03.000000 multifocal-stitching-0.1.1/README.md
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1566 2023-07-27 05:29:05.000000 multifocal-stitching-0.1.1/pyproject.toml
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/setup.cfg
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/multifocal_stitching/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       41 2023-07-27 04:00:42.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/__init__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1166 2023-07-27 05:25:55.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/__main__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1816 2023-07-27 04:19:13.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/merge_imgs.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5107 2023-07-27 05:23:29.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/stitching.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1185 2023-07-27 04:26:53.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/utils.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5037 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      480 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       91 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/requires.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/top_level.txt
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/tests/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1906 2023-07-27 05:07:49.000000 multifocal-stitching-0.1.1/tests/test_stitching.py
```

### Comparing `multifocal-stitching-0.1/LICENSE` & `multifocal-stitching-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.1/pyproject.toml` & `multifocal-stitching-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multifocal-stitching"
-version = "0.1"
+version = "0.1.1"
 description = "Algorithms and tools for stitching microscopy images taken at different focal lengths"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "Chenyang Yuan", email = "yuanchenyang@gmail.com" }
 ]
```

### Comparing `multifocal-stitching-0.1/src/multifocal_stitching/merge_imgs.py` & `multifocal-stitching-0.1.1/src/multifocal_stitching/merge_imgs.py`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.1/src/multifocal_stitching/stitching.py` & `multifocal-stitching-0.1.1/src/multifocal_stitching/stitching.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,26 +119,7 @@
     parser.add_argument('--peaks_dist_threshold', type=float,
                         help='Distance to consider as part of same cluster when finding peak centroid',
                         default=25)
     parser.add_argument('--filter_radius', nargs="+", type=int,
                         default=(100,50,20),
                         help='Low-pass filter radii to try, smaller matches coarser/out-of-focus features')
     return parser
-
-def main():
-    parser = add_stitching_args(add_merge_args(get_default_parser()))
-    args = parser.parse_args()
-    img_names = sorted(get_filenames(args))
-    with open(get_full_path(args, args.stitching_result), 'w') as outfile:
-        writer = csv.writer(outfile, delimiter=',')
-        writer.writerow(['Img 1', 'Img 2', 'X offset', 'Y offset', 'Corr Value', 'Area', 'r', 'use_win'])
-        for img_names in pairwise(img_names):
-            if args.verbose: print('Stitching', *img_names)
-            corr, res, (dx, dy), val, area, r, use_win = stitch(args, *map(read_img, img_names))
-            img_name1, img_name2 = map(get_name, img_names)
-            writer.writerow([img_name1, img_name2, dx, dy, corr, area, r, use_win])
-            if not args.no_merge:
-                res_dir = get_full_path(args, args.result_dir, mkdir=True)
-                merge_imgs(args, res_dir, img_name1, img_name2, dx, dy)
-
-if __name__=='__main__':
-    main()
```

### Comparing `multifocal-stitching-0.1/src/multifocal_stitching/utils.py` & `multifocal-stitching-0.1.1/src/multifocal_stitching/utils.py`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.1/tests/test_stitching.py` & `multifocal-stitching-0.1.1/tests/test_stitching.py`

 * *Files identical despite different names*

