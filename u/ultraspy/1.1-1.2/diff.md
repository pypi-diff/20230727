# Comparing `tmp/ultraspy-1.1.tar.gz` & `tmp/ultraspy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultraspy-1.1.tar", last modified: Fri Jun 30 16:46:58 2023, max compression
+gzip compressed data, was "ultraspy-1.2.tar", last modified: Thu Jul 27 08:45:44 2023, max compression
```

## Comparing `ultraspy-1.1.tar` & `ultraspy-1.2.tar`

### file list

```diff
@@ -1,632 +1,696 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.026367 ultraspy-1.1/
--rw-rw-rw-   0        0        0      256 2023-06-07 09:00:51.000000 ultraspy-1.1/.readthedocs.yml
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.124384 ultraspy-1.1/.tox/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.042948 ultraspy-1.1/.tox/docs/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.043849 ultraspy-1.1/.tox/docs/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.047892 ultraspy-1.1/.tox/docs/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.043849 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.271403 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-21 10:38:14.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.046882 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.309397 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.046882 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.319587 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.049959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.047892 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.048959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.340518 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-21 10:37:24.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-21 10:37:24.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.049959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.050959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.351050 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-21 10:37:25.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.051960 ultraspy-1.1/.tox/py310-cpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.051960 ultraspy-1.1/.tox/py310-cpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.052959 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.355168 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-21 10:45:09.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.367471 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.371548 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.092481 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.091421 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.091421 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.378622 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-21 10:44:26.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-21 10:44:26.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.093519 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.093519 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.380717 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-21 10:44:27.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.095517 ultraspy-1.1/.tox/py310-gpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.095517 ultraspy-1.1/.tox/py310-gpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.110788 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.105182 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.097035 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.098127 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.104134 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.103129 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.100127 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.423269 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
--rw-rw-rw-   0        0        0    11047 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
--rw-rw-rw-   0        0        0     9934 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
--rw-rw-rw-   0        0        0    11663 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
--rw-rw-rw-   0        0        0     1611 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.533382 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
--rw-rw-rw-   0        0        0     8406 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
--rw-rw-rw-   0        0        0     8480 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
--rw-rw-rw-   0        0        0     8529 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
--rw-rw-rw-   0        0        0     6005 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
--rw-rw-rw-   0        0        0     6193 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
--rw-rw-rw-   0        0        0     8389 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
--rw-rw-rw-   0        0        0     8452 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
--rw-rw-rw-   0        0        0     7714 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
--rw-rw-rw-   0        0        0    13661 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.557319 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.582777 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
--rw-rw-rw-   0        0        0    38255 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
--rw-rw-rw-   0        0        0    97459 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
--rw-rw-rw-   0        0        0    22413 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
--rw-rw-rw-   0        0        0    31573 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.794513 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
--rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
--rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
--rw-rw-rw-   0        0        0    17023 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
--rw-rw-rw-   0        0        0     9933 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
--rw-rw-rw-   0        0        0    20045 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
--rw-rw-rw-   0        0        0    26109 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
--rw-rw-rw-   0        0        0    27450 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
--rw-rw-rw-   0        0        0    35739 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
--rw-rw-rw-   0        0        0    71982 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
--rw-rw-rw-   0        0        0    47767 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
--rw-rw-rw-   0        0        0    51261 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
--rw-rw-rw-   0        0        0    31216 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
--rw-rw-rw-   0        0        0    32082 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
--rw-rw-rw-   0        0        0    34615 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
--rw-rw-rw-   0        0        0    38679 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
--rw-rw-rw-   0        0        0    22169 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
--rw-rw-rw-   0        0        0     5284 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
--rw-rw-rw-   0        0        0    26354 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
--rw-rw-rw-   0        0        0    28026 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
--rw-rw-rw-   0        0        0    21011 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.806202 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
--rw-rw-rw-   0        0        0    28426 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.816915 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
--rw-rw-rw-   0        0        0    42322 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.844151 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/
--rw-rw-rw-   0        0        0    31907 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
--rw-rw-rw-   0        0        0     2900 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
--rw-rw-rw-   0        0        0    18156 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.852347 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/
--rw-rw-rw-   0        0        0    29209 2023-06-21 12:46:33.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.107700 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.856858 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.109790 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.869560 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.109790 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.872644 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.112787 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.111788 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.112787 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.878716 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-21 12:45:19.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-21 12:45:19.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.113863 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.113863 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.881766 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-21 12:45:21.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.114863 ultraspy-1.1/.tox/py38-cpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.114863 ultraspy-1.1/.tox/py38-cpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.120386 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.116373 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.884808 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.118383 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.899297 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.119380 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.902334 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.122384 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.121385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.121385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.908453 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.122384 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.123385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.911577 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.124384 ultraspy-1.1/.tox/py38-gpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.125386 ultraspy-1.1/.tox/py38-gpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.140890 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.135675 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.126382 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.127505 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.133587 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.133587 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.130580 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.956167 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
--rw-rw-rw-   0        0        0    11047 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
--rw-rw-rw-   0        0        0     9934 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
--rw-rw-rw-   0        0        0    11663 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
--rw-rw-rw-   0        0        0     1611 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.086785 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
--rw-rw-rw-   0        0        0     8406 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
--rw-rw-rw-   0        0        0     8480 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
--rw-rw-rw-   0        0        0     8529 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
--rw-rw-rw-   0        0        0     6005 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
--rw-rw-rw-   0        0        0     6193 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
--rw-rw-rw-   0        0        0     8389 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
--rw-rw-rw-   0        0        0     8452 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
--rw-rw-rw-   0        0        0     7714 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
--rw-rw-rw-   0        0        0    13661 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.118214 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.147184 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
--rw-rw-rw-   0        0        0    38255 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
--rw-rw-rw-   0        0        0    97459 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
--rw-rw-rw-   0        0        0    22413 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
--rw-rw-rw-   0        0        0    31573 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.363725 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
--rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
--rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
--rw-rw-rw-   0        0        0    17023 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
--rw-rw-rw-   0        0        0     9933 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
--rw-rw-rw-   0        0        0    20045 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
--rw-rw-rw-   0        0        0    26109 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
--rw-rw-rw-   0        0        0    27450 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
--rw-rw-rw-   0        0        0    35739 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
--rw-rw-rw-   0        0        0    71982 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
--rw-rw-rw-   0        0        0    47767 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
--rw-rw-rw-   0        0        0    51261 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
--rw-rw-rw-   0        0        0    31216 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
--rw-rw-rw-   0        0        0    32082 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
--rw-rw-rw-   0        0        0    34615 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
--rw-rw-rw-   0        0        0    38679 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
--rw-rw-rw-   0        0        0    22169 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
--rw-rw-rw-   0        0        0     5284 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
--rw-rw-rw-   0        0        0    26354 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
--rw-rw-rw-   0        0        0    28026 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
--rw-rw-rw-   0        0        0    21011 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.376220 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
--rw-rw-rw-   0        0        0    28426 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.386321 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
--rw-rw-rw-   0        0        0    42322 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.408625 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/
--rw-rw-rw-   0        0        0    31907 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
--rw-rw-rw-   0        0        0     2900 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
--rw-rw-rw-   0        0        0    18156 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.419670 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/
--rw-rw-rw-   0        0        0    29209 2023-06-21 12:59:08.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.136671 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.419670 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-21 12:59:16.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.139845 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.430997 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.139845 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.436506 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.143888 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.141887 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.142895 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.442127 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-21 12:58:24.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-21 12:58:24.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.144892 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.144892 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.446133 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-21 12:58:25.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
--rw-rw-rw-   0        0        0       68 2022-08-03 15:17:56.000000 ultraspy-1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0      217 2023-06-30 16:44:31.000000 ultraspy-1.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2367 2023-04-20 15:30:24.000000 ultraspy-1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1091 2022-06-22 12:40:44.000000 ultraspy-1.1/LICENSE
--rw-rw-rw-   0        0        0      278 2023-04-20 15:30:24.000000 ultraspy-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3545 2023-06-30 16:46:58.026367 ultraspy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2023-06-07 11:18:20.000000 ultraspy-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.464228 ultraspy-1.1/docs/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.466234 ultraspy-1.1/docs/_static/
--rw-rw-rw-   0        0        0      235 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1119 2023-06-30 15:44:47.000000 ultraspy-1.1/docs/acknowledgements.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.497892 ultraspy-1.1/docs/algorithms/
--rw-rw-rw-   0        0        0     3530 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/das_algo.rst
--rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/fdmas_algo.rst
--rw-rw-rw-   0        0        0      187 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/index.rst
--rw-rw-rw-   0        0        0     2452 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/pdas_algo.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.536139 ultraspy-1.1/docs/api_references/
--rw-rw-rw-   0        0        0      488 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/beamformers.rst
--rw-rw-rw-   0        0        0      905 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/api_references/classes.rst
--rw-rw-rw-   0        0        0       94 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/gpu_utils.rst
--rw-rw-rw-   0        0        0      143 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/index.rst
--rw-rw-rw-   0        0        0       88 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/metrics.rst
--rw-rw-rw-   0        0        0     1624 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/api_references/ultraspy.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.587452 ultraspy-1.1/docs/architecture/
--rw-rw-rw-   0        0        0    11787 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/architecture/beamformer_class.rst
--rw-rw-rw-   0        0        0     4254 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/common_methods.rst
--rw-rw-rw-   0        0        0     1987 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/index.rst
--rw-rw-rw-   0        0        0      421 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/probe_class.rst
--rw-rw-rw-   0        0        0       65 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/reader_class.rst
--rw-rw-rw-   0        0        0       60 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/scan_class.rst
--rw-rw-rw-   0        0        0     2884 2023-06-21 10:05:36.000000 ultraspy-1.1/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.654499 ultraspy-1.1/docs/contribute/
--rw-rw-rw-   0        0        0     2037 2023-06-07 11:48:18.000000 ultraspy-1.1/docs/contribute/devops_routine.rst
--rw-rw-rw-   0        0        0      625 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/index.rst
--rw-rw-rw-   0        0        0     3923 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_beamformer.rst
--rw-rw-rw-   0        0        0      677 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_methods.rst
--rw-rw-rw-   0        0        0      911 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_setups_options.rst
--rw-rw-rw-   0        0        0     2456 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/preparation.rst
--rw-rw-rw-   0        0        0     1594 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/tdd.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.706507 ultraspy-1.1/docs/examples/
--rw-rw-rw-   0        0        0     9976 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/das.rst
--rw-rw-rw-   0        0        0     6125 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/doppler.rst
--rw-rw-rw-   0        0        0      327 2023-06-07 09:00:51.000000 ultraspy-1.1/docs/examples/index.rst
--rw-rw-rw-   0        0        0    12052 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/metrics.rst
--rw-rw-rw-   0        0        0     7211 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/examples/simu_data.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.816570 ultraspy-1.1/docs/images/
--rw-rw-rw-   0        0        0    34289 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/block_grid.png
--rw-rw-rw-   0        0        0   132410 2023-01-25 18:21:44.000000 ultraspy-1.1/docs/images/convex_delays.png
--rw-rw-rw-   0        0        0   114606 2023-01-25 18:21:44.000000 ultraspy-1.1/docs/images/convex_probe.png
--rw-rw-rw-   0        0        0    18675 2023-06-21 10:27:54.000000 ultraspy-1.1/docs/images/creatis_logo.png
--rw-rw-rw-   0        0        0    35256 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/das_algo.png
--rw-rw-rw-   0        0        0    32371 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/das_bmode.png
--rw-rw-rw-   0        0        0    54387 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/das_dam.png
--rw-rw-rw-   0        0        0   229452 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/doppler.png
--rw-rw-rw-   0        0        0    87019 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fdmas_optim_gpu.png
--rw-rw-rw-   0        0        0   180354 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fdmas_spectra.png
--rw-rw-rw-   0        0        0    12459 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fnumber.png
--rw-rw-rw-   0        0        0    99220 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/gpu_architecture.png
--rw-rw-rw-   0        0        0   110727 2023-06-21 10:17:27.000000 ultraspy-1.1/docs/images/image4us.png
--rw-rw-rw-   0        0        0    64454 2023-06-21 10:27:24.000000 ultraspy-1.1/docs/images/image4us_logo.png
--rw-rw-rw-   0        0        0    87661 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/interpolation_beamforming.png
--rw-rw-rw-   0        0        0    66458 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes.png
--rw-rw-rw-   0        0        0    31442 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes_axial.png
--rw-rw-rw-   0        0        0    46092 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes_lateral.png
--rw-rw-rw-   0        0        0    51462 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_masks.png
--rw-rw-rw-   0        0        0    74436 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_raw_data.png
--rw-rw-rw-   0        0        0    41500 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_snr_correct.png
--rw-rw-rw-   0        0        0    31289 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_snr_wrong.png
--rw-rw-rw-   0        0        0   260166 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_spectra.png
--rw-rw-rw-   0        0        0   299480 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/pdas_spectra.png
--rw-rw-rw-   0        0        0    24721 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/polar_system.png
--rw-rw-rw-   0        0        0    96279 2023-06-21 10:28:29.000000 ultraspy-1.1/docs/images/tpac_logo.jpg
--rw-rw-rw-   0        0        0   114889 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/ultraspy_classes.png
--rw-rw-rw-   0        0        0     3166 2023-06-21 10:31:57.000000 ultraspy-1.1/docs/index.rst
--rw-rw-rw-   0        0        0     4063 2023-06-07 11:21:30.000000 ultraspy-1.1/docs/installation.rst
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.856184 ultraspy-1.1/docs/tech_choices/
--rw-rw-rw-   0        0        0     3692 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/beamforming_choices.rst
--rw-rw-rw-   0        0        0     2436 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/gpu_beamformers.rst
--rw-rw-rw-   0        0        0     5834 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/gpu_configs.rst
--rw-rw-rw-   0        0        0      248 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/index.rst
--rw-rw-rw-   0        0        0      110 2023-04-20 15:30:24.000000 ultraspy-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 16:46:58.026367 ultraspy-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-06-30 16:44:39.000000 ultraspy-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.856184 ultraspy-1.1/src/
--rw-rw-rw-   0        0        0        0 2022-06-22 12:40:44.000000 ultraspy-1.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.866115 ultraspy-1.1/src/ultraspy/
--rw-rw-rw-   0        0        0      892 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/TODO.md
--rw-rw-rw-   0        0        0     1068 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.906328 ultraspy-1.1/src/ultraspy/beamformers/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/beamformers/__init__.py
--rw-rw-rw-   0        0        0    30236 2023-06-26 16:05:31.000000 ultraspy-1.1/src/ultraspy/beamformers/beamformer.py
--rw-rw-rw-   0        0        0    17908 2023-06-06 13:22:47.000000 ultraspy-1.1/src/ultraspy/beamformers/das.py
--rw-rw-rw-   0        0        0    26096 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/fdmas.py
--rw-rw-rw-   0        0        0     2381 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/options.py
--rw-rw-rw-   0        0        0    22921 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/pdas.py
--rw-rw-rw-   0        0        0     1105 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/beamformers/setups.py
--rw-rw-rw-   0        0        0      786 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/config.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.909850 ultraspy-1.1/src/ultraspy/cpu/
--rw-rw-rw-   0        0        0      642 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/__init__.py
--rw-rw-rw-   0        0        0     2702 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/display.py
--rw-rw-rw-   0        0        0     9390 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/doppler.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.156486 ultraspy-1.1/src/ultraspy/cpu/kernels/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.926119 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/__init__.py
--rw-rw-rw-   0        0        0     2804 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py
--rw-rw-rw-   0        0        0     1960 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/apodization.py
--rw-rw-rw-   0        0        0    13231 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/das.py
--rw-rw-rw-   0        0        0    16093 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/fdmas.py
--rw-rw-rw-   0        0        0     1808 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/interpolation.py
--rw-rw-rw-   0        0        0      457 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/maths_utils.py
--rw-rw-rw-   0        0        0    15618 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/pdas.py
--rw-rw-rw-   0        0        0     1133 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.943302 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py
--rw-rw-rw-   0        0        0     5983 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/das.py
--rw-rw-rw-   0        0        0     8235 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py
--rw-rw-rw-   0        0        0     5075 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py
--rw-rw-rw-   0        0        0     8892 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/pdas.py
--rw-rw-rw-   0        0        0     1097 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py
--rw-rw-rw-   0        0        0     2663 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/post_processing.py
--rw-rw-rw-   0        0        0     7395 2023-04-26 16:33:32.000000 ultraspy-1.1/src/ultraspy/cpu/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.956318 ultraspy-1.1/src/ultraspy/gpu/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/display.py
--rw-rw-rw-   0        0        0    12887 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/doppler.py
--rw-rw-rw-   0        0        0     3032 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/gpu_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.966356 ultraspy-1.1/src/ultraspy/gpu/kernels/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.977531 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/
--rw-rw-rw-   0        0        0     1742 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
--rw-rw-rw-   0        0        0     2656 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/apodization.cu
--rw-rw-rw-   0        0        0    18518 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/das.cu
--rw-rw-rw-   0        0        0    22384 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/fdmas.cu
--rw-rw-rw-   0        0        0     4039 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/interpolation.cu
--rw-rw-rw-   0        0        0    23418 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/pdas.cu
--rw-rw-rw-   0        0        0     2435 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu
--rw-rw-rw-   0        0        0     4641 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
--rw-rw-rw-   0        0        0     2298 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.988573 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/
--rw-rw-rw-   0        0        0     1600 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/color_map.cu
--rw-rw-rw-   0        0        0     2188 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
--rw-rw-rw-   0        0        0     3096 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
--rw-rw-rw-   0        0        0     4122 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
--rw-rw-rw-   0        0        0     1558 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/power_map.cu
--rw-rw-rw-   0        0        0     3749 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.988573 ultraspy-1.1/src/ultraspy/gpu/kernels/headers/
--rw-rw-rw-   0        0        0      124 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/headers/cupy_header.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.004622 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/
--rw-rw-rw-   0        0        0     1737 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/by2.cu
--rw-rw-rw-   0        0        0     7248 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/convolve.cu
--rw-rw-rw-   0        0        0     1681 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/divide_by.cu
--rw-rw-rw-   0        0        0     8193 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/flip.cu
--rw-rw-rw-   0        0        0     1274 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/get_modulo.cu
--rw-rw-rw-   0        0        0     3695 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/median_filter.cu
--rw-rw-rw-   0        0        0     1552 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/to_db.cu
--rw-rw-rw-   0        0        0     4802 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.010925 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/
--rw-rw-rw-   0        0        0     2288 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/down_mix.cu
--rw-rw-rw-   0        0        0     4618 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/filter0.cu
--rw-rw-rw-   0        0        0     2460 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_end_sig.cu
--rw-rw-rw-   0        0        0     2906 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_filter.cu
--rw-rw-rw-   0        0        0     2512 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_start_sig.cu
--rw-rw-rw-   0        0        0     2432 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal_kernels.py
--rw-rw-rw-   0        0        0     3413 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/utils.py
--rw-rw-rw-   0        0        0     2801 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/post_processing.py
--rw-rw-rw-   0        0        0    12741 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.022239 ultraspy-1.1/src/ultraspy/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/doppler_helpers.py
--rw-rw-rw-   0        0        0     4037 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/metrics_helpers.py
--rw-rw-rw-   0        0        0     6240 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/signal_helpers.py
--rw-rw-rw-   0        0        0    11815 2023-06-26 16:21:58.000000 ultraspy-1.1/src/ultraspy/helpers/transmit_delays_helpers.py
--rw-rw-rw-   0        0        0      530 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.026248 ultraspy-1.1/src/ultraspy/io/
--rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.041217 ultraspy-1.1/src/ultraspy/io/file_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/factory.py
--rw-rw-rw-   0        0        0     1267 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/file_loader.py
--rw-rw-rw-   0        0        0     2023 2023-06-26 15:49:38.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/h5_loader.py
--rw-rw-rw-   0        0        0     2063 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/mat_loader.py
--rw-rw-rw-   0        0        0     7828 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/rff256_loader.py
--rw-rw-rw-   0        0        0    26165 2023-06-29 12:01:56.000000 ultraspy-1.1/src/ultraspy/io/reader.py
--rw-rw-rw-   0        0        0    15946 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.046233 ultraspy-1.1/src/ultraspy/probes/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/probes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.056595 ultraspy-1.1/src/ultraspy/probes/configs/
--rw-rw-rw-   0        0        0      182 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/c5-2v.ini
--rw-rw-rw-   0        0        0      164 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l11-4v.ini
--rw-rw-rw-   0        0        0      165 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l11-5v.ini
--rw-rw-rw-   0        0        0      170 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l14-5w.ini
--rw-rw-rw-   0        0        0      160 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l7-4.ini
--rw-rw-rw-   0        0        0      208 2023-06-19 15:40:23.000000 ultraspy-1.1/src/ultraspy/probes/configs/mux_1024_8MHz.ini
--rw-rw-rw-   0        0        0      164 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/probes/configs/p4-2v.ini
--rw-rw-rw-   0        0        0     2635 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/convex_probe.py
--rw-rw-rw-   0        0        0     5382 2023-06-19 15:41:35.000000 ultraspy-1.1/src/ultraspy/probes/factory.py
--rw-rw-rw-   0        0        0     1571 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/linear_probe.py
--rw-rw-rw-   0        0        0     2359 2023-06-16 13:59:32.000000 ultraspy-1.1/src/ultraspy/probes/matricial_probe.py
--rw-rw-rw-   0        0        0     8325 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/probe.py
--rw-rw-rw-   0        0        0    17720 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/scan.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.076306 ultraspy-1.1/src/ultraspy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/__init__.py
--rw-rw-rw-   0        0        0      585 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/beamformers.py
--rw-rw-rw-   0        0        0     3648 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/linear_decomposition.py
--rw-rw-rw-   0        0        0     2331 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/masks.py
--rw-rw-rw-   0        0        0     1292 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/matplot.py
--rw-rw-rw-   0        0        0     3336 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/print.py
--rw-rw-rw-   0        0        0      495 2023-06-07 14:21:21.000000 ultraspy-1.1/src/ultraspy/utils/scan.py
--rw-rw-rw-   0        0        0      711 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/string.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.887743 ultraspy-1.1/src/ultraspy.egg-info/
--rw-rw-rw-   0        0        0     3545 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    24698 2023-06-30 16:46:55.000000 ultraspy-1.1/src/ultraspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.086353 ultraspy-1.1/tests/
--rw-rw-rw-   0        0        0     6137 2023-06-07 09:02:02.000000 ultraspy-1.1/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.146471 ultraspy-1.1/tests/test_cpu/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.216366 ultraspy-1.1/tests/test_cpu/beamformers/
--rw-rw-rw-   0        0        0     7493 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_beamformer.py
--rw-rw-rw-   0        0        0    51386 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_das.py
--rw-rw-rw-   0        0        0    14986 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_fdmas.py
--rw-rw-rw-   0        0        0    18333 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_pdas.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.267958 ultraspy-1.1/tests/test_cpu/helpers/
--rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_doppler_helpers.py
--rw-rw-rw-   0        0        0      674 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_signal_helpers.py
--rw-rw-rw-   0        0        0      295 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_transmit_delays_helpers.py
--rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.277541 ultraspy-1.1/tests/test_cpu/io/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.306916 ultraspy-1.1/tests/test_cpu/io/file_loaders/
--rw-rw-rw-   0        0        0      183 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_h5_loaders.py
--rw-rw-rw-   0        0        0      191 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_mat_loader.py
--rw-rw-rw-   0        0        0      203 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_rff256_loader.py
--rw-rw-rw-   0        0        0     1453 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/test_reader.py
--rw-rw-rw-   0        0        0    11386 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/test_doppler.py
--rw-rw-rw-   0        0        0     8264 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/test_metrics.py
--rw-rw-rw-   0        0        0     1093 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/test_post_processing.py
--rw-rw-rw-   0        0        0     1074 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/test_probes.py
--rw-rw-rw-   0        0        0     4333 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/test_scan.py
--rw-rw-rw-   0        0        0     6287 2023-04-26 16:33:32.000000 ultraspy-1.1/tests/test_cpu/test_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.357591 ultraspy-1.1/tests/test_cpu/utils/
--rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_linear_decomposition.py
--rw-rw-rw-   0        0        0     1478 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_masks.py
--rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_print_utils.py
--rw-rw-rw-   0        0        0      261 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_scans_utils.py
--rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_string.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.419695 ultraspy-1.1/tests/test_gpu/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.466396 ultraspy-1.1/tests/test_gpu/beamformers/
--rw-rw-rw-   0        0        0     6486 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_beamformer.py
--rw-rw-rw-   0        0        0    16206 2023-06-27 12:49:38.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_das.py
--rw-rw-rw-   0        0        0     7610 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_fdmas.py
--rw-rw-rw-   0        0        0     6963 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_pdas.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.476539 ultraspy-1.1/tests/test_gpu/helpers/
--rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_doppler_helpers.py
--rw-rw-rw-   0        0        0      872 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_signal_helpers.py
--rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.519386 ultraspy-1.1/tests/test_gpu/kernels/
--rw-rw-rw-   0        0        0      112 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_beamformers_kernels.py
--rw-rw-rw-   0        0        0     4328 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_doppler_kernels.py
--rw-rw-rw-   0        0        0     8108 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_operators_kernels.py
--rw-rw-rw-   0        0        0     3203 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_signal_kernels.py
--rw-rw-rw-   0        0        0      248 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_display.py
--rw-rw-rw-   0        0        0     4997 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_doppler.py
--rw-rw-rw-   0        0        0     3960 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/test_filtfilts.py
--rw-rw-rw-   0        0        0     1881 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_gpu_utils.py
--rw-rw-rw-   0        0        0      176 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_post_processing.py
--rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/test_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.526397 ultraspy-1.1/tests/test_gpu/utils/
--rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_linear_decomposition.py
--rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_print_utils.py
--rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_string_utils.py
--rw-rw-rw-   0        0        0      798 2023-06-30 15:51:44.000000 ultraspy-1.1/tox.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.178639 ultraspy-1.1/venv/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.178639 ultraspy-1.1/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.209871 ultraspy-1.1/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.191260 ultraspy-1.1/venv/Lib/site-packages/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.180640 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.180640 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.189267 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.188251 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.183729 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.563619 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
--rw-rw-rw-   0        0        0    11047 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
--rw-rw-rw-   0        0        0     9934 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
--rw-rw-rw-   0        0        0    11663 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
--rw-rw-rw-   0        0        0     1611 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.646607 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
--rw-rw-rw-   0        0        0     8406 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
--rw-rw-rw-   0        0        0     8480 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
--rw-rw-rw-   0        0        0     8529 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
--rw-rw-rw-   0        0        0     6005 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
--rw-rw-rw-   0        0        0     6193 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
--rw-rw-rw-   0        0        0     8389 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
--rw-rw-rw-   0        0        0     8452 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
--rw-rw-rw-   0        0        0     7714 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
--rw-rw-rw-   0        0        0    13661 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.665398 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.676482 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
--rw-rw-rw-   0        0        0    38255 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
--rw-rw-rw-   0        0        0    97459 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
--rw-rw-rw-   0        0        0    22413 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
--rw-rw-rw-   0        0        0    31573 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.886616 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/
--rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
--rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
--rw-rw-rw-   0        0        0    17023 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
--rw-rw-rw-   0        0        0     9933 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
--rw-rw-rw-   0        0        0    20045 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
--rw-rw-rw-   0        0        0    26109 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
--rw-rw-rw-   0        0        0    27450 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
--rw-rw-rw-   0        0        0    35739 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
--rw-rw-rw-   0        0        0    71982 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
--rw-rw-rw-   0        0        0    47767 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
--rw-rw-rw-   0        0        0    51261 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
--rw-rw-rw-   0        0        0    31216 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
--rw-rw-rw-   0        0        0    32082 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
--rw-rw-rw-   0        0        0    34615 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
--rw-rw-rw-   0        0        0    38679 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
--rw-rw-rw-   0        0        0    22169 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
--rw-rw-rw-   0        0        0     5284 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
--rw-rw-rw-   0        0        0    26354 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
--rw-rw-rw-   0        0        0    28026 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
--rw-rw-rw-   0        0        0    21011 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.898019 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
--rw-rw-rw-   0        0        0    28426 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.906567 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/
--rw-rw-rw-   0        0        0    42322 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.926133 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/
--rw-rw-rw-   0        0        0    31907 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu
--rw-rw-rw-   0        0        0     2900 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
--rw-rw-rw-   0        0        0    18156 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.936167 ultraspy-1.1/venv/Lib/site-packages/cupy/random/
--rw-rw-rw-   0        0        0    29209 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/random/cupy_distributions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.193259 ultraspy-1.1/venv/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.946589 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-02 15:39:03.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.195541 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.962426 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.195541 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.965490 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.199655 ultraspy-1.1/venv/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.197651 ultraspy-1.1/venv/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.198652 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.969894 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-02 15:39:09.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-02 15:39:09.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.199655 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.200650 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.969894 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-02 15:39:10.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.204212 ultraspy-1.1/venv/Lib/site-packages/~-mpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.202649 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.202649 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.976402 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-02 15:35:42.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-02 15:35:42.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.204212 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.205238 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.981145 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-02 15:35:43.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.205238 ultraspy-1.1/venv/Lib/site-packages/~umba/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.206751 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.208772 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.207759 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.006554 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/
--rw-rw-rw-   0        0        0      294 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/cuda_include.cu
--rw-rw-rw-   0        0        0      138 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/error.cu
--rw-rw-rw-   0        0        0      214 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/jitlink.cu
--rw-rw-rw-   0        0        0      172 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.208772 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.016536 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      292 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.212910 ultraspy-1.1/venv/Lib/site-packages/~umpy/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.210911 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.211910 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.025862 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.212910 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.213909 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.026367 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.166483 ultraspy-1.2/
+-rw-rw-rw-   0        0        0      256 2023-06-07 09:00:51.000000 ultraspy-1.2/.readthedocs.yml
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.184867 ultraspy-1.2/.tox/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.118576 ultraspy-1.2/.tox/docs/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.118576 ultraspy-1.2/.tox/docs/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.137896 ultraspy-1.2/.tox/docs/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.118576 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.319102 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 10:38:14.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.136801 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.374755 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 10:38:15.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 10:38:15.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 10:38:15.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 10:38:15.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.137896 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.384016 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 10:38:15.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.137896 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.137896 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.137896 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.413791 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 10:37:24.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 10:37:24.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.144149 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.144149 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.427881 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 10:37:25.000000 ultraspy-1.2/.tox/docs/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.147278 ultraspy-1.2/.tox/py310-cpu_tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.147278 ultraspy-1.2/.tox/py310-cpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.156003 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.148977 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.437299 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 10:45:09.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.151286 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.453666 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 10:45:10.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 10:45:10.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 10:45:10.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 10:45:10.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.151286 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.455212 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 10:45:10.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.156003 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.156003 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.156003 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.468086 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 10:44:26.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 10:44:26.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.156003 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.158393 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.471352 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 10:44:27.000000 ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.158393 ultraspy-1.2/.tox/py310-gpu_tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.158393 ultraspy-1.2/.tox/py310-gpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.172031 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.167519 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.158393 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.158393 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.167519 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.166960 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.163613 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.510544 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.650942 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.664993 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.681182 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.950439 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.975888 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.983465 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-06-21 12:46:31.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.035101 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-06-21 12:46:32.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-06-21 12:46:32.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-06-21 12:46:32.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.047974 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-06-21 12:46:33.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.168915 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.065412 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.170586 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.082389 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.170586 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.083959 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 12:46:14.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.173552 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.172031 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.173552 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.092481 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 12:45:19.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 12:45:19.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.174582 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.174582 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.099624 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 12:45:21.000000 ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.175087 ultraspy-1.2/.tox/py38-cpu_tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.175087 ultraspy-1.2/.tox/py38-cpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.179732 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.176988 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.099624 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.178415 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.114163 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.178415 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.117061 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 11:28:38.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.181211 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.180702 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.181211 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.119306 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 11:27:53.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 11:27:53.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.181211 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.183722 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.119306 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 11:27:53.000000 ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.184867 ultraspy-1.2/.tox/py38-gpu_tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.184867 ultraspy-1.2/.tox/py38-gpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.196435 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.191989 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.186149 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.187467 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.191989 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.190736 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.189460 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.161441 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.235830 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.253333 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.268907 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.469410 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.476314 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.482861 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-06-21 12:59:06.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.517934 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-06-21 12:59:07.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-06-21 12:59:07.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-06-21 12:59:07.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.534612 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-06-21 12:59:08.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.193353 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.534612 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 12:59:16.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.194547 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.553019 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 12:59:17.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 12:59:17.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 12:59:17.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 12:59:17.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.195807 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.557364 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 12:59:17.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.196942 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.196942 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.196942 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.565313 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 12:58:24.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 12:58:24.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.199352 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.200488 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.567773 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 12:58:25.000000 ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+-rw-rw-rw-   0        0        0       68 2022-08-03 15:17:56.000000 ultraspy-1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0      223 2023-07-13 16:34:15.000000 ultraspy-1.2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2367 2023-04-20 15:30:24.000000 ultraspy-1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1091 2022-06-22 12:40:44.000000 ultraspy-1.2/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-04-20 15:30:24.000000 ultraspy-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3609 2023-07-27 08:45:44.166483 ultraspy-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-20 13:22:21.000000 ultraspy-1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.609377 ultraspy-1.2/docs/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.625007 ultraspy-1.2/docs/_static/
+-rw-rw-rw-   0        0        0      235 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1252 2023-07-19 08:30:52.000000 ultraspy-1.2/docs/acknowledgements.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.691226 ultraspy-1.2/docs/algorithms/
+-rw-rw-rw-   0        0        0     4694 2023-07-13 09:36:57.000000 ultraspy-1.2/docs/algorithms/capon_algo.rst
+-rw-rw-rw-   0        0        0     3530 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/algorithms/das_algo.rst
+-rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/algorithms/fdmas_algo.rst
+-rw-rw-rw-   0        0        0      202 2023-07-13 09:04:37.000000 ultraspy-1.2/docs/algorithms/index.rst
+-rw-rw-rw-   0        0        0     2863 2023-07-13 10:06:20.000000 ultraspy-1.2/docs/algorithms/pdas_algo.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.745283 ultraspy-1.2/docs/api_references/
+-rw-rw-rw-   0        0        0      571 2023-07-19 14:40:10.000000 ultraspy-1.2/docs/api_references/beamformers.rst
+-rw-rw-rw-   0        0        0      905 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/api_references/classes.rst
+-rw-rw-rw-   0        0        0       94 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/api_references/gpu_utils.rst
+-rw-rw-rw-   0        0        0      143 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/api_references/index.rst
+-rw-rw-rw-   0        0        0       88 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/api_references/metrics.rst
+-rw-rw-rw-   0        0        0     2096 2023-07-19 15:08:27.000000 ultraspy-1.2/docs/api_references/ultraspy.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.831035 ultraspy-1.2/docs/architecture/
+-rw-rw-rw-   0        0        0    11787 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/architecture/beamformer_class.rst
+-rw-rw-rw-   0        0        0     4484 2023-07-19 15:09:28.000000 ultraspy-1.2/docs/architecture/common_methods.rst
+-rw-rw-rw-   0        0        0     1987 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/architecture/index.rst
+-rw-rw-rw-   0        0        0     2207 2023-07-14 16:10:42.000000 ultraspy-1.2/docs/architecture/probe_class.rst
+-rw-rw-rw-   0        0        0     1927 2023-07-19 14:38:40.000000 ultraspy-1.2/docs/architecture/reader_class.rst
+-rw-rw-rw-   0        0        0     1278 2023-07-14 16:35:29.000000 ultraspy-1.2/docs/architecture/scan_class.rst
+-rw-rw-rw-   0        0        0     2941 2023-07-13 09:36:33.000000 ultraspy-1.2/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:41.914435 ultraspy-1.2/docs/contribute/
+-rw-rw-rw-   0        0        0     2037 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/contribute/devops_routine.rst
+-rw-rw-rw-   0        0        0      625 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/contribute/index.rst
+-rw-rw-rw-   0        0        0     3923 2023-07-11 12:52:40.000000 ultraspy-1.2/docs/contribute/own_beamformer.rst
+-rw-rw-rw-   0        0        0      677 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/contribute/own_methods.rst
+-rw-rw-rw-   0        0        0      911 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/contribute/own_setups_options.rst
+-rw-rw-rw-   0        0        0     2456 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/contribute/preparation.rst
+-rw-rw-rw-   0        0        0     1594 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/contribute/tdd.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.037618 ultraspy-1.2/docs/examples/
+-rw-rw-rw-   0        0        0    10180 2023-07-19 09:19:58.000000 ultraspy-1.2/docs/examples/das.rst
+-rw-rw-rw-   0        0        0     6201 2023-07-19 09:21:03.000000 ultraspy-1.2/docs/examples/doppler.rst
+-rw-rw-rw-   0        0        0      351 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/examples/index.rst
+-rw-rw-rw-   0        0        0    12052 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/examples/metrics.rst
+-rw-rw-rw-   0        0        0     7211 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/examples/simu_data.rst
+-rw-rw-rw-   0        0        0     5254 2023-07-13 16:47:42.000000 ultraspy-1.2/docs/examples/torch_compatibility.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.181912 ultraspy-1.2/docs/images/
+-rw-rw-rw-   0        0        0    34289 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/block_grid.png
+-rw-rw-rw-   0        0        0    65413 2023-07-13 10:00:23.000000 ultraspy-1.2/docs/images/capon_cholesky.png
+-rw-rw-rw-   0        0        0    51011 2023-07-13 09:52:14.000000 ultraspy-1.2/docs/images/capon_gpu_allocation.png
+-rw-rw-rw-   0        0        0    20144 2023-07-13 09:13:40.000000 ultraspy-1.2/docs/images/capon_windows.png
+-rw-rw-rw-   0        0        0   132410 2023-01-25 18:21:44.000000 ultraspy-1.2/docs/images/convex_delays.png
+-rw-rw-rw-   0        0        0   114606 2023-01-25 18:21:44.000000 ultraspy-1.2/docs/images/convex_probe.png
+-rw-rw-rw-   0        0        0    18675 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/images/creatis_logo.png
+-rw-rw-rw-   0        0        0    35256 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/das_algo.png
+-rw-rw-rw-   0        0        0    32371 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/das_bmode.png
+-rw-rw-rw-   0        0        0    54387 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/das_dam.png
+-rw-rw-rw-   0        0        0   229452 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/images/doppler.png
+-rw-rw-rw-   0        0        0    87019 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/fdmas_optim_gpu.png
+-rw-rw-rw-   0        0        0   180354 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/fdmas_spectra.png
+-rw-rw-rw-   0        0        0    12459 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/fnumber.png
+-rw-rw-rw-   0        0        0    99220 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/gpu_architecture.png
+-rw-rw-rw-   0        0        0   110727 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/images/image4us.png
+-rw-rw-rw-   0        0        0    64454 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/images/image4us_logo.png
+-rw-rw-rw-   0        0        0    87661 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/interpolation_beamforming.png
+-rw-rw-rw-   0        0        0    66458 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_lobes.png
+-rw-rw-rw-   0        0        0    31442 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_lobes_axial.png
+-rw-rw-rw-   0        0        0    46092 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_lobes_lateral.png
+-rw-rw-rw-   0        0        0    51462 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_masks.png
+-rw-rw-rw-   0        0        0    74436 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_raw_data.png
+-rw-rw-rw-   0        0        0    41500 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_snr_correct.png
+-rw-rw-rw-   0        0        0    31289 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_snr_wrong.png
+-rw-rw-rw-   0        0        0   260166 2022-08-03 15:17:56.000000 ultraspy-1.2/docs/images/metrics_spectra.png
+-rw-rw-rw-   0        0        0   299480 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/images/pdas_spectra.png
+-rw-rw-rw-   0        0        0    24721 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/images/polar_system.png
+-rw-rw-rw-   0        0        0   402970 2023-07-14 16:10:08.000000 ultraspy-1.2/docs/images/probes.png
+-rw-rw-rw-   0        0        0    96279 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/images/tpac_logo.jpg
+-rw-rw-rw-   0        0        0   114889 2023-04-20 15:30:24.000000 ultraspy-1.2/docs/images/ultraspy_classes.png
+-rw-rw-rw-   0        0        0     3945 2023-07-20 13:22:21.000000 ultraspy-1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     4063 2023-06-30 16:50:55.000000 ultraspy-1.2/docs/installation.rst
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.233644 ultraspy-1.2/docs/tech_choices/
+-rw-rw-rw-   0        0        0     4175 2023-07-20 12:28:51.000000 ultraspy-1.2/docs/tech_choices/beamforming_choices.rst
+-rw-rw-rw-   0        0        0    10105 2023-07-13 12:01:26.000000 ultraspy-1.2/docs/tech_choices/gpu_beamformers.rst
+-rw-rw-rw-   0        0        0     5834 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/tech_choices/gpu_configs.rst
+-rw-rw-rw-   0        0        0      248 2023-04-26 14:04:14.000000 ultraspy-1.2/docs/tech_choices/index.rst
+-rw-rw-rw-   0        0        0      110 2023-04-20 15:30:24.000000 ultraspy-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:45:44.169310 ultraspy-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-07-13 11:37:21.000000 ultraspy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.247487 ultraspy-1.2/src/
+-rw-rw-rw-   0        0        0        0 2022-06-22 12:40:44.000000 ultraspy-1.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.281003 ultraspy-1.2/src/ultraspy/
+-rw-rw-rw-   0        0        0     1068 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.444704 ultraspy-1.2/src/ultraspy/beamformers/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/beamformers/__init__.py
+-rw-rw-rw-   0        0        0    30236 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/beamformers/beamformer.py
+-rw-rw-rw-   0        0        0    18562 2023-07-12 15:57:12.000000 ultraspy-1.2/src/ultraspy/beamformers/capon.py
+-rw-rw-rw-   0        0        0    17642 2023-07-20 15:57:00.000000 ultraspy-1.2/src/ultraspy/beamformers/das.py
+-rw-rw-rw-   0        0        0    25842 2023-07-20 15:58:29.000000 ultraspy-1.2/src/ultraspy/beamformers/fdmas.py
+-rw-rw-rw-   0        0        0     2430 2023-07-20 13:19:19.000000 ultraspy-1.2/src/ultraspy/beamformers/options.py
+-rw-rw-rw-   0        0        0    22667 2023-07-20 15:58:52.000000 ultraspy-1.2/src/ultraspy/beamformers/pdas.py
+-rw-rw-rw-   0        0        0     1157 2023-07-20 13:18:58.000000 ultraspy-1.2/src/ultraspy/beamformers/setups.py
+-rw-rw-rw-   0        0        0      786 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/config.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.484121 ultraspy-1.2/src/ultraspy/cpu/
+-rw-rw-rw-   0        0        0      642 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/cpu/__init__.py
+-rw-rw-rw-   0        0        0     2702 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/display.py
+-rw-rw-rw-   0        0        0    12872 2023-07-13 15:45:38.000000 ultraspy-1.2/src/ultraspy/cpu/doppler.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.210611 ultraspy-1.2/src/ultraspy/cpu/kernels/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.501876 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/__init__.py
+-rw-rw-rw-   0        0        0     2804 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py
+-rw-rw-rw-   0        0        0     1960 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/apodization.py
+-rw-rw-rw-   0        0        0    16395 2023-07-21 16:18:10.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/capon.py
+-rw-rw-rw-   0        0        0    13231 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/das.py
+-rw-rw-rw-   0        0        0    16093 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/fdmas.py
+-rw-rw-rw-   0        0        0     1808 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/interpolation.py
+-rw-rw-rw-   0        0        0      457 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/maths_utils.py
+-rw-rw-rw-   0        0        0    15618 2023-07-11 14:25:39.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/pdas.py
+-rw-rw-rw-   0        0        0     1133 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.559816 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py
+-rw-rw-rw-   0        0        0     5983 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/das.py
+-rw-rw-rw-   0        0        0     8235 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py
+-rw-rw-rw-   0        0        0     5075 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py
+-rw-rw-rw-   0        0        0     8892 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/pdas.py
+-rw-rw-rw-   0        0        0     1097 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py
+-rw-rw-rw-   0        0        0     2663 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/cpu/post_processing.py
+-rw-rw-rw-   0        0        0     7395 2023-04-26 16:33:32.000000 ultraspy-1.2/src/ultraspy/cpu/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.583369 ultraspy-1.2/src/ultraspy/gpu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/__init__.py
+-rw-rw-rw-   0        0        0     3257 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/display.py
+-rw-rw-rw-   0        0        0    16802 2023-07-21 16:22:04.000000 ultraspy-1.2/src/ultraspy/gpu/doppler.py
+-rw-rw-rw-   0        0        0     3032 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/gpu/gpu_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.665233 ultraspy-1.2/src/ultraspy/gpu/kernels/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.699076 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/
+-rw-rw-rw-   0        0        0     1742 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
+-rw-rw-rw-   0        0        0     2656 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/apodization.cu
+-rw-rw-rw-   0        0        0    26811 2023-07-21 16:18:36.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/capon.cu
+-rw-rw-rw-   0        0        0      311 2023-07-12 13:58:03.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/complex_utils.cu
+-rw-rw-rw-   0        0        0    18518 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/das.cu
+-rw-rw-rw-   0        0        0    22384 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/fdmas.cu
+-rw-rw-rw-   0        0        0     4039 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/interpolation.cu
+-rw-rw-rw-   0        0        0    23418 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/pdas.cu
+-rw-rw-rw-   0        0        0     2435 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu
+-rw-rw-rw-   0        0        0     4641 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
+-rw-rw-rw-   0        0        0     2620 2023-07-20 16:33:36.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers_kernels.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.708354 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/
+-rw-rw-rw-   0        0        0     1600 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/color_map.cu
+-rw-rw-rw-   0        0        0     2188 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
+-rw-rw-rw-   0        0        0     3096 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
+-rw-rw-rw-   0        0        0     4122 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
+-rw-rw-rw-   0        0        0     1558 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/power_map.cu
+-rw-rw-rw-   0        0        0     3749 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/doppler_kernels.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.710431 ultraspy-1.2/src/ultraspy/gpu/kernels/headers/
+-rw-rw-rw-   0        0        0      124 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/headers/cupy_header.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.715604 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/
+-rw-rw-rw-   0        0        0     1737 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/by2.cu
+-rw-rw-rw-   0        0        0     7449 2023-07-20 16:49:45.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/convolve.cu
+-rw-rw-rw-   0        0        0     1681 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/divide_by.cu
+-rw-rw-rw-   0        0        0     8186 2023-07-21 16:22:22.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/flip.cu
+-rw-rw-rw-   0        0        0     1274 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/get_modulo.cu
+-rw-rw-rw-   0        0        0     3718 2023-07-21 16:23:02.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/median_filter.cu
+-rw-rw-rw-   0        0        0     1552 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators/to_db.cu
+-rw-rw-rw-   0        0        0     4771 2023-07-21 14:19:00.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/operators_kernels.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.729664 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/
+-rw-rw-rw-   0        0        0     2288 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/down_mix.cu
+-rw-rw-rw-   0        0        0     5011 2023-07-20 16:49:00.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/filter0.cu
+-rw-rw-rw-   0        0        0     2572 2023-07-21 15:58:10.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/init_end_sig.cu
+-rw-rw-rw-   0        0        0     3094 2023-07-20 16:45:50.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/init_filter.cu
+-rw-rw-rw-   0        0        0     2698 2023-07-20 16:47:50.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal/init_start_sig.cu
+-rw-rw-rw-   0        0        0     2129 2023-07-20 16:32:03.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/signal_kernels.py
+-rw-rw-rw-   0        0        0     3413 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/gpu/kernels/utils.py
+-rw-rw-rw-   0        0        0     2801 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/gpu/post_processing.py
+-rw-rw-rw-   0        0        0    12593 2023-07-21 16:23:20.000000 ultraspy-1.2/src/ultraspy/gpu/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.759618 ultraspy-1.2/src/ultraspy/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/helpers/doppler_helpers.py
+-rw-rw-rw-   0        0        0     4037 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/helpers/metrics_helpers.py
+-rw-rw-rw-   0        0        0     6172 2023-07-21 16:21:13.000000 ultraspy-1.2/src/ultraspy/helpers/signal_helpers.py
+-rw-rw-rw-   0        0        0    11815 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/helpers/transmit_delays_helpers.py
+-rw-rw-rw-   0        0        0      530 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/helpers/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.769138 ultraspy-1.2/src/ultraspy/io/
+-rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.809130 ultraspy-1.2/src/ultraspy/io/file_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/factory.py
+-rw-rw-rw-   0        0        0     1267 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/file_loader.py
+-rw-rw-rw-   0        0        0     2023 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/h5_loader.py
+-rw-rw-rw-   0        0        0     1934 2023-07-21 16:23:28.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/mat_loader.py
+-rw-rw-rw-   0        0        0     7840 2023-07-24 13:08:26.000000 ultraspy-1.2/src/ultraspy/io/file_loaders/rff256_loader.py
+-rw-rw-rw-   0        0        0    26119 2023-07-24 13:04:14.000000 ultraspy-1.2/src/ultraspy/io/reader.py
+-rw-rw-rw-   0        0        0    15832 2023-07-24 13:06:33.000000 ultraspy-1.2/src/ultraspy/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.847565 ultraspy-1.2/src/ultraspy/probes/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/probes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.888983 ultraspy-1.2/src/ultraspy/probes/configs/
+-rw-rw-rw-   0        0        0      182 2023-01-25 18:21:44.000000 ultraspy-1.2/src/ultraspy/probes/configs/c5-2v.ini
+-rw-rw-rw-   0        0        0      164 2023-01-25 18:21:44.000000 ultraspy-1.2/src/ultraspy/probes/configs/l11-4v.ini
+-rw-rw-rw-   0        0        0      165 2023-01-25 18:21:44.000000 ultraspy-1.2/src/ultraspy/probes/configs/l11-5v.ini
+-rw-rw-rw-   0        0        0      170 2023-01-25 18:21:44.000000 ultraspy-1.2/src/ultraspy/probes/configs/l14-5w.ini
+-rw-rw-rw-   0        0        0      160 2023-01-25 18:21:44.000000 ultraspy-1.2/src/ultraspy/probes/configs/l7-4.ini
+-rw-rw-rw-   0        0        0      208 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/probes/configs/mux_1024_8MHz.ini
+-rw-rw-rw-   0        0        0      164 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/probes/configs/p4-2v.ini
+-rw-rw-rw-   0        0        0     2635 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/probes/convex_probe.py
+-rw-rw-rw-   0        0        0     5382 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/probes/factory.py
+-rw-rw-rw-   0        0        0     1571 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/probes/linear_probe.py
+-rw-rw-rw-   0        0        0     2359 2023-06-30 16:50:55.000000 ultraspy-1.2/src/ultraspy/probes/matricial_probe.py
+-rw-rw-rw-   0        0        0     8325 2023-04-26 14:04:14.000000 ultraspy-1.2/src/ultraspy/probes/probe.py
+-rw-rw-rw-   0        0        0    17720 2023-06-07 09:00:51.000000 ultraspy-1.2/src/ultraspy/scan.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.925050 ultraspy-1.2/src/ultraspy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/__init__.py
+-rw-rw-rw-   0        0        0      585 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/beamformers.py
+-rw-rw-rw-   0        0        0     3594 2023-07-24 13:08:26.000000 ultraspy-1.2/src/ultraspy/utils/linear_decomposition.py
+-rw-rw-rw-   0        0        0     2331 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/masks.py
+-rw-rw-rw-   0        0        0     1292 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/matplot.py
+-rw-rw-rw-   0        0        0     3336 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/print.py
+-rw-rw-rw-   0        0        0      527 2023-07-24 13:28:50.000000 ultraspy-1.2/src/ultraspy/utils/scan.py
+-rw-rw-rw-   0        0        0      711 2023-04-20 15:30:24.000000 ultraspy-1.2/src/ultraspy/utils/string.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.341308 ultraspy-1.2/src/ultraspy.egg-info/
+-rw-rw-rw-   0        0        0     3609 2023-07-27 08:45:30.000000 ultraspy-1.2/src/ultraspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    27481 2023-07-27 08:45:40.000000 ultraspy-1.2/src/ultraspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:45:30.000000 ultraspy-1.2/src/ultraspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-27 08:45:30.000000 ultraspy-1.2/src/ultraspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 08:45:30.000000 ultraspy-1.2/src/ultraspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.938020 ultraspy-1.2/tests/
+-rw-rw-rw-   0        0        0     6137 2023-06-07 09:02:02.000000 ultraspy-1.2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:42.998300 ultraspy-1.2/tests/test_cpu/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.051967 ultraspy-1.2/tests/test_cpu/beamformers/
+-rw-rw-rw-   0        0        0     7493 2023-06-07 09:00:51.000000 ultraspy-1.2/tests/test_cpu/beamformers/test_beamformer.py
+-rw-rw-rw-   0        0        0      944 2023-07-13 09:04:07.000000 ultraspy-1.2/tests/test_cpu/beamformers/test_capon.py
+-rw-rw-rw-   0        0        0    52861 2023-07-20 16:02:39.000000 ultraspy-1.2/tests/test_cpu/beamformers/test_das.py
+-rw-rw-rw-   0        0        0    14986 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/beamformers/test_fdmas.py
+-rw-rw-rw-   0        0        0    18333 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/beamformers/test_pdas.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.078633 ultraspy-1.2/tests/test_cpu/helpers/
+-rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/helpers/test_doppler_helpers.py
+-rw-rw-rw-   0        0        0      674 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/helpers/test_signal_helpers.py
+-rw-rw-rw-   0        0        0      295 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/helpers/test_transmit_delays_helpers.py
+-rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/helpers/test_windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.094159 ultraspy-1.2/tests/test_cpu/io/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.117148 ultraspy-1.2/tests/test_cpu/io/file_loaders/
+-rw-rw-rw-   0        0        0      183 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/io/file_loaders/test_h5_loaders.py
+-rw-rw-rw-   0        0        0      191 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/io/file_loaders/test_mat_loader.py
+-rw-rw-rw-   0        0        0      203 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/io/file_loaders/test_rff256_loader.py
+-rw-rw-rw-   0        0        0     1453 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/io/test_reader.py
+-rw-rw-rw-   0        0        0    11386 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/test_doppler.py
+-rw-rw-rw-   0        0        0     8264 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_cpu/test_metrics.py
+-rw-rw-rw-   0        0        0     1093 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/test_post_processing.py
+-rw-rw-rw-   0        0        0     1074 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/test_probes.py
+-rw-rw-rw-   0        0        0     4333 2023-06-07 09:00:51.000000 ultraspy-1.2/tests/test_cpu/test_scan.py
+-rw-rw-rw-   0        0        0     6287 2023-04-26 16:33:32.000000 ultraspy-1.2/tests/test_cpu/test_signal.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.157265 ultraspy-1.2/tests/test_cpu/utils/
+-rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/utils/test_linear_decomposition.py
+-rw-rw-rw-   0        0        0     1478 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/utils/test_masks.py
+-rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/utils/test_print_utils.py
+-rw-rw-rw-   0        0        0      261 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/utils/test_scans_utils.py
+-rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_cpu/utils/test_string.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.209329 ultraspy-1.2/tests/test_gpu/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.267685 ultraspy-1.2/tests/test_gpu/beamformers/
+-rw-rw-rw-   0        0        0     6486 2023-06-07 09:00:51.000000 ultraspy-1.2/tests/test_gpu/beamformers/test_beamformer.py
+-rw-rw-rw-   0        0        0     1459 2023-07-13 11:49:04.000000 ultraspy-1.2/tests/test_gpu/beamformers/test_capon.py
+-rw-rw-rw-   0        0        0    16206 2023-06-27 12:49:38.000000 ultraspy-1.2/tests/test_gpu/beamformers/test_das.py
+-rw-rw-rw-   0        0        0     7610 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_gpu/beamformers/test_fdmas.py
+-rw-rw-rw-   0        0        0     6963 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_gpu/beamformers/test_pdas.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.282436 ultraspy-1.2/tests/test_gpu/helpers/
+-rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/helpers/test_doppler_helpers.py
+-rw-rw-rw-   0        0        0      872 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/helpers/test_signal_helpers.py
+-rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/helpers/test_windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.319390 ultraspy-1.2/tests/test_gpu/kernels/
+-rw-rw-rw-   0        0        0      112 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/kernels/test_beamformers_kernels.py
+-rw-rw-rw-   0        0        0     4328 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/kernels/test_doppler_kernels.py
+-rw-rw-rw-   0        0        0     8108 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/kernels/test_operators_kernels.py
+-rw-rw-rw-   0        0        0     3203 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/kernels/test_signal_kernels.py
+-rw-rw-rw-   0        0        0      248 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/test_display.py
+-rw-rw-rw-   0        0        0     4997 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/test_doppler.py
+-rw-rw-rw-   0        0        0     3960 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_gpu/test_filtfilts.py
+-rw-rw-rw-   0        0        0     1881 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/test_gpu_utils.py
+-rw-rw-rw-   0        0        0      176 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/test_post_processing.py
+-rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.2/tests/test_gpu/test_signal.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.328217 ultraspy-1.2/tests/test_gpu/utils/
+-rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/utils/test_linear_decomposition.py
+-rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/utils/test_print_utils.py
+-rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.2/tests/test_gpu/utils/test_string_utils.py
+-rw-rw-rw-   0        0        0      798 2023-07-27 08:42:44.000000 ultraspy-1.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.228314 ultraspy-1.2/venv/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.230568 ultraspy-1.2/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.265478 ultraspy-1.2/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.238012 ultraspy-1.2/venv/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.231087 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.231087 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.236518 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.236518 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.233472 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.355872 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.424331 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.452802 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.467603 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.656319 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.679489 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.688044 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.719721 ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.735781 ultraspy-1.2/venv/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-02-22 11:49:00.000000 ultraspy-1.2/venv/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.239206 ultraspy-1.2/venv/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.735781 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-02 15:39:03.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.240969 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.746122 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-02 15:39:04.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-02 15:39:04.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-02 15:39:04.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-02 15:39:04.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.240969 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.753521 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-02 15:39:04.000000 ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.243993 ultraspy-1.2/venv/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.240969 ultraspy-1.2/venv/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.243993 ultraspy-1.2/venv/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.754039 ultraspy-1.2/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-07-19 13:06:01.000000 ultraspy-1.2/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-07-19 13:06:01.000000 ultraspy-1.2/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.245999 ultraspy-1.2/venv/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.245999 ultraspy-1.2/venv/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.754039 ultraspy-1.2/venv/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-07-19 13:06:02.000000 ultraspy-1.2/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.252600 ultraspy-1.2/venv/Lib/site-packages/ultraspy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.245999 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.252600 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.815843 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/
+-rw-rw-rw-   0        0        0     1742 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
+-rw-rw-rw-   0        0        0     2656 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/apodization.cu
+-rw-rw-rw-   0        0        0    18518 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/das.cu
+-rw-rw-rw-   0        0        0    22384 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/fdmas.cu
+-rw-rw-rw-   0        0        0     4039 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/interpolation.cu
+-rw-rw-rw-   0        0        0    23418 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/pdas.cu
+-rw-rw-rw-   0        0        0     2435 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/probe_distances.cu
+-rw-rw-rw-   0        0        0     4641 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.862529 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/
+-rw-rw-rw-   0        0        0     1600 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/color_map.cu
+-rw-rw-rw-   0        0        0     2188 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
+-rw-rw-rw-   0        0        0     3096 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
+-rw-rw-rw-   0        0        0     4122 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
+-rw-rw-rw-   0        0        0     1558 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/power_map.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.863808 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/headers/
+-rw-rw-rw-   0        0        0      124 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/headers/cupy_header.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:43.941827 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/
+-rw-rw-rw-   0        0        0     1737 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/by2.cu
+-rw-rw-rw-   0        0        0     7248 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/convolve.cu
+-rw-rw-rw-   0        0        0     1681 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/divide_by.cu
+-rw-rw-rw-   0        0        0     8193 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/flip.cu
+-rw-rw-rw-   0        0        0     1274 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/get_modulo.cu
+-rw-rw-rw-   0        0        0     3695 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/median_filter.cu
+-rw-rw-rw-   0        0        0     1552 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/to_db.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.004890 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/
+-rw-rw-rw-   0        0        0     2288 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/down_mix.cu
+-rw-rw-rw-   0        0        0     4618 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/filter0.cu
+-rw-rw-rw-   0        0        0     2460 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_end_sig.cu
+-rw-rw-rw-   0        0        0     2906 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_filter.cu
+-rw-rw-rw-   0        0        0     2512 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_start_sig.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.252600 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.068297 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/
+-rw-rw-rw-   0        0        0      182 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/c5-2v.ini
+-rw-rw-rw-   0        0        0      164 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/l11-4v.ini
+-rw-rw-rw-   0        0        0      165 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/l11-5v.ini
+-rw-rw-rw-   0        0        0      170 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/l14-5w.ini
+-rw-rw-rw-   0        0        0      160 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/l7-4.ini
+-rw-rw-rw-   0        0        0      208 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/mux_1024_8MHz.ini
+-rw-rw-rw-   0        0        0      164 2023-07-19 15:01:55.000000 ultraspy-1.2/venv/Lib/site-packages/ultraspy/probes/configs/p4-2v.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.256153 ultraspy-1.2/venv/Lib/site-packages/~-mpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.254818 ultraspy-1.2/venv/Lib/site-packages/~-mpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.254818 ultraspy-1.2/venv/Lib/site-packages/~-mpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.068297 ultraspy-1.2/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-02 15:35:42.000000 ultraspy-1.2/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-02 15:35:42.000000 ultraspy-1.2/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.256153 ultraspy-1.2/venv/Lib/site-packages/~-mpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.256153 ultraspy-1.2/venv/Lib/site-packages/~-mpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.068297 ultraspy-1.2/venv/Lib/site-packages/~-mpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-02 15:35:43.000000 ultraspy-1.2/venv/Lib/site-packages/~-mpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.257766 ultraspy-1.2/venv/Lib/site-packages/~umba/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.257766 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.260789 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.259782 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.115663 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/
+-rw-rw-rw-   0        0        0      294 2022-08-02 14:53:44.000000 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      138 2022-08-02 14:53:44.000000 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/error.cu
+-rw-rw-rw-   0        0        0      214 2022-08-02 14:53:44.000000 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/jitlink.cu
+-rw-rw-rw-   0        0        0      172 2022-08-02 14:53:44.000000 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.260789 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.131290 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      292 2022-08-02 14:53:44.000000 ultraspy-1.2/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.263474 ultraspy-1.2/venv/Lib/site-packages/~umpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.262024 ultraspy-1.2/venv/Lib/site-packages/~umpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.262024 ultraspy-1.2/venv/Lib/site-packages/~umpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.146909 ultraspy-1.2/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-05-03 12:33:57.000000 ultraspy-1.2/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-05-03 12:33:57.000000 ultraspy-1.2/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.263474 ultraspy-1.2/venv/Lib/site-packages/~umpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.263474 ultraspy-1.2/venv/Lib/site-packages/~umpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.146909 ultraspy-1.2/venv/Lib/site-packages/~umpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-05-03 12:33:57.000000 ultraspy-1.2/venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.268613 ultraspy-1.2/venv/Lib/site-packages/~~mpy/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.266585 ultraspy-1.2/venv/Lib/site-packages/~~mpy/core/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.266585 ultraspy-1.2/venv/Lib/site-packages/~~mpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.153709 ultraspy-1.2/venv/Lib/site-packages/~~mpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-02 15:39:09.000000 ultraspy-1.2/venv/Lib/site-packages/~~mpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-02 15:39:09.000000 ultraspy-1.2/venv/Lib/site-packages/~~mpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.268613 ultraspy-1.2/venv/Lib/site-packages/~~mpy/typing/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:40.268613 ultraspy-1.2/venv/Lib/site-packages/~~mpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:45:44.162770 ultraspy-1.2/venv/Lib/site-packages/~~mpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-02 15:39:10.000000 ultraspy-1.2/venv/Lib/site-packages/~~mpy/typing/tests/data/mypy.ini
```

### Comparing `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/CONTRIBUTING.rst` & `ultraspy-1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/LICENSE` & `ultraspy-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/PKG-INFO` & `ultraspy-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultraspy
-Version: 1.1
+Version: 1.2
 Summary: Ultrasound toolbox for GPU
 Home-page: https://gitlab.com/pecarlat/ultraspy
 Author: Pierre Ecarlat
 Author-email: pierre.ecarlat@gmail.com
 Project-URL: Documentation, https://ultraspy.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/pecarlat/ultraspy/-/issues/
 Keywords: ultrasound,python,beamforming,doppler
