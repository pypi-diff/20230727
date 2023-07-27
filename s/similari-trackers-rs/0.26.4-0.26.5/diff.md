# Comparing `tmp/similari_trackers_rs-0.26.4.tar.gz` & `tmp/similari_trackers_rs-0.26.5.tar.gz`

## Comparing `similari_trackers_rs-0.26.4.tar` & `similari_trackers_rs-0.26.5.tar`

### file list

```diff
@@ -1,135 +1,134 @@
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.4/Cargo.toml
--rw-r--r--   0     1001      123      274 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.cargo/config
--rw-r--r--   0     1001      123       62 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.dockerignore
--rw-r--r--   0     1001      123     2086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_10.yml
--rw-r--r--   0     1001      123     2086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_11.yml
--rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_8.yml
--rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_9.yml
--rw-r--r--   0     1001      123     2082 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-rust-1_67.yml
--rw-r--r--   0     1001      123     2206 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      346 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.github/workflows/rust.yml
--rw-r--r--   0     1001      123       48 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/.gitignore
--rw-r--r--   0     1001      123    29851 2023-06-03 08:29:31.000000 similari_trackers_rs-0.26.4/Cargo.lock
--rw-r--r--   0     1001      123    11384 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/LICENSE
--rw-r--r--   0     1001      123    15407 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/README.md
--rw-r--r--   0     1001      123     5748 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/assets/benchmarks/benchmarks.md
--rw-r--r--   0     1001      123    14603 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/assets/documentation/python/api.md
--rw-r--r--   0     1001      123     2418 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/batch_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     2307 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/batch_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     1344 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/bbox_own_areas.rs
--rw-r--r--   0     1001      123     5023 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/feature_tracker.rs
--rw-r--r--   0     1001      123      841 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/kalman_2d_point.rs
--rw-r--r--   0     1001      123      952 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/kalman_bbox.rs
--rw-r--r--   0     1001      123      986 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/nms.rs
--rw-r--r--   0     1001      123     1182 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/nms_oriented.rs
--rw-r--r--   0     1001      123     2084 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_search.rs
--rw-r--r--   0     1001      123     2209 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     2379 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker_oriented.rs
--rw-r--r--   0     1001      123     2123 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     2271 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker_oriented.rs
--rw-r--r--   0     1001      123     4354 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/simple_visual_sort_tracker.rs
--rw-r--r--   0     1001      123     2052 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/benches/track_search.rs
--rw-r--r--   0     1001      123       71 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/build.rs
--rw-r--r--   0     1001      123      392 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/common/install-basic-deps.sh
--rw-r--r--   0     1001      123      641 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.10/Dockerfile
--rw-r--r--   0     1001      123      641 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.11/Dockerfile
--rw-r--r--   0     1001      123      638 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.8/Dockerfile
--rw-r--r--   0     1001      123      640 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/python_3.9/Dockerfile
--rw-r--r--   0     1001      123      634 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/docker/rust_1.67/Dockerfile
--rw-r--r--   0     1001      123     1737 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/batch_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     5285 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/incremental_track_build.rs
--rw-r--r--   0     1001      123     3086 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/middleware_sort_tracker.rs
--rw-r--r--   0     1001      123     2427 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple.rs
--rw-r--r--   0     1001      123     1385 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker.rs
--rw-r--r--   0     1001      123     1280 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker_oriented.rs
--rw-r--r--   0     1001      123     1256 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker.rs
--rw-r--r--   0     1001      123     1136 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker_oriented.rs
--rw-r--r--   0     1001      123    16013 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/examples/track_merging.rs
--rw-r--r--   0     1001      123      469 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/pyproject.toml
--rw-r--r--   0     1001      123      850 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bb.py
--rw-r--r--   0     1001      123     2539 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/bug_visual_sort.py
--rw-r--r--   0     1001      123    25550 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json
--rw-r--r--   0     1001      123    25569 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json
--rw-r--r--   0     1001      123    25393 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-1.json
--rw-r--r--   0     1001      123    25550 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-2.json
--rw-r--r--   0     1001      123     5744 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/bugfixes/github-84.py
--rw-r--r--   0     1001      123      650 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/clipping_intersection.py
--rw-r--r--   0     1001      123      369 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_2d_point.py
--rw-r--r--   0     1001      123      508 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_2d_vec.py
--rw-r--r--   0     1001      123      916 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/kalman_bbox.py
--rw-r--r--   0     1001      123     1391 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/Dockerfile
--rw-r--r--   0     1001      123     2564 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/README.md
--rw-r--r--   0     1001      123        0 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/__init__.py
--rw-r--r--   0     1001      123     2879 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/__main__.py
--rw-r--r--   0     1001      123     3639 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/config.py
--rw-r--r--   0     1001      123     1923 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/config.yml
--rw-r--r--   0     1001      123     1940 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/confs/original-sort-config.yml
--rw-r--r--   0     1001      123     1506 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/confs/similari-maha-sort-config.yml
--rw-r--r--   0     1001      123     1437 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/evaluator.py
--rw-r--r--   0     1001      123       38 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/requirements.txt
--rw-r--r--   0     1001      123     4126 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/trackers.py
--rw-r--r--   0     1001      123     1116 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/motchallenge/utils.py
--rw-r--r--   0     1001      123      576 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/nms.py
--rw-r--r--   0     1001      123     1156 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/batch_sort_iou.py
--rw-r--r--   0     1001      123     1406 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/batch_sort_iou_bench.py
--rw-r--r--   0     1001      123      665 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_idle.py
--rw-r--r--   0     1001      123      797 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou.py
--rw-r--r--   0     1001      123      987 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_bench.py
--rw-r--r--   0     1001      123     1071 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_rotated.py
--rw-r--r--   0     1001      123     1009 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_iou_scene_id.py
--rw-r--r--   0     1001      123      806 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/sort/sort_maha.py
--rw-r--r--   0     1001      123     5068 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort/batch_visual_sort.py
--rw-r--r--   0     1001      123     3363 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort/visual_sort.py
--rw-r--r--   0     1001      123     1574 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/python/visual_sort.py
--rw-r--r--   0     1001      123     2297 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/distance.rs
--rw-r--r--   0     1001      123     2452 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/examples/iou.rs
--rw-r--r--   0     1001      123     7222 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/examples.rs
--rw-r--r--   0     1001      123     5508 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/lib.rs
--rw-r--r--   0     1001      123      836 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/prelude.rs
--rw-r--r--   0     1001      123     6390 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/builder.rs
--rw-r--r--   0     1001      123      221 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/notify.rs
--rw-r--r--   0     1001      123     2732 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/builder.rs
--rw-r--r--   0     1001      123    19590 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/store_tests.rs
--rw-r--r--   0     1001      123     9338 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store/track_distance.rs
--rw-r--r--   0     1001      123    25504 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/store.rs
--rw-r--r--   0     1001      123     2649 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/utils.rs
--rw-r--r--   0     1001      123     3928 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting/best.rs
--rw-r--r--   0     1001      123     8799 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting/topn.rs
--rw-r--r--   0     1001      123      759 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track/voting.rs
--rw-r--r--   0     1001      123    42240 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/track.rs
--rw-r--r--   0     1001      123     3425 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/batch.rs
--rw-r--r--   0     1001      123     3825 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/epoch_db.rs
--rw-r--r--   0     1001      123      944 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/kalman_prediction.rs
--rw-r--r--   0     1001      123    16922 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/batch_api.rs
--rw-r--r--   0     1001      123     6729 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/metric.rs
--rw-r--r--   0     1001      123    19512 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/simple_api.rs
--rw-r--r--   0     1001      123      787 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/sort_py.rs
--rw-r--r--   0     1001      123     4986 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort/voting.rs
--rw-r--r--   0     1001      123    13720 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/sort.rs
--rw-r--r--   0     1001      123     3374 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/spatio_temporal_constraints.rs
--rw-r--r--   0     1001      123     3783 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/tracker_api.rs
--rw-r--r--   0     1001      123    20356 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/batch_api.rs
--rw-r--r--   0     1001      123     8106 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric/builder.rs
--rw-r--r--   0     1001      123    36076 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric.rs
--rw-r--r--   0     1001      123     3904 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/observation_attributes.rs
--rw-r--r--   0     1001      123    14760 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/options.rs
--rw-r--r--   0     1001      123    30552 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/simple_api.rs
--rw-r--r--   0     1001      123     8182 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/track_attributes.rs
--rw-r--r--   0     1001      123     2640 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/visual_sort_py.rs
--rw-r--r--   0     1001      123     7537 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort/voting.rs
--rw-r--r--   0     1001      123     2614 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers/visual_sort.rs
--rw-r--r--   0     1001      123      643 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/trackers.rs
--rw-r--r--   0     1001      123    18919 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/bbox.rs
--rw-r--r--   0     1001      123     2613 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping/bbox_own_areas.rs
--rw-r--r--   0     1001      123     1803 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping/clipping_py.rs
--rw-r--r--   0     1001      123     3347 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/clipping.rs
--rw-r--r--   0     1001      123    11445 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_box.rs
--rw-r--r--   0     1001      123    10152 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point.rs
--rw-r--r--   0     1001      123     5029 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point_vec.rs
--rw-r--r--   0     1001      123     2435 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/kalman.rs
--rw-r--r--   0     1001      123     2104 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/nms/nms_py.rs
--rw-r--r--   0     1001      123     5115 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/nms.rs
--rw-r--r--   0     1001      123       30 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/point.rs
--rw-r--r--   0     1001      123      612 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils/primitive.rs
--rw-r--r--   0     1001      123      466 2023-06-03 08:27:21.000000 similari_trackers_rs-0.26.4/src/utils.rs
--rw-r--r--   0        0        0    16190 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.4/PKG-INFO
+-rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.5/Cargo.toml
+-rw-r--r--   0     1001      123      274 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.cargo/config
+-rw-r--r--   0     1001      123       62 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.dockerignore
+-rw-r--r--   0     1001      123     2086 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_10.yml
+-rw-r--r--   0     1001      123     2086 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_11.yml
+-rw-r--r--   0     1001      123     2084 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_8.yml
+-rw-r--r--   0     1001      123     2084 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_9.yml
+-rw-r--r--   0     1001      123     2082 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-rust-1_67.yml
+-rw-r--r--   0     1001      123     2206 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      346 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123       48 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/.gitignore
+-rw-r--r--   0     1001      123    28060 2023-07-27 06:37:24.000000 similari_trackers_rs-0.26.5/Cargo.lock
+-rw-r--r--   0     1001      123    11384 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/LICENSE
+-rw-r--r--   0     1001      123    15407 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/README.md
+-rw-r--r--   0     1001      123     5748 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/assets/benchmarks/benchmarks.md
+-rw-r--r--   0     1001      123    14603 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/assets/documentation/python/api.md
+-rw-r--r--   0     1001      123     2418 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/batch_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     2307 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/batch_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     1344 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/bbox_own_areas.rs
+-rw-r--r--   0     1001      123     5023 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/feature_tracker.rs
+-rw-r--r--   0     1001      123      841 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/kalman_2d_point.rs
+-rw-r--r--   0     1001      123      952 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/kalman_bbox.rs
+-rw-r--r--   0     1001      123      986 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/nms.rs
+-rw-r--r--   0     1001      123     1200 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/nms_oriented.rs
+-rw-r--r--   0     1001      123     2084 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_search.rs
+-rw-r--r--   0     1001      123     2209 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     2379 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_sort_iou_tracker_oriented.rs
+-rw-r--r--   0     1001      123     2123 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     2271 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_sort_maha_tracker_oriented.rs
+-rw-r--r--   0     1001      123     4354 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/simple_visual_sort_tracker.rs
+-rw-r--r--   0     1001      123     2052 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/benches/track_search.rs
+-rw-r--r--   0     1001      123      102 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/build.rs
+-rw-r--r--   0     1001      123      392 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/common/install-basic-deps.sh
+-rw-r--r--   0     1001      123      641 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/python_3.10/Dockerfile
+-rw-r--r--   0     1001      123      641 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/python_3.11/Dockerfile
+-rw-r--r--   0     1001      123      638 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/python_3.8/Dockerfile
+-rw-r--r--   0     1001      123      640 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/python_3.9/Dockerfile
+-rw-r--r--   0     1001      123      634 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/docker/rust_1.67/Dockerfile
+-rw-r--r--   0     1001      123     1737 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/batch_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     5285 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/incremental_track_build.rs
+-rw-r--r--   0     1001      123     3086 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/middleware_sort_tracker.rs
+-rw-r--r--   0     1001      123     2427 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/simple.rs
+-rw-r--r--   0     1001      123     1385 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/simple_sort_iou_tracker.rs
+-rw-r--r--   0     1001      123     1280 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/simple_sort_iou_tracker_oriented.rs
+-rw-r--r--   0     1001      123     1256 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/simple_sort_maha_tracker.rs
+-rw-r--r--   0     1001      123     1136 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/simple_sort_maha_tracker_oriented.rs
+-rw-r--r--   0     1001      123    16013 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/examples/track_merging.rs
+-rw-r--r--   0     1001      123      469 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/pyproject.toml
+-rw-r--r--   0     1001      123      850 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bb.py
+-rw-r--r--   0     1001      123     2539 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/bug_visual_sort.py
+-rw-r--r--   0     1001      123    25550 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json
+-rw-r--r--   0     1001      123    25569 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json
+-rw-r--r--   0     1001      123    25393 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/in-1.json
+-rw-r--r--   0     1001      123    25550 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/in-2.json
+-rw-r--r--   0     1001      123     5744 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/bugfixes/github-84.py
+-rw-r--r--   0     1001      123      650 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/clipping_intersection.py
+-rw-r--r--   0     1001      123      369 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/kalman_2d_point.py
+-rw-r--r--   0     1001      123      508 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/kalman_2d_vec.py
+-rw-r--r--   0     1001      123      916 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/kalman_bbox.py
+-rw-r--r--   0     1001      123     1391 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/Dockerfile
+-rw-r--r--   0     1001      123     2564 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/README.md
+-rw-r--r--   0     1001      123        0 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/__init__.py
+-rw-r--r--   0     1001      123     2879 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/__main__.py
+-rw-r--r--   0     1001      123     3639 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/config.py
+-rw-r--r--   0     1001      123     1923 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/config.yml
+-rw-r--r--   0     1001      123     1940 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/confs/original-sort-config.yml
+-rw-r--r--   0     1001      123     1506 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/confs/similari-maha-sort-config.yml
+-rw-r--r--   0     1001      123     1437 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/evaluator.py
+-rw-r--r--   0     1001      123       38 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/requirements.txt
+-rw-r--r--   0     1001      123     4126 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/trackers.py
+-rw-r--r--   0     1001      123     1116 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/motchallenge/utils.py
+-rw-r--r--   0     1001      123      576 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/nms.py
+-rw-r--r--   0     1001      123     1156 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/batch_sort_iou.py
+-rw-r--r--   0     1001      123     1406 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/batch_sort_iou_bench.py
+-rw-r--r--   0     1001      123      665 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_idle.py
+-rw-r--r--   0     1001      123      797 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_iou.py
+-rw-r--r--   0     1001      123      987 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_iou_bench.py
+-rw-r--r--   0     1001      123     1071 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_iou_rotated.py
+-rw-r--r--   0     1001      123     1009 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_iou_scene_id.py
+-rw-r--r--   0     1001      123      806 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/sort/sort_maha.py
+-rw-r--r--   0     1001      123     5068 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/visual_sort/batch_visual_sort.py
+-rw-r--r--   0     1001      123     3376 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/visual_sort/visual_sort.py
+-rw-r--r--   0     1001      123     1574 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/python/visual_sort.py
+-rw-r--r--   0     1001      123     2297 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/distance.rs
+-rw-r--r--   0     1001      123     2452 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/examples/iou.rs
+-rw-r--r--   0     1001      123     7222 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/examples.rs
+-rw-r--r--   0     1001      123     5729 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/lib.rs
+-rw-r--r--   0     1001      123      836 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/prelude.rs
+-rw-r--r--   0     1001      123     6390 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/builder.rs
+-rw-r--r--   0     1001      123      221 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/notify.rs
+-rw-r--r--   0     1001      123     2732 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/store/builder.rs
+-rw-r--r--   0     1001      123    19590 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/store/store_tests.rs
+-rw-r--r--   0     1001      123     9338 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/store/track_distance.rs
+-rw-r--r--   0     1001      123    25504 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/store.rs
+-rw-r--r--   0     1001      123     2649 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/utils.rs
+-rw-r--r--   0     1001      123     3928 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/voting/best.rs
+-rw-r--r--   0     1001      123     8799 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/voting/topn.rs
+-rw-r--r--   0     1001      123      759 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track/voting.rs
+-rw-r--r--   0     1001      123    42240 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/track.rs
+-rw-r--r--   0     1001      123     3966 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/batch.rs
+-rw-r--r--   0     1001      123     3825 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/epoch_db.rs
+-rw-r--r--   0     1001      123      944 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/kalman_prediction.rs
+-rw-r--r--   0     1001      123    19041 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/sort/batch_api.rs
+-rw-r--r--   0     1001      123     6796 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/sort/metric.rs
+-rw-r--r--   0     1001      123    19933 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/sort/simple_api.rs
+-rw-r--r--   0     1001      123     4986 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/sort/voting.rs
+-rw-r--r--   0     1001      123    16863 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/sort.rs
+-rw-r--r--   0     1001      123     4094 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/spatio_temporal_constraints.rs
+-rw-r--r--   0     1001      123     3779 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/tracker_api.rs
+-rw-r--r--   0     1001      123    22805 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/batch_api.rs
+-rw-r--r--   0     1001      123     7565 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/metric/builder.rs
+-rw-r--r--   0     1001      123    36434 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/metric.rs
+-rw-r--r--   0     1001      123     3904 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/observation_attributes.rs
+-rw-r--r--   0     1001      123    15368 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/options.rs
+-rw-r--r--   0     1001      123    30609 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/simple_api.rs
+-rw-r--r--   0     1001      123     8182 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/track_attributes.rs
+-rw-r--r--   0     1001      123     2640 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/visual_sort_py.rs
+-rw-r--r--   0     1001      123     7537 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort/voting.rs
+-rw-r--r--   0     1001      123     6418 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers/visual_sort.rs
+-rw-r--r--   0     1001      123      643 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/trackers.rs
+-rw-r--r--   0     1001      123    24289 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/bbox.rs
+-rw-r--r--   0     1001      123     2613 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/clipping/bbox_own_areas.rs
+-rw-r--r--   0     1001      123     1163 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/clipping/clipping_py.rs
+-rw-r--r--   0     1001      123     3374 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/clipping.rs
+-rw-r--r--   0     1001      123    11559 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_box.rs
+-rw-r--r--   0     1001      123    10179 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_point.rs
+-rw-r--r--   0     1001      123     5056 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_point_vec.rs
+-rw-r--r--   0     1001      123     2435 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/kalman.rs
+-rw-r--r--   0     1001      123     2323 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/nms/nms_py.rs
+-rw-r--r--   0     1001      123     5142 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/nms.rs
+-rw-r--r--   0     1001      123       30 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/point.rs
+-rw-r--r--   0     1001      123      612 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils/primitive.rs
+-rw-r--r--   0     1001      123      466 2023-07-27 06:37:19.000000 similari_trackers_rs-0.26.5/src/utils.rs
+-rw-r--r--   0        0        0    16190 1970-01-01 00:00:00.000000 similari_trackers_rs-0.26.5/PKG-INFO
```

