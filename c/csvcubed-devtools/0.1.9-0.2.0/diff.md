# Comparing `tmp/csvcubed_devtools-0.1.9-py3-none-any.whl.zip` & `tmp/csvcubed_devtools-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 17067 bytes, number of entries: 20
+Zip file size: 17258 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 csvcubeddevtools/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/__init__.py
 -rw-r--r--  2.0 unx     5448 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/csv2rdf.py
--rw-r--r--  2.0 unx     1975 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/csvlint.py
+-rw-r--r--  2.0 unx     3729 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/csvlint.py
 -rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/dockerornot.py
 -rw-r--r--  2.0 unx      220 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/environment.py
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/file.py
 -rw-r--r--  2.0 unx     3606 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/rdf.py
 -rw-r--r--  2.0 unx     3000 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/sparqltests.py
 -rw-r--r--  2.0 unx     1223 b- defN 80-Jan-01 00:00 csvcubeddevtools/behaviour/temporarydirectory.py
 -rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/__init__.py
 -rw-r--r--  2.0 unx      841 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/csvwhelpers.py
 -rw-r--r--  2.0 unx      684 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/file.py
 -rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/rdflibhelpers.py
 -rw-r--r--  2.0 unx     1310 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/shell.py
 -rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 csvcubeddevtools/helpers/tar.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx     2137 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.1.9.dist-info/METADATA
-?rw-r--r--  2.0 unx     1826 b- defN 16-Jan-01 00:00 csvcubed_devtools-0.1.9.dist-info/RECORD
-20 files, 38225 bytes uncompressed, 14021 bytes compressed:  63.3%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2137 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed_devtools-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1826 b- defN 16-Jan-01 00:00 csvcubed_devtools-0.2.0.dist-info/RECORD
+20 files, 39979 bytes uncompressed, 14212 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: csvcubeddevtools/helpers/shell.py
 Comment: 
 
 Filename: csvcubeddevtools/helpers/tar.py
 Comment: 
 
-Filename: csvcubed_devtools-0.1.9.dist-info/LICENSE
+Filename: csvcubed_devtools-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: csvcubed_devtools-0.1.9.dist-info/WHEEL
+Filename: csvcubed_devtools-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: csvcubed_devtools-0.1.9.dist-info/METADATA
+Filename: csvcubed_devtools-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: csvcubed_devtools-0.1.9.dist-info/RECORD
+Filename: csvcubed_devtools-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## csvcubeddevtools/behaviour/csvlint.py

```diff
@@ -14,14 +14,16 @@
 from csvcubeddevtools.behaviour.temporarydirectory import get_context_temp_dir_path
 from csvcubeddevtools.helpers.shell import run_command_in_dir
 from .dockerornot import SHOULD_USE_DOCKER
 
 if SHOULD_USE_DOCKER:
     client = docker.from_env()
     client.images.pull("gsscogs/csvlint")
+    csvwcheckclient = docker.from_env()
+    csvwcheckclient.images.pull("gsscogs/csvw-check:latest")
 
 
 def _run_csvlint(metadata_file_path: Path) -> Tuple[int, str]:
     if SHOULD_USE_DOCKER:
         csvlint = client.containers.create(
             "gsscogs/csvlint", command=f"csvlint -s '/tmp/{metadata_file_path.name}'"
         )
@@ -32,14 +34,30 @@
         sys.stdout.write(csvlint.logs().decode("utf-8"))
         return exit_code, csvlint.logs().decode("utf-8")
     else:
         return run_command_in_dir(
             f'csvlint -s "{metadata_file_path.resolve()}"', metadata_file_path.parent
         )
 
+def _run_csvwcheck(metadata_file_path: Path) -> Tuple[int, str]:
+    if SHOULD_USE_DOCKER:
+        csvwcheck = csvwcheckclient.containers.create(
+            "gsscogs/csvw-check:latest", command=f"bin/csvw-check -s '/tmp/{metadata_file_path.name}'"
+        )
+        csvwcheck.put_archive("/tmp", dir_to_tar(metadata_file_path.parent))
+        csvwcheck.start()
+        response: dict = csvwcheck.wait()
+        exit_code = response["StatusCode"]
+        sys.stdout.write(csvwcheck.logs().decode("utf-8"))
+        return exit_code, csvwcheck.logs().decode("utf-8")
+    else:
+        # If SHOULD_USE_DOCKER is false then we assume we are in the windows environment. Windows tests will be done as part of next ticket
+        return run_command_in_dir(
+            f'csvlint -s "{metadata_file_path.resolve()}"', metadata_file_path.parent
+        )
 
 @step("csvlint validation of all CSV-Ws should succeed")
 def step_impl(context):
     temp_dir = get_context_temp_dir_path(context)
     for file in temp_dir.rglob("*.csv-metadata.json"):
         exit_code, logs = _run_csvlint(temp_dir / file)
         assert exit_code == 0, logs
@@ -54,7 +72,30 @@
 
 @step('csvlint validation of "{file}" should fail with "{expected}"')
 def step_impl(context, file: str, expected: str):
     temp_dir = get_context_temp_dir_path(context)
     exit_code, logs = _run_csvlint(temp_dir / file)
     assert exit_code == 1, logs
     assert expected in logs, logs
+
+
+@step("csvwcheck validation of all CSV-Ws should succeed")
+def step_impl(context):
+    temp_dir = get_context_temp_dir_path(context)
+    for file in temp_dir.rglob("*.csv-metadata.json"):
+        exit_code, logs = _run_csvwcheck(temp_dir / file)
+        assert exit_code == 0, logs
+
+
+@step('csvwcheck validation of "{file}" should succeed')
+def step_impl(context, file: str):
+    temp_dir = get_context_temp_dir_path(context)
+    exit_code, logs = _run_csvwcheck(temp_dir / file)
+    assert exit_code == 0, logs
+
+
+@step('csvwcheck validation of "{file}" should fail with "{expected}"')
+def step_impl(context, file: str, expected: str):
+    temp_dir = get_context_temp_dir_path(context)
+    exit_code, logs = _run_csvwcheck(temp_dir / file)
+    assert exit_code == 1, logs
+    assert expected in logs, logs
```