@@ -40,23 +40,23 @@
 
 Features
 ========
 - General beamforming methods, flexible to Radio-Frequency or In-phase
   Quadrature data, working on CPU and GPU. Mainly DAS and FDMAS for the
   plane-wave imaging, but also TFM for Beam Focusing imaging
 
-- Advanced beamforming methods (p-DAS or Capon (TODO)), with a dedicated
-  tutorial to understand how these are implemented and how to implement your
-  own methods
+- Advanced beamforming methods (p-DAS or Capon), with a dedicated tutorial to
+  understand how these are implemented and how to implement your own methods
 
 - Basic Doppler methods (Color and Power maps), and their dedicated utilities
   functions (matched filtering, RF to I/Qs conversion)
 
-- Advanced Doppler methods, such as Vector Doppler (TODO) or propositions for
-  alias-free alias-free Doppler velocities (dual-wavelength method)
+- Advanced Doppler methods, such as a proposition for alias-free alias-free
+  Doppler velocities (using dual-wavelength method). This still lacks of
+  methods, and should include Vector Doppler or so in future releases
 
 - Basic metrics for evaluation of the data quality (SNR), or of our beamforming
   algorithms (FWHM, PSL, CNR)
 
 
 Documentation
 =============
```

### Comparing `ultraspy-1.1/README.rst` & `ultraspy-1.2/src/ultraspy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: ultraspy
+Version: 1.2
+Summary: Ultrasound toolbox for GPU
+Home-page: https://gitlab.com/pecarlat/ultraspy
+Author: Pierre Ecarlat
+Author-email: pierre.ecarlat@gmail.com
+Project-URL: Documentation, https://ultraspy.readthedocs.io/en/latest/
+Project-URL: Bug Tracker, https://gitlab.com/pecarlat/ultraspy/-/issues/
+Keywords: ultrasound,python,beamforming,doppler
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 What is ultraspy?
 -----------------
 Ultraspy is a package designed to efficiently manipulate ultrasound data using
 GPU. The most common beamforming or Doppler methods are implemented (such as
 DAS, RF to I/Qs, Color/Power Doppler, ...), along with some state-of-the-art
 methods (Capon beamforming, Vector Doppler, alias-free Doppler velocity, ...).
 A set of metrics (PSL, FWHM, SNR) is also provided so anyone can validate the
 quality of their ultrasound data and beamforming operations.
 
 The package is designed to work with both RF and I/Q signals, in 2D or 3D, and
 with any type of probe (linear, convex, or matrix). The core code can run both
 on CPU and GPU, making it ideal for any real-time application. All beamforming