### Comparing `similari_trackers_rs-0.26.4/Cargo.toml` & `similari_trackers_rs-0.26.5/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,45 +3,54 @@
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Machine learning framework for building object trackers and similarity search engines"
 homepage = "https://github.com/insight-platform/Similari"
 repository = "https://github.com/insight-platform/Similari"
 readme = "README.md"
 keywords = ["machine-learning", "similarity", "tracking", "SORT", "DeepSORT"]
 categories = ["algorithms", "data-structures", "computer-vision", "science"]
-version = "0.26.4"
+version = "0.26.5"
 edition = "2021"
 license="Apache-2.0"
 rust-version = "1.66"
 
 [lib]
 crate-type = ["cdylib", "lib"]
 name = "similari"
 
+[features]
+default = ["python"]
+python = ["dep:pyo3", "dep:pyo3-build-config","dep:pyo3-log"]
+
 [dependencies]
 itertools = "0.10"
 anyhow = "1.0"
 thiserror = "1.0"
 once_cell = "1.17"
 num_cpus = "1.15"
 ultraviolet = "0.9"
 crossbeam = "0.8"
 rand = "0.8"
 log = "0.4"
 nalgebra = "0.32"
-pathfinding = "4.2"
-geo = "0.23"
+pathfinding = "4.3"
+geo = "0.25"
 rayon = "1.7"
 env_logger = "0.10"
 
 [dependencies.pyo3]
 version = "0.18"
 features = ["extension-module"]
+optional = true
+
+[dependencies.pyo3-log]
+version = "0.8"
+optional = true
 
 [build-dependencies]
-pyo3-build-config = "0.18"
+pyo3-build-config = { version = "0.18", optional = true }
 
 [dev-dependencies]
 wide = "0.7"
 
 [profile.dev]
 opt-level = 3
```

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_10.yml` & `similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_10.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_11.yml` & `similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_11.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_8.yml` & `similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_8.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-python-3_9.yml` & `similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-python-3_9.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/docker-maturin-rust-1_67.yml` & `similari_trackers_rs-0.26.5/.github/workflows/docker-maturin-rust-1_67.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/.github/workflows/maturin.yml` & `similari_trackers_rs-0.26.5/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/Cargo.lock` & `similari_trackers_rs-0.26.5/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "accurate"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f209f0bc218ee6cf50db56ec0d9fe10b3cbfb6f3900d019b36c8fdb6d3bc03e"
-dependencies = [
- "cfg-if",
- "ieee754",
- "num-traits",
-]
-
-[[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "arc-swap"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+
+[[package]]
 name = "atomic-polyfill"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
 dependencies = [
  "critical-section",
 ]
@@ -55,14 +50,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "byteorder"
@@ -121,22 +122,22 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -144,26 +145,36 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "earcutr"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0812b44697951d35fde8fcb0da81c9de7e809e825a66bbf1ecb79d9829d4ca3d"
+dependencies = [
+ "itertools",
+ "num-traits",
+]
+
+[[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "env_logger"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
 dependencies = [
@@ -178,15 +189,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -199,63 +210,60 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "float_next_after"
-version = "0.1.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fc612c5837986b7104a87a0df74a5460931f1c5274be12f8d0f40aa2f30d632"
-dependencies = [
- "num-traits",
-]
+checksum = "8bf7cc16383c4b8d58b9905a8509f02926ce3058053c056376248d958c9df1e8"
 
 [[package]]
 name = "geo"
-version = "0.23.1"
+version = "0.25.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b39f57e9624b1a17ce621375464e9878c705d0aaadaf25cb44e4e0005a16de2f"
+checksum = "a5d07d2288645058f3c78bc64eadd615335791cd5adb632e9865840afbc13dad"
 dependencies = [
+ "earcutr",
  "float_next_after",
  "geo-types",
  "geographiclib-rs",
  "log",
  "num-traits",
  "robust",
  "rstar",
 ]
 
 [[package]]
 name = "geo-types"
-version = "0.7.9"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5f0b3068e1537a4b861ec3734f4aa9c317d537cf0845bf6fb6221973499d26c"
+checksum = "9705398c5c7b26132e74513f4ee7c1d7dafd786004991b375c172be2be0eecaa"
 dependencies = [
  "approx",
  "num-traits",
  "rstar",
  "serde",
 ]
 
 [[package]]
 name = "geographiclib-rs"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ea804e7bd3c6a4ca6a01edfa35231557a8a81d4d3f3e1e2b650d028c42592be"
 dependencies = [
- "accurate",
  "lazy_static",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -284,40 +292,25 @@
  "rustc_version",
  "spin",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
-name = "ieee754"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9007da9cacbd3e6343da136e98b0d2df013f553d35bdec8b518f07bea768e19c"
-
-[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -335,34 +328,22 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "276ec31bcb4a9ee45f58bec6f9ec700ae4cf4f4f8f2fa7e06cb406bd5ffdd770"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
-dependencies = [
- "hermit-abi 0.3.1",
- "libc",
- "windows-sys 0.48.0",
-]
-
-[[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
+ "hermit-abi",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -374,45 +355,45 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
@@ -432,34 +413,43 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "nalgebra"
-version = "0.32.2"
+version = "0.32.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d68d47bba83f9e2006d117a9a33af1524e655516b8919caac694427a6fb1e511"
+checksum = "307ed9b18cc2423f29e83f84fd23a8e73628727990181f18641a8b5dc2ab1caa"
 dependencies = [
  "approx",
  "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
  "simba",
  "typenum",
 ]
 
 [[package]]
 name = "nalgebra-macros"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d232c68884c0c99810a5a4d333ef7e47689cfd0edc85efc9e54e1e6bf5212766"
+checksum = "91761aed67d03ad966ef783ae962ef9bbaca728d2dd7ceb7939ec110fffad998"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -490,66 +480,66 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pathfinding"
 version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc597cf0c06c15bcca90fba95ee81b3a80a934403562001d0ed7d8626f7c6ae"
 dependencies = [
@@ -565,31 +555,31 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -610,14 +600,25 @@
 checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
@@ -634,17 +635,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -701,49 +702,61 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "robust"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5864e7ef1a6b7bcf1d6ca3f655e65e724ed3b52546a0d0a663c991522f552ea"
 
 [[package]]
 name = "rstar"
-version = "0.9.3"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b40f1bfe5acdab44bc63e6699c28b74f75ec43afb59f3eda01e145aff86a25fa"
+checksum = "1f39465655a1e3d8ae79c6d9e007f4953bfc5d55297602df9dc38f9ae9f1359a"
 dependencies = [
  "heapless",
  "num-traits",
  "smallvec",
 ]
 
 [[package]]
@@ -759,65 +772,64 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
- "bitflags",
+ "bitflags 2.3.3",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "safe_arch"
-version = "0.6.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.176"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "76dc28c9523c5d70816e393136b86d48909cfb27cecaa902d338c19ed47164dc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.176"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "a4e7b8c5dc823e3b90651ff1d3808419cd14e5ad76de04feaf37da114e7a306f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
@@ -827,40 +839,41 @@
  "num-traits",
  "paste",
  "wide",
 ]
 
 [[package]]
 name = "similari-trackers-rs"
-version = "0.26.4"
+version = "0.26.5"
 dependencies = [
  "anyhow",
  "crossbeam",
  "env_logger",
  "geo",
  "itertools",
  "log",
  "nalgebra",
  "num_cpus",
  "once_cell",
  "pathfinding",
  "pyo3",
  "pyo3-build-config",
+ "pyo3-log",
  "rand",
  "rayon",
  "thiserror",
  "ultraviolet",
  "wide",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
@@ -882,56 +895,56 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
@@ -943,17 +956,17 @@
 checksum = "ca0b28b9a6ce66d47e3c5666aa738c5ec5223fcdd4c263f3edc98ab6fef618b3"
 dependencies = [
  "wide",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -961,17 +974,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.9"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cd0496a71f3cc6bc4bf0ed91346426a5099e93d89807e663162dc5a1069ff65"
+checksum = "aa469ffa65ef7e0ba0f164183697b89b854253fd31aeb92358b7b6155177d62f"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1002,136 +1015,70 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `similari_trackers_rs-0.26.4/LICENSE` & `similari_trackers_rs-0.26.5/LICENSE`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/README.md` & `similari_trackers_rs-0.26.5/README.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/assets/benchmarks/benchmarks.md` & `similari_trackers_rs-0.26.5/assets/benchmarks/benchmarks.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/assets/documentation/python/api.md` & `similari_trackers_rs-0.26.5/assets/documentation/python/api.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/batch_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.5/benches/batch_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/batch_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.5/benches/batch_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/bbox_own_areas.rs` & `similari_trackers_rs-0.26.5/benches/bbox_own_areas.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/feature_tracker.rs` & `similari_trackers_rs-0.26.5/benches/feature_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/kalman_2d_point.rs` & `similari_trackers_rs-0.26.5/benches/kalman_2d_point.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/kalman_bbox.rs` & `similari_trackers_rs-0.26.5/benches/kalman_bbox.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/nms.rs` & `similari_trackers_rs-0.26.5/benches/nms.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/nms_oriented.rs` & `similari_trackers_rs-0.26.5/benches/nms_oriented.rs`

 * *Files 6% similar despite different names*

```diff
@@ -43,12 +43,12 @@
     }
 
     b.iter(|| {
         let mut observations = Vec::new();
         for (indx, i) in iterators.iter_mut().enumerate() {
             let b = i.next();
             let bb: Universal2DBox = b.unwrap().into();
-            observations.push((bb.rotate(indx as f32 / 10.0).gen_vertices(), None));
+            observations.push((bb.rotate(indx as f32 / 10.0).gen_vertices().clone(), None));
         }
-        nms(&observations, 0.8, None);
+        nms(observations.as_slice(), 0.8, None);
     });
 }
```

### Comparing `similari_trackers_rs-0.26.4/benches/simple_search.rs` & `similari_trackers_rs-0.26.5/benches/simple_search.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.5/benches/simple_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/simple_sort_iou_tracker_oriented.rs` & `similari_trackers_rs-0.26.5/benches/simple_sort_iou_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.5/benches/simple_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/simple_sort_maha_tracker_oriented.rs` & `similari_trackers_rs-0.26.5/benches/simple_sort_maha_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/simple_visual_sort_tracker.rs` & `similari_trackers_rs-0.26.5/benches/simple_visual_sort_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/benches/track_search.rs` & `similari_trackers_rs-0.26.5/benches/track_search.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/docker/python_3.10/Dockerfile` & `similari_trackers_rs-0.26.5/docker/python_3.10/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/docker/python_3.11/Dockerfile` & `similari_trackers_rs-0.26.5/docker/python_3.11/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/docker/python_3.8/Dockerfile` & `similari_trackers_rs-0.26.5/docker/python_3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/docker/python_3.9/Dockerfile` & `similari_trackers_rs-0.26.5/docker/python_3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/docker/rust_1.67/Dockerfile` & `similari_trackers_rs-0.26.5/docker/rust_1.67/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/batch_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.5/examples/batch_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/incremental_track_build.rs` & `similari_trackers_rs-0.26.5/examples/incremental_track_build.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/middleware_sort_tracker.rs` & `similari_trackers_rs-0.26.5/examples/middleware_sort_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/simple.rs` & `similari_trackers_rs-0.26.5/examples/simple.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker.rs` & `similari_trackers_rs-0.26.5/examples/simple_sort_iou_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/simple_sort_iou_tracker_oriented.rs` & `similari_trackers_rs-0.26.5/examples/simple_sort_iou_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker.rs` & `similari_trackers_rs-0.26.5/examples/simple_sort_maha_tracker.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/simple_sort_maha_tracker_oriented.rs` & `similari_trackers_rs-0.26.5/examples/simple_sort_maha_tracker_oriented.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/examples/track_merging.rs` & `similari_trackers_rs-0.26.5/examples/track_merging.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bb.py` & `similari_trackers_rs-0.26.5/python/bb.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/bug_visual_sort.py` & `similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/bug_visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json` & `similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_1.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json` & `similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/fixed-1/bug_vs_2.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-1.json` & `similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/in-1.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/bug_vs_1/in/in-2.json` & `similari_trackers_rs-0.26.5/python/bugfixes/bug_vs_1/in/in-2.json`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/bugfixes/github-84.py` & `similari_trackers_rs-0.26.5/python/bugfixes/github-84.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/clipping_intersection.py` & `similari_trackers_rs-0.26.5/python/clipping_intersection.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/kalman_bbox.py` & `similari_trackers_rs-0.26.5/python/kalman_bbox.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/Dockerfile` & `similari_trackers_rs-0.26.5/python/motchallenge/Dockerfile`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/README.md` & `similari_trackers_rs-0.26.5/python/motchallenge/README.md`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/__main__.py` & `similari_trackers_rs-0.26.5/python/motchallenge/__main__.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/config.py` & `similari_trackers_rs-0.26.5/python/motchallenge/config.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/config.yml` & `similari_trackers_rs-0.26.5/python/motchallenge/config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/confs/original-sort-config.yml` & `similari_trackers_rs-0.26.5/python/motchallenge/confs/original-sort-config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/confs/similari-maha-sort-config.yml` & `similari_trackers_rs-0.26.5/python/motchallenge/confs/similari-maha-sort-config.yml`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/evaluator.py` & `similari_trackers_rs-0.26.5/python/motchallenge/evaluator.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/trackers.py` & `similari_trackers_rs-0.26.5/python/motchallenge/trackers.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/motchallenge/utils.py` & `similari_trackers_rs-0.26.5/python/motchallenge/utils.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/nms.py` & `similari_trackers_rs-0.26.5/python/nms.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/batch_sort_iou.py` & `similari_trackers_rs-0.26.5/python/sort/batch_sort_iou.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/batch_sort_iou_bench.py` & `similari_trackers_rs-0.26.5/python/sort/batch_sort_iou_bench.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_idle.py` & `similari_trackers_rs-0.26.5/python/sort/sort_idle.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_iou.py` & `similari_trackers_rs-0.26.5/python/sort/sort_iou.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_iou_bench.py` & `similari_trackers_rs-0.26.5/python/sort/sort_iou_bench.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_iou_rotated.py` & `similari_trackers_rs-0.26.5/python/sort/sort_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_iou_scene_id.py` & `similari_trackers_rs-0.26.5/python/sort/sort_iou_scene_id.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/sort/sort_maha.py` & `similari_trackers_rs-0.26.5/python/sort/sort_maha.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/visual_sort/batch_visual_sort.py` & `similari_trackers_rs-0.26.5/python/visual_sort/batch_visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/python/visual_sort/visual_sort.py` & `similari_trackers_rs-0.26.5/python/visual_sort/visual_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     opts.visual_max_observations(25)
     opts.visual_min_votes(5)
     return opts
 
 tracker = VisualSort(shards=1, opts=get_opts())
 
 
+assert False
 
 # let's say frame_objs is a list of objs detected in a frame
 for frame_objs in frames:
     # for each set of detected objects
     # a VisualSortObservationSet object needs to be initialized
     # and filled with VisualSortObservation structures
     observation_set = VisualSortObservationSet()
```

### Comparing `similari_trackers_rs-0.26.4/python/visual_sort.py` & `similari_trackers_rs-0.26.5/python/visual_sort.py`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/distance.rs` & `similari_trackers_rs-0.26.5/src/distance.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/examples/iou.rs` & `similari_trackers_rs-0.26.5/src/examples/iou.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/examples.rs` & `similari_trackers_rs-0.26.5/src/examples.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/lib.rs` & `similari_trackers_rs-0.26.5/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -75,28 +75,31 @@
     /// Index is out of range
     #[error("The index is out of range")]
     OutOfRange,
 }
 
 pub const EPS: f32 = 0.00001;
 
+#[cfg(feature = "python")]
 mod python {
-    use crate::prelude::{
-        BatchSort, BoundingBox, Sort, SortTrack, SpatioTemporalConstraints, Universal2DBox,
-        VisualSort, VisualSortOptions,
+    use crate::trackers::batch::python::PyPredictionBatchResult;
+    use crate::trackers::sort::batch_api::python::{PyBatchSort, PySortPredictionBatchRequest};
+    use crate::trackers::sort::python::{PyPositionalMetricType, PySortTrack, PyWastedSortTrack};
+    use crate::trackers::sort::simple_api::python::PySort;
+    use crate::trackers::spatio_temporal_constraints::python::PySpatioTemporalConstraints;
+    use crate::trackers::visual_sort::batch_api::python::{
+        PyBatchVisualSort, PyVisualSortPredictionBatchRequest,
     };
-    use crate::trackers::batch::PredictionBatchResult;
-    use crate::trackers::sort::sort_py::PySortPredictionBatchRequest;
-    use crate::trackers::sort::{PyPositionalMetricType, PyWastedSortTrack};
-    use crate::trackers::visual_sort::batch_api::BatchVisualSort;
-    use crate::trackers::visual_sort::metric::PyVisualSortMetricType;
-    use crate::trackers::visual_sort::visual_sort_py::{
-        PyVisualSortObservation, PyVisualSortObservationSet, PyVisualSortPredictionBatchRequest,
+    use crate::trackers::visual_sort::metric::python::PyVisualSortMetricType;
+    use crate::trackers::visual_sort::options::python::PyVisualSortOptions;
+    use crate::trackers::visual_sort::python::{
+        PyVisualSortObservation, PyVisualSortObservationSet, PyWastedVisualSortTrack,
     };
-    use crate::trackers::visual_sort::PyWastedVisualSortTrack;
+    use crate::trackers::visual_sort::simple_api::python::PyVisualSort;
+    use crate::utils::bbox::python::{PyBoundingBox, PyUniversal2DBox};
     use crate::utils::clipping::clipping_py::{
         intersection_area_py, sutherland_hodgman_clip_py, PyPolygon,
     };
     use crate::utils::kalman::kalman_2d_box::python::{
         PyUniversal2DBoxKalmanFilter, PyUniversal2DBoxKalmanFilterState,
     };
     use crate::utils::kalman::kalman_2d_point::python::{
@@ -110,50 +113,49 @@
     pub fn version() -> String {
         env!("CARGO_PKG_VERSION").to_string()
     }
 
     #[pymodule]
     #[pyo3(name = "similari")]
     fn similari(_py: Python, m: &PyModule) -> PyResult<()> {
-        let _ = env_logger::try_init();
+        pyo3_log::init();
 
-        m.add_class::<BoundingBox>()?;
-        m.add_class::<Universal2DBox>()?;
+        m.add_class::<PyBoundingBox>()?;
+        m.add_class::<PyUniversal2DBox>()?;
         m.add_class::<PyPolygon>()?;
-        m.add_class::<SortTrack>()?;
+        m.add_class::<PySortTrack>()?;
         m.add_class::<PyWastedSortTrack>()?;
 
         m.add_class::<PyUniversal2DBoxKalmanFilterState>()?;
         m.add_class::<PyUniversal2DBoxKalmanFilter>()?;
 
         m.add_class::<PyPoint2DKalmanFilterState>()?;
         m.add_class::<PyPoint2DKalmanFilter>()?;
 
         m.add_class::<PyVec2DKalmanFilter>()?;
 
         m.add_class::<PySortPredictionBatchRequest>()?;
-        m.add_class::<SpatioTemporalConstraints>()?;
-        m.add_class::<Sort>()?;
+        m.add_class::<PySpatioTemporalConstraints>()?;
+        m.add_class::<PySort>()?;
 
         m.add_class::<PyPositionalMetricType>()?;
         m.add_class::<PyVisualSortMetricType>()?;
-        m.add_class::<VisualSortOptions>()?;
+        m.add_class::<PyVisualSortOptions>()?;
         m.add_class::<PyVisualSortObservation>()?;
         m.add_class::<PyVisualSortObservationSet>()?;
         m.add_class::<PyVisualSortPredictionBatchRequest>()?;
         m.add_class::<PyWastedVisualSortTrack>()?;
-        m.add_class::<VisualSort>()?;
+        m.add_class::<PyVisualSort>()?;
 
-        m.add_class::<PredictionBatchResult>()?;
+        m.add_class::<PyPredictionBatchResult>()?;
 
         m.add_class::<PySortPredictionBatchRequest>()?;
-        m.add_class::<BatchSort>()?;
+        m.add_class::<PyBatchSort>()?;
 
-        m.add_class::<PyVisualSortPredictionBatchRequest>()?;
-        m.add_class::<BatchVisualSort>()?;
+        m.add_class::<PyBatchVisualSort>()?;
 
         m.add_function(wrap_pyfunction!(version, m)?)?;
         m.add_function(wrap_pyfunction!(nms_py, m)?)?;
         m.add_function(wrap_pyfunction!(sutherland_hodgman_clip_py, m)?)?;
         m.add_function(wrap_pyfunction!(intersection_area_py, m)?)?;
         Ok(())
     }
```

