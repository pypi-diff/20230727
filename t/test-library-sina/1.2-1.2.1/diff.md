# Comparing `tmp/test-library-sina-1.2.tar.gz` & `tmp/test_library_sina-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-library-sina-1.2.tar", last modified: Thu Jul 27 09:58:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