-parameters (f-number, compounding, apodization…) can be freely customized at
+parameters (f-number, compounding, apodizationâ€¦) can be freely customized at
 any time for research purposes.
 
 The package has been thought to be as flexible as possible, so that anyone
 could eventually clone it and add its own research methods and test it in real
 time. A set of tutorials is provided to facilitate user learning and adoption,
 along with some instruction on how to contribute to the lib if you feel like
 your research method should be added to help the community.
@@ -22,23 +40,23 @@
 
 Features
 ========
 - General beamforming methods, flexible to Radio-Frequency or In-phase
   Quadrature data, working on CPU and GPU. Mainly DAS and FDMAS for the
   plane-wave imaging, but also TFM for Beam Focusing imaging
 
-- Advanced beamforming methods (p-DAS or Capon (TODO)), with a dedicated
-  tutorial to understand how these are implemented and how to implement your
-  own methods
+- Advanced beamforming methods (p-DAS or Capon), with a dedicated tutorial to
+  understand how these are implemented and how to implement your own methods
 
 - Basic Doppler methods (Color and Power maps), and their dedicated utilities
   functions (matched filtering, RF to I/Qs conversion)
 
-- Advanced Doppler methods, such as Vector Doppler (TODO) or propositions for
-  alias-free alias-free Doppler velocities (dual-wavelength method)
+- Advanced Doppler methods, such as a proposition for alias-free alias-free
+  Doppler velocities (using dual-wavelength method). This still lacks of
+  methods, and should include Vector Doppler or so in future releases
 
 - Basic metrics for evaluation of the data quality (SNR), or of our beamforming
   algorithms (FWHM, PSL, CNR)
 
 
 Documentation
 =============