### Comparing `similari_trackers_rs-0.26.4/src/prelude.rs` & `similari_trackers_rs-0.26.5/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/builder.rs` & `similari_trackers_rs-0.26.5/src/track/builder.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/store/builder.rs` & `similari_trackers_rs-0.26.5/src/track/store/builder.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/store/store_tests.rs` & `similari_trackers_rs-0.26.5/src/track/store/store_tests.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/store/track_distance.rs` & `similari_trackers_rs-0.26.5/src/track/store/track_distance.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/store.rs` & `similari_trackers_rs-0.26.5/src/track/store.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/utils.rs` & `similari_trackers_rs-0.26.5/src/track/utils.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/voting/best.rs` & `similari_trackers_rs-0.26.5/src/track/voting/best.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/voting/topn.rs` & `similari_trackers_rs-0.26.5/src/track/voting/topn.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track/voting.rs` & `similari_trackers_rs-0.26.5/src/track/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/track.rs` & `similari_trackers_rs-0.26.5/src/track.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/batch.rs` & `similari_trackers_rs-0.26.5/src/trackers/batch.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,74 @@
 use crate::prelude::SortTrack;
 use crossbeam::channel::{Receiver, Sender};
 use log::debug;
-use pyo3::prelude::*;
+
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 pub type BatchRecords<T> = HashMap<u64, Vec<T>>;
 pub type SceneTracks = (u64, Vec<SortTrack>);
 
 #[derive(Debug, Clone)]
 pub struct PredictionBatchRequest<T> {
     batch: BatchRecords<T>,
     sender: Sender<SceneTracks>,
     batch_size: Arc<Mutex<usize>>,
 }
 
-#[pyclass]
 #[derive(Clone, Debug)]
 pub struct PredictionBatchResult {
     receiver: Receiver<SceneTracks>,
     batch_size: Arc<Mutex<usize>>,
 }
 
-#[pymethods]
 impl PredictionBatchResult {
     pub fn ready(&self) -> bool {
         !self.receiver.is_empty()
     }
 
-    #[pyo3(name = "get", signature = ())]
-    fn get_py(&self) -> SceneTracks {
-        Python::with_gil(|py| py.allow_threads(|| self.get()))
+    pub fn get(&self) -> SceneTracks {
+        self.receiver
+            .recv()
+            .expect("Receiver must always receive batch computation result")
     }
 
     pub fn batch_size(&self) -> usize {
         *self.batch_size.lock().unwrap()
     }
 }
 
-impl PredictionBatchResult {
-    pub fn get(&self) -> SceneTracks {
-        self.receiver
-            .recv()
-            .expect("Receiver must always receive batch computation result")
+#[cfg(feature = "python")]
+pub mod python {
+    use crate::trackers::sort::python::PySortTrack;
+
+    use super::PredictionBatchResult;
+    use pyo3::prelude::*;
+
+    pub type PySceneTracks = (u64, Vec<PySortTrack>);
+
+    #[pyclass]
+    #[derive(Clone, Debug)]
+    #[pyo3(name = "PredictionBatchResult")]
+    pub struct PyPredictionBatchResult(pub(crate) PredictionBatchResult);
+
+    #[pymethods]
+    impl PyPredictionBatchResult {
+        pub fn ready(&self) -> bool {
+            self.0.ready()
+        }
+
+        #[pyo3(signature = ())]
+        fn get(&self) -> PySceneTracks {
+            Python::with_gil(|py| py.allow_threads(|| unsafe { std::mem::transmute(self.0.get()) }))
+        }
+
+        pub fn batch_size(&self) -> usize {
+            self.0.batch_size()
+        }
     }
 }
 
 impl<T> PredictionBatchRequest<T> {
     pub fn get_sender(&self) -> Sender<SceneTracks> {
         self.sender.clone()
     }
@@ -108,16 +130,15 @@
 
     #[test]
     fn test() {
         let (mut request, result) = PredictionBatchRequest::<Universal2DBox>::new();
         request.add(0, Universal2DBox::new(0.0, 0.0, Some(0.5), 1.0, 5.0));
         request.add(0, Universal2DBox::new(5.0, 5.0, Some(0.0), 1.5, 10.0));
         request.add(1, Universal2DBox::new(0.0, 0.0, Some(1.0), 0.7, 5.1));
-        let batch = request.get_batch();
-        drop(batch);
+        let _batch = request.get_batch();
         assert_eq!(result.batch_size(), 2);
 
         assert!(request.send((0, vec![])));
         assert_eq!(result.ready(), true);
         let res = result.get();
         assert_eq!(res.0, 0);
         assert!(res.1.is_empty());
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/epoch_db.rs` & `similari_trackers_rs-0.26.5/src/trackers/epoch_db.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/kalman_prediction.rs` & `similari_trackers_rs-0.26.5/src/trackers/kalman_prediction.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/sort/batch_api.rs` & `similari_trackers_rs-0.26.5/src/trackers/sort/batch_api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 };
 use crate::store::track_distance::TrackDistanceOkIterator;
 use crate::store::TrackStore;
 use crate::track::Track;
 use crate::trackers::batch::{PredictionBatchRequest, PredictionBatchResult, SceneTracks};
 use crate::trackers::epoch_db::EpochDb;
 use crate::trackers::sort::metric::SortMetric;
-use crate::trackers::sort::sort_py::PySortPredictionBatchRequest;
 use crate::trackers::sort::voting::SortVoting;
 use crate::trackers::sort::{
-    AutoWaste, PyPositionalMetricType, PyWastedSortTrack, SortAttributes, SortAttributesOptions,
-    SortAttributesUpdate, SortLookup, DEFAULT_AUTO_WASTE_PERIODICITY,
-    MAHALANOBIS_NEW_TRACK_THRESHOLD,
+    AutoWaste, SortAttributes, SortAttributesOptions, SortAttributesUpdate, SortLookup,
+    DEFAULT_AUTO_WASTE_PERIODICITY, MAHALANOBIS_NEW_TRACK_THRESHOLD,
 };
+
 use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
 use crate::trackers::tracker_api::TrackerAPI;
 use crate::voting::Voting;
 use crossbeam::channel::{Receiver, Sender};
 use log::warn;
-use pyo3::prelude::*;
 use rand::Rng;
 use std::collections::HashMap;
 use std::mem;
 use std::sync::{Arc, Condvar, Mutex, RwLock, RwLockReadGuard, RwLockWriteGuard};
 use std::thread::{spawn, JoinHandle};
 
 type VotingSenderChannel = Sender<VotingCommands>;
@@ -41,15 +39,14 @@
         channel: Sender<SceneTracks>,
         tracks: Vec<MiddlewareSortTrack>,
         monitor: BatchBusyMonitor,
     },
     Exit,
 }
 
-#[pyclass]
 pub struct BatchSort {
     monitor: Option<BatchBusyMonitor>,
     store: Arc<RwLock<MiddlewareSortTrackStore>>,
     wasted_store: RwLock<MiddlewareSortTrackStore>,
     opts: Arc<SortAttributesOptions>,
     voting_threads: Vec<(VotingSenderChannel, JoinHandle<()>)>,
     auto_waste: AutoWaste,
@@ -330,14 +327,219 @@
     }
 
     fn get_wasted_store(&self) -> RwLockReadGuard<MiddlewareSortTrackStore> {
         self.wasted_store.read().unwrap()
     }
 }
 
+#[derive(Debug, Clone)]
+pub struct SortPredictionBatchRequest {
+    pub batch: PredictionBatchRequest<(Universal2DBox, Option<i64>)>,
+    pub result: Option<PredictionBatchResult>,
+}
+
+impl SortPredictionBatchRequest {
+    pub fn new() -> Self {
+        let (batch, result) = PredictionBatchRequest::new();
+
+        Self {
+            batch,
+            result: Some(result),
+        }
+    }
+
+    pub fn add(&mut self, scene_id: u64, bbox: Universal2DBox, custom_object_id: Option<i64>) {
+        self.batch.add(scene_id, (bbox, custom_object_id))
+    }
+}
+
+impl Default for SortPredictionBatchRequest {
+    fn default() -> Self {
+        Self::new()
+    }
+}
+
+#[cfg(feature = "python")]
+pub mod python {
+    use crate::{
+        trackers::{
+            batch::python::PyPredictionBatchResult,
+            sort::{
+                python::{PyPositionalMetricType, PySortTrack, PyWastedSortTrack},
+                WastedSortTrack,
+            },
+            spatio_temporal_constraints::python::PySpatioTemporalConstraints,
+            tracker_api::TrackerAPI,
+        },
+        utils::bbox::python::PyUniversal2DBox,
+    };
+
+    use super::{BatchSort, SortPredictionBatchRequest};
+    use pyo3::prelude::*;
+
+    #[pyclass]
+    #[pyo3(name = "BatchSort")]
+    pub struct PyBatchSort(pub(crate) BatchSort);
+
+    #[pymethods]
+    impl PyBatchSort {
+        #[new]
+        #[pyo3(signature = (
+        distance_shards = 4,
+        voting_shards = 4,
+        bbox_history = 1,
+        max_idle_epochs = 5,
+        method = None,
+        min_confidence = 0.05,
+        spatio_temporal_constraints = None,
+    ))]
+        pub fn new(
+            distance_shards: i64,
+            voting_shards: i64,
+            bbox_history: i64,
+            max_idle_epochs: i64,
+            method: Option<PyPositionalMetricType>,
+            min_confidence: f32,
+            spatio_temporal_constraints: Option<PySpatioTemporalConstraints>,
+        ) -> Self {
+            Self(BatchSort::new(
+                distance_shards
+                    .try_into()
+                    .expect("Positive number expected"),
+                voting_shards.try_into().expect("Positive number expected"),
+                bbox_history.try_into().expect("Positive number expected"),
+                max_idle_epochs
+                    .try_into()
+                    .expect("Positive number expected"),
+                method.unwrap_or(PyPositionalMetricType::maha()).0,
+                min_confidence,
+                spatio_temporal_constraints.map(|x| x.0),
+            ))
+        }
+
+        #[pyo3(signature = (n))]
+        fn skip_epochs(&mut self, n: i64) {
+            assert!(n > 0);
+            self.0.skip_epochs(n.try_into().unwrap())
+        }
+
+        #[pyo3(signature = (scene_id, n))]
+        fn skip_epochs_for_scene(&mut self, scene_id: i64, n: i64) {
+            assert!(n > 0 && scene_id >= 0);
+            self.0
+                .skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
+        }
+
+        /// Get the amount of stored tracks per shard
+        ///
+        #[pyo3(signature = ())]
+        fn shard_stats(&self) -> Vec<i64> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .store
+                        .read()
+                        .unwrap()
+                        .shard_stats()
+                        .into_iter()
+                        .map(|e| i64::try_from(e).unwrap())
+                        .collect()
+                })
+            })
+        }
+
+        /// Get the current epoch for `scene_id` == 0
+        ///
+        #[pyo3(signature = ())]
+        fn current_epoch(&self) -> i64 {
+            self.0.current_epoch_with_scene(0).try_into().unwrap()
+        }
+
+        /// Get the current epoch for `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id
+        ///
+        #[pyo3(
+        signature = (scene_id)
+    )]
+        fn current_epoch_with_scene(&self, scene_id: i64) -> isize {
+            assert!(scene_id >= 0);
+            self.0
+                .current_epoch_with_scene(scene_id.try_into().unwrap())
+                .try_into()
+                .unwrap()
+        }
+
+        /// Receive tracking information for observed bboxes of `scene_id` == 0
+        ///
+        /// # Parameters
+        /// * `bboxes` - bounding boxes received from a detector
+        ///
+        #[pyo3(signature = (batch))]
+        fn predict(&mut self, mut batch: PySortPredictionBatchRequest) -> PyPredictionBatchResult {
+            self.0.predict(batch.0.batch);
+            PyPredictionBatchResult(batch.0.result.take().unwrap())
+        }
+
+        /// Remove all the tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        fn wasted(&mut self) -> Vec<PyWastedSortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .wasted()
+                        .into_iter()
+                        .map(WastedSortTrack::from)
+                        .map(PyWastedSortTrack)
+                        .collect()
+                })
+            })
+        }
+
+        /// Clear all tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn clear_wasted(&mut self) {
+            Python::with_gil(|py| {
+                py.allow_threads(|| self.0.clear_wasted());
+            })
+        }
+
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn idle_tracks(&mut self, scene_id: i64) -> Vec<PySortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(self.0.idle_tracks_with_scene(scene_id.try_into().unwrap()))
+                })
+            })
+        }
+    }
+
+    #[pyclass]
+    #[pyo3(name = "SortPredictionBatchRequest")]
+    #[derive(Debug, Clone)]
+    pub struct PySortPredictionBatchRequest(pub(crate) SortPredictionBatchRequest);
+
+    #[pymethods]
+    impl PySortPredictionBatchRequest {
+        #[new]
+        fn new() -> Self {
+            Self(SortPredictionBatchRequest::new())
+        }
+
+        fn add(&mut self, scene_id: u64, bbox: PyUniversal2DBox, custom_object_id: Option<i64>) {
+            self.0.add(scene_id, bbox.0, custom_object_id)
+        }
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use crate::prelude::BoundingBox;
     use crate::prelude::PositionalMetricType::Mahalanobis;
     use crate::trackers::batch::PredictionBatchRequest;
     use crate::trackers::sort::batch_api::BatchSort;
     use crate::trackers::sort::metric::DEFAULT_MINIMAL_SORT_CONFIDENCE;
@@ -361,142 +563,7 @@
 
         for _ in 0..res.batch_size() {
             let data = res.get();
             dbg!(data);
         }
     }
 }