## Comparing `csvcubed_devtools-0.1.9.dist-info/LICENSE` & `csvcubed_devtools-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csvcubed_devtools-0.1.9.dist-info/METADATA` & `csvcubed_devtools-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvcubed-devtools
-Version: 0.1.9
+Version: 0.2.0
 Summary: Development tools and dependencies for use in the csvcubed tooling.
 License: Apache-2.0
 Author: Integrated Data Service - Dissemination
 Author-email: csvcubed@gsscogs.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `csvcubed_devtools-0.1.9.dist-info/RECORD` & `csvcubed_devtools-0.2.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 csvcubeddevtools/__init__.py,sha256=GHzaAzMw_Accc8kxOwh_tNHeKdVBmS23ga0iSoIH4oQ,179
 csvcubeddevtools/behaviour/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubeddevtools/behaviour/csv2rdf.py,sha256=dFhfd80FCd8D1FD30DbT6FJKlUWlI3NghnZgGtx2Amk,5448
-csvcubeddevtools/behaviour/csvlint.py,sha256=Mv0vc_BoZqP9cD2N_AyhWAUTObjTSq7tT7247GJ0teI,1975
+csvcubeddevtools/behaviour/csvlint.py,sha256=cXSgH9RsrJxKUoVFhNIAjeyup4gJU1ccMZbn71MQVRQ,3729
 csvcubeddevtools/behaviour/dockerornot.py,sha256=dgd6mPkAXK_K7Augum0-38rrQrVyg6-cVYOMO0e1G-g,218
 csvcubeddevtools/behaviour/environment.py,sha256=rRc_S9MLOh2c0NRV1LCZ0cOM_eg9XCEmWIpgaegqZNw,220
 csvcubeddevtools/behaviour/file.py,sha256=TZc9_BbUafwBQaCxlab0xwuZF7qCXo1I6gayDpam_fs,2437
 csvcubeddevtools/behaviour/rdf.py,sha256=9yHFfDEjtxKJQ_wdKS8z_-dT90ueK01bURiZlHL7QS4,3606
 csvcubeddevtools/behaviour/sparqltests.py,sha256=ZMOAdj1hzn7h-O0EScEPB6G5qkL0UbDOTDLQDAJCsR0,3000
 csvcubeddevtools/behaviour/temporarydirectory.py,sha256=YbT137YQx8ibI-DUOu5yQGqsgdPGe2oPKgF5XnsMbnw,1223
 csvcubeddevtools/helpers/__init__.py,sha256=cv-P2ZvuZiUQtuKLndf5fwP6oaDPmFNDJM4UpIbWYDs,46
 csvcubeddevtools/helpers/csvwhelpers.py,sha256=a5Lnq6LehHhfFSrLtE31GniieEq6_yhSPYP5PqQGsqg,841
 csvcubeddevtools/helpers/file.py,sha256=WFrpseUqu1YwDQfOH_ZqAtrIif1fYm-f5jnsdddvRH0,684
 csvcubeddevtools/helpers/rdflibhelpers.py,sha256=EVZ8UPOYh3bp-OrwKoxA3G29vNcQ958cpNTGx0Ro2Vw,591
 csvcubeddevtools/helpers/shell.py,sha256=kxG-Nq1J4FMU21-H1T1MxnC7ZUkvhy2AFnrekAD2Udk,1310
 csvcubeddevtools/helpers/tar.py,sha256=FkNc2bboC5AOk4YXa_YVMhUTwSMca5_D--15R0f_dG4,1038
-csvcubed_devtools-0.1.9.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-csvcubed_devtools-0.1.9.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-csvcubed_devtools-0.1.9.dist-info/METADATA,sha256=_qrrqY3CSzq87EheUkL6gbaAZCsMTvip_p4UnnB-DFg,2137
-csvcubed_devtools-0.1.9.dist-info/RECORD,,
+csvcubed_devtools-0.2.0.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+csvcubed_devtools-0.2.0.dist-info/METADATA,sha256=0OUxxYLZ6570JGnSpvxpYCWybDJqrV-MrKPDImufmo8,2137
+csvcubed_devtools-0.2.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+csvcubed_devtools-0.2.0.dist-info/RECORD,,
```