```

### Comparing `ultraspy-1.1/docs/algorithms/das_algo.rst` & `ultraspy-1.2/docs/algorithms/das_algo.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/algorithms/fdmas_algo.rst` & `ultraspy-1.2/docs/algorithms/fdmas_algo.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/algorithms/pdas_algo.rst` & `ultraspy-1.2/docs/algorithms/pdas_algo.rst`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,22 @@
 Same as for the baseband DMAS version, when we extend it to a degree p, we see
 on figure 3b that we don’t need any additional filtering. However, since we
 only do the p-th root of the signal magnitude and not its phase, the
 frequencies of our signal is only affected by the p-power step, which means
 that the new central frequency of our beamformed signal becomes
 :math:`p.f_{0}`.
 
-TODO: Should add Ecarlat paper
+An alternative has been proposed by [3], that preserves the central frequency
+of the beamformed signals to the original :math:`f_{0}`. This method is the
+default one, using the same formula as [1], but with the sign of a complex
+number defined as:
+
+.. math::
+    \text{sign}(s_n)=\frac{s_n}{|s_n|}=\frac{a_n . e^{j\phi_n}}{a_n}=e^{j\phi_n}
 
 
 - [1] A Nonlinear Beamformer Based on p-th Root Compression—Application to Plane
   Wave Ultrasound Imaging, Polichetti & al.
 - [2] Ultrasound Baseband Delay-Multiply-and-Sum (BB-DMAS) nonlinear Beamforming,
   Shen & al.
+- [3] BB p-DAS, an extension of p-DAS to baseband domain for Doppler imaging,
+  Ecarlat & al.
```

### Comparing `ultraspy-1.1/docs/api_references/classes.rst` & `ultraspy-1.2/docs/api_references/classes.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/api_references/ultraspy.rst` & `ultraspy-1.2/docs/api_references/ultraspy.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Main methods
 ============
 
+.. _api_signal:
+
 Signal methods
 --------------
 
 .. tabs::
 
     .. group-tab:: GPU version
 
@@ -27,14 +29,16 @@
         .. autofunction:: ultraspy.cpu.rf2iq
 
         .. autofunction:: ultraspy.cpu.matched_filter
 
         .. autofunction:: ultraspy.cpu.normalize
 
 
+.. _api_doppler:
+
 Doppler methods
 ---------------
 
 .. tabs::
 
     .. group-tab:: GPU version
 
@@ -42,24 +46,30 @@
 
         .. autofunction:: ultraspy.spatial_smoothing
 
         .. autofunction:: ultraspy.get_color_doppler_map
 
         .. autofunction:: ultraspy.get_power_doppler_map
 
+        .. autofunction:: ultraspy.gpu.doppler.dual_frequency_unalias
+
     .. group-tab:: CPU version
 
         .. autofunction:: ultraspy.cpu.apply_wall_filter
 
         .. autofunction:: ultraspy.cpu.spatial_smoothing
 
         .. autofunction:: ultraspy.cpu.get_color_doppler_map
 
         .. autofunction:: ultraspy.cpu.get_power_doppler_map
 
+        .. autofunction:: ultraspy.cpu.doppler.dual_frequency_unalias
+
+
+.. _api_display:
 
 Display methods
 ---------------
 
 .. tabs::
 
     .. group-tab:: GPU version
@@ -71,7 +81,23 @@
         .. autofunction:: ultraspy.get_doppler_colormap
 
     .. group-tab:: CPU version
 
         .. autofunction:: ultraspy.cpu.to_b_mode
 
         .. autofunction:: ultraspy.cpu.get_spectrum
+
+
+.. _api_postpro:
+
+Post-processing methods
+-----------------------
+
+.. tabs::
+
+    .. group-tab:: GPU version
+
+        .. autofunction:: ultraspy.distort_dynamic
+
+    .. group-tab:: CPU version
+
+        .. autofunction:: ultraspy.cpu.distort_dynamic
```

### Comparing `ultraspy-1.1/docs/architecture/beamformer_class.rst` & `ultraspy-1.2/docs/architecture/beamformer_class.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/architecture/common_methods.rst` & `ultraspy-1.2/docs/architecture/common_methods.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     # Call the CPU alternative
     out = us.cpu.some_method(input, ...)
 
 
 Signal-related methods
 ----------------------
-The detailed description can be found in the API reference (TODO).
+The detailed description can be found in the :ref:`API reference<api_signal>`.
 
 * :code:`down_mix`: Down-mixing operation, performs a phase rotation on our
   data to move the spectrum around 0 Hz (involving the returned signal to be
   complex).
 
 * :code:`filtfilt`: Butterworth filtfilt, greatly inspired by Matlab's filtfilt
   version, zero-phase forward and reverse digital filtering.
@@ -39,15 +39,15 @@
   reference signal which is supposed to match.
 
 * :code:`normalize`: Simply normalizes a signal to values between -1 and 1.
 
 
 Doppler-related methods
 -----------------------
