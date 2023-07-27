# Comparing `tmp/mypy-boto3-apigatewayv2-1.28.10.tar.gz` & `tmp/mypy_boto3_apigatewayv2-1.28.12-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

