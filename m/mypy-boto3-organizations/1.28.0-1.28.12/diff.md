# Comparing `tmp/mypy-boto3-organizations-1.28.0.tar.gz` & `tmp/mypy_boto3_organizations-1.28.12-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-organizations-1.28.0.tar", last modified: Thu Jul  6 21:00:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