-
-#[pymethods]
-impl BatchSort {
-    #[new]
-    #[pyo3(signature = (
-        distance_shards = 4,
-        voting_shards = 4,
-        bbox_history = 1,
-        max_idle_epochs = 5,
-        method = None,
-        min_confidence = 0.05,
-        spatio_temporal_constraints = None,
-    ))]
-    pub fn new_py(
-        distance_shards: i64,
-        voting_shards: i64,
-        bbox_history: i64,
-        max_idle_epochs: i64,
-        method: Option<PyPositionalMetricType>,
-        min_confidence: f32,
-        spatio_temporal_constraints: Option<SpatioTemporalConstraints>,
-    ) -> Self {
-        Self::new(
-            distance_shards
-                .try_into()
-                .expect("Positive number expected"),
-            voting_shards.try_into().expect("Positive number expected"),
-            bbox_history.try_into().expect("Positive number expected"),
-            max_idle_epochs
-                .try_into()
-                .expect("Positive number expected"),
-            method.unwrap_or(PyPositionalMetricType::maha()).0,
-            min_confidence,
-            spatio_temporal_constraints,
-        )
-    }
-
-    #[pyo3(name = "skip_epochs", signature = (n))]
-    fn skip_epochs_py(&mut self, n: i64) {
-        assert!(n > 0);
-        self.skip_epochs(n.try_into().unwrap())
-    }
-
-    #[pyo3(
-        name = "skip_epochs_for_scene",
-        signature = (scene_id, n)
-    )]
-    fn skip_epochs_for_scene_py(&mut self, scene_id: i64, n: i64) {
-        assert!(n > 0 && scene_id >= 0);
-        self.skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
-    }
-
-    /// Get the amount of stored tracks per shard
-    ///
-    #[pyo3(name = "shard_stats", signature = ())]
-    fn shard_stats_py(&self) -> Vec<i64> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.store
-                    .read()
-                    .unwrap()
-                    .shard_stats()
-                    .into_iter()
-                    .map(|e| i64::try_from(e).unwrap())
-                    .collect()
-            })
-        })
-    }
-
-    /// Get the current epoch for `scene_id` == 0
-    ///
-    #[pyo3(name = "current_epoch", signature = ())]
-    fn current_epoch_py(&self) -> i64 {
-        self.current_epoch_with_scene(0).try_into().unwrap()
-    }
-
-    /// Get the current epoch for `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id
-    ///
-    #[pyo3(
-        name = "current_epoch_with_scene",
-        signature = (scene_id)
-    )]
-    fn current_epoch_with_scene_py(&self, scene_id: i64) -> isize {
-        assert!(scene_id >= 0);
-        self.current_epoch_with_scene(scene_id.try_into().unwrap())
-            .try_into()
-            .unwrap()
-    }
-
-    /// Receive tracking information for observed bboxes of `scene_id` == 0
-    ///
-    /// # Parameters
-    /// * `bboxes` - bounding boxes received from a detector
-    ///
-    #[pyo3(name = "predict", signature = (batch))]
-    fn predict_py(&mut self, mut batch: PySortPredictionBatchRequest) -> PredictionBatchResult {
-        self.predict(batch.batch);
-        batch.result.take().unwrap()
-    }
-
-    /// Remove all the tracks with expired life
-    ///
-    #[pyo3(name = "wasted", signature = ())]
-    fn wasted_py(&mut self) -> Vec<PyWastedSortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.wasted()
-                    .into_iter()
-                    .map(PyWastedSortTrack::from)
-                    .collect()
-            })
-        })
-    }
-
-    /// Clear all tracks with expired life
-    ///
-    #[pyo3(name = "clear_wasted", signature = ())]
-    pub fn clear_wasted_py(&mut self) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.clear_wasted());
-        })
-    }
-
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks", signature = (scene_id))]
-    pub fn idle_tracks_py(&mut self, scene_id: i64) -> Vec<SortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.idle_tracks_with_scene(scene_id.try_into().unwrap()))
-        })
-    }
-}
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/sort/metric.rs` & `similari_trackers_rs-0.26.5/src/trackers/sort/metric.rs`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,23 @@
         _prev_length: usize,
         _is_merge: bool,
     ) -> anyhow::Result<()> {
         let mut observation = features.pop().unwrap();
         let observation_bbox = observation.attr().as_ref().unwrap();
         features.clear();
 
-        let predicted_bbox = attrs.make_prediction(observation_bbox);
+        let mut predicted_bbox = attrs.make_prediction(observation_bbox);
         attrs.update_history(observation_bbox, &predicted_bbox);
 
         *observation.attr_mut() = Some(match self.method {
             PositionalMetricType::Mahalanobis => predicted_bbox,
-            PositionalMetricType::IoU(_) => predicted_bbox.gen_vertices(),
+            PositionalMetricType::IoU(_) => {
+                predicted_bbox.gen_vertices();
+                predicted_bbox
+            }
         });
 
         features.push(observation);
         Ok(())
     }
 
     fn postprocess_distances(
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/sort/simple_api.rs` & `similari_trackers_rs-0.26.5/src/trackers/sort/simple_api.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 use crate::prelude::{NoopNotifier, ObservationBuilder, TrackStoreBuilder};
 use crate::store::TrackStore;
 use crate::track::Track;
 use crate::trackers::epoch_db::EpochDb;
-use crate::trackers::sort::metric::SortMetric;
-use crate::trackers::sort::voting::SortVoting;
 use crate::trackers::sort::{
-    AutoWaste, PositionalMetricType, PyPositionalMetricType, SortLookup,
+    metric::SortMetric, voting::SortVoting, AutoWaste, PositionalMetricType, SortAttributes,
+    SortAttributesOptions, SortAttributesUpdate, SortLookup, SortTrack, VotingType,
     DEFAULT_AUTO_WASTE_PERIODICITY, MAHALANOBIS_NEW_TRACK_THRESHOLD,
 };
-use crate::trackers::sort::{
-    PyWastedSortTrack, SortAttributes, SortAttributesOptions, SortAttributesUpdate, SortTrack,
-    VotingType,
-};
 use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
 use crate::trackers::tracker_api::TrackerAPI;
 use crate::utils::bbox::Universal2DBox;
 use crate::voting::Voting;
-use pyo3::prelude::*;
 use rand::Rng;
 use std::collections::HashMap;
 use std::sync::{Arc, RwLock, RwLockReadGuard, RwLockWriteGuard};
 
 /// Easy to use SORT tracker implementation
 ///
-#[pyclass(text_signature = "(shards, bbox_history, max_idle_epochs, threshold)")]
 pub struct Sort {
     store: RwLock<TrackStore<SortAttributes, SortMetric, Universal2DBox>>,
     wasted_store: RwLock<TrackStore<SortAttributes, SortMetric, Universal2DBox>>,
     method: PositionalMetricType,
     opts: Arc<SortAttributesOptions>,
     auto_waste: AutoWaste,
     track_id: u64,
@@ -264,30 +257,14 @@
             observed_bbox: attrs.observed_boxes.back().unwrap().clone(),
             predicted_bbox: attrs.predicted_boxes.back().unwrap().clone(),
             length: attrs.track_length,
         }
     }
 }
 
-impl From<Track<SortAttributes, SortMetric, Universal2DBox>> for PyWastedSortTrack {
-    fn from(track: Track<SortAttributes, SortMetric, Universal2DBox>) -> Self {
-        let attrs = track.get_attributes();
-        PyWastedSortTrack {
-            id: track.get_track_id(),
-            epoch: attrs.last_updated_epoch,
-            scene_id: attrs.scene_id,
-            length: attrs.track_length,
-            observed_bbox: attrs.observed_boxes.back().unwrap().clone(),
-            predicted_bbox: attrs.predicted_boxes.back().unwrap().clone(),
-            predicted_boxes: attrs.predicted_boxes.clone().into_iter().collect(),
-            observed_boxes: attrs.observed_boxes.clone().into_iter().collect(),
-        }
-    }
-}
-
 #[cfg(test)]
 mod tests {
     use crate::trackers::sort::metric::DEFAULT_MINIMAL_SORT_CONFIDENCE;
     use crate::trackers::sort::simple_api::Sort;
     use crate::trackers::sort::PositionalMetricType::IoU;
     use crate::trackers::sort::DEFAULT_SORT_IOU_THRESHOLD;
     use crate::trackers::tracker_api::TrackerAPI;
@@ -436,147 +413,189 @@
                 .iter()
                 .sum::<usize>(),
             0
         );
     }
 }
 
-#[pymethods]
-impl Sort {
-    #[new]
-    #[pyo3(signature = (shards=4, bbox_history=1, max_idle_epochs=5, method = None, min_confidence=0.05, spatio_temporal_constraints=None))]
-    pub fn new_py(
-        shards: i64,
-        bbox_history: i64,
-        max_idle_epochs: i64,
-        method: Option<PyPositionalMetricType>,
-        min_confidence: f32,
-        spatio_temporal_constraints: Option<SpatioTemporalConstraints>,
-    ) -> Self {
-        Self::new(
-            shards.try_into().expect("Positive number expected"),
-            bbox_history.try_into().expect("Positive number expected"),
-            max_idle_epochs
-                .try_into()
-                .expect("Positive number expected"),
-            method.unwrap_or(PyPositionalMetricType::maha()).0,
-            min_confidence,
-            spatio_temporal_constraints,
-        )
-    }
+#[cfg(feature = "python")]
+pub mod python {
+    use crate::{
+        prelude::Universal2DBox,
+        trackers::{
+            sort::{
+                python::{PyPositionalMetricType, PySortTrack, PyWastedSortTrack},
+                WastedSortTrack,
+            },
+            spatio_temporal_constraints::python::PySpatioTemporalConstraints,
+            tracker_api::TrackerAPI,
+        },
+        utils::bbox::python::PyUniversal2DBox,
+    };
+
+    use super::Sort;
+    use pyo3::prelude::*;
+
+    #[pyclass(
+        name = "Sort",
+        text_signature = "(shards, bbox_history, max_idle_epochs, threshold)"
+    )]
+    pub struct PySort(pub Sort);
+
+    #[pymethods]
+    impl PySort {
+        #[new]
+        #[pyo3(signature = (shards=4, bbox_history=1, max_idle_epochs=5, method = None, min_confidence=0.05, spatio_temporal_constraints=None))]
+        pub fn new_py(
+            shards: i64,
+            bbox_history: i64,
+            max_idle_epochs: i64,
+            method: Option<PyPositionalMetricType>,
+            min_confidence: f32,
+            spatio_temporal_constraints: Option<PySpatioTemporalConstraints>,
+        ) -> Self {
+            Self(Sort::new(
+                shards.try_into().expect("Positive number expected"),
+                bbox_history.try_into().expect("Positive number expected"),
+                max_idle_epochs
+                    .try_into()
+                    .expect("Positive number expected"),
+                method.unwrap_or(PyPositionalMetricType::maha()).0,
+                min_confidence,
+                spatio_temporal_constraints.map(|x| x.0),
+            ))
+        }
 
-    #[pyo3(name = "skip_epochs", signature = (n))]
-    pub fn skip_epochs_py(&mut self, n: i64) {
-        assert!(n > 0);
-        self.skip_epochs(n.try_into().unwrap())
-    }
+        #[pyo3(signature = (n))]
+        pub fn skip_epochs(&mut self, n: i64) {
+            assert!(n > 0);
+            self.0.skip_epochs(n.try_into().unwrap())
+        }
 
-    #[pyo3(name = "skip_epochs_for_scene", signature = (scene_id, n))]
-    pub fn skip_epochs_for_scene_py(&mut self, scene_id: i64, n: i64) {
-        assert!(n > 0 && scene_id >= 0);
-        self.skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
-    }
+        #[pyo3(signature = (scene_id, n))]
+        pub fn skip_epochs_for_scene(&mut self, scene_id: i64, n: i64) {
+            assert!(n > 0 && scene_id >= 0);
+            self.0
+                .skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
+        }
 
-    /// Get the amount of stored tracks per shard
-    ///
-    #[pyo3(name = "shard_stats", signature = ())]
-    pub fn shard_stats_py(&self) -> Vec<i64> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.store
-                    .read()
-                    .unwrap()
-                    .shard_stats()
-                    .into_iter()
-                    .map(|e| i64::try_from(e).unwrap())
-                    .collect()
+        /// Get the amount of stored tracks per shard
+        ///
+        #[pyo3(signature = ())]
+        pub fn shard_stats(&self) -> Vec<i64> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .store
+                        .read()
+                        .unwrap()
+                        .shard_stats()
+                        .into_iter()
+                        .map(|e| i64::try_from(e).unwrap())
+                        .collect()
+                })
             })
-        })
-    }
+        }
 
-    /// Get the current epoch for `scene_id` == 0
-    ///
-    #[pyo3(name = "current_epoch", signature = ())]
-    pub fn current_epoch_py(&self) -> i64 {
-        self.current_epoch_with_scene(0).try_into().unwrap()
-    }
+        /// Get the current epoch for `scene_id` == 0
+        ///
+        #[pyo3(signature = ())]
+        pub fn current_epoch(&self) -> i64 {
+            self.0.current_epoch_with_scene(0).try_into().unwrap()
+        }
 
-    /// Get the current epoch for `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id
-    ///
-    #[pyo3(name = "current_epoch_with_scene", signature = (scene_id))]
-    pub fn current_epoch_with_scene_py(&self, scene_id: i64) -> isize {
-        assert!(scene_id >= 0);
-        self.current_epoch_with_scene(scene_id.try_into().unwrap())
-            .try_into()
-            .unwrap()
-    }
+        /// Get the current epoch for `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn current_epoch_with_scene(&self, scene_id: i64) -> isize {
+            assert!(scene_id >= 0);
+            self.0
+                .current_epoch_with_scene(scene_id.try_into().unwrap())
+                .try_into()
+                .unwrap()
+        }
 
-    /// Receive tracking information for observed bboxes of `scene_id` == 0
-    ///
-    /// # Parameters
-    /// * `bboxes` - bounding boxes received from a detector
-    ///
-    #[pyo3(name = "predict", signature = (bboxes))]
-    pub fn predict_py(&mut self, bboxes: Vec<(Universal2DBox, Option<i64>)>) -> Vec<SortTrack> {
-        self.predict_with_scene_py(0, bboxes)
-    }
+        /// Receive tracking information for observed bboxes of `scene_id` == 0
+        ///
+        /// # Parameters
+        /// * `bboxes` - bounding boxes received from a detector
+        ///
+        #[pyo3(signature = (bboxes))]
+        pub fn predict(
+            &mut self,
+            bboxes: Vec<(PyUniversal2DBox, Option<i64>)>,
+        ) -> Vec<PySortTrack> {
+            self.predict_with_scene(0, bboxes)
+        }
 
-    /// Receive tracking information for observed bboxes of `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id provided by a user (class, camera id, etc...)
-    /// * `bboxes` - bounding boxes received from a detector
-    ///
-    #[pyo3(name = "predict_with_scene", signature = (scene_id, bboxes))]
-    pub fn predict_with_scene_py(
-        &mut self,
-        scene_id: i64,
-        bboxes: Vec<(Universal2DBox, Option<i64>)>,
-    ) -> Vec<SortTrack> {
-        assert!(scene_id >= 0);
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.predict_with_scene(scene_id.try_into().unwrap(), &bboxes))
-        })
-    }
+        /// Receive tracking information for observed bboxes of `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id provided by a user (class, camera id, etc...)
+        /// * `bboxes` - bounding boxes received from a detector
+        ///
+        #[pyo3(signature = (scene_id, bboxes))]
+        pub fn predict_with_scene(
+            &mut self,
+            scene_id: i64,
+            bboxes: Vec<(PyUniversal2DBox, Option<i64>)>,
+        ) -> Vec<PySortTrack> {
+            assert!(scene_id >= 0);
+            let bboxes: Vec<(Universal2DBox, Option<i64>)> = unsafe { std::mem::transmute(bboxes) };
+
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(
+                        self.0
+                            .predict_with_scene(scene_id.try_into().unwrap(), &bboxes),
+                    )
+                })
+            })
+        }
 
-    /// Fetch and remove all the tracks with expired life
-    ///
-    #[pyo3(name = "wasted", signature = ())]
-    pub fn wasted_py(&mut self) -> Vec<PyWastedSortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.wasted()
-                    .into_iter()
-                    .map(PyWastedSortTrack::from)
-                    .collect()
+        /// Fetch and remove all the tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn wasted(&mut self) -> Vec<PyWastedSortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .wasted()
+                        .into_iter()
+                        .map(WastedSortTrack::from)
+                        .map(PyWastedSortTrack)
+                        .collect()
+                })
             })
-        })
-    }
+        }
 
-    /// Clear all tracks with expired life
-    ///
-    #[pyo3(name = "clear_wasted", signature = ())]
-    pub fn clear_wasted_py(&mut self) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.clear_wasted());
-        })
-    }
+        /// Clear all tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn clear_wasted(&mut self) {
+            Python::with_gil(|py| {
+                py.allow_threads(|| self.0.clear_wasted());
+            })
+        }
 
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks", signature = ())]
-    pub fn idle_tracks_py(&mut self) -> Vec<SortTrack> {
-        self.idle_tracks_with_scene_py(0)
-    }
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3( signature = ())]
+        pub fn idle_tracks(&mut self) -> Vec<PySortTrack> {
+            self.idle_tracks_with_scene(0)
+        }
 
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks_with_scene", signature = (scene_id))]
-    pub fn idle_tracks_with_scene_py(&mut self, scene_id: i64) -> Vec<SortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.idle_tracks_with_scene(scene_id.try_into().unwrap()))
-        })
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn idle_tracks_with_scene(&mut self, scene_id: i64) -> Vec<PySortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(self.0.idle_tracks_with_scene(scene_id.try_into().unwrap()))
+                })
+            })
+        }
     }
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/sort/voting.rs` & `similari_trackers_rs-0.26.5/src/trackers/sort/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/sort.rs` & `similari_trackers_rs-0.26.5/src/trackers/sort.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 use crate::track::{
-    LookupRequest, ObservationsDb, TrackAttributes, TrackAttributesUpdate, TrackStatus,
+    LookupRequest, ObservationsDb, Track, TrackAttributes, TrackAttributesUpdate, TrackStatus,
 };
 use crate::trackers::epoch_db::EpochDb;
 use crate::trackers::kalman_prediction::TrackAttributesKalmanPrediction;
 use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
 use crate::utils::bbox::Universal2DBox;
 use crate::utils::kalman::kalman_2d_box::DIM_2D_BOX_X2;
 use crate::utils::kalman::KalmanState;
 use anyhow::Result;
-use pyo3::prelude::*;
+
 use std::collections::{HashMap, VecDeque};
 use std::sync::{Arc, RwLock};
 
+use self::metric::SortMetric;
+
 /// SORT metric implementation with IoU and Mahalanobis distances
 pub mod metric;
 
 /// SORT implementation with a very tiny interface
 pub mod simple_api;
 
 /// Voting engine with Hungarian algorithm
 ///
 pub mod voting;
 
-/// Python bindings for SORT objects
-///
-pub mod sort_py;
-
 /// SORT tracker with Batch API
 pub mod batch_api;
 
 /// Default IoU threshold that is defined by SORT author in the original repo
 pub const DEFAULT_SORT_IOU_THRESHOLD: f32 = 0.3;
 
 #[derive(Debug, Default)]
@@ -251,254 +249,356 @@
     }
 
     fn baked(&self, _observations: &ObservationsDb<Universal2DBox>) -> Result<TrackStatus> {
         self.opts.baked(self.scene_id, self.last_updated_epoch)
     }
 }
 
-#[cfg(test)]
-mod track_tests {
-    use crate::prelude::{NoopNotifier, ObservationBuilder, TrackBuilder};
-    use crate::trackers::sort::metric::{SortMetric, DEFAULT_MINIMAL_SORT_CONFIDENCE};
-    use crate::trackers::sort::PositionalMetricType::IoU;
-    use crate::trackers::sort::{SortAttributes, DEFAULT_SORT_IOU_THRESHOLD};
-    use crate::utils::bbox::BoundingBox;
-    use crate::utils::kalman::kalman_2d_box::Universal2DBoxKalmanFilter;
-
-    #[test]
-    fn construct() {
-        let observation_bb_0 = BoundingBox::new(1.0, 1.0, 10.0, 15.0);
-        let observation_bb_1 = BoundingBox::new(1.1, 1.3, 10.0, 15.0);
-
-        let f = Universal2DBoxKalmanFilter::default();
-        let init_state = f.initiate(&observation_bb_0.into());
-
-        let mut t1 = TrackBuilder::new(1)
-            .attributes(SortAttributes::default())
-            .metric(SortMetric::new(
-                IoU(DEFAULT_SORT_IOU_THRESHOLD),
-                DEFAULT_MINIMAL_SORT_CONFIDENCE,
-            ))
-            .notifier(NoopNotifier)
-            .observation(
-                ObservationBuilder::new(0)
-                    .observation_attributes(observation_bb_0.into())
-                    .build(),
-            )
-            .build()
-            .unwrap();
-
-        assert!(t1.get_attributes().state.is_some());
-        assert_eq!(t1.get_attributes().predicted_boxes.len(), 1);
-        assert_eq!(t1.get_attributes().observed_boxes.len(), 1);
-        assert_eq!(t1.get_merge_history().len(), 1);
-        assert_eq!(
-            t1.get_attributes().predicted_boxes[0],
-            observation_bb_0.into()
-        );
-
-        let predicted_state = f.predict(&init_state);
-        assert_eq!(
-            BoundingBox::try_from(predicted_state).unwrap(),
-            observation_bb_0
-        );
-
-        let t2 = TrackBuilder::new(2)
-            .attributes(SortAttributes::default())
-            .metric(SortMetric::new(
-                IoU(DEFAULT_SORT_IOU_THRESHOLD),
-                DEFAULT_MINIMAL_SORT_CONFIDENCE,
-            ))
-            .notifier(NoopNotifier)
-            .observation(
-                ObservationBuilder::new(0)
-                    .observation_attributes(observation_bb_1.into())
-                    .build(),
-            )
-            .build()
-            .unwrap();
-
-        t1.merge(&t2, &[0], false).unwrap();
-
-        assert!(t1.get_attributes().state.is_some());
-        assert_eq!(t1.get_attributes().predicted_boxes.len(), 2);
-        assert_eq!(t1.get_attributes().observed_boxes.len(), 2);
-    }
-}
-
 /// Online track structure that contains tracking information for the last tracker epoch
 ///
 #[derive(Debug, Clone)]
-#[pyclass]
 pub struct SortTrack {
     /// id of the track
     ///
-    #[pyo3(get)]
     pub id: u64,
     /// when the track was lastly updated
     ///
-    #[pyo3(get)]
     pub epoch: usize,
     /// the bbox predicted by KF
     ///
-    #[pyo3(get)]
     pub predicted_bbox: Universal2DBox,
     /// the bbox passed by detector
     ///
-    #[pyo3(get)]
     pub observed_bbox: Universal2DBox,
     /// user-defined scene id that splits tracking space on isolated realms
     ///
-    #[pyo3(get)]
     pub scene_id: u64,
     /// current track length
     ///
-    #[pyo3(get)]
     pub length: usize,
     /// what kind of voting was led to the current merge
     ///
-    #[pyo3(get)]
     pub voting_type: VotingType,
     /// custom object id passed by the user to find the track easily
     ///
-    #[pyo3(get)]
     pub custom_object_id: Option<i64>,
 }
 
 /// Online track structure that contains tracking information for the last tracker epoch
 ///
 #[derive(Debug, Clone)]