-The detailed description can be found in the API reference (TODO).
+The detailed description can be found in the :ref:`API reference<api_doppler>`.
 
 * :code:`apply_wall_filter`: Applies a clutter filter along slow time. The
   clutter type can be either 'mean' (subtract the mean of the data), 'poly'
   (applies a polynomial filter) or 'hp_filter' (applies a high-pass butterworth
   filter).
 
 * :code:`spatial_smoothing`: Performs a spatial smoothing on data, using a
@@ -59,41 +59,45 @@
   doppler velocity using the Doppler formula. It also can perform a spatial
   smoothing of a given number of pixels.
 
 * :code:`get_power_doppler_map`: Computes the power doppler map, which is using
   the mean of squared values along slow time. The result is then returned in
   dB. It can also perform a spatial smoothing of a given number of pixels.
 
+* :code:`gpu.dual_frequency_unalias`: Uses the dual-frequency approach to
+  compute two Doppler map that can be matched together to remove aliasing
+  ambiguity.
+
 
 Displaying methods
 ------------------
-The detailed description can be found in the API reference (TODO).
+The detailed description can be found in the :ref:`API reference<api_display>`.
 
 * :code:`to_b_mode`: Computes the B-Mode of our beamformed data. Simply returns
   20 * log10(data).
 
 * :code:`get_spectrum`: Returns the spectrum of a data signal.
 
 * :code:`get_doppler_colormap`: Returns a color map proposition for Doppler,
   based on typical echographs, from blue (flow going away from the probe), to
   red (going toward to).
 
 
 Post-processing methods
 -----------------------
-The detailed description can be found in the API reference (TODO).
+The detailed description can be found in the :ref:`API reference<api_postpro>`.
 
 * :code:`distort_dynamic`: Post-processing method to distort the dynamic of a
   B-Mode image (already in dB). This is applying a mathematical function,
   either curved or sigmoid to distort the values of the image.
 
 
 Metrics methods
 ---------------
-The detailed description can be found in the API reference (TODO).
+The detailed description can be found in the :ref:`API reference<api_metrics>`.
 
 * :code:`metrics.signal_noise_ratio`: Returns the Signal to Noise ratio of the
   sample, based on the location of both the pulse and the noise.
 
 * :code:`metrics.get_full_width_at_half_maximum`: Returns the Full-Width at
   Half Maximum of a signal, given a focus index. It is basically the width of
   the focused lobe at -6dB.
```

### Comparing `ultraspy-1.1/docs/architecture/index.rst` & `ultraspy-1.2/docs/architecture/index.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/conf.py` & `ultraspy-1.2/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,18 @@
 }
 
 
 # -- Options for LaTex output -------------------------------------------------
 
 # Avoid blank page used for duplex printing.
 latex_elements = {
-  'extraclassoptions': 'openany,oneside'
+  'extraclassoptions': 'openany,oneside',
+  'preamble': r'''
+      \usepackage{mathdots}
+  '''
 }
 
 
 # -- Additional ---------------------------------------------------------------
 
 # This value contains a list of modules to be mocked up. This is useful when
 # some external dependencies are not met at build time and break the building
```

### Comparing `ultraspy-1.1/docs/contribute/devops_routine.rst` & `ultraspy-1.2/docs/contribute/devops_routine.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/contribute/index.rst` & `ultraspy-1.2/docs/contribute/index.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/contribute/own_beamformer.rst` & `ultraspy-1.2/docs/contribute/own_beamformer.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 the :code:`beamform_gpu` or :code:`beamform_cpu` methods (or, better, both).
 The 'clean' way to implement them is to use them to call the kernels of the
 beamforming directly. Those can be implemented along with others in either:
 
 - :code:`gpu/kernels/beamformers/xdas.cu` for the GPU kernel, in CUDA
 - :code:`cpu/kernels/numba_cores/xdas.py` for the CPU kernel, in Numba, using
   @nopython mode
-- :code:`cpu/kernels/numpy_cores/xdas.py` for the GPU kernel, in Numpy, using
+- :code:`cpu/kernels/numpy_cores/xdas.py` for the CPU kernel, in Numpy, using
   matricial operations
 
 The minimum arguments for the :code:`beamform` methods (both CPU and GPU) are
 the data and a scan, with the information of the pixels to beamform.
 
 
 Notes on CUDA kernels
```

### Comparing `ultraspy-1.1/docs/contribute/own_methods.rst` & `ultraspy-1.2/docs/contribute/own_methods.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/contribute/own_setups_options.rst` & `ultraspy-1.2/docs/contribute/own_setups_options.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/contribute/preparation.rst` & `ultraspy-1.2/docs/contribute/preparation.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/contribute/tdd.rst` & `ultraspy-1.2/docs/contribute/tdd.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/examples/das.rst` & `ultraspy-1.2/docs/examples/das.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 Delay And Sum
 =============
 
 Read data
 ---------
 In this example, we are going to go through a Delay And Sum (DAS) routine using
