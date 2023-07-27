# Comparing `tmp/PyTangtv-0.2.9.tar.gz` & `tmp/PyTangtv-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTangtv-0.2.9.tar", last modified: Fri Aug 27 21:16:45 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