-#[pyclass]
-#[pyo3(name = "WastedSortTrack")]
-pub struct PyWastedSortTrack {
+pub struct WastedSortTrack {
     /// id of the track
     ///
-    #[pyo3(get)]
     pub id: u64,
     /// when the track was lastly updated
     ///
-    #[pyo3(get)]
     pub epoch: usize,
     /// the bbox predicted by KF
     ///
-    #[pyo3(get)]
     pub predicted_bbox: Universal2DBox,
     /// the bbox passed by detector
     ///
-    #[pyo3(get)]
     pub observed_bbox: Universal2DBox,
     /// user-defined scene id that splits tracking space on isolated realms
     ///
-    #[pyo3(get)]
     pub scene_id: u64,
     /// current track length
     ///
-    #[pyo3(get)]
     pub length: usize,
     /// history of predicted boxes
     ///
-    #[pyo3(get)]
     pub predicted_boxes: Vec<Universal2DBox>,
     /// history of observed boxes
     ///
-    #[pyo3(get)]
     pub observed_boxes: Vec<Universal2DBox>,
 }
 
-#[pymethods]
-impl SortTrack {
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
-
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
-    }
-
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
-    }
-}
-
-#[pymethods]
-impl PyWastedSortTrack {
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
-
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
-    }
-
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
+impl From<Track<SortAttributes, SortMetric, Universal2DBox>> for WastedSortTrack {
+    fn from(track: Track<SortAttributes, SortMetric, Universal2DBox>) -> Self {
+        let attrs = track.get_attributes();
+        WastedSortTrack {
+            id: track.get_track_id(),
+            epoch: attrs.last_updated_epoch,
+            scene_id: attrs.scene_id,
+            length: attrs.track_length,
+            observed_bbox: attrs.observed_boxes.back().unwrap().clone(),
+            predicted_bbox: attrs.predicted_boxes.back().unwrap().clone(),
+            predicted_boxes: attrs.predicted_boxes.clone().into_iter().collect(),
+            observed_boxes: attrs.observed_boxes.clone().into_iter().collect(),
+        }
     }
 }
 
-#[pyclass]
 #[derive(Default, Debug, Clone, Copy)]
 pub enum VotingType {
     #[default]
     Visual,
     Positional,
 }
 
-#[pymethods]
-impl VotingType {
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
-
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
-    }
-
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
-    }
-}
-
 #[derive(Clone, Default, Copy, Debug)]
 pub enum PositionalMetricType {
     #[default]
     Mahalanobis,
     IoU(f32),
 }
 
-#[pyclass]
-#[pyo3(name = "PositionalMetricType")]
-#[derive(Clone, Debug)]
-pub struct PyPositionalMetricType(pub PositionalMetricType);
+pub struct AutoWaste {
+    pub periodicity: usize,
+    pub counter: usize,
+}
+
+pub(crate) const DEFAULT_AUTO_WASTE_PERIODICITY: usize = 100;
+pub(crate) const MAHALANOBIS_NEW_TRACK_THRESHOLD: f32 = 1.0;
 
-#[pymethods]
-impl PyPositionalMetricType {
-    #[staticmethod]
-    pub fn maha() -> Self {
-        PyPositionalMetricType(PositionalMetricType::Mahalanobis)
+#[cfg(feature = "python")]
+pub mod python {
+    use pyo3::prelude::*;
+
+    use crate::utils::bbox::python::PyUniversal2DBox;
+
+    use super::{PositionalMetricType, SortTrack, VotingType, WastedSortTrack};
+
+    #[pyclass]
+    #[pyo3(name = "PositionalMetricType")]
+    #[derive(Clone, Debug)]
+    pub struct PyPositionalMetricType(pub PositionalMetricType);
+
+    #[pymethods]
+    impl PyPositionalMetricType {
+        #[staticmethod]
+        pub fn maha() -> Self {
+            PyPositionalMetricType(PositionalMetricType::Mahalanobis)
+        }
+
+        #[staticmethod]
+        pub fn iou(threshold: f32) -> Self {
+            assert!(
+                threshold > 0.0 && threshold < 1.0,
+                "Threshold must lay between (0.0 and 1.0)"
+            );
+
+            PyPositionalMetricType(PositionalMetricType::IoU(threshold))
+        }
+
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
+
+        fn __repr__(&self) -> String {
+            format!("{self:?}")
+        }
+
+        fn __str__(&self) -> String {
+            format!("{self:#?}")
+        }
     }
 
-    #[staticmethod]
-    pub fn iou(threshold: f32) -> Self {
-        assert!(
-            threshold > 0.0 && threshold < 1.0,
-            "Threshold must lay between (0.0 and 1.0)"
-        );
-        PyPositionalMetricType(PositionalMetricType::IoU(threshold))
+    #[pyclass]
+    #[pyo3(name = "SortTrack")]
+    #[derive(Debug, Clone)]
+    #[repr(transparent)]
+    pub struct PySortTrack(pub(crate) SortTrack);
+
+    #[pymethods]
+    impl PySortTrack {
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
+
+        fn __repr__(&self) -> String {
+            format!("{self:?}")
+        }
+
+        fn __str__(&self) -> String {
+            format!("{self:#?}")
+        }
+
+        #[getter]
+        fn get_id(&self) -> u64 {
+            self.0.id
+        }
+
+        #[getter]
+        fn get_epoch(&self) -> usize {
+            self.0.epoch
+        }
+
+        #[getter]
+        fn get_predicted_bbox(&self) -> PyUniversal2DBox {
+            PyUniversal2DBox(self.0.predicted_bbox.clone())
+        }
+
+        #[getter]
+        fn get_observed_bbox(&self) -> PyUniversal2DBox {
+            PyUniversal2DBox(self.0.observed_bbox.clone())
+        }
+
+        #[getter]
+        fn get_scene_id(&self) -> u64 {
+            self.0.scene_id
+        }
+
+        #[getter]
+        fn get_length(&self) -> usize {
+            self.0.length
+        }
+
+        #[getter]
+        fn get_voting_type(&self) -> PyVotingType {
+            PyVotingType(self.0.voting_type)
+        }
+
+        #[getter]
+        fn get_custom_object_id(&self) -> Option<i64> {
+            self.0.custom_object_id
+        }
     }
 
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
+    #[pyclass]
+    #[pyo3(name = "WastedSortTrack")]
+    #[derive(Debug, Clone)]
+    #[repr(transparent)]
+    pub struct PyWastedSortTrack(pub(crate) WastedSortTrack);
+
+    #[pymethods]
+    impl PyWastedSortTrack {
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
+
+        fn __repr__(&self) -> String {
+            format!("{:?}", self.0)
+        }
+
+        fn __str__(&self) -> String {
+            format!("{:#?}", self.0)
+        }
+
+        #[getter]
+        fn id(&self) -> u64 {
+            self.0.id
+        }
+
+        #[getter]
+        fn epoch(&self) -> usize {
+            self.0.epoch
+        }
+
+        #[getter]
+        fn predicted_bbox(&self) -> PyUniversal2DBox {
+            PyUniversal2DBox(self.0.predicted_bbox.clone())
+        }
+
+        #[getter]
+        fn observed_bbox(&self) -> PyUniversal2DBox {
+            PyUniversal2DBox(self.0.observed_bbox.clone())
+        }
+
+        #[getter]
+        fn scene_id(&self) -> u64 {
+            self.0.scene_id
+        }
+
+        #[getter]
+        fn length(&self) -> usize {
+            self.0.length
+        }
 
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
+        #[getter]
+        fn predicted_boxes(&self) -> Vec<PyUniversal2DBox> {
+            unsafe { std::mem::transmute(self.0.predicted_boxes.clone()) }
+        }
+
+        #[getter]
+        fn observed_boxes(&self) -> Vec<PyUniversal2DBox> {
+            unsafe { std::mem::transmute(self.0.observed_boxes.clone()) }
+        }
     }
 
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
+    #[pyclass]
+    #[pyo3(name = "VotingType")]
+    #[derive(Default, Debug, Clone, Copy)]
+    pub struct PyVotingType(pub(crate) VotingType);
+
+    #[pymethods]
+    impl PyVotingType {
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
+
+        fn __repr__(&self) -> String {
+            format!("{self:?}")
+        }
+
+        fn __str__(&self) -> String {
+            format!("{self:#?}")
+        }
     }
 }
 
-pub struct AutoWaste {
-    pub periodicity: usize,
-    pub counter: usize,
-}
+#[cfg(test)]
+mod track_tests {
+    use crate::prelude::{NoopNotifier, ObservationBuilder, TrackBuilder};
+    use crate::trackers::sort::metric::{SortMetric, DEFAULT_MINIMAL_SORT_CONFIDENCE};
+    use crate::trackers::sort::PositionalMetricType::IoU;
+    use crate::trackers::sort::{SortAttributes, DEFAULT_SORT_IOU_THRESHOLD};
+    use crate::utils::bbox::BoundingBox;
+    use crate::utils::kalman::kalman_2d_box::Universal2DBoxKalmanFilter;
 
-pub(crate) const DEFAULT_AUTO_WASTE_PERIODICITY: usize = 100;
+    #[test]
+    fn construct() {
+        let observation_bb_0 = BoundingBox::new(1.0, 1.0, 10.0, 15.0);
+        let observation_bb_1 = BoundingBox::new(1.1, 1.3, 10.0, 15.0);
 
-pub(crate) const MAHALANOBIS_NEW_TRACK_THRESHOLD: f32 = 1.0;
+        let f = Universal2DBoxKalmanFilter::default();
+        let init_state = f.initiate(&observation_bb_0.into());
+
+        let mut t1 = TrackBuilder::new(1)
+            .attributes(SortAttributes::default())
+            .metric(SortMetric::new(
+                IoU(DEFAULT_SORT_IOU_THRESHOLD),
+                DEFAULT_MINIMAL_SORT_CONFIDENCE,
+            ))
+            .notifier(NoopNotifier)
+            .observation(
+                ObservationBuilder::new(0)
+                    .observation_attributes(observation_bb_0.into())
+                    .build(),
+            )
+            .build()
+            .unwrap();
+
+        assert!(t1.get_attributes().state.is_some());
+        assert_eq!(t1.get_attributes().predicted_boxes.len(), 1);
+        assert_eq!(t1.get_attributes().observed_boxes.len(), 1);
+        assert_eq!(t1.get_merge_history().len(), 1);
+        assert_eq!(
+            t1.get_attributes().predicted_boxes[0],
+            observation_bb_0.into()
+        );
+
+        let predicted_state = f.predict(&init_state);
+        assert_eq!(
+            BoundingBox::try_from(predicted_state).unwrap(),
+            observation_bb_0
+        );
+
+        let t2 = TrackBuilder::new(2)
+            .attributes(SortAttributes::default())
+            .metric(SortMetric::new(
+                IoU(DEFAULT_SORT_IOU_THRESHOLD),
+                DEFAULT_MINIMAL_SORT_CONFIDENCE,
+            ))
+            .notifier(NoopNotifier)
+            .observation(
+                ObservationBuilder::new(0)
+                    .observation_attributes(observation_bb_1.into())
+                    .build(),
+            )
+            .build()
+            .unwrap();
+
+        t1.merge(&t2, &[0], false).unwrap();
+
+        assert!(t1.get_attributes().state.is_some());
+        assert_eq!(t1.get_attributes().predicted_boxes.len(), 2);
+        assert_eq!(t1.get_attributes().observed_boxes.len(), 2);
+    }
+}
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/spatio_temporal_constraints.rs` & `similari_trackers_rs-0.26.5/src/trackers/spatio_temporal_constraints.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-use pyo3::prelude::*;
-
 /// The struct allows defining the constraints for objects comprared across different epochs.
 ///
 /// When the new objects batch is passed to the tracker it has a newer epoch that the tracks that are kept
 /// within the trackers. It may happen that epoch difference is 1 when the track was updated in the previous
 /// epoch or more than one, if the track wasn't updated lastly.
 ///
 /// The constraint defines how far the object may be from the track for certain epoch difference to still count
 /// that it can relate to it. The distance is measured in Nx(R_Obj+R_Track), where
 /// * `N` is the float number that defines the expected maximal distance;
 /// * `R_Obj` - radius of the circle surrounding the candidate object;
 /// * `R_Track` - radius of the circle surrounding the last bounding box of the track.
 ///
 
-#[pyclass]
 #[derive(Default, Debug, Clone)]
 pub struct SpatioTemporalConstraints {
     constraints: Vec<(usize, f32)>,
 }
 
 impl SpatioTemporalConstraints {
     /// Allows adding new constraints to the constraints engine
@@ -27,56 +24,82 @@
     ///
     pub fn constraints(mut self, constraints: &[(usize, f32)]) -> Self {
         self.add_constraints(constraints.to_vec());
         self
     }
 }
 
-#[pymethods]
 impl SpatioTemporalConstraints {
-    #[new]
-    fn new() -> Self {
+    pub fn new() -> Self {
         Self::default()
     }
 
-    /// Allows adding new constraints to the constraints engine
-    ///
-    /// # Parameters
-    /// * `constraints` - Vec of tuples (epoch_delta, max_allowed_distance)
-    ///
-    #[pyo3(text_signature = "($self, l: [(epoch_delta, max_allowed_distance)]")]
     pub fn add_constraints(&mut self, constraints: Vec<(usize, f32)>) {
         for (delta, max_distance) in constraints {
             assert!(
                 max_distance > 0.0,
                 "The distance is expected to be a positive float"
             );
             self.constraints.push((delta, max_distance));
         }
         self.constraints.sort_by(|(e1, _), (e2, _)| e1.cmp(e2));
         self.constraints.dedup_by(|(e1, _), (e2, _)| *e1 == *e2);
     }
 
-    /// Validates the distance for specified epoch delta
-    ///
-    #[pyo3(text_signature = "($self, epoch_delta, dist)")]
     pub fn validate(&self, epoch_delta: usize, dist: f32) -> bool {
         assert!(
             dist >= 0.0,
             "The distance is expected to be a positive float"
         );
         let constraint = self.constraints.iter().find(|(d, _)| *d >= epoch_delta);
 
         match constraint {
             None => true,
             Some((_, max_dist)) => dist <= *max_dist,
         }
     }
 }
 
+#[cfg(feature = "python")]
+pub mod python {
+    use pyo3::prelude::*;
+
+    use super::SpatioTemporalConstraints;
+
+    #[pyclass]
+    #[derive(Default, Debug, Clone)]
+    #[pyo3(name = "SpatioTemporalConstraints")]
+    pub struct PySpatioTemporalConstraints(pub(crate) SpatioTemporalConstraints);
+
+    #[pymethods]
+    impl PySpatioTemporalConstraints {
+        #[new]
+        pub fn new() -> Self {
+            Self(SpatioTemporalConstraints::default())
+        }
+
+        /// Allows adding new constraints to the constraints engine
+        ///
+        /// # Parameters
+        /// * `constraints` - Vec of tuples (epoch_delta, max_allowed_distance)
+        ///
+        #[pyo3(text_signature = "($self, l: [(epoch_delta, max_allowed_distance)]")]
+        pub fn add_constraints(&mut self, constraints: Vec<(usize, f32)>) {
+            self.0.add_constraints(constraints)
+        }
+
+        /// Validates the distance for specified epoch delta
+        ///
+        #[pyo3(text_signature = "($self, epoch_delta, dist)")]
+        pub fn validate(&self, epoch_delta: usize, dist: f32) -> bool {
+            self.0.validate(epoch_delta, dist)
+        }
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
 
     #[test]
     fn test() {
         let mut spc = SpatioTemporalConstraints::default();
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/tracker_api.rs` & `similari_trackers_rs-0.26.5/src/trackers/tracker_api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     fn get_main_store(&self) -> RwLockReadGuard<TrackStore<TA, M, OA, N>>;
     fn get_wasted_store(&self) -> RwLockReadGuard<TrackStore<TA, M, OA, N>>;
 
     /// change auto waste job periodicity
     ///
     fn set_auto_waste(&mut self, periodicity: usize) {
-        let mut obj = self.get_auto_waste_obj_mut();
+        let obj = self.get_auto_waste_obj_mut();
         obj.periodicity = periodicity;
         obj.counter = 0;
     }
 
     /// Skip number of epochs to force tracks to turn to terminal state
     ///
     /// # Parameters
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/batch_api.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/batch_api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 };
 use crate::trackers::tracker_api::TrackerAPI;
 use crate::trackers::visual_sort::metric::{VisualMetric, VisualMetricOptions};
 use crate::trackers::visual_sort::observation_attributes::VisualObservationAttributes;
 use crate::trackers::visual_sort::track_attributes::{
     VisualAttributes, VisualAttributesUpdate, VisualSortLookup,
 };
-use crate::trackers::visual_sort::visual_sort_py::PyVisualSortPredictionBatchRequest;
 use crate::trackers::visual_sort::voting::VisualVoting;
-use crate::trackers::visual_sort::PyWastedVisualSortTrack;
 use crate::utils::clipping::bbox_own_areas::{
     exclusively_owned_areas, exclusively_owned_areas_normalized_shares,
 };
 use crate::voting::Voting;
 use crossbeam::channel::{Receiver, Sender};
 use log::warn;
-use pyo3::prelude::*;
 use rand::Rng;
 use std::mem;
 use std::sync::{Arc, Condvar, Mutex, RwLock, RwLockReadGuard, RwLockWriteGuard};
 use std::thread::{spawn, JoinHandle};
 
 type VotingSenderChannel = Sender<VotingCommands>;
 type VotingReceiverChannel = Receiver<VotingCommands>;
@@ -50,15 +47,14 @@
         monitor: BatchBusyMonitor,
     },
     Exit,
 }
 
 // /// Easy to use Visual SORT tracker implementation
 // ///
-#[pyclass(text_signature = "(distance_shards, voting_shards, opts)")]
 pub struct BatchVisualSort {
     monitor: Option<BatchBusyMonitor>,
     store: Arc<RwLock<MiddlewareVisualSortTrackStore>>,
     wasted_store: RwLock<MiddlewareVisualSortTrackStore>,
     metric_opts: Arc<VisualMetricOptions>,
     track_opts: Arc<SortAttributesOptions>,
     voting_threads: Vec<(VotingSenderChannel, JoinHandle<()>)>,
@@ -275,16 +271,16 @@
                                     VisualObservationAttributes::new(
                                         o.feature_quality.unwrap_or(1.0),
                                         o.bounding_box.clone(),
                                     )
                                 },
                             );
 
-                            if let Some(feature) = o.feature {
-                                obs = obs.observation(Feature::from_vec(feature));
+                            if let Some(feature) = &o.feature {
+                                obs = obs.observation(Feature::from_vec(feature.to_vec()));
                             }
 
                             obs.track_attributes_update(
                                 VisualAttributesUpdate::new_init_with_scene(
                                     epoch,
                                     *scene_id,
                                     o.custom_object_id,
@@ -453,135 +449,217 @@
         for _ in 0..predictions.batch_size() {
             let (scene, tracks) = predictions.get();
             dbg!(scene, tracks);
         }
     }
 }
 
-#[pymethods]
-impl BatchVisualSort {
-    #[new]
-    #[pyo3(signature = (distance_shards, voting_shards, opts))]
-    pub fn new_py(distance_shards: i64, voting_shards: i64, opts: &VisualSortOptions) -> Self {
-        Self::new(
-            distance_shards
-                .try_into()
-                .expect("Positive number expected"),
-            voting_shards.try_into().expect("Positive number expected"),
-            opts,
-        )
+#[derive(Debug, Clone)]
+pub struct VisualSortPredictionBatchRequest<'a> {
+    pub batch: PredictionBatchRequest<VisualSortObservation<'a>>,
+    pub result: Option<PredictionBatchResult>,
+}
+
+impl<'a> VisualSortPredictionBatchRequest<'a> {
+    pub fn new() -> Self {
+        let (batch, result) = PredictionBatchRequest::new();
+        Self {
+            batch,
+            result: Some(result),
+        }
     }
 
-    #[pyo3(name = "skip_epochs", signature = (n))]
-    fn skip_epochs_py(&mut self, n: i64) {
-        assert!(n > 0);
-        self.skip_epochs(n.try_into().unwrap())
+    pub fn prediction(&mut self) -> Option<PredictionBatchResult> {
+        self.result.take()
     }
 
-    #[pyo3(
-        name = "skip_epochs_for_scene",
-        signature = (scene_id, n)
-    )]
-    fn skip_epochs_for_scene_py(&mut self, scene_id: i64, n: i64) {
-        assert!(n > 0 && scene_id >= 0);
-        self.skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
-    }
-
-    /// Get the amount of stored tracks per shard
-    ///
-    #[pyo3(name = "shard_stats", signature = ())]
-    fn shard_stats_py(&self) -> Vec<i64> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.store
-                    .read()
-                    .unwrap()
-                    .shard_stats()
-                    .into_iter()
-                    .map(|e| i64::try_from(e).unwrap())
-                    .collect()
-            })
-        })
+    pub fn add(&mut self, scene_id: u64, elt: VisualSortObservation<'a>) {
+        self.batch.add(scene_id, elt);
+    }
+}
+
+impl<'a> Default for VisualSortPredictionBatchRequest<'a> {
+    fn default() -> Self {
+        Self::new()
     }
+}
 