-`ultraspy` on raw RFs simulated data from the PICMUS challenge. Those
+`ultraspy` on raw RFs simulated data from the `PICMUS challenge
+<https://www.creatis.insa-lyon.fr/Challenge/IEEE_IUS_2016/>`_ (you can download
+them directly from their website, the one used here is the
+:code:`resolution_distorsion_simu_dataset_rf.hdf5` data file. Those
 Radio-Frequencies were simulated using FieldII on a few scatterers in an empty
 homogeneous medium. We provide a Reader object to read saved data.
 
 .. code-block:: python
     :linenos:
 
     from ultraspy.io.reader import Reader
```

### Comparing `ultraspy-1.1/docs/examples/doppler.rst` & `ultraspy-1.2/docs/examples/doppler.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .. _doppler_example:
 
 Doppler
 =======
 Detailed example of a color and power doppler on raw RF real data, scanning a
-rotating disk. Few steps will be seen very quickly, as we assume you've already
+rotating disk. Data can be found in `MUST <https://www.biomecardio.com/MUST/>`_
+directory Few steps will be seen very quickly, as we assume you've already
 checked out the :ref:`DAS example <das_example>`.
 
 
 Beamforming process
 -------------------
 
 We first read the data (`'must'` reader), initialize the scan we'd like to
```

### Comparing `ultraspy-1.1/docs/examples/metrics.rst` & `ultraspy-1.2/docs/examples/metrics.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/examples/simu_data.rst` & `ultraspy-1.2/docs/examples/simu_data.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/block_grid.png` & `ultraspy-1.2/docs/images/block_grid.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/convex_delays.png` & `ultraspy-1.2/docs/images/convex_delays.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/convex_probe.png` & `ultraspy-1.2/docs/images/convex_probe.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/creatis_logo.png` & `ultraspy-1.2/docs/images/creatis_logo.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/das_algo.png` & `ultraspy-1.2/docs/images/das_algo.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/das_bmode.png` & `ultraspy-1.2/docs/images/das_bmode.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/das_dam.png` & `ultraspy-1.2/docs/images/das_dam.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/doppler.png` & `ultraspy-1.2/docs/images/doppler.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/fdmas_optim_gpu.png` & `ultraspy-1.2/docs/images/fdmas_optim_gpu.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/fdmas_spectra.png` & `ultraspy-1.2/docs/images/fdmas_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/fnumber.png` & `ultraspy-1.2/docs/images/fnumber.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/gpu_architecture.png` & `ultraspy-1.2/docs/images/gpu_architecture.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/image4us.png` & `ultraspy-1.2/docs/images/image4us.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/image4us_logo.png` & `ultraspy-1.2/docs/images/image4us_logo.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/interpolation_beamforming.png` & `ultraspy-1.2/docs/images/interpolation_beamforming.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_lobes.png` & `ultraspy-1.2/docs/images/metrics_lobes.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_lobes_axial.png` & `ultraspy-1.2/docs/images/metrics_lobes_axial.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_lobes_lateral.png` & `ultraspy-1.2/docs/images/metrics_lobes_lateral.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_masks.png` & `ultraspy-1.2/docs/images/metrics_masks.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_raw_data.png` & `ultraspy-1.2/docs/images/metrics_raw_data.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_snr_correct.png` & `ultraspy-1.2/docs/images/metrics_snr_correct.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_snr_wrong.png` & `ultraspy-1.2/docs/images/metrics_snr_wrong.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/metrics_spectra.png` & `ultraspy-1.2/docs/images/metrics_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/pdas_spectra.png` & `ultraspy-1.2/docs/images/pdas_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/polar_system.png` & `ultraspy-1.2/docs/images/polar_system.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/tpac_logo.jpg` & `ultraspy-1.2/docs/images/tpac_logo.jpg`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/images/ultraspy_classes.png` & `ultraspy-1.2/docs/images/ultraspy_classes.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/index.rst` & `ultraspy-1.2/docs/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -31,34 +31,55 @@
 
 What can it do?
 ---------------
 - General beamforming methods, flexible to Radio-Frequency or In-phase
   Quadrature data, working on CPU and GPU. Mainly DAS and FDMAS for the
   plane-wave imaging, but also TFM for Beam Focusing imaging
 
-- Advanced beamforming methods (p-DAS or Capon (TODO)), with a dedicated
-  tutorial to understand how these are implemented and how to implement your
-  own methods
+- Advanced beamforming methods (p-DAS or Capon), with a dedicated tutorial to
+  understand how these are implemented and how to implement your own methods
 
 - Basic Doppler methods (Color and Power maps), and their dedicated utilities
   functions (matched filtering, RF to I/Qs conversion)
 
-- Advanced Doppler methods, such as Vector Doppler (TODO) or propositions for
-  alias-free alias-free Doppler velocities (dual-wavelength method)
+- Advanced Doppler methods, such as a proposition for alias-free alias-free
+  Doppler velocities (using dual-wavelength method). This still lacks of
+  methods, and should include Vector Doppler or so in future releases
 
 - Basic metrics for evaluation of the data quality (SNR), or of our beamforming
   algorithms (FWHM, PSL, CNR)
 
 
 Great, I'm in! What should I do?
 --------------------------------
 First thing first, you'll have to :ref:`install it<installation>`, then you can
 have a look to the :ref:`examples<examples>`. Enjoy! :-)
 
 
+Use ultraspy
+------------
+An IEEE IUS proceeding has been published to introduce \textit{ultraspy},
+please cite it whenever you use the library.
+
+P. Ecarlat, E. Carcreff, F. Varray, H. Liebgott, and B. Nicolas,
+“Get ready to spy on Ultrasound: Meet ultraspy”, in International Ultrasonics
+Symposium (IUS). IEEE, 2023
+
+::
+
+    @inproceedings{ecarlat2023ultraspy,
+        title={Get ready to {S}py on {U}ltrasound: {M}eet ultraspy},
+        author={Ecarlat, Pierre and Carcreff, Ewen and Varray, François and Liebgott, Hervé and Nicolas, Barbara},
+        booktitle={International Ultrasonics Symposium (IUS)},
+        pages={1--4},
+        year={2023},
+        organization={IEEE}
+    }
+
+
 Special thanks
 --------------
 The list of contributors and advisors can be found in the :ref:`dedicated
 section<thanks>`.
 
 .. image:: images/creatis_logo.png
    :height: 40
```

### Comparing `ultraspy-1.1/docs/installation.rst` & `ultraspy-1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/docs/tech_choices/beamforming_choices.rst` & `ultraspy-1.2/docs/tech_choices/beamforming_choices.rst`

 * *Files 16% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 beamform pixels out of bound, (2) pad the data by zero values, or (3) put the
 out of bound values of the vector to zero. We are doing the latest.
 
 .. image:: ../images/fnumber.png
    :width: 300
    :align: center
 
+When using a 2-dimensional f-number, the aperture is computed as a rectangle
+(it does the same as above, but for both the lateral and the elevational axes).
+This might be less precise than an "ovale" or "round" f-number, but:
 
-TODO: Add how we deal with convex
-
-TODO: Add emitted_aperture option
-
-TODO: Add 2D f# when done
+- it adds complexity to the computation process that we chose to avoid
+- this way is the one used by MUST, which make the comparisons easier
 
 
 Delay And Sum... or Mean?
 -------------------------
 In DAS, as its name states, we are summing the vector of delays for the
 reduction step. This works in practice, but since we are setting f#>0, every
 pixel will have a different number of elements to reduce depending on its depth
@@ -69,13 +69,15 @@
 dataset.
 
 .. image:: ../images/das_dam.png
    :width: 400
    :align: center
 
 
-TODO: This is why DAM affects the compound / reduce options
-
-
 Apodization
 -----------
-TODO: Explain the tukey window depending on f#
+In our algorithms, the apodization is applied to the raw focused data directly,
+before reduction (sum or mean). This means that the apodization window will be
+wider as wego deeper in the medium.
+
+Also, as for the borders of the medium, we consider the apodization window as
+wide as the other windows at the same depth.
```

### Comparing `ultraspy-1.1/docs/tech_choices/gpu_configs.rst` & `ultraspy-1.2/docs/tech_choices/gpu_configs.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/setup.py` & `ultraspy-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Contents of local files
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 
 setup(
     name='ultraspy',
-    version='1.1',
+    version='1.2',
     author='Pierre Ecarlat',
     author_email='pierre.ecarlat@gmail.com',
     description='Ultrasound toolbox for GPU',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pecarlat/ultraspy',
     project_urls={
```

### Comparing `ultraspy-1.1/src/ultraspy/__init__.py` & `ultraspy-1.2/src/ultraspy/__init__.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/beamformers/beamformer.py` & `ultraspy-1.2/src/ultraspy/beamformers/beamformer.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/beamformers/das.py` & `ultraspy-1.2/src/ultraspy/beamformers/das.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def beamform_gpu(self, d_data, scan):
         """Runs the DAS beamformer using cupy (CUDA kernel on GPU).
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but its last dimensions will be the one requested in
             scan.shape. If reduce option is set to False, it will also preserve
             the delays per elements (nb_received_elements, \\*scan.shape). If
             compound is set to False, it will also preserve the transmissions
@@ -147,15 +147,15 @@
         """Runs the DAS beamformer on a packet of data using cupy (CUDA kernel
         on GPU).
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_frames, nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but if compound and reduce are set to True, its shape
             would be (\\*scan.shape, nb_frames). If reduce or compound are set
             to False, their respective dimensions will be preserved in the first
             dimensions as for the ::code::`beamform` method above
@@ -260,38 +260,32 @@
             options['interpolation'], options['reduction'],
             options['emitted_aperture'], options['reduce'], options['compound'],
             self.is_same_probe)
 
     def _beamform_packet_numpy(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numpy beamforming kernel on a packet of frames.
 
-        TODO: I think the packet with no reduce / compound doesn't work here,
-              this should be checked / tested
-
         :param numpy.ndarray data: the data to beamform, either in float or
             complex, based on the beamforming mode. The shape should be
             (nb_frames, nb_transmissions, nb_emitted_elements, nb_time_samples)
         :param numpy.ndarray xs: the lateral coordinates of the pixels, ravelled
         :param numpy.ndarray ys: the elevational coordinates of the pixels,
             ravelled
         :param numpy.ndarray zs: the axial coordinates of the pixels, ravelled
         :param dict setups: the dictionary with the setups info
         :param dict options: the dictionary with the options info
 
         :returns: The beamformed data, of shape (nb_kept_transmissions,
             nb_kept_elements, nb_pixels, nb_frames)
         :return type: numpy.ndarray
         """
-        packet_size = data.shape[0]
-        packet = np.zeros((xs.size, packet_size))
-        for f in range(packet_size):
-            tmp = self._beamform_numpy(data[f], xs, ys, zs, setups, options)
-            packet = packet.astype(tmp.dtype)
-            packet[..., f] = tmp
-        return packet
+        p = []
+        for frame in data:
+            p.append(self._beamform_numpy(frame, xs, ys, zs, setups, options))
+        return np.moveaxis(np.array(p), 0, -1)
 
     ###########################################################################
     # Numba callers
     ###########################################################################
     def _beamform_numba(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numba beamforming kernel.
```

### Comparing `ultraspy-1.1/src/ultraspy/beamformers/fdmas.py` & `ultraspy-1.2/src/ultraspy/beamformers/fdmas.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         performed after computing the envelope, which will restore the scan to
         its original dimensions.
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but its last dimensions will be the one requested in
             scan.shape. If compound option is set to False, it will preserve
             the transmissions and look like (nb_transmissions, \\*scan.shape)
         :return type: cupy.array
@@ -205,15 +205,15 @@
         """Runs the FDMAS beamformer on a packet of data using cupy (CUDA
         kernel on GPU).
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_frames, nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but if compound and reduce are set to True, its shape
             would be (\\*scan.shape, nb_frames). If reduce or compound are set
             to False, their respective dimensions will be preserved in the first
             dimensions as for the ::code::`beamform` method above
@@ -442,37 +442,32 @@
             options['interpolation'], options['reduction'],
             options['emitted_aperture'], options['reduce'], options['compound'],
             self.is_same_probe)
 
     def _beamform_packet_numpy(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numpy beamforming kernel on a packet of frames.
 
-        TODO: I think the packet with no compound doesn't work here, this
-            should be checked / tested
-
         :param numpy.ndarray data: the data to beamform, either in float or
             complex, based on the beamforming mode. The shape should be
             (nb_frames, nb_transmissions, nb_emitted_elements, nb_time_samples)
         :param numpy.ndarray xs: the lateral coordinates of the pixels, ravelled
         :param numpy.ndarray ys: the elevational coordinates of the pixels,
             ravelled
         :param numpy.ndarray zs: the axial coordinates of the pixels, ravelled
         :param dict setups: the dictionary with the setups info
         :param dict options: the dictionary with the options info
 
         :returns: The beamformed data, of shape (nb_kept_transmissions,
             nb_kept_elements, nb_pixels, nb_frames)
         :return type: numpy.ndarray
         """
-        packet_size = data.shape[0]
-        packet = np.zeros((xs.size, packet_size), dtype=data.dtype)
-        for f in range(packet_size):
-            packet[..., f] = self._beamform_numpy(data[f], xs, ys, zs,
-                                                  setups, options)
-        return packet
+        p = []
+        for frame in data:
+            p.append(self._beamform_numpy(frame, xs, ys, zs, setups, options))
+        return np.moveaxis(np.array(p), 0, -1)
 
     ###########################################################################
     # Numba callers
     ###########################################################################
     def _beamform_numba(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numba beamforming kernel.
```

### Comparing `ultraspy-1.1/src/ultraspy/beamformers/options.py` & `ultraspy-1.2/src/ultraspy/beamformers/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Helpers needed for Beamformers, mainly used to deal with the available
 options (apodization, interpolation, ...). If you update this file, make sure
-you also add the relevant information within the (TODO).
+you also add the relevant information within the Architecture / Beamformer
+section in the documentation.
 """
 import numpy as np
 from enum import Enum
 
 
 # The default values for the options in our classes, the format is:
 # { name: (default_value, type, is_an_array?), ... }
```

### Comparing `ultraspy-1.1/src/ultraspy/beamformers/pdas.py` & `ultraspy-1.2/src/ultraspy/beamformers/pdas.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     def beamform_gpu(self, d_data, scan):
         """Runs the p-DAS beamformer using cupy (CUDA kernel on GPU).
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but its last dimensions will be the one requested in
             scan.shape. If compound option is set to False, it will preserve
             the transmissions and look like (nb_transmissions, \\*scan.shape)
         :return type: cupy.array
@@ -208,15 +208,15 @@
         """Runs the p-DAS beamformer on a packet of data using cupy (CUDA
         kernel on GPU).
 
         :param cupy.array d_data: The cupy.array data to beamform, stored on
             GPU, either in float or complex, based on the beamforming mode. The
             shape should be (nb_frames, nb_transmissions, nb_emitted_elements,
             nb_time_samples)
-        :param Scan scan: The  scan to beamform, with the pixels we are willing
+        :param Scan scan: The scan to beamform, with the pixels we are willing
             to process
 
         :returns: The beamformed data. Its shape depends on the beamforming
             options, but if compound and reduce are set to True, its shape
             would be (\\*scan.shape, nb_frames). If reduce or compound are set
             to False, their respective dimensions will be preserved in the first
             dimensions as for the ::code::`beamform` method above
@@ -388,37 +388,32 @@
             options['interpolation'], options['reduction'],
             options['emitted_aperture'], options['reduce'], options['compound'],
             self.is_same_probe)
 
     def _beamform_packet_numpy(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numpy beamforming kernel on a packet of frames.
 
-        TODO: I think the packet with no compound doesn't work here, this
-            should be checked / tested
-
         :param numpy.ndarray data: the data to beamform, either in float or
             complex, based on the beamforming mode. The shape should be
             (nb_frames, nb_transmissions, nb_emitted_elements, nb_time_samples)
         :param numpy.ndarray xs: the lateral coordinates of the pixels, ravelled
         :param numpy.ndarray ys: the elevational coordinates of the pixels,
             ravelled
         :param numpy.ndarray zs: the axial coordinates of the pixels, ravelled
         :param dict setups: the dictionary with the setups info
         :param dict options: the dictionary with the options info
 
         :returns: The beamformed data, of shape (nb_kept_transmissions,
             nb_kept_elements, nb_pixels, nb_frames)
         :return type: numpy.ndarray
         """
-        packet_size = data.shape[0]
-        packet = np.zeros((xs.size, packet_size), dtype=data.dtype)
-        for f in range(packet_size):
-            packet[..., f] = self._beamform_numpy(data[f], xs, ys, zs,
-                                                  setups, options)
-        return packet
+        p = []
+        for frame in data:
+            p.append(self._beamform_numpy(frame, xs, ys, zs, setups, options))
+        return np.moveaxis(np.array(p), 0, -1)
 
     ###########################################################################
     # Numba callers
     ###########################################################################
     def _beamform_numba(self, data, xs, ys, zs, setups, options):
         """Caller, will call Numba beamforming kernel.
```

### Comparing `ultraspy-1.1/src/ultraspy/config.py` & `ultraspy-1.2/src/ultraspy/config.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/__init__.py` & `ultraspy-1.2/src/ultraspy/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/display.py` & `ultraspy-1.2/src/ultraspy/cpu/display.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/doppler.py` & `ultraspy-1.2/src/ultraspy/cpu/doppler.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import scipy.signal
 import scipy.ndimage
 
 from .signal import _filtfilt_wn
 from ultraspy.helpers.doppler_helpers import get_polynomial_coefficients
 from ultraspy.helpers.windows_helpers import get_hamming_squared_kernel
 
+import ultraspy as us
+
 
 def apply_wall_filter(data, mode, degree=1, axis=-1):
     """Applies a clutter filter along slow time (last dimension of our data by
     default). Four modes are available:
 
         - none: when there are no wall filter to apply, doesn't do anything
         - mean: applies a basic mean filter (subtract the mean of the data
@@ -154,14 +156,53 @@
     :return type: numpy.ndarray
     """
     power = np.mean(np.abs(data) ** 2, axis=-1)
     power = spatial_smoothing(power, kernel, smoothing)
     return 10 * np.log10(power / np.max(power))
 
 
+def dual_frequency_unalias(data, beamformed_fs, f01, p, band, sound_speed, prf,
+                           smoothing='hamming', kernel=1):
+    """Computes two Doppler maps with different central frequencies, that can
+    be mapped together to propose an alias-free Color map. This is based on
+    works of Ecarlat et al., IUS 2022, "Alias-free color Doppler using chirps"
+
+    :param numpy.ndarray data: The beamformed IQs data
+    :param float beamformed_fs: The sampling frequency along the beamformed
+        signal, in Hz
+    :param float f01: The first central frequency to use, in Hz
+    :param int p: The p relation between f01 and f02
+    :param float band: The band of the filter, in Hz
+    :param float sound_speed: The speed of sound of the medium
+    :param float prf: The PRF used during the acquisition
+    :param str smoothing: The smoothing method to use (either hamming or median)
+    :param int kernel: The size of the squared kernel for smoothing
+
+    :returns: The unaliased color map
+    :return type: numpy.ndarray
+    """
+    # Get central frequencies and nyquist velocities
+    f02 = f01 * (p + 1) / p
+    nyquist_1 = sound_speed * prf / (4 * f01)
+    nyquist_2 = sound_speed * prf / (4 * f02)
+
+    # Central freq 1
+    iqs1 = _filtfilt_band(data, f01, beamformed_fs, band)
+    cmap1 = get_color_doppler_map(iqs1, nyquist_1,
+                                  smoothing=smoothing, kernel=kernel)
+
+    # Central freq 2
+    iqs2 = _filtfilt_band(data, f02, beamformed_fs, band)
+    cmap2 = get_color_doppler_map(iqs2, nyquist_2,
+                                  smoothing=smoothing, kernel=kernel)
+
+    # De-aliasing
+    return _unalias([cmap1, cmap2], [nyquist_1, nyquist_2], p)
+
+
 def _apply_mean_wall_filter(data, axis=-1):
     """Applies a basic mean filter on our data along slow time (default axis is
     the last one). It simply subtracts the mean of the pixels along slow time.
 
     :param numpy.ndarray data: The numpy array on which to perform the mean
         wall filter
     :param int axis: The axis on which to perform the clutter filter (slow time
@@ -225,7 +266,54 @@
         dimension), default to -1
 
     :returns: The filtered data along slow time.
     :return type: numpy.ndarray
     """
     w_n = np.array(w_n)
     return _filtfilt_wn(data, w_n, 'high', 5, axis=axis)
+
+
+def _filtfilt_band(data, cutoff, sampling_freq, band, axis=-2):
+    """Filters an IQs map along the axial dimension. The band filtering is
+    performed between [cutoff - band / 2 ; cutoff + band / 2].
+
+    :param numpy.ndarray data: The beamformed IQs to filter (along axial axis)
+    :param float cutoff: The cutoff frequency, in Hz
+    :param float sampling_freq: The beamformed sampling frequency, in Hz
+    :param float band: The band of the filter, in Hz
+    :param int axis: The axis on which to perform the filtering
+
+    :returns: The filtered data along axial time.
+    :return type: numpy.ndarray
+    """
+    lf = cutoff - band / 2
+    hf = cutoff + band / 2
+    if lf / (sampling_freq / 2) > 0.1:
+        data = us.cpu.filtfilt(data, lf, sampling_freq, 'high', axis=axis)
+    if hf / (sampling_freq / 2) < 0.9:
+        data = us.cpu.filtfilt(data, hf, sampling_freq, 'low', axis=axis)
+    return data
+
+
+def _unalias(cmaps, nyquists, p):
+    """Conversion using the lookup tables, for Alias free.
+
+    :param list cmaps: The Doppler color maps of each central frequencies
+    :param list nyquists: The list of nyquists of each central frequencies
+    :param int p: The p relation between f01 and f02
+
+    :returns: The unaliased map.
+    :return type: numpy.ndarray
+    """
+    q = p + 1
+
+    # Lookup table
+    cases = np.round(q * (cmaps[1] - cmaps[0]) / (2 * nyquists[0]))
+    nn1 = cases.copy()
+    nn1[(cases == -2) | (cases == 2)] = 0
+    nn2 = cases.copy()
+    nn2[cases == -2] = 1
+    nn2[cases == 2] = -1
+
+    # Unaliased map
+    return (p / (p + q)) * (cmaps[0] + (q / p) * cmaps[1] +
+                            2 * nyquists[0] * (nn1 + nn2))
```

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/apodization.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/apodization.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/das.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/fdmas.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/interpolation.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/interpolation.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/pdas.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/pdas.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     :param int reduce: Not implemented in FDMAS, always True
     :param int compound: If set to 1 (True), we compound the data
     :param int is_same_probe: If True, the emitted and received probes are the
         same
 
     :returns: Beamformed grid of shape (1, 1, nb_p,). If the `compound` option
         is set to False, the transmission dimension is preserved, leading to
-        the shape (nb_t, 1, nb_p). `reduce` needs to be performed using FDMAS
+        the shape (nb_t, 1, nb_p). `reduce` needs to be performed using p-DAS
     :return type: numpy.ndarray
     """
     # Probes for emission / reception
     _, e_nb_elements = emitted_probe[0].shape
     nb_t, r_nb_elements = received_probe[0].shape
 
     e_dist2x = np.zeros(e_nb_elements)
```

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/das.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/pdas.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py` & `ultraspy-1.2/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/post_processing.py` & `ultraspy-1.2/src/ultraspy/cpu/post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/cpu/signal.py` & `ultraspy-1.2/src/ultraspy/cpu/signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/display.py` & `ultraspy-1.2/src/ultraspy/gpu/display.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/doppler.py` & `ultraspy-1.2/src/ultraspy/gpu/doppler.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ultraspy.helpers.doppler_helpers import get_polynomial_coefficients
 from ultraspy.helpers.windows_helpers import get_hamming_squared_kernel
 import ultraspy as us
 
 from ultraspy.config import cfg
 if cfg.GPU_AVAILABLE:
+    import cupy as cp
     import cupyx.scipy.ndimage
 
     from ultraspy.gpu import gpu_utils
     from ultraspy.gpu.kernels.operators_kernels import (k_divide_by,
                                                         k_power_to_db,
                                                         k_max,
                                                         k_convolve2d)
@@ -91,16 +92,16 @@
 
         - hamming: Performs a convolution with a squared hamming window of size
           (k_size, k_size)
         - median: applies a median filter on a squared spatial matrix (of size
           (k_size, k_size)). If complex numbers, do the median of both real and
           imaginary parts separately
 
-    TODO: Median smoother is very slow for big sizes (expected by cupyx, as
-        detailed in github.com/cupy/cupy/issues/6453)
+    Note: Median smoother is very slow for big sizes (expected by cupyx, as
+          detailed in github.com/cupy/cupy/issues/6453)
 
     :param cupy.array d_data: The 2D GPUArray data stored on GPU, of dtype
         complex64 or float32
     :param int k_size: The kernel size. Works better if it is an odd number, as
         the kernel can be centered on each pixel.
     :param str window_type: The name of the windowing function to use, only
         'hamming' (default) and 'median' are supported for now.
@@ -144,23 +145,30 @@
             # d_tmp = gpu_utils.initialize_empty(d_data.shape, d_data.dtype)
             # g_dim, b_dim = gpu_utils.compute_flat_grid_size(nb_x * nb_y)
             # k_median_filter(g_dim, b_dim,
             #                 (d_data, d_tmp, np.uint32(nb_x), np.uint32(nb_y),
             #                  np.uint32(k_size)))
             # gpu_utils.set_values(d_data, d_tmp)
         else:
-            nb_x, nb_y = d_data.shape
-            k = get_hamming_squared_kernel(k_size)
-            d_tmp = gpu_utils.initialize_empty(d_data.shape, d_data.dtype)
-            d_kernel = gpu_utils.send_to_gpu(k, np.float32)
-            g_dim, b_dim = gpu_utils.compute_flat_grid_size(d_data.size)
-            k_convolve2d(g_dim, b_dim,
-                         (d_data, d_tmp, d_kernel, np.uint32(nb_x),
-                          np.uint32(nb_y), np.uint32(k_size)))
-            gpu_utils.set_values(d_data, d_tmp)
+            if d_data.ndim == 2:
+                nb_x, nb_y = d_data.shape
+                k = get_hamming_squared_kernel(k_size)
+                d_tmp = gpu_utils.initialize_empty(d_data.shape, d_data.dtype)
+                d_kernel = gpu_utils.send_to_gpu(k, np.float32)
+                g_dim, b_dim = gpu_utils.compute_flat_grid_size(d_data.size)
+                k_convolve2d(g_dim, b_dim,
+                             (d_data, d_tmp, d_kernel, np.uint32(nb_x),
+                              np.uint32(nb_y), np.uint32(k_size)))
+                gpu_utils.set_values(d_data, d_tmp)
+            else:
+                v = np.hamming(k_size)
+                k = (v[:, None] * v)[..., None] * (v[:, None] * v)
+                d_kernel = gpu_utils.send_to_gpu(k, np.float32)
+                d_tmp = cupyx.scipy.ndimage.convolve(d_data, d_kernel)
+                gpu_utils.set_values(d_data, d_tmp)
 
 
 def get_color_doppler_map(d_data, nyquist_velocity, smoothing='hamming',
                           kernel=1):
     """Computes the color doppler map, which is using the correlation of our
     data along slow time (last dimension of data), which are then converted to
     doppler velocity using the Doppler formula. It also can perform a spatial
@@ -229,14 +237,54 @@
     k_divide_by(g_dim, b_dim,
                 (d_power_doppler, np.float32(k_max(d_power_doppler)),
                  np.uint32(nb_pixels)))
     k_power_to_db(g_dim, b_dim, (d_power_doppler, np.uint32(nb_pixels)))
     return d_power_doppler
 
 
+def dual_frequency_unalias(d_data, beamformed_fs, f01, p, band, sound_speed,
+                           prf, smoothing='hamming', kernel=1):
+    """Computes two Doppler maps with different central frequencies, that can
+    be mapped together to propose an alias-free Color map. This is based on
+    works of Ecarlat et al., IUS 2022, "Alias-free color Doppler using chirps"
+
+    :param numpy.ndarray d_data: The GPUArray beamformed IQs data stored on
+        GPU, of dtype complex64
+    :param float beamformed_fs: The sampling frequency along the beamformed
+        signal, in Hz
+    :param float f01: The first central frequency to use, in Hz
+    :param int p: The p relation between f01 and f02
+    :param float band: The band of the filter, in Hz
+    :param float sound_speed: The speed of sound of the medium
+    :param float prf: The PRF used during the acquisition
+    :param str smoothing: The smoothing method to use (either hamming or median)
+    :param int kernel: The size of the squared kernel for smoothing
+
+    :returns: The unaliased color map
+    :return type: numpy.ndarray
+    """
+    # Get central frequencies and nyquist velocities
+    f02 = f01 * (p + 1) / p
+    nyquist_1 = sound_speed * prf / (4 * f01)
+    nyquist_2 = sound_speed * prf / (4 * f02)
+
+    # Central freq 1
+    d_iqs1 = _filtfilt_band(d_data, f01, beamformed_fs, band)
+    d_cmap1 = get_color_doppler_map(d_iqs1, nyquist_1,
+                                    smoothing=smoothing, kernel=kernel)
+
+    # Central freq 2
+    d_iqs2 = _filtfilt_band(d_data, f02, beamformed_fs, band)
+    d_cmap2 = get_color_doppler_map(d_iqs2, nyquist_2,
+                                    smoothing=smoothing, kernel=kernel)
+
+    # De-aliasing
+    return _unalias([d_cmap1, d_cmap2], [nyquist_1, nyquist_2], p)
+
+
 def _apply_mean_wall_filter(d_data):
     """Applies a basic mean filter on our data along slow time (last axis). It
     simply subtracts the mean of the pixels along slow time.
 
     :param cupy.array d_data: The GPUArray data stored on GPU, of dtype
         complex64
     """
@@ -253,16 +301,14 @@
 def _apply_poly_wall_filter(d_data, degree):
     """Applies a polynomial clutter filter on our data along slow time (should
     be the last axis). The polynomial regression consists in using orthogonal
     Legendre polynomial coefficients to remove the fitting polynomials from the
     data, which ends up to remove the low frequencies components. The degree is
     the upper degree of the polynomials we want to remove.
 
-    TODO: Test with the MemoryHandler
-
     :param cupy.array d_data: The GPUArray data stored on GPU, of dtype
         complex64
     :param int degree: The upper degree of the polynomials we want to remove
     """
     nb_pixels = int(np.prod(d_data.shape[:-1]))
     nb_frames = d_data.shape[-1]
     polys = get_polynomial_coefficients(nb_frames, degree)
@@ -278,15 +324,64 @@
 def _apply_hp_wall_filter(d_data, w_n):
     """Applies a high-pass butterworth filter on our data along slow time which
     should be the last dimension. The w_n parameter is the critical frequency
     where the gain will drop to 1 / sqrt(2). As we are working with digital
     filters, it is normalized from 0 to 1 where 1 is the Nyquist frequency. The
     clutter filter is performed on GPU, and will modify d_data directly.
 
-    TODO: There is still a choice that need to be done here: should we peak
-          pycuda_filtfilt2..? 3..? or 1?
-
     :param cupy.array d_data: The GPUArray data stored on GPU, of dtype
         complex64
     :param float w_n: The normalized critical frequency to use for filtering
     """
     us.gpu.signal._filtfilt_wn(d_data, w_n, 'high')
+
+
+def _filtfilt_band(d_data, cutoff, sampling_freq, band, axis=-2):
+    """Filters an IQs map along the axial dimension. The band filtering is
+    performed between [cutoff - band / 2 ; cutoff + band / 2].
+
+    :param numpy.ndarray d_data: The GPUArray beamformed IQs to filter (along
+        axial axis)
+    :param float cutoff: The cutoff frequency, in Hz
+    :param float sampling_freq: The beamformed sampling frequency, in Hz
+    :param float band: The band of the filter, in Hz
+    :param int axis: The axis on which to perform the filtering
+
+    :returns: The filtered data along axial time.
+    :return type: numpy.ndarray
+    """
+    lf = cutoff - band / 2
+    hf = cutoff + band / 2
+    d_filtered = d_data.copy()
+    if lf / (sampling_freq / 2) > 0.1:
+        us.filtfilt(d_filtered, lf, sampling_freq, 'high', axis=axis)
+    if hf / (sampling_freq / 2) < 0.9:
+        us.filtfilt(d_filtered, hf, sampling_freq, 'low', axis=axis)
+    return d_filtered.copy()
+
+
+def _unalias(d_cmaps, nyquists, p):
+    """Conversion using the lookup tables, for Alias free.
+
+    :param list d_cmaps: The GPUArray Doppler color maps of each central
+        frequencies
+    :param list nyquists: The list of nyquists of each central frequencies
+    :param int p: The p relation between f01 and f02
+
+    :returns: The unaliased map.
+    :return type: numpy.ndarray
+    """
+    q = p + 1
+
+    # Lookup table
+    cases = cp.round(q * (d_cmaps[1] - d_cmaps[0]) / (2 * nyquists[0]))
+    nn1 = cases.copy()
+    nn1[(cases == -2) | (cases == 2)] = 0
+    nn2 = cases.copy()
+    nn2[cases == -2] = 1
+    nn2[cases == 2] = -1
+
+    # Unaliased map
+    d_unalias = (p / (p + q)) * (d_cmaps[0] + (q / p) * d_cmaps[1] +
+                                 2 * nyquists[0] * (nn1 + nn2))
+
+    return d_unalias.copy()
```

### Comparing `ultraspy-1.1/src/ultraspy/gpu/gpu_utils.py` & `ultraspy-1.2/src/ultraspy/gpu/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/apodization.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/apodization.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/das.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/das.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/fdmas.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/fdmas.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/interpolation.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/interpolation.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/pdas.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/pdas.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers_kernels.py` & `ultraspy-1.2/src/ultraspy/gpu/kernels/beamformers_kernels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """Factory for the beamformers kernels. Reads the cuda code and extract their
 functions, so they can be called by the library.
 Note: This should not be accessible by users
-
-The following kernels can be imported from the factory:
-- k_das: The DAS kernel, which can be either performed on RFs (if data is of
-         type np.float32) or I/Qs (np.complex64).
 """
 from ultraspy.config import cfg
 
 from .utils import (compile_bin,
                     call_function_given_type,
                     GPUTypes)
 
@@ -18,14 +14,15 @@
 RECOMPILE = cfg.RECOMPILE_CUBIN
 
 
 # Re-compile the code if requested
 mod_das = compile_bin(DIR, 'das.cu', RECOMPILE)
 mod_fdmas = compile_bin(DIR, 'fdmas.cu', RECOMPILE)
 mod_pdas = compile_bin(DIR, 'pdas.cu', RECOMPILE)
+mod_capon = compile_bin(DIR, 'capon.cu', RECOMPILE)
 
 
 # Local kernels, based on the type of the first argument (often the array we
 # want to perform operation on)
 _k_das_types = {
     GPUTypes.FLOAT.value: mod_das.get_function('das_float'),
     GPUTypes.COMPLEX.value: mod_das.get_function('das_complex'),
@@ -46,16 +43,26 @@
     GPUTypes.FLOAT.value: mod_pdas.get_function('pdas_float'),
     GPUTypes.COMPLEX.value: mod_pdas.get_function('pdas_complex'),
 }
 _k_packet_pdas_types = {
     GPUTypes.FLOAT.value: mod_pdas.get_function('packet_pdas_float'),
     GPUTypes.COMPLEX.value: mod_pdas.get_function('packet_pdas_complex'),
 }
+_k_capon_types = {
+    GPUTypes.FLOAT.value: mod_capon.get_function('capon_float'),
+    GPUTypes.COMPLEX.value: mod_capon.get_function('capon_complex'),
+}
+_k_packet_capon_types = {
+    GPUTypes.FLOAT.value: mod_capon.get_function('packet_capon_float'),
+    GPUTypes.COMPLEX.value: mod_capon.get_function('packet_capon_complex'),
+}
 
 
 # Kernels
 k_das = call_function_given_type(_k_das_types)
 k_packet_das = call_function_given_type(_k_packet_das_types)
 k_fdmas = call_function_given_type(_k_fdmas_types)
 k_packet_fdmas = call_function_given_type(_k_packet_fdmas_types)
 k_pdas = call_function_given_type(_k_pdas_types)
 k_packet_pdas = call_function_given_type(_k_packet_pdas_types)
+k_capon = call_function_given_type(_k_capon_types)
+k_packet_capon = call_function_given_type(_k_packet_capon_types)
```

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/color_map.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/color_map.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/power_map.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler/power_map.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler_kernels.py` & `ultraspy-1.2/src/ultraspy/gpu/kernels/doppler_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/by2.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/operators/by2.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/convolve.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/convolve.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/divide_by.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/operators/divide_by.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/flip.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/flip.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/get_modulo.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/operators/get_modulo.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/median_filter.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/operators/median_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/to_db.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/operators/to_db.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/operators_kernels.py` & `ultraspy-1.2/src/ultraspy/gpu/kernels/operators_kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,9 +100,8 @@
 k_to_db = call_function_given_type(_k_to_db_types)
 k_power_to_db = call_function_given_type(_k_power_to_db_types)
 k_convolve1d = call_function_given_type(_k_convolve1d_types)
 k_convolve2d = call_function_given_type(_k_convolve2d_types)
 k_median_filter = call_function_given_type(_k_median_filter_types)
 
 # Min / Max are already implemented reduction kernels, use them
-# TODO: Should be removed now
 k_max = lambda d: d.max().get().item()
```

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/down_mix.cu` & `ultraspy-1.2/src/ultraspy/gpu/kernels/signal/down_mix.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/filter0.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/filter0.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_end_sig.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_end_sig.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_filter.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_start_sig.cu` & `ultraspy-1.2/venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_start_sig.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/signal_kernels.py` & `ultraspy-1.2/src/ultraspy/gpu/kernels/signal_kernels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 """Factory for the signal kernels. Reads the cuda code and extract their
-functions so they can be called by the library.
+functions, so they can be called by the library.
 Note: This should not be accessible by users
-
-The following kernels can be imported from the factory:
-- k_down_mix: Used to mix a signal with a complex sinusoid signal
-- k_init_filter: TODO: Complete
-- k_init_start_sig: TODO: Complete
-- k_filter0: TODO: Complete
-- k_init_end_sig: TODO: Complete
-
-TODO: Should test the filtfilt with floats
 """
 from ultraspy.config import cfg
 
 from .utils import (compile_bin,
                     call_function_given_type,
                     GPUTypes)
```

### Comparing `ultraspy-1.1/src/ultraspy/gpu/kernels/utils.py` & `ultraspy-1.2/src/ultraspy/gpu/kernels/utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/post_processing.py` & `ultraspy-1.2/src/ultraspy/gpu/post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/gpu/signal.py` & `ultraspy-1.2/src/ultraspy/gpu/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,14 @@
           axis=-1, implementation='all_in_one', inplace=True):
     """Converts raw RFs data signals into I/Qs (In-Phase Quadrature) using
     CUDA kernels on GPU. Consists in a down-mixing operation (centers the
     spectrum at 0Hz), followed by a low-pass filter to keep only the newly
     centered at 0 spectrum (remove the old negative component). Note that it
     assumes that the time samples (fast time) are in the last axis of d_data.
 
-    TODO: Not exactly the same for envelope from RFs, should check
-
     :param cupy.array d_data: The GPUArray data to convert (along the last axis)
     :param float central_freq: The central frequency of the signal
     :param float sampling_freq: The sampling frequency of the data
     :param float t0: The initial time of recording (in s)
     :param int order: The order of the low-pass filter
     :param int axis: The axis of the data to convert
     :param float bandwidth: The bandwidth of the probes. Default is set to 100,
@@ -181,16 +179,14 @@
 def matched_filter(d_data, ref_signal, domain='time', inplace=True):
     """Applies a matched filter to our data along the last axis, given a
     reference signal which is supposed to match. Only the version on time
     domain currently works, which is basically a cross-correlation of our data
     with the reference signal, using a zero padding to keep it center all the
     time.
 
-    TODO: Didn't work on chirps tests (consecutive calls), check TODO list
-
     :param cupy.array d_data: The GPUArray data where to apply the filter
         (along the last axis)
     :param numpy.ndarray ref_signal: The reference signal (1D)
     :param str domain: The domain to use ('time' (default) or 'spectral')
     :param bool inplace: If set to True, d_data is directly modified. Else
         case, a new slot is allocated on GPU, and the result is returned while
         d_data is kept
```

### Comparing `ultraspy-1.1/src/ultraspy/helpers/doppler_helpers.py` & `ultraspy-1.2/src/ultraspy/helpers/doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/helpers/metrics_helpers.py` & `ultraspy-1.2/src/ultraspy/helpers/metrics_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/helpers/signal_helpers.py` & `ultraspy-1.2/src/ultraspy/helpers/signal_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
                                                      k_filter0,
                                                      k_init_end_sig)
 
 
 def get_filter_initial_conditions(order, a, b):
     """Returns the initial conditions for filtering. These are used to reduce
     startup and ending transients.
-    TODO: read https://www.radioeng.cz/fulltexts/2000/00_02_14_17.pdf
-    TODO: maybe remove order? We can extract it with a / b dimensions
-    TODO: Maybe p_k would be easier to read in 2d
+
+    Note: maybe remove order? We can extract it with a / b dimensions, and p_k
+          would be easier to read in 2d
 
     :param int order: The order of the filter
     :param numpy.ndarray a: The A coefficients of the filter (see butter)
     :param numpy.ndarray b: The B coefficients of the filter (see butter)
 
     :returns: The initial conditions for filtering
     :return type: numpy.ndarray
@@ -52,17 +52,18 @@
 def filtfilt_routine(d_data, nb_data, nb_time_samples, order, d_b, d_a, d_ics,
                      nb_ext, d_x, d_y, d_z):
     """Routine for the filtfilt method, calls the kernels to initialize the
     signals based on the initial conditions and filtering coefficients. The
     filtering is performed on the last dimension, but the d_data array can have
     more than 2 or 3 dimensions. All the operations are performed on GPU, and
     the resulting filtered data is stored in d_data.
-    TODO: I think d_y isn't mandatory, it could be replaced by 'd_x2'
-    TODO: The dimensions are unclear of tmp arrays to me, it'd worth an
-          investigation, especially if it is confusing
+
+    Note: d_y doesn't seem mandatory, it could be replaced by 'd_x2'. Also, the
+          dimensions of tmp arrays are unclear, it'd worth an investigation,
+          especially if it is confusing
 
     :param cupy.array d_data: The GPUArray data where to apply the filter
         (along the last axis)
     :param np.uint32 nb_data: The number of independent data to filter (all the
         dimensions but the last will be 'flatten' into nb_data samples)
     :param np.uint32 nb_time_samples: The number of time samples along the axis
         to filter (last one)
```

### Comparing `ultraspy-1.1/src/ultraspy/helpers/transmit_delays_helpers.py` & `ultraspy-1.2/src/ultraspy/helpers/transmit_delays_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/helpers/windows_helpers.py` & `ultraspy-1.2/src/ultraspy/helpers/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/io/file_loaders/factory.py` & `ultraspy-1.2/src/ultraspy/io/file_loaders/factory.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/io/file_loaders/file_loader.py` & `ultraspy-1.2/src/ultraspy/io/file_loaders/file_loader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/io/file_loaders/h5_loader.py` & `ultraspy-1.2/src/ultraspy/io/file_loaders/h5_loader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/io/file_loaders/mat_loader.py` & `ultraspy-1.2/src/ultraspy/io/file_loaders/mat_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Loader for .mat data, reads all the data and recovers it based on the format
 of the data.
-TODO: Check the way to deal the keys of the matlab objects, check on Vera data,
-      there are plenty of unused data on there
 """
 import scipy.io
 
 from .file_loader import FileLoader
 
 
 class MatLoader(FileLoader):
```

### Comparing `ultraspy-1.1/src/ultraspy/io/file_loaders/rff256_loader.py` & `ultraspy-1.2/src/ultraspy/io/file_loaders/rff256_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Loader for .rff256 data, reads all the data and recovers it based on the
 format of the data.
-TODO: Clean up the code, especially when we have many plane waves. Also should
-      check the data from Andrei.
+
+Note: Clean up the code, especially when we have many plane waves.
 """
 import os
 import io
 import configparser
 import re
 
 from array import array
@@ -32,15 +32,16 @@
 
     def __init__(self, filepath):
         """Parent initializer, then load the mat file into the data dict.
 
         :param str filepath: The path where to find the data (.rff256)
         """
         super().__init__(filepath)
-        # TODO: Not always the same as the one in the config file, should be
+        # Note: This is not always the same as the one in the config file,
+        # which seems a bit weird, should be investigated
         self.nb_boards = 4
         self.filter_low_freqs = False
 
         directory, data_file = os.path.split(filepath)
         basename = '_'.join(data_file.split('_')[:-1])
         configs_file = os.path.splitext(data_file)[0] + '.uos'
         params_file = basename + '_params.uop'
```

### Comparing `ultraspy-1.1/src/ultraspy/io/reader.py` & `ultraspy-1.2/src/ultraspy/io/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -496,16 +496,14 @@
         }
         self.probe = probe
 
     def __extract_vera_data(self, loaded_dict):
         """Extracts the relevant data, considering it is coming from the Vera
         echograph (.mat).
 
-        TODO: Should not work anymore, not flexible to probes / delays
-
         :param dict loaded_dict: The dictionary extracted from the data file
         """
         if 'Connector' in loaded_dict['Trans']:
             pin_map = [x - 1 for x in loaded_dict['Trans']['Connector']]
         else:
             nb_e = loaded_dict['Resource']['Parameters']['numTransmit']
             pin_map = list(range(nb_e))
@@ -544,25 +542,23 @@
         if nb_f > 1:
             fs = central_freq * sample[0].samplesPerWave
         else:
             fs = central_freq * sample['samplesPerWave']
         bounds = loaded_dict['Trans']['Bandwidth'] * 1e6
         bandwidth = abs(bounds[1] - bounds[0]) * 100 / central_freq
 
-        # Build the probe
+        # Build the probe, in a super-high level way. The position of the probe
+        # elements is unknown, but if provided, it should be used here
         pitch = loaded_dict['Trans']['spacingMm'] * 1e-3
-        # probe_geometry = np.zeros(3, nb_e)
-        # probe_geometry[0, :] = ((np.arange(nb_e) - ((nb_e - 1) / 2)) * pitch)
-        # TODO: Super high level, but not sure how to do it differently
         geometry_type = 'linear'
         probe = build_probe(geometry_type, nb_e, pitch, central_freq,
                             bandwidth=bandwidth)
 
-        # Compute the delays
-        # TODO: Should check if they arent in the data
+        # Compute the delays, we compute them using the angles, but a better
+        # way would be to get them somewhere from the workspace
         delays = compute_pw_delays(angles, probe,
                                    speed_of_sound=speed_of_sound)
 
         # The PRF and t0 were added lately in my saved workspaces... Those
         # might be missing
         prf = None
         if 'PRF' in loaded_dict:
@@ -593,36 +589,36 @@
         }
         self.probe = probe
 
     def __extract_ulaop_data(self, loaded_dict):
         """Extracts the relevant data, considering it is coming from the Ula-Op
         echograph (rff256). Currently only works for RFs.
 
-        TODO: Should not work anymore, not flexible to probes / delays
+        Note: Should not work anymore, not flexible to probes / delays
 
         :param dict loaded_dict: The dictionary extracted from the data file
         """
         speed_of_sound = loaded_dict['params']['sound_speed']
         data = loaded_dict['data']
         angles = np.radians(loaded_dict['angles'])
         ulaop_fs = 78.125 * 1e6
         real_fs = ulaop_fs / loaded_dict['params']['downsampled']
 
-        # Build the probes
-        # TODO: Super high level, but not sure how to do it differently
+        # Build the probes in a super high level way. There should be another
+        # way to know the probe geometry
         geometry_type = 'linear'
         _, nb_t, nb_e, _ = data.shape
         pitch = loaded_dict['params']['pitch']
         central_freq = loaded_dict['params']['tx_freq']
         probe = build_probe(geometry_type, nb_e, pitch, central_freq)
         # probe_geometry = np.zeros(3, nb_e)
         # probe_geometry[0, :] = ((np.arange(nb_e) - ((nb_e - 1) / 2)) * pitch)
 
-        # Compute the delays
-        # TODO: Should check if they arent in the data
+        # Compute the delays, but these should be extracted directly from the
+        # data or UlaOp setups
         delays = compute_pw_delays(angles, probe,
                                    speed_of_sound=speed_of_sound)
 
         self.data = data
         self.data_info = {
             'data_shape': data.shape,
             'data_type': data.dtype,
```

### Comparing `ultraspy-1.1/src/ultraspy/metrics.py` & `ultraspy-1.2/src/ultraspy/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,14 @@
 
 
 def get_full_width_at_half_maximum(signal, focus_idx, line_axis, half=-6,
                                    local=True, get_details=False, show=False):
     """Returns the Full-Width at Half Maximum of a signal, given a focus index.
     It is basically the width of the focused lobe at -6dB.
 
-    TODO: It'd be easier to always return the details
-
     :param numpy.ndarray signal: The sample of data to evaluate
     :param int focus_idx: The index to focus on, we'll look for the lobe around
         this index
     :param numpy.ndarray line_axis: The spatial axis to know the location of
         each pixel
     :param int half: Where to cut the lobe (default to -6dB)
     :param bool local: If set to True, consider local maximum (FWHM is bound to
@@ -194,16 +192,14 @@
 
 def get_peak_side_lobe(signal, focus_idx, line_axis, get_details=False,
                        show=False):
     """Returns the Peak Side Lobe of a signal, given a focus index. It is
     basically the difference in dB between the focused lobe and its closest
     neighbor.
 
-    TODO: It'd be easier to always return the details
-
     :param numpy.ndarray signal: The sample of data to evaluate
     :param int focus_idx: The index to focus on, we'll look for the lobe around
         this index
     :param numpy.ndarray line_axis: The spatial axis to know the location of
         each pixel
     :param bool get_details: If set to True, the function will return the
         details of the computation, which is useful for visualization
```

### Comparing `ultraspy-1.1/src/ultraspy/probes/convex_probe.py` & `ultraspy-1.2/src/ultraspy/probes/convex_probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/probes/factory.py` & `ultraspy-1.2/src/ultraspy/probes/factory.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/probes/linear_probe.py` & `ultraspy-1.2/src/ultraspy/probes/linear_probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/probes/matricial_probe.py` & `ultraspy-1.2/src/ultraspy/probes/matricial_probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/probes/probe.py` & `ultraspy-1.2/src/ultraspy/probes/probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/scan.py` & `ultraspy-1.2/src/ultraspy/scan.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/utils/beamformers.py` & `ultraspy-1.2/src/ultraspy/utils/beamformers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/utils/linear_decomposition.py` & `ultraspy-1.2/src/ultraspy/utils/linear_decomposition.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,14 @@
     return mat_a, indices
 
 
 def lubksb(mat_a, n, indices, mat_b):
     """Solves the set of n linear equations Ax = b, reusing the indices and
     matrix returned by ludcmp.
 
-    TODO: Should be documented a bit more in depth
-
     :param numpy.ndarray mat_a: The permuted matrix returned by LUDCMP
         routine
     :param int n: The size of a row in our flatten array
     :param numpy.ndarray indices: The pivot indices returned by the LUDCMP
         routine
     :param numpy.ndarray mat_b: The final matrix to return with the results
```

### Comparing `ultraspy-1.1/src/ultraspy/utils/masks.py` & `ultraspy-1.2/src/ultraspy/utils/masks.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/utils/matplot.py` & `ultraspy-1.2/src/ultraspy/utils/matplot.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/utils/print.py` & `ultraspy-1.2/src/ultraspy/utils/print.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy/utils/string.py` & `ultraspy-1.2/src/ultraspy/utils/string.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/src/ultraspy.egg-info/PKG-INFO` & `ultraspy-1.2/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: ultraspy
-Version: 1.1
-Summary: Ultrasound toolbox for GPU
-Home-page: https://gitlab.com/pecarlat/ultraspy
-Author: Pierre Ecarlat
-Author-email: pierre.ecarlat@gmail.com
-Project-URL: Documentation, https://ultraspy.readthedocs.io/en/latest/
-Project-URL: Bug Tracker, https://gitlab.com/pecarlat/ultraspy/-/issues/
-Keywords: ultrasound,python,beamforming,doppler
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 What is ultraspy?
 -----------------
 Ultraspy is a package designed to efficiently manipulate ultrasound data using
 GPU. The most common beamforming or Doppler methods are implemented (such as
 DAS, RF to I/Qs, Color/Power Doppler, ...), along with some state-of-the-art
 methods (Capon beamforming, Vector Doppler, alias-free Doppler velocity, ...).
 A set of metrics (PSL, FWHM, SNR) is also provided so anyone can validate the
 quality of their ultrasound data and beamforming operations.
 
 The package is designed to work with both RF and I/Q signals, in 2D or 3D, and
 with any type of probe (linear, convex, or matrix). The core code can run both
 on CPU and GPU, making it ideal for any real-time application. All beamforming
-parameters (f-number, compounding, apodizationâ€¦) can be freely customized at
+parameters (f-number, compounding, apodization…) can be freely customized at
 any time for research purposes.
 
 The package has been thought to be as flexible as possible, so that anyone
 could eventually clone it and add its own research methods and test it in real
 time. A set of tutorials is provided to facilitate user learning and adoption,
 along with some instruction on how to contribute to the lib if you feel like
 your research method should be added to help the community.
@@ -40,23 +22,23 @@
 
 Features
 ========
 - General beamforming methods, flexible to Radio-Frequency or In-phase
   Quadrature data, working on CPU and GPU. Mainly DAS and FDMAS for the
   plane-wave imaging, but also TFM for Beam Focusing imaging
 
-- Advanced beamforming methods (p-DAS or Capon (TODO)), with a dedicated
-  tutorial to understand how these are implemented and how to implement your
-  own methods
+- Advanced beamforming methods (p-DAS or Capon), with a dedicated tutorial to
+  understand how these are implemented and how to implement your own methods
 
 - Basic Doppler methods (Color and Power maps), and their dedicated utilities
   functions (matched filtering, RF to I/Qs conversion)
 
-- Advanced Doppler methods, such as Vector Doppler (TODO) or propositions for
-  alias-free alias-free Doppler velocities (dual-wavelength method)
+- Advanced Doppler methods, such as a proposition for alias-free alias-free
+  Doppler velocities (using dual-wavelength method). This still lacks of
+  methods, and should include Vector Doppler or so in future releases
 
 - Basic metrics for evaluation of the data quality (SNR), or of our beamforming
   algorithms (FWHM, PSL, CNR)
 
 
 Documentation
 =============
```

### Comparing `ultraspy-1.1/src/ultraspy.egg-info/SOURCES.txt` & `ultraspy-1.2/src/ultraspy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 .tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
 .tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
 docs/acknowledgements.rst
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/_static/custom.css
+docs/algorithms/capon_algo.rst
 docs/algorithms/das_algo.rst
 docs/algorithms/fdmas_algo.rst
 docs/algorithms/index.rst
 docs/algorithms/pdas_algo.rst
 docs/api_references/beamformers.rst
 docs/api_references/classes.rst
 docs/api_references/gpu_utils.rst
@@ -168,15 +169,19 @@
 docs/contribute/preparation.rst
 docs/contribute/tdd.rst
 docs/examples/das.rst
 docs/examples/doppler.rst
 docs/examples/index.rst
 docs/examples/metrics.rst
 docs/examples/simu_data.rst
+docs/examples/torch_compatibility.rst
 docs/images/block_grid.png
+docs/images/capon_cholesky.png
+docs/images/capon_gpu_allocation.png
+docs/images/capon_windows.png
 docs/images/convex_delays.png
 docs/images/convex_probe.png
 docs/images/creatis_logo.png
 docs/images/das_algo.png
 docs/images/das_bmode.png
 docs/images/das_dam.png
 docs/images/doppler.png
@@ -193,46 +198,48 @@
 docs/images/metrics_masks.png
 docs/images/metrics_raw_data.png
 docs/images/metrics_snr_correct.png
 docs/images/metrics_snr_wrong.png
 docs/images/metrics_spectra.png
 docs/images/pdas_spectra.png
 docs/images/polar_system.png
+docs/images/probes.png
 docs/images/tpac_logo.jpg
 docs/images/ultraspy_classes.png
 docs/tech_choices/beamforming_choices.rst
 docs/tech_choices/gpu_beamformers.rst
 docs/tech_choices/gpu_configs.rst
 docs/tech_choices/index.rst
 src/__init__.py
-src/ultraspy/TODO.md
 src/ultraspy/__init__.py
 src/ultraspy/config.py
 src/ultraspy/metrics.py
 src/ultraspy/scan.py
 src/ultraspy.egg-info/PKG-INFO
 src/ultraspy.egg-info/SOURCES.txt
 src/ultraspy.egg-info/dependency_links.txt
 src/ultraspy.egg-info/requires.txt
 src/ultraspy.egg-info/top_level.txt
 src/ultraspy/beamformers/__init__.py
 src/ultraspy/beamformers/beamformer.py
+src/ultraspy/beamformers/capon.py
 src/ultraspy/beamformers/das.py
 src/ultraspy/beamformers/fdmas.py
 src/ultraspy/beamformers/options.py
 src/ultraspy/beamformers/pdas.py
 src/ultraspy/beamformers/setups.py
 src/ultraspy/cpu/__init__.py
 src/ultraspy/cpu/display.py
 src/ultraspy/cpu/doppler.py
 src/ultraspy/cpu/post_processing.py
 src/ultraspy/cpu/signal.py
 src/ultraspy/cpu/kernels/numba_cores/__init__.py
 src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py
 src/ultraspy/cpu/kernels/numba_cores/apodization.py
+src/ultraspy/cpu/kernels/numba_cores/capon.py
 src/ultraspy/cpu/kernels/numba_cores/das.py
 src/ultraspy/cpu/kernels/numba_cores/fdmas.py
 src/ultraspy/cpu/kernels/numba_cores/interpolation.py
 src/ultraspy/cpu/kernels/numba_cores/maths_utils.py
 src/ultraspy/cpu/kernels/numba_cores/pdas.py
 src/ultraspy/cpu/kernels/numba_cores/probe_distances.py
 src/ultraspy/cpu/kernels/numpy_cores/__init__.py
@@ -252,14 +259,16 @@
 src/ultraspy/gpu/kernels/beamformers_kernels.py
 src/ultraspy/gpu/kernels/doppler_kernels.py
 src/ultraspy/gpu/kernels/operators_kernels.py
 src/ultraspy/gpu/kernels/signal_kernels.py
 src/ultraspy/gpu/kernels/utils.py
 src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
 src/ultraspy/gpu/kernels/beamformers/apodization.cu
+src/ultraspy/gpu/kernels/beamformers/capon.cu
+src/ultraspy/gpu/kernels/beamformers/complex_utils.cu
 src/ultraspy/gpu/kernels/beamformers/das.cu
 src/ultraspy/gpu/kernels/beamformers/fdmas.cu
 src/ultraspy/gpu/kernels/beamformers/interpolation.cu
 src/ultraspy/gpu/kernels/beamformers/pdas.cu
 src/ultraspy/gpu/kernels/beamformers/probe_distances.cu
 src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
 src/ultraspy/gpu/kernels/doppler/color_map.cu
@@ -320,14 +329,15 @@
 tests/test_cpu/test_doppler.py
 tests/test_cpu/test_metrics.py
 tests/test_cpu/test_post_processing.py
 tests/test_cpu/test_probes.py
 tests/test_cpu/test_scan.py
 tests/test_cpu/test_signal.py
 tests/test_cpu/beamformers/test_beamformer.py
+tests/test_cpu/beamformers/test_capon.py
 tests/test_cpu/beamformers/test_das.py
 tests/test_cpu/beamformers/test_fdmas.py
 tests/test_cpu/beamformers/test_pdas.py
 tests/test_cpu/helpers/test_doppler_helpers.py
 tests/test_cpu/helpers/test_signal_helpers.py
 tests/test_cpu/helpers/test_transmit_delays_helpers.py
 tests/test_cpu/helpers/test_windows_helpers.py
@@ -343,14 +353,15 @@
 tests/test_gpu/test_display.py
 tests/test_gpu/test_doppler.py
 tests/test_gpu/test_filtfilts.py
 tests/test_gpu/test_gpu_utils.py
 tests/test_gpu/test_post_processing.py
 tests/test_gpu/test_signal.py
 tests/test_gpu/beamformers/test_beamformer.py
+tests/test_gpu/beamformers/test_capon.py
 tests/test_gpu/beamformers/test_das.py
 tests/test_gpu/beamformers/test_fdmas.py
 tests/test_gpu/beamformers/test_pdas.py
 tests/test_gpu/helpers/test_doppler_helpers.py
 tests/test_gpu/helpers/test_signal_helpers.py
 tests/test_gpu/helpers/test_windows_helpers.py
 tests/test_gpu/kernels/test_beamformers_kernels.py
@@ -408,18 +419,54 @@
 venv/Lib/site-packages/numba/cuda/tests/data/error.cu
 venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
 venv/Lib/site-packages/numba/cuda/tests/data/warn.cu
 venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
 venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
 venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
 venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/apodization.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/das.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/fdmas.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/interpolation.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/pdas.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/probe_distances.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/color_map.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/doppler/power_map.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/headers/cupy_header.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/by2.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/convolve.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/divide_by.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/flip.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/get_modulo.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/median_filter.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/operators/to_db.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/signal/down_mix.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/signal/filter0.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_end_sig.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_filter.cu
+venv/Lib/site-packages/ultraspy/gpu/kernels/signal/init_start_sig.cu
+venv/Lib/site-packages/ultraspy/probes/configs/c5-2v.ini
+venv/Lib/site-packages/ultraspy/probes/configs/l11-4v.ini
+venv/Lib/site-packages/ultraspy/probes/configs/l11-5v.ini
+venv/Lib/site-packages/ultraspy/probes/configs/l14-5w.ini
+venv/Lib/site-packages/ultraspy/probes/configs/l7-4.ini
+venv/Lib/site-packages/ultraspy/probes/configs/mux_1024_8MHz.ini
+venv/Lib/site-packages/ultraspy/probes/configs/p4-2v.ini
 venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/mlib.ini
 venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/npymath.ini
 venv/Lib/site-packages/~-mpy/typing/tests/data/mypy.ini
 venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/cuda_include.cu
 venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/error.cu
 venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/jitlink.cu
 venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/warn.cu
 venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/functions.cu
 venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/mlib.ini
 venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/npymath.ini
-venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
+venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
+venv/Lib/site-packages/~~mpy/core/lib/npy-pkg-config/mlib.ini
+venv/Lib/site-packages/~~mpy/core/lib/npy-pkg-config/npymath.ini
+venv/Lib/site-packages/~~mpy/typing/tests/data/mypy.ini
```

### Comparing `ultraspy-1.1/tests/conftest.py` & `ultraspy-1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/beamformers/test_beamformer.py` & `ultraspy-1.2/tests/test_cpu/beamformers/test_beamformer.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/beamformers/test_das.py` & `ultraspy-1.2/tests/test_cpu/beamformers/test_das.py`

 * *Files 2% similar despite different names*

```diff
@@ -1136,7 +1136,43 @@
     beamformed_tr2 = beamformer.beamform(reader.data[0, [pw[1]]], scan)
     beamformer.update_setup('transmissions_idx', [pw[2]])
     beamformed_tr3 = beamformer.beamform(reader.data[0, [pw[2]]], scan)
 
     assert np.allclose(beamformed[0], beamformed_tr1)
     assert np.allclose(beamformed[1], beamformed_tr2)
     assert np.allclose(beamformed[2], beamformed_tr3)
+
+
+def test_packet_das_no_compounding_sum():
+    # Compare our results with or without compounding
+    # Get the data
+    rsc_dir = cfg.PATHS_RESOURCES
+    reader = Reader(os.path.join(rsc_dir, 'picmus_simu_rfs.hdf5'), 'picmus')
+    x = np.linspace(-20, 20, 200) * 1e-3
+    z = np.linspace(5, 30, 500) * 1e-3
+    scan = GridScan(x, z, on_gpu=False)
+    beamformer = DelayAndSum(on_gpu=False)
+    beamformer.automatic_setup(reader.acquisition_info, reader.probe)
+    frame1 = reader.data[0, [0, 37, 74]]
+    frame2 = reader.data[0, [15, 37, 60]]
+    frame3 = reader.data[0, [0, 1, 2]]
+    frame4 = reader.data[0, [72, 73, 74]]
+    data = np.array([frame1, frame2, frame3, frame4])
+    beamformer.update_setup('transmissions_idx', [0, 1, 2])
+    beamformer.update_setup('signal_duration', 0)
+    beamformer.update_setup('f_number', 1.)
+    beamformer.update_option('reduction', 'sum')
+
+    # Beamformed
+    beamformed = beamformer.beamform_packet(data, scan)
+
+    # Same with no compounding
+    beamformer.update_option('compound', False)
+    beamformed_wo_compound = beamformer.beamform_packet(data, scan)
+
+    vmax = min(np.max(beamformed), np.max(beamformed_wo_compound))
+    vmin = max(np.min(beamformed), np.min(beamformed_wo_compound))
+    tol = (vmax - vmin) / 1e6
+    assert beamformed.ndim == 3
+    assert beamformed_wo_compound.ndim == 4
+    assert np.allclose(
+        np.sum(beamformed_wo_compound, axis=0), beamformed, atol=tol)
```

### Comparing `ultraspy-1.1/tests/test_cpu/beamformers/test_fdmas.py` & `ultraspy-1.2/tests/test_cpu/beamformers/test_fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/beamformers/test_pdas.py` & `ultraspy-1.2/tests/test_cpu/beamformers/test_pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/helpers/test_doppler_helpers.py` & `ultraspy-1.2/tests/test_cpu/helpers/test_doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/helpers/test_signal_helpers.py` & `ultraspy-1.2/tests/test_cpu/helpers/test_signal_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/helpers/test_windows_helpers.py` & `ultraspy-1.2/tests/test_cpu/helpers/test_windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/io/test_reader.py` & `ultraspy-1.2/tests/test_cpu/io/test_reader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_doppler.py` & `ultraspy-1.2/tests/test_cpu/test_doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_metrics.py` & `ultraspy-1.2/tests/test_cpu/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_post_processing.py` & `ultraspy-1.2/tests/test_cpu/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_probes.py` & `ultraspy-1.2/tests/test_cpu/test_probes.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_scan.py` & `ultraspy-1.2/tests/test_cpu/test_scan.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/test_signal.py` & `ultraspy-1.2/tests/test_cpu/test_signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/utils/test_linear_decomposition.py` & `ultraspy-1.2/tests/test_cpu/utils/test_linear_decomposition.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_cpu/utils/test_masks.py` & `ultraspy-1.2/tests/test_cpu/utils/test_masks.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/beamformers/test_beamformer.py` & `ultraspy-1.2/tests/test_gpu/beamformers/test_beamformer.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/beamformers/test_das.py` & `ultraspy-1.2/tests/test_gpu/beamformers/test_das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/beamformers/test_fdmas.py` & `ultraspy-1.2/tests/test_gpu/beamformers/test_fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/beamformers/test_pdas.py` & `ultraspy-1.2/tests/test_gpu/beamformers/test_pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/helpers/test_doppler_helpers.py` & `ultraspy-1.2/tests/test_gpu/helpers/test_doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/helpers/test_signal_helpers.py` & `ultraspy-1.2/tests/test_gpu/helpers/test_signal_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/helpers/test_windows_helpers.py` & `ultraspy-1.2/tests/test_gpu/helpers/test_windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/kernels/test_doppler_kernels.py` & `ultraspy-1.2/tests/test_gpu/kernels/test_doppler_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/kernels/test_operators_kernels.py` & `ultraspy-1.2/tests/test_gpu/kernels/test_operators_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/kernels/test_signal_kernels.py` & `ultraspy-1.2/tests/test_gpu/kernels/test_signal_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/test_doppler.py` & `ultraspy-1.2/tests/test_gpu/test_doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/test_filtfilts.py` & `ultraspy-1.2/tests/test_gpu/test_filtfilts.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/test_gpu_utils.py` & `ultraspy-1.2/tests/test_gpu/test_gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/test_signal.py` & `ultraspy-1.2/tests/test_gpu/test_signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tests/test_gpu/utils/test_linear_decomposition.py` & `ultraspy-1.2/tests/test_gpu/utils/test_linear_decomposition.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/tox.ini` & `ultraspy-1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/cupy/random/cupy_distributions.cu` & `ultraspy-1.2/venv/Lib/site-packages/cupy/random/cupy_distributions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.2/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.2/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

