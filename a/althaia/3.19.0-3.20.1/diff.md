# Comparing `tmp/althaia-3.19.0.tar.gz` & `tmp/althaia-3.20.1-cp39-cp39-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "althaia-3.19.0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