-    /// Get the current epoch for `scene_id` == 0
-    ///
-    #[pyo3(name = "current_epoch", signature = ())]
-    fn current_epoch_py(&self) -> i64 {
-        self.current_epoch_with_scene(0).try_into().unwrap()
-    }
-
-    /// Get the current epoch for `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id
-    ///
-    #[pyo3(
-        name = "current_epoch_with_scene",
+#[cfg(feature = "python")]
+pub mod python {
+    use pyo3::prelude::*;
+
+    use crate::{
+        prelude::VisualSortObservation,
+        trackers::{
+            batch::{python::PyPredictionBatchResult, PredictionBatchRequest},
+            sort::python::PySortTrack,
+            tracker_api::TrackerAPI,
+            visual_sort::{
+                options::python::PyVisualSortOptions,
+                python::{PyVisualSortObservation, PyWastedVisualSortTrack},
+                WastedVisualSortTrack,
+            },
+        },
+    };
+
+    use super::{BatchVisualSort, VisualSortPredictionBatchRequest};
+
+    #[pyclass(text_signature = "(distance_shards, voting_shards, opts)")]
+    #[pyo3(name = "BatchVisualSort")]
+    pub struct PyBatchVisualSort(pub(crate) BatchVisualSort);
+
+    #[pymethods]
+    impl PyBatchVisualSort {
+        #[new]
+        #[pyo3(signature = (distance_shards, voting_shards, opts))]
+        pub fn new(distance_shards: i64, voting_shards: i64, opts: &PyVisualSortOptions) -> Self {
+            Self(BatchVisualSort::new(
+                distance_shards
+                    .try_into()
+                    .expect("Positive number expected"),
+                voting_shards.try_into().expect("Positive number expected"),
+                &opts.0,
+            ))
+        }
+
+        #[pyo3(signature = (n))]
+        fn skip_epochs(&mut self, n: i64) {
+            assert!(n > 0);
+            self.0.skip_epochs(n.try_into().unwrap())
+        }
+
+        #[pyo3(signature = (scene_id, n))]
+        fn skip_epochs_for_scene(&mut self, scene_id: i64, n: i64) {
+            assert!(n > 0 && scene_id >= 0);
+            self.0
+                .skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
+        }
+
+        /// Get the amount of stored tracks per shard
+        ///
+        #[pyo3(signature = ())]
+        fn shard_stats(&self) -> Vec<i64> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .store
+                        .read()
+                        .unwrap()
+                        .shard_stats()
+                        .into_iter()
+                        .map(|e| i64::try_from(e).unwrap())
+                        .collect()
+                })
+            })
+        }
+
+        /// Get the current epoch for `scene_id` == 0
+        ///
+        #[pyo3( signature = ())]
+        fn current_epoch(&self) -> i64 {
+            self.current_epoch_with_scene(0).try_into().unwrap()
+        }
+
+        /// Get the current epoch for `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id
+        ///
+        #[pyo3(
         signature = (scene_id)
     )]
-    fn current_epoch_with_scene_py(&self, scene_id: i64) -> isize {
-        assert!(scene_id >= 0);
-        self.current_epoch_with_scene(scene_id.try_into().unwrap())
-            .try_into()
-            .unwrap()
-    }
-
-    /// Receive tracking information for observed bboxes of `scene_id` == 0
-    ///
-    /// # Parameters
-    /// * `bboxes` - bounding boxes received from a detector
-    ///
-    #[pyo3(name = "predict", signature = (py_batch))]
-    fn predict_py(
-        &mut self,
-        py_batch: PyVisualSortPredictionBatchRequest,
-    ) -> PredictionBatchResult {
-        let (mut batch, res) = PredictionBatchRequest::<VisualSortObservation>::new();
-        for (scene_id, observations) in py_batch.batch.get_batch() {
-            for o in observations {
-                let f = o.feature.as_ref();
-                batch.add(
-                    *scene_id,
-                    VisualSortObservation::new(
-                        f,
-                        o.feature_quality,
-                        o.bounding_box.clone(),
-                        o.custom_object_id,
-                    ),
-                );
+        fn current_epoch_with_scene(&self, scene_id: i64) -> isize {
+            assert!(scene_id >= 0);
+            self.0
+                .current_epoch_with_scene(scene_id.try_into().unwrap())
+                .try_into()
+                .unwrap()
+        }
+
+        /// Receive tracking information for observed bboxes of `scene_id` == 0
+        ///
+        /// # Parameters
+        /// * `bboxes` - bounding boxes received from a detector
+        ///
+        #[pyo3(signature = (py_batch))]
+        fn predict(
+            &mut self,
+            py_batch: PyVisualSortPredictionBatchRequest,
+        ) -> PyPredictionBatchResult {
+            let (mut batch, res) = PredictionBatchRequest::<VisualSortObservation>::new();
+            for (scene_id, observations) in py_batch.0.batch.get_batch() {
+                for o in observations {
+                    let f = o.feature.as_ref();
+                    batch.add(
+                        *scene_id,
+                        VisualSortObservation::new(
+                            f.map(|x| x.as_ref()),
+                            o.feature_quality,
+                            o.bounding_box.clone(),
+                            o.custom_object_id,
+                        ),
+                    );
+                }
             }
+            self.0.predict(batch);
+
+            PyPredictionBatchResult(res)
+        }
+
+        /// Remove all the tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        fn wasted(&mut self) -> Vec<PyWastedVisualSortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .wasted()
+                        .into_iter()
+                        .map(WastedVisualSortTrack::from)
+                        .map(PyWastedVisualSortTrack)
+                        .collect()
+                })
+            })
         }
-        self.predict(batch);
-        res
-    }
 
-    /// Remove all the tracks with expired life
-    ///
-    #[pyo3(name = "wasted", signature = ())]
-    fn wasted_py(&mut self) -> Vec<PyWastedVisualSortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.wasted()
-                    .into_iter()
-                    .map(PyWastedVisualSortTrack::from)
-                    .collect()
+        /// Clear all tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn clear_wasted(&mut self) {
+            Python::with_gil(|py| py.allow_threads(|| self.0.clear_wasted()));
+        }
+
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn idle_tracks(&mut self, scene_id: i64) -> Vec<PySortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(self.0.idle_tracks_with_scene(scene_id.try_into().unwrap()))
+                })
             })
-        })
+        }
     }
 
-    /// Clear all tracks with expired life
-    ///
-    #[pyo3(name = "clear_wasted", signature = ())]
-    pub fn clear_wasted_py(&mut self) {
-        Python::with_gil(|py| py.allow_threads(|| self.clear_wasted()));
-    }
-
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks", signature = (scene_id))]
-    pub fn idle_tracks_py(&mut self, scene_id: i64) -> Vec<SortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.idle_tracks_with_scene(scene_id.try_into().unwrap()))
-        })
+    #[derive(Debug, Clone)]
+    #[pyclass]
+    #[pyo3(name = "VisualSortPredictionBatchRequest")]
+    pub(crate) struct PyVisualSortPredictionBatchRequest(
+        pub(crate) VisualSortPredictionBatchRequest<'static>,
+    );
+
+    #[pymethods]
+    impl PyVisualSortPredictionBatchRequest {
+        #[new]
+        fn new() -> Self {
+            Self(VisualSortPredictionBatchRequest::new())
+        }
+
+        fn prediction(&mut self) -> Option<PyPredictionBatchResult> {
+            self.0.prediction().map(PyPredictionBatchResult)
+        }
+
+        fn add(&mut self, scene_id: u64, elt: PyVisualSortObservation) {
+            self.0.add(scene_id, elt.0)
+        }
     }
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric/builder.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/metric/builder.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use crate::trackers::sort::PositionalMetricType;
 use crate::trackers::visual_sort::metric::{
-    PyVisualSortMetricType, VisualMetric, VisualMetricOptions, VisualSortMetricType,
+    VisualMetric, VisualMetricOptions, VisualSortMetricType,
 };
+
 use std::sync::Arc;
 
 #[derive(Debug, Clone)]
 pub struct VisualMetricBuilder {
     visual_kind: VisualSortMetricType,
     positional_kind: PositionalMetricType,
     visual_minimal_track_length: usize,
@@ -37,102 +38,29 @@
             visual_minimal_own_area_percentage_collect: 0.0,
             positional_min_confidence: 0.1,
         }
     }
 }
 
 impl VisualMetricBuilder {
-    pub(crate) fn visual_metric_py(&mut self, metric: PyVisualSortMetricType) {
-        self.visual_kind = metric.0;
-    }
-
-    pub(crate) fn positional_min_confidence_py(&mut self, conf: f32) {
-        assert!(
-            (0.01..=1.0).contains(&conf),
-            "Confidence must lay between (0.01 and 1.0)"
-        );
-        self.positional_min_confidence = conf;
-    }
-
-    pub(crate) fn visual_min_votes_py(&mut self, n: i64) {
-        self.visual_min_votes =
-            usize::try_from(n).expect("The number of required votes must be a positive number.");
-    }
-
-    pub(crate) fn positional_metric_py(&mut self, metric: PositionalMetricType) {
-        if let PositionalMetricType::IoU(t) = metric {
-            assert!(
-                t > 0.0 && t < 1.0,
-                "Threshold must lay between (0.0 and 1.0)"
-            );
-        }
-        self.positional_kind = metric;
-    }
-
-    pub(crate) fn visual_minimal_track_length_py(&mut self, length: usize) {
-        assert!(
-            length > 0,
-            "The minimum amount of visual_sort features collected before visual_sort metric is applied should be greater than 0."
-        );
-        self.visual_minimal_track_length = length;
-    }
-
-    pub(crate) fn visual_minimal_area_py(&mut self, area: f32) {
-        assert!(
-            area >= 0.0,
-            "The minimum area of bbox for visual_sort feature distance calculated and feature collected should be greater than 0."
-        );
-        self.visual_minimal_area = area;
-    }
-
-    pub(crate) fn visual_minimal_own_area_percentage_use_py(&mut self, area: f32) {
+    pub fn visual_minimal_own_area_percentage_use(mut self, area: f32) -> Self {
         assert!(
             (0.0..=1.0).contains(&area),
             "Argument must be contained within (0.0..=1.0)"
         );
         self.visual_minimal_own_area_percentage_use = area;
+        self
     }
 
-    pub(crate) fn visual_minimal_own_area_percentage_collect_py(&mut self, area: f32) {
+    pub fn visual_minimal_own_area_percentage_collect(mut self, area: f32) -> Self {
         assert!(
             (0.0..=1.0).contains(&area),
             "Argument must be contained within (0.0..=1.0)"
         );
         self.visual_minimal_own_area_percentage_collect = area;
-    }
-
-    pub(crate) fn visual_minimal_quality_use_py(&mut self, q: f32) {
-        assert!(
-            q >= 0.0,
-            "The minimum quality of visual_sort feature should be greater than or equal to 0.0."
-        );
-        self.visual_minimal_quality_use = q;
-    }
-
-    pub(crate) fn visual_max_observations_py(&mut self, n: usize) {
-        self.visual_max_observations = n;
-    }
-
-    pub(crate) fn visual_minimal_quality_collect_py(&mut self, q: f32) {
-        assert!(
-            q >= 0.0,
-            "The minimum quality of visual_sort feature should be greater than or equal to 0.0."
-        );
-        self.visual_minimal_quality_collect = q;
-    }
-}
-
-impl VisualMetricBuilder {
-    pub fn visual_minimal_own_area_percentage_use(mut self, area: f32) -> Self {
-        self.visual_minimal_own_area_percentage_use_py(area);
-        self
-    }
-
-    pub fn visual_minimal_own_area_percentage_collect(mut self, area: f32) -> Self {
-        self.visual_minimal_own_area_percentage_collect_py(area);
         self
     }
 
     pub fn visual_min_votes(mut self, n: usize) -> Self {
         self.visual_min_votes = n;
         self
     }
@@ -223,8 +151,68 @@
                 visual_min_votes: self.visual_min_votes,
                 visual_minimal_own_area_percentage_use: self.visual_minimal_own_area_percentage_use,
                 visual_minimal_own_area_percentage_collect: self
                     .visual_minimal_own_area_percentage_collect,
             }),
         }
     }
+
+    #[inline]
+    pub fn set_visual_minimal_area(&mut self, visual_minimal_area: f32) {
+        self.visual_minimal_area = visual_minimal_area;
+    }
+
+    #[inline]
+    pub fn set_positional_kind(&mut self, positional_kind: PositionalMetricType) {
+        self.positional_kind = positional_kind;
+    }
+
+    #[inline]
+    pub fn set_visual_minimal_track_length(&mut self, visual_minimal_track_length: usize) {
+        self.visual_minimal_track_length = visual_minimal_track_length;
+    }
+
+    #[inline]
+    pub fn set_visual_minimal_quality_use(&mut self, visual_minimal_quality_use: f32) {
+        self.visual_minimal_quality_use = visual_minimal_quality_use;
+    }
+
+    #[inline]
+    pub fn set_visual_minimal_quality_collect(&mut self, visual_minimal_quality_collect: f32) {
+        self.visual_minimal_quality_collect = visual_minimal_quality_collect;
+    }
+
+    #[inline]
+    pub fn set_visual_max_observations(&mut self, visual_max_observations: usize) {
+        self.visual_max_observations = visual_max_observations;
+    }
+
+    #[inline]
+    pub fn set_visual_min_votes(&mut self, visual_min_votes: usize) {
+        self.visual_min_votes = visual_min_votes;
+    }
+
+    #[inline]
+    pub fn set_visual_minimal_own_area_percentage_use(
+        &mut self,
+        visual_minimal_own_area_percentage_use: f32,
+    ) {
+        self.visual_minimal_own_area_percentage_use = visual_minimal_own_area_percentage_use;
+    }
+    #[inline]
+    pub fn set_visual_minimal_own_area_percentage_collect(
+        &mut self,
+        visual_minimal_own_area_percentage_collect: f32,
+    ) {
+        self.visual_minimal_own_area_percentage_collect =
+            visual_minimal_own_area_percentage_collect;
+    }
+
+    #[inline]
+    pub fn set_positional_min_confidence(&mut self, positional_min_confidence: f32) {
+        self.positional_min_confidence = positional_min_confidence;
+    }
+
+    pub fn set_visual_kind(&mut self, visual_kind: VisualSortMetricType) {
+        self.visual_kind = visual_kind;
+    }
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/metric.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/metric.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 use crate::trackers::visual_sort::metric::builder::VisualMetricBuilder;
 use crate::trackers::visual_sort::metric::VisualSortMetricType::{Cosine, Euclidean};
 use crate::trackers::visual_sort::observation_attributes::VisualObservationAttributes;
 use crate::trackers::visual_sort::track_attributes::VisualAttributes;
 use crate::utils::bbox::Universal2DBox;
 use crate::utils::kalman::kalman_2d_box::Universal2DBoxKalmanFilter;
 use anyhow::Result;
-use pyo3::prelude::*;
 use std::default::Default;
 use std::iter::Iterator;
 use std::sync::Arc;
 
 #[derive(Clone, Copy, Debug)]
 pub enum VisualSortMetricType {
     Euclidean(f32),
@@ -61,40 +60,46 @@
         match self {
             Euclidean(_) => dist,
             Cosine(_) => 1.0 - dist,
         }
     }
 }
 
-#[pyclass]
-#[pyo3(name = "VisualSortMetricType")]
-#[derive(Clone, Debug)]
-pub struct PyVisualSortMetricType(pub VisualSortMetricType);
-
-#[pymethods]
-impl PyVisualSortMetricType {
-    #[staticmethod]
-    pub fn euclidean(threshold: f32) -> Self {
-        PyVisualSortMetricType(VisualSortMetricType::euclidean(threshold))
-    }
+#[cfg(feature = "python")]
+pub mod python {
+    use super::VisualSortMetricType;
+    use pyo3::prelude::*;
+
+    #[pyclass]
+    #[pyo3(name = "VisualSortMetricType")]
+    #[derive(Clone, Debug)]
+    pub struct PyVisualSortMetricType(pub VisualSortMetricType);
+
+    #[pymethods]
+    impl PyVisualSortMetricType {
+        #[staticmethod]
+        pub fn euclidean(threshold: f32) -> Self {
+            PyVisualSortMetricType(VisualSortMetricType::euclidean(threshold))
+        }
 
-    #[staticmethod]
-    pub fn cosine(threshold: f32) -> Self {
-        PyVisualSortMetricType(VisualSortMetricType::cosine(threshold))
-    }
+        #[staticmethod]
+        pub fn cosine(threshold: f32) -> Self {
+            PyVisualSortMetricType(VisualSortMetricType::cosine(threshold))
+        }
 
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
 
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
-    }
+        fn __repr__(&self) -> String {
+            format!("{self:?}")
+        }
 
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
+        fn __str__(&self) -> String {
+            format!("{self:#?}")
+        }
     }
 }
 
 #[derive(Debug)]
 pub struct VisualMetricOptions {
     pub visual_max_observations: usize,
     pub visual_min_votes: usize,
@@ -304,15 +309,15 @@
             .as_ref()
             .expect("Observation attributes must always present.");
 
         let observation_bbox = obs_attrs.unchecked_bbox_ref();
         let feature_quality = obs_attrs.visual_quality();
         let own_area_percentage_opt = *obs_attrs.own_area_percentage_opt();
 
-        let predicted_bbox = attrs.make_prediction(observation_bbox);
+        let mut predicted_bbox = attrs.make_prediction(observation_bbox);
         attrs.update_history(
             observation_bbox,
             &predicted_bbox,
             observation.feature().clone(),
         );
 
         if is_merge
@@ -328,24 +333,30 @@
         }
 
         *observation.attr_mut() = Some(if let Some(percentage) = own_area_percentage_opt {
             VisualObservationAttributes::with_own_area_percentage(
                 feature_quality,
                 match self.opts.positional_kind {
                     PositionalMetricType::Mahalanobis => predicted_bbox,
-                    PositionalMetricType::IoU(_) => predicted_bbox.gen_vertices(),
+                    PositionalMetricType::IoU(_) => {
+                        predicted_bbox.gen_vertices();
+                        predicted_bbox
+                    }
                 },
                 percentage,
             )
         } else {
             VisualObservationAttributes::new(
                 feature_quality,
                 match self.opts.positional_kind {
                     PositionalMetricType::Mahalanobis => predicted_bbox,
-                    PositionalMetricType::IoU(_) => predicted_bbox.gen_vertices(),
+                    PositionalMetricType::IoU(_) => {
+                        predicted_bbox.gen_vertices();
+                        predicted_bbox
+                    }
                 },
             )
         });
 
         self.optimize_observations(observations);
         observations.push(observation);
         let current_len = observations.len();
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/observation_attributes.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/observation_attributes.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/options.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/options.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-use crate::trackers::sort::{PositionalMetricType, PyPositionalMetricType, SortAttributesOptions};
+use crate::trackers::sort::{PositionalMetricType, SortAttributesOptions};
 use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
 use crate::trackers::visual_sort::metric::builder::VisualMetricBuilder;
