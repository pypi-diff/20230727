# Comparing `tmp/rocketsim-0.3.0.tar.gz` & `tmp/RocketSim-1.3.0a1-cp34-abi3-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