-use crate::trackers::visual_sort::metric::{
-    PyVisualSortMetricType, VisualMetric, VisualSortMetricType,
-};
-use pyo3::prelude::*;
+use crate::trackers::visual_sort::metric::{VisualMetric, VisualSortMetricType};
 use std::collections::HashMap;
 use std::sync::RwLock;
 
 /// Class that is used to configure the Visual Tracker
-#[pyclass]
 #[derive(Debug, Clone)]
 pub struct VisualSortOptions {
     max_idle_epochs: usize,
     kept_history_length: usize,
     spatio_temporal_constraints: SpatioTemporalConstraints,
     metric_builder: VisualMetricBuilder,
 }
@@ -188,132 +184,144 @@
             kept_history_length: 10,
             metric_builder: VisualMetricBuilder::default(),
             spatio_temporal_constraints: SpatioTemporalConstraints::default(),
         }
     }
 }
 
-#[pymethods]
-impl VisualSortOptions {
-    #[new]
-    fn new() -> Self {
-        Self::default()
-    }
+#[cfg(feature = "python")]
+pub mod python {
+    use crate::trackers::sort::python::PyPositionalMetricType;
+    use crate::trackers::spatio_temporal_constraints::python::PySpatioTemporalConstraints;
+    use crate::trackers::visual_sort::metric::python::PyVisualSortMetricType;
+
+    use super::VisualSortOptions;
+    use pyo3::prelude::*;
+
+    #[pyclass]
+    #[pyo3(name = "VisualSortOptions")]
+    pub struct PyVisualSortOptions(pub(crate) VisualSortOptions);
+
+    #[pymethods]
+    impl PyVisualSortOptions {
+        #[new]
+        pub(crate) fn new() -> Self {
+            Self(VisualSortOptions::default())
+        }
 
-    #[pyo3(name = "max_idle_epochs", text_signature = "($self, n)")]
-    fn max_idle_epochs_py(&mut self, n: i64) {
-        self.max_idle_epochs = n.try_into().expect("Parameter must be a positive number");
-    }
+        #[pyo3(text_signature = "($self, n)")]
+        pub(crate) fn max_idle_epochs(&mut self, n: i64) {
+            self.0.max_idle_epochs = n.try_into().expect("Parameter must be a positive number");
+        }
 
-    #[pyo3(name = "kept_history_length", text_signature = "($self, n)")]
-    fn kept_history_length_py(&mut self, n: i64) {
-        self.kept_history_length = n.try_into().expect("Parameter must be a positive number");
-    }
+        #[pyo3(text_signature = "($self, n)")]
+        pub(crate) fn kept_history_length(&mut self, n: i64) {
+            self.0.kept_history_length = n.try_into().expect("Parameter must be a positive number");
+        }
 
-    #[pyo3(name = "visual_min_votes", text_signature = "($self, n)")]
-    fn visual_min_votes_py(&mut self, n: i64) {
-        self.metric_builder.visual_min_votes_py(n);
-    }
+        #[pyo3(text_signature = "($self, n)")]
+        pub(crate) fn visual_min_votes(&mut self, n: i64) {
+            self.0.metric_builder.set_visual_min_votes(n as _);
+        }
 
-    #[pyo3(name = "visual_metric", text_signature = "($self, metric)")]
-    fn visual_metric_py(&mut self, metric: PyVisualSortMetricType) {
-        self.metric_builder.visual_metric_py(metric);
-    }
+        #[pyo3(text_signature = "($self, metric)")]
+        pub(crate) fn visual_metric(&mut self, metric: PyVisualSortMetricType) {
+            self.0.metric_builder.set_visual_kind(metric.0);
+        }
 
-    #[pyo3(
-        name = "spatio_temporal_constraints",
-        text_signature = "($self, constraints)"
-    )]
-    fn spatio_temporal_constraints_py(&mut self, constraints: SpatioTemporalConstraints) {
-        self.spatio_temporal_constraints = constraints;
-    }
+        #[pyo3(text_signature = "($self, constraints)")]
+        pub(crate) fn spatio_temporal_constraints(
+            &mut self,
+            constraints: PySpatioTemporalConstraints,
+        ) {
+            self.0.spatio_temporal_constraints = constraints.0;
+        }
 
-    #[pyo3(name = "positional_metric", text_signature = "($self, metric)")]
-    fn positional_metric_py(&mut self, metric: PyPositionalMetricType) {
-        self.metric_builder.positional_metric_py(metric.0);
-    }
+        #[pyo3(text_signature = "($self, metric)")]
+        pub(crate) fn positional_metric(&mut self, metric: PyPositionalMetricType) {
+            self.0.metric_builder.set_positional_kind(metric.0);
+        }
 
-    #[pyo3(
-        name = "visual_minimal_track_length",
-        text_signature = "($self, length)"
-    )]
-    fn visual_minimal_track_length_py(&mut self, length: i64) {
-        self.metric_builder.visual_minimal_track_length_py(
-            length
-                .try_into()
-                .expect("Parameter must be a positive number"),
-        );
-    }
+        #[pyo3(text_signature = "($self, length)")]
+        pub(crate) fn visual_minimal_track_length(&mut self, length: i64) {
+            self.0.metric_builder.set_visual_minimal_track_length(
+                length
+                    .try_into()
+                    .expect("Parameter must be a positive number"),
+            );
+        }
 
-    #[pyo3(name = "visual_minimal_area", text_signature = "($self, area)")]
-    fn visual_minimal_area_py(&mut self, area: f32) {
-        self.metric_builder.visual_minimal_area_py(area);
-    }
+        #[pyo3(text_signature = "($self, area)")]
+        pub(crate) fn visual_minimal_area(&mut self, area: f32) {
+            self.0.metric_builder.set_visual_minimal_area(area);
+        }
 
-    #[pyo3(name = "visual_minimal_quality_use", text_signature = "($self, q)")]
-    fn visual_minimal_quality_use_py(&mut self, q: f32) {
-        self.metric_builder.visual_minimal_quality_use_py(q);
-    }
+        #[pyo3(text_signature = "($self, q)")]
+        pub(crate) fn visual_minimal_quality_use(&mut self, q: f32) {
+            self.0.metric_builder.set_visual_minimal_quality_use(q);
+        }
 
-    #[pyo3(name = "positional_min_confidence", text_signature = "($self, conf)")]
-    fn positional_min_confidence_py(&mut self, conf: f32) {
-        self.metric_builder.positional_min_confidence_py(conf);
-    }
+        #[pyo3(text_signature = "($self, conf)")]
+        pub(crate) fn positional_min_confidence(&mut self, conf: f32) {
+            self.0.metric_builder.set_positional_min_confidence(conf);
+        }
 
-    #[pyo3(name = "visual_max_observations", text_signature = "($self, n)")]
-    fn visual_max_observations_py(&mut self, n: i64) {
-        self.metric_builder
-            .visual_max_observations_py(n.try_into().expect("Parameter must be a positive number"));
-    }
+        #[pyo3(text_signature = "($self, n)")]
+        pub(crate) fn visual_max_observations(&mut self, n: i64) {
+            self.0.metric_builder.set_visual_max_observations(
+                n.try_into().expect("Parameter must be a positive number"),
+            );
+        }
 
-    #[pyo3(name = "visual_minimal_quality_collect", text_signature = "($self, q)")]
-    fn visual_minimal_quality_collect_py(&mut self, q: f32) {
-        self.metric_builder.visual_minimal_quality_collect_py(q);
-    }
+        #[pyo3(text_signature = "($self, q)")]
+        pub(crate) fn visual_minimal_quality_collect(&mut self, q: f32) {
+            self.0.metric_builder.set_visual_minimal_quality_collect(q);
+        }
 
-    #[pyo3(
-        name = "visual_minimal_own_area_percentage_use",
-        text_signature = "($self, area)"
-    )]
-    fn visual_minimal_own_area_percentage_use_py(&mut self, area: f32) {
-        self.metric_builder
-            .visual_minimal_own_area_percentage_use_py(area);
-    }
+        #[pyo3(text_signature = "($self, area)")]
+        pub(crate) fn visual_minimal_own_area_percentage_use(&mut self, area: f32) {
+            self.0
+                .metric_builder
+                .set_visual_minimal_own_area_percentage_use(area);
+        }
 
-    #[pyo3(
-        name = "visual_minimal_own_area_percentage_collect",
-        text_signature = "($self, area)"
-    )]
-    fn visual_minimal_own_area_percentage_collect_py(&mut self, area: f32) {
-        self.metric_builder
-            .visual_minimal_own_area_percentage_collect_py(area);
-    }
+        #[pyo3(text_signature = "($self, area)")]
+        pub(crate) fn visual_minimal_own_area_percentage_collect(&mut self, area: f32) {
+            self.0
+                .metric_builder
+                .set_visual_minimal_own_area_percentage_collect(area);
+        }
 
-    #[classattr]
-    const __hash__: Option<Py<PyAny>> = None;
+        #[classattr]
+        const __hash__: Option<Py<PyAny>> = None;
 
-    fn __repr__(&self) -> String {
-        format!("{self:?}")
-    }
+        fn __repr__(&self) -> String {
+            format!("{:?}", self.0)
+        }
 
-    fn __str__(&self) -> String {
-        format!("{self:#?}")
+        fn __str__(&self) -> String {
+            format!("{:#?}", self.0)
+        }
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::trackers::sort::{PositionalMetricType, PyPositionalMetricType};
+    use crate::trackers::sort::python::PyPositionalMetricType;
+    use crate::trackers::sort::PositionalMetricType;
+    use crate::trackers::spatio_temporal_constraints::python::PySpatioTemporalConstraints;
     use crate::trackers::spatio_temporal_constraints::SpatioTemporalConstraints;
-    use crate::trackers::visual_sort::metric::{PyVisualSortMetricType, VisualSortMetricType};
+    use crate::trackers::visual_sort::metric::python::PyVisualSortMetricType;
+    use crate::trackers::visual_sort::metric::VisualSortMetricType;
+    use crate::trackers::visual_sort::options::python::PyVisualSortOptions;
     use crate::trackers::visual_sort::options::VisualSortOptions;
 
     #[test]
     fn visual_sort_options_builder() {
-        let (opts, metric) = dbg!(VisualSortOptions::new()
+        let (opts, metric) = dbg!(VisualSortOptions::default()
             .max_idle_epochs(3)
             .kept_history_length(10)
             .visual_metric(VisualSortMetricType::Euclidean(100.0))
             .positional_metric(PositionalMetricType::Mahalanobis)
             .visual_minimal_track_length(3)
             .visual_minimal_area(5.0)
             .visual_minimal_quality_use(0.45)
@@ -324,30 +332,30 @@
             .visual_minimal_own_area_percentage_use(0.1)
             .visual_minimal_own_area_percentage_collect(0.2)
             .spatio_temporal_constraints(
                 SpatioTemporalConstraints::default().constraints(&[(5, 7.0)])
             )
             .build());
 
-        let mut opts_builder = VisualSortOptions::new();
-        opts_builder.max_idle_epochs_py(3);
-        opts_builder.kept_history_length_py(10);
-        opts_builder.visual_metric_py(PyVisualSortMetricType::euclidean(100.0));
-        opts_builder.positional_metric_py(PyPositionalMetricType::maha());
-        opts_builder.visual_minimal_track_length_py(3);
-        opts_builder.visual_minimal_area_py(5.0);
-        opts_builder.visual_minimal_quality_use_py(0.45);
-        opts_builder.visual_minimal_quality_collect_py(0.5);
-        opts_builder.visual_max_observations_py(25);
-        opts_builder.positional_min_confidence_py(0.13);
-        opts_builder.visual_minimal_own_area_percentage_use_py(0.1);
-        opts_builder.visual_minimal_own_area_percentage_collect_py(0.2);
-        opts_builder.visual_min_votes_py(5);
-        let mut constraints = SpatioTemporalConstraints::default();
+        let mut opts_builder = PyVisualSortOptions::new();
+        opts_builder.max_idle_epochs(3);
+        opts_builder.kept_history_length(10);
+        opts_builder.visual_metric(PyVisualSortMetricType::euclidean(100.0));
+        opts_builder.positional_metric(PyPositionalMetricType::maha());
+        opts_builder.visual_minimal_track_length(3);
+        opts_builder.visual_minimal_area(5.0);
+        opts_builder.visual_minimal_quality_use(0.45);
+        opts_builder.visual_minimal_quality_collect(0.5);
+        opts_builder.visual_max_observations(25);
+        opts_builder.positional_min_confidence(0.13);
+        opts_builder.visual_minimal_own_area_percentage_use(0.1);
+        opts_builder.visual_minimal_own_area_percentage_collect(0.2);
+        opts_builder.visual_min_votes(5);
+        let mut constraints = PySpatioTemporalConstraints::new();
         constraints.add_constraints(vec![(5, 7.0)]);
-        opts_builder.spatio_temporal_constraints_py(constraints);
-        let (opts_py, metric_py) = dbg!(opts_builder.build());
+        opts_builder.spatio_temporal_constraints(constraints);
+        let (opts_py, metric_py) = dbg!(opts_builder.0.build());
 
         assert_eq!(format!("{:?}", opts), format!("{:?}", opts_py));
         assert_eq!(format!("{:?}", metric), format!("{:?}", metric_py));
     }
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/simple_api.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/simple_api.rs`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,25 @@
 use crate::trackers::tracker_api::TrackerAPI;
 use crate::trackers::visual_sort::metric::{VisualMetric, VisualMetricOptions};
 use crate::trackers::visual_sort::observation_attributes::VisualObservationAttributes;
 use crate::trackers::visual_sort::options::VisualSortOptions;
 use crate::trackers::visual_sort::track_attributes::{
     VisualAttributes, VisualAttributesUpdate, VisualSortLookup,
 };
-use crate::trackers::visual_sort::visual_sort_py::PyVisualSortObservationSet;
 use crate::trackers::visual_sort::voting::VisualVoting;
-use crate::trackers::visual_sort::{PyWastedVisualSortTrack, VisualSortObservation};
+use crate::trackers::visual_sort::VisualSortObservation;
 use crate::utils::clipping::bbox_own_areas::{
     exclusively_owned_areas, exclusively_owned_areas_normalized_shares,
 };
 use crate::voting::Voting;
-use pyo3::prelude::*;
 use rand::Rng;
 use std::sync::{Arc, RwLock, RwLockReadGuard, RwLockWriteGuard};
 
 // /// Easy to use Visual SORT tracker implementation
 // ///
-#[pyclass(text_signature = "(shards, opts)")]
 pub struct VisualSort {
     store: RwLock<TrackStore<VisualAttributes, VisualMetric, VisualObservationAttributes>>,
     wasted_store: RwLock<TrackStore<VisualAttributes, VisualMetric, VisualObservationAttributes>>,
     metric_opts: Arc<VisualMetricOptions>,
     track_opts: Arc<SortAttributesOptions>,
     auto_waste: AutoWaste,
     track_id: u64,
@@ -152,16 +149,16 @@
                                 VisualObservationAttributes::new(
                                     o.feature_quality.unwrap_or(1.0),
                                     o.bounding_box.clone(),
                                 )
                             },
                         );
 
-                        if let Some(feature) = o.feature {
-                            obs = obs.observation(Feature::from_vec(feature));
+                        if let Some(feature) = &o.feature {
+                            obs = obs.observation(Feature::from_vec(feature.to_vec()));
                         }
 
                         obs.track_attributes_update(VisualAttributesUpdate::new_init_with_scene(
                             epoch,
                             scene_id,
                             o.custom_object_id,
                         ))
@@ -234,15 +231,14 @@
 
     pub fn idle_tracks(&mut self) -> Vec<SortTrack> {
         self.idle_tracks_with_scene(0)
     }
 
     pub fn idle_tracks_with_scene(&mut self, scene_id: u64) -> Vec<SortTrack> {
         let store = self.store.read().unwrap();
-
         store
             .lookup(VisualSortLookup::IdleLookup(scene_id))
             .iter()
             .map(|(track_id, _status)| {
                 let shard = store.get_store(*track_id as usize);
                 let track = shard.get(track_id).unwrap();
                 SortTrack::from(track)
@@ -313,48 +309,24 @@
             observed_bbox: attrs.observed_boxes.back().unwrap().clone(),
             predicted_bbox: attrs.predicted_boxes.back().unwrap().clone(),
             length: attrs.track_length,
         }
     }
 }
 
-impl From<Track<VisualAttributes, VisualMetric, VisualObservationAttributes>>
-    for PyWastedVisualSortTrack
-{
-    fn from(track: Track<VisualAttributes, VisualMetric, VisualObservationAttributes>) -> Self {
-        let attrs = track.get_attributes();
-        PyWastedVisualSortTrack {
-            id: track.get_track_id(),
-            epoch: attrs.last_updated_epoch,
-            scene_id: attrs.scene_id,
-            length: attrs.track_length,
-            observed_bbox: attrs.observed_boxes.back().unwrap().clone(),
-            predicted_bbox: attrs.predicted_boxes.back().unwrap().clone(),
-            predicted_boxes: attrs.predicted_boxes.clone().into_iter().collect(),
-            observed_boxes: attrs.observed_boxes.clone().into_iter().collect(),
-            observed_features: attrs
-                .observed_features
-                .clone()
-                .iter()
-                .map(|f_opt| f_opt.as_ref().map(Vec::from_vec))
-                .collect(),
-        }
-    }
-}
-
 #[cfg(test)]
 mod tests {
     use crate::track::Observation;
     use crate::trackers::sort::{PositionalMetricType, VotingType};
     use crate::trackers::tracker_api::TrackerAPI;
     use crate::trackers::visual_sort::metric::VisualSortMetricType;
     use crate::trackers::visual_sort::observation_attributes::VisualObservationAttributes;
     use crate::trackers::visual_sort::options::VisualSortOptions;
     use crate::trackers::visual_sort::simple_api::VisualSort;
-    use crate::trackers::visual_sort::{PyWastedVisualSortTrack, VisualSortObservation};
+    use crate::trackers::visual_sort::{VisualSortObservation, WastedVisualSortTrack};
     use crate::utils::bbox::BoundingBox;
 
     #[test]
     fn visual_sort() {
         let opts = VisualSortOptions::default()
             .max_idle_epochs(3)
             .kept_history_length(3)
@@ -684,156 +656,185 @@
         assert_eq!(attrs.predicted_boxes.len(), 3);
         assert_eq!(attrs.observed_features.len(), 3);
 
         tracker.skip_epochs_for_scene(10, 5);
         let tracks = tracker
             .wasted()
             .into_iter()
-            .map(PyWastedVisualSortTrack::from)
+            .map(WastedVisualSortTrack::from)
             .collect::<Vec<_>>();
         dbg!(&tracks);
     }
 }
 
-#[pymethods]
-impl VisualSort {
-    #[new]
-    pub fn new_py(shards: i64, opts: &VisualSortOptions) -> Self {
-        assert!(shards > 0);
-        Self::new(shards.try_into().unwrap(), opts)
-    }
+#[cfg(feature = "python")]
+pub mod python {
+    use pyo3::prelude::*;
+
+    use crate::{
+        prelude::VisualSortObservation,
+        trackers::{
+            sort::python::PySortTrack,
+            tracker_api::TrackerAPI,
+            visual_sort::{
+                options::python::PyVisualSortOptions,
+                python::{PyVisualSortObservationSet, PyWastedVisualSortTrack},
+                WastedVisualSortTrack,
+            },
+        },
+    };
 
-    #[pyo3(name = "skip_epochs", signature = (n))]
-    pub fn skip_epochs_py(&mut self, n: i64) {
-        assert!(n > 0);
-        self.skip_epochs(n.try_into().unwrap())
-    }
+    use super::VisualSort;
 
-    #[pyo3(
-        name = "skip_epochs_for_scene",
-        signature = (scene_id, n)
-    )]
-    pub fn skip_epochs_for_scene_py(&mut self, scene_id: i64, n: i64) {
-        assert!(n > 0 && scene_id >= 0);
-        self.skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
-    }
+    #[pyclass(text_signature = "(shards, opts)")]
+    #[pyo3(name = "VisualSort")]
+    pub struct PyVisualSort(pub(crate) VisualSort);
+
+    #[pymethods]
+    impl PyVisualSort {
+        #[new]
+        pub fn new(shards: i64, opts: &PyVisualSortOptions) -> Self {
+            assert!(shards > 0);
+            Self(VisualSort::new(shards.try_into().unwrap(), &opts.0))
+        }
 
-    /// Get the amount of stored tracks per shard
-    ///
-    #[pyo3(name = "shard_stats", signature = ())]
-    pub fn shard_stats_py(&self) -> Vec<i64> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.active_shard_stats()
-                    .into_iter()
-                    .map(|e| i64::try_from(e).unwrap())
-                    .collect()
+        #[pyo3(signature = (n))]
+        pub fn skip_epochs(&mut self, n: i64) {
+            assert!(n > 0);
+            self.0.skip_epochs(n.try_into().unwrap())
+        }
+
+        #[pyo3(signature = (scene_id, n))]
+        pub fn skip_epochs_for_scene(&mut self, scene_id: i64, n: i64) {
+            assert!(n > 0 && scene_id >= 0);
+            self.0
+                .skip_epochs_for_scene(scene_id.try_into().unwrap(), n.try_into().unwrap())
+        }
+
+        /// Get the amount of stored tracks per shard
+        ///
+        #[pyo3(signature = ())]
+        pub fn shard_stats(&self) -> Vec<i64> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .active_shard_stats()
+                        .into_iter()
+                        .map(|e| i64::try_from(e).unwrap())
+                        .collect()
+                })
             })
-        })
-    }
+        }
 
-    /// Get the current epoch for `scene_id` == 0
-    ///
-    #[pyo3(name = "current_epoch", signature = ())]
-    pub fn current_epoch_py(&self) -> i64 {
-        self.current_epoch_with_scene(0).try_into().unwrap()
-    }
+        /// Get the current epoch for `scene_id` == 0
+        ///
+        #[pyo3(signature = ())]
+        pub fn current_epoch(&self) -> i64 {
+            self.0.current_epoch_with_scene(0).try_into().unwrap()
+        }
 
-    /// Get the current epoch for `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id
-    ///
-    #[pyo3(
-        name = "current_epoch_with_scene",
-        signature = (scene_id)
-    )]
-    pub fn current_epoch_with_scene_py(&self, scene_id: i64) -> isize {
-        assert!(scene_id >= 0);
-        self.current_epoch_with_scene(scene_id.try_into().unwrap())
-            .try_into()
-            .unwrap()
-    }
+        /// Get the current epoch for `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn current_epoch_with_scene(&self, scene_id: i64) -> isize {
+            assert!(scene_id >= 0);
+            self.0
+                .current_epoch_with_scene(scene_id.try_into().unwrap())
+                .try_into()
+                .unwrap()
+        }
 
-    /// Receive tracking information for observed bboxes of `scene_id` == 0
-    ///
-    /// # Parameters
-    /// * `bboxes` - bounding boxes received from a detector
-    ///
-    #[pyo3(name = "predict", signature = (observation_set))]
-    pub fn predict_py(&mut self, observation_set: &PyVisualSortObservationSet) -> Vec<SortTrack> {
-        self.predict_with_scene_py(0, observation_set)
-    }
+        /// Receive tracking information for observed bboxes of `scene_id` == 0
+        ///
+        /// # Parameters
+        /// * `bboxes` - bounding boxes received from a detector
+        ///
+        #[pyo3(signature = (observation_set))]
+        pub fn predict(
+            &mut self,
+            observation_set: &PyVisualSortObservationSet,
+        ) -> Vec<PySortTrack> {
+            unsafe { std::mem::transmute(self.0.predict_with_scene(0, &observation_set.0.inner)) }
+        }
 
-    /// Receive tracking information for observed bboxes of `scene_id`
-    ///
-    /// # Parameters
-    /// * `scene_id` - scene id provided by a user (class, camera id, etc...)
-    /// * `observation_set` - observation set
-    ///
-    #[pyo3(
-        name = "predict_with_scene",
-        signature = (scene_id, observation_set)
-    )]
-    pub fn predict_with_scene_py(
-        &mut self,
-        scene_id: i64,
-        observation_set: &PyVisualSortObservationSet,
-    ) -> Vec<SortTrack> {
-        assert!(scene_id >= 0);
-        let observations = observation_set
-            .inner
-            .iter()
-            .map(|e| {
-                VisualSortObservation::new(
-                    e.feature.as_ref(),
-                    e.feature_quality,
-                    e.bounding_box.clone(),
-                    e.custom_object_id,
-                )
-            })
-            .collect::<Vec<_>>();
+        /// Receive tracking information for observed bboxes of `scene_id`
+        ///
+        /// # Parameters
+        /// * `scene_id` - scene id provided by a user (class, camera id, etc...)
+        /// * `observation_set` - observation set
+        ///
+        #[pyo3(signature = (scene_id, observation_set))]
+        pub fn predict_with_scene(
+            &mut self,
+            scene_id: i64,
+            observation_set: &PyVisualSortObservationSet,
+        ) -> Vec<PySortTrack> {
+            assert!(scene_id >= 0);
+            let observations = observation_set
+                .0
+                .inner
+                .iter()
+                .map(|e| {
+                    VisualSortObservation::new(
+                        e.feature.as_deref(),
+                        e.feature_quality,
+                        e.bounding_box.clone(),
+                        e.custom_object_id,
+                    )
+                })
+                .collect::<Vec<_>>();
 
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.predict_with_scene(scene_id.try_into().unwrap(), &observations)
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(
+                        self.0
+                            .predict_with_scene(scene_id.try_into().unwrap(), &observations),
+                    )
+                })
             })
-        })
-    }
+        }
 
-    /// Remove all the tracks with expired life
-    ///
-    #[pyo3(name = "wasted", signature = ())]
-    pub fn wasted_py(&mut self) -> Vec<PyWastedVisualSortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.wasted()
-                    .into_iter()
-                    .map(PyWastedVisualSortTrack::from)
-                    .collect()
+        /// Remove all the tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn wasted(&mut self) -> Vec<PyWastedVisualSortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| {
+                    self.0
+                        .wasted()
+                        .into_iter()
+                        .map(WastedVisualSortTrack::from)
+                        .map(PyWastedVisualSortTrack)
+                        .collect()
+                })
             })
-        })
-    }
+        }
 
-    /// Clear all tracks with expired life
-    ///
-    #[pyo3(name = "clear_wasted", signature = ())]
-    pub fn clear_wasted_py(&mut self) {
-        Python::with_gil(|py| py.allow_threads(|| self.clear_wasted()));
-    }
+        /// Clear all tracks with expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn clear_wasted(&mut self) {
+            Python::with_gil(|py| py.allow_threads(|| self.0.clear_wasted()));
+        }
 
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks", signature = ())]
-    pub fn idle_tracks_py(&mut self) -> Vec<SortTrack> {
-        self.idle_tracks_with_scene_py(0)
-    }
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3(signature = ())]
+        pub fn idle_tracks(&mut self) -> Vec<PySortTrack> {
+            unsafe { std::mem::transmute(self.0.idle_tracks_with_scene(0)) }
+        }
 
-    /// Get idle tracks with not expired life
-    ///
-    #[pyo3(name = "idle_tracks_with_scene", signature = (scene_id))]
-    pub fn idle_tracks_with_scene_py(&mut self, scene_id: i64) -> Vec<SortTrack> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.idle_tracks_with_scene(scene_id.try_into().unwrap()))
-        })
+        /// Get idle tracks with not expired life
+        ///
+        #[pyo3(signature = (scene_id))]
+        pub fn idle_tracks_with_scene_py(&mut self, scene_id: i64) -> Vec<PySortTrack> {
+            Python::with_gil(|py| {
+                py.allow_threads(|| unsafe {
+                    std::mem::transmute(self.0.idle_tracks_with_scene(scene_id.try_into().unwrap()))
+                })
+            })
+        }
     }
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/track_attributes.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/track_attributes.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/visual_sort_py.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/visual_sort_py.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers/visual_sort/voting.rs` & `similari_trackers_rs-0.26.5/src/trackers/visual_sort/voting.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/trackers.rs` & `similari_trackers_rs-0.26.5/src/trackers.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/utils/clipping/bbox_own_areas.rs` & `similari_trackers_rs-0.26.5/src/utils/clipping/bbox_own_areas.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/utils/clipping/clipping_py.rs` & `similari_trackers_rs-0.26.5/src/utils/clipping/clipping_py.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-use crate::utils::bbox::Universal2DBox;
-use crate::utils::clipping::sutherland_hodgman_clip;
+use crate::utils::bbox::python::PyUniversal2DBox;
 use geo::{Area, CoordsIter, Polygon};
 use pyo3::prelude::*;
 
 #[derive(Debug)]
 #[pyclass]
 #[pyo3(name = "Polygon")]
-pub struct PyPolygon {
-    polygon: Polygon<f64>,
-}
-
-impl PyPolygon {
-    pub fn new(polygon: Polygon<f64>) -> Self {
-        Self { polygon }
-    }
-}
+pub struct PyPolygon(pub(crate) Polygon<f64>);
 
 #[pymethods]
 impl PyPolygon {
     #[pyo3(text_signature = "($self)")]
     pub fn get_points(&self) -> Vec<(f64, f64)> {
-        self.polygon.coords_iter().map(|c| (c.x, c.y)).collect()
+        self.0.coords_iter().map(|c| (c.x, c.y)).collect()
     }
 
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -36,40 +27,20 @@
 }
 
 #[pyfunction]
 #[pyo3(
     name = "sutherland_hodgman_clip",
     text_signature = "(subject, clipping)"
 )]
-pub fn sutherland_hodgman_clip_py(subject: Universal2DBox, clipping: Universal2DBox) -> PyPolygon {
-    let mut subject = subject;
-    let mut clipping = clipping;
-
-    if subject.angle.is_none() {
-        subject.rotate_py(0.0);
-    }
-
-    if clipping.angle.is_none() {
-        clipping.rotate_py(0.0);
-    }
-
-    if subject.get_vertices().is_none() {
-        subject.gen_vertices_py();
-    }
-
-    if clipping.get_vertices().is_none() {
-        clipping.gen_vertices_py();
-    }
-
-    let clip = sutherland_hodgman_clip(
-        subject.get_vertices().as_ref().unwrap(),
-        clipping.get_vertices().as_ref().unwrap(),
-    );
-    PyPolygon { polygon: clip }
+pub fn sutherland_hodgman_clip_py(
+    subject: PyUniversal2DBox,
+    clipping: PyUniversal2DBox,
+) -> PyPolygon {
+    PyPolygon(subject.0.sutherland_hodgman_clip(clipping.0))
 }
 
 #[pyfunction]
 #[pyo3(name = "intersection_area", text_signature = "(subject, clipping)")]
-pub fn intersection_area_py(subject: Universal2DBox, clipping: Universal2DBox) -> f64 {
+pub fn intersection_area_py(subject: PyUniversal2DBox, clipping: PyUniversal2DBox) -> f64 {
     let poly = sutherland_hodgman_clip_py(subject, clipping);
-    poly.polygon.unsigned_area()
+    poly.0.unsigned_area()
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/clipping.rs` & `similari_trackers_rs-0.26.5/src/utils/clipping.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 /// Python interface for `sutherland_hodgman_clip`
 ///
+#[cfg(feature = "python")]
 pub mod clipping_py;
 
 /// The function to calculate polygons solely owned by a bounding box
 ///
 pub mod bbox_own_areas;
 
 use geo::{Coord, CoordsIter, LineString, Polygon};
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_box.rs` & `similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_box.rs`

 * *Files 2% similar despite different names*

```diff
@@ -245,16 +245,18 @@
         let dist = f.distance(state, &new_bbox_2.into());
         let dist = Universal2DBoxKalmanFilter::calculate_cost(dist, false);
         dbg!(&dist);
         assert!(dist > CHI2INV95[4]);
     }
 }
 
+#[cfg(feature = "python")]
 pub mod python {
-    use crate::prelude::{BoundingBox, Universal2DBox};
+    use crate::prelude::Universal2DBox;
+    use crate::utils::bbox::python::{PyBoundingBox, PyUniversal2DBox};
     use crate::utils::kalman::kalman_2d_box::{Universal2DBoxKalmanFilter, DIM_2D_BOX_X2};
     use crate::utils::kalman::KalmanState;
     use pyo3::prelude::*;
 
     #[pyclass]
     #[pyo3(name = "Universal2DBoxKalmanFilter")]
     pub struct PyUniversal2DBoxKalmanFilter {
@@ -267,38 +269,38 @@
     pub struct PyUniversal2DBoxKalmanFilterState {
         state: KalmanState<{ DIM_2D_BOX_X2 }>,
     }
 
     #[pymethods]
     impl PyUniversal2DBoxKalmanFilterState {
         #[pyo3(signature = ())]
-        pub fn universal_bbox(&self) -> Universal2DBox {
-            Universal2DBox::try_from(self.state).unwrap()
+        pub fn universal_bbox(&self) -> PyUniversal2DBox {
+            PyUniversal2DBox(Universal2DBox::try_from(self.state).unwrap())
         }
 
         #[pyo3(signature = ())]
-        pub fn bbox(&self) -> PyResult<BoundingBox> {
-            self.universal_bbox().as_ltwh_py()
+        pub fn bbox(&self) -> PyResult<PyBoundingBox> {
+            self.universal_bbox().as_ltwh()
         }
     }
 
     #[pymethods]
     impl PyUniversal2DBoxKalmanFilter {
         #[new]
         #[pyo3(signature = (position_weight = 0.05, velocity_weight = 0.00625))]
         pub fn new(position_weight: f32, velocity_weight: f32) -> Self {
             Self {
                 filter: Universal2DBoxKalmanFilter::new(position_weight, velocity_weight),
             }
         }
 
         #[pyo3(signature = (bbox))]
-        pub fn initiate(&self, bbox: Universal2DBox) -> PyUniversal2DBoxKalmanFilterState {
+        pub fn initiate(&self, bbox: PyUniversal2DBox) -> PyUniversal2DBoxKalmanFilterState {
             PyUniversal2DBoxKalmanFilterState {
-                state: self.filter.initiate(&bbox),
+                state: self.filter.initiate(&bbox.0),
             }
         }
 
         #[pyo3(signature = (state))]
         pub fn predict(
             &self,
             state: PyUniversal2DBoxKalmanFilterState,
@@ -308,28 +310,28 @@
             }
         }
 
         #[pyo3(signature = (state, bbox))]
         pub fn update(
             &self,
             state: PyUniversal2DBoxKalmanFilterState,
-            bbox: Universal2DBox,
+            bbox: PyUniversal2DBox,
         ) -> PyUniversal2DBoxKalmanFilterState {
             PyUniversal2DBoxKalmanFilterState {
-                state: self.filter.update(&state.state, &bbox),
+                state: self.filter.update(&state.state, &bbox.0),
             }
         }
 
         #[pyo3(signature = (state, bbox))]
         pub fn distance(
             &self,
             state: PyUniversal2DBoxKalmanFilterState,
-            bbox: Universal2DBox,
+            bbox: PyUniversal2DBox,
         ) -> f32 {
-            self.filter.distance(state.state, &bbox)
+            self.filter.distance(state.state, &bbox.0)
         }
 
         #[staticmethod]
         #[pyo3(signature = (distance, inverted))]
         pub fn calculate_cost(distance: f32, inverted: bool) -> f32 {
             Universal2DBoxKalmanFilter::calculate_cost(distance, inverted)
         }
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point.rs` & `similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_point.rs`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
         dbg!(Point2::from(state));
 
         let dist = f.distance(&state, &Point2::from([2.0, 0.57]));
         dbg!(&dist);
     }
 }
 
+#[cfg(feature = "python")]
 pub mod python {
     use crate::utils::kalman::kalman_2d_point::{Point2DKalmanFilter, DIM_2D_POINT_X2};
     use crate::utils::kalman::KalmanState;
     use nalgebra::Point2;
     use pyo3::prelude::*;
 
     #[pyclass]
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/kalman/kalman_2d_point_vec.rs` & `similari_trackers_rs-0.26.5/src/utils/kalman/kalman_2d_point_vec.rs`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         distances
             .iter()
             .map(|d| Point2DKalmanFilter::calculate_cost(*d, inverted))
             .collect()
     }
 }
 
+#[cfg(feature = "python")]
 pub mod python {
     use crate::utils::kalman::kalman_2d_point::python::PyPoint2DKalmanFilterState;
     use crate::utils::kalman::kalman_2d_point_vec::Vec2DKalmanFilter;
     use nalgebra::Point2;
     use pyo3::prelude::*;
 
     #[pyclass]
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/kalman.rs` & `similari_trackers_rs-0.26.5/src/utils/kalman.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/src/utils/nms/nms_py.rs` & `similari_trackers_rs-0.26.5/src/utils/nms/nms_py.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use crate::utils::bbox::python::PyUniversal2DBox;
 use crate::utils::bbox::Universal2DBox;
 use crate::utils::nms::nms;
 use pyo3::prelude::*;
 
 /// # NMS Python interface
 ///
 /// The python function name is `nms`. When the function is called, the GIL is released until the end of its execution.
@@ -41,20 +42,24 @@
 */
 #[pyfunction]
 #[pyo3(
     name = "nms",
     signature = (detections, nms_threshold, score_threshold)
 )]
 pub fn nms_py(
-    detections: Vec<(Universal2DBox, Option<f32>)>,
+    detections: Vec<(PyUniversal2DBox, Option<f32>)>,
     nms_threshold: f32,
     score_threshold: Option<f32>,
-) -> Vec<Universal2DBox> {
+) -> Vec<PyUniversal2DBox> {
     Python::with_gil(|py| {
         py.allow_threads(|| {
+            let detections: Vec<(Universal2DBox, Option<f32>)> =
+                unsafe { std::mem::transmute(detections) };
+
             nms(&detections, nms_threshold, score_threshold)
                 .into_iter()
                 .cloned()
+                .map(PyUniversal2DBox)
                 .collect()
         })
     })
 }
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/nms.rs` & `similari_trackers_rs-0.26.5/src/utils/nms.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#[cfg(feature = "python")]
 pub mod nms_py;
 
 use crate::utils::bbox::Universal2DBox;
 use itertools::Itertools;
 use std::collections::HashSet;
 
 #[derive(Clone, Debug)]
```

### Comparing `similari_trackers_rs-0.26.4/src/utils/primitive.rs` & `similari_trackers_rs-0.26.5/src/utils/primitive.rs`

 * *Files identical despite different names*

### Comparing `similari_trackers_rs-0.26.4/PKG-INFO` & `similari_trackers_rs-0.26.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similari-trackers-rs
-Version: 0.26.4
+Version: 0.26.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Machine learning framework for building object trackers and similarity search engines
 Keywords: machine-learning,similarity,tracking,SORT,DeepSORT
 Home-Page: https://github.com/insight-platform/Similari
```

