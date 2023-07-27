# Comparing `tmp/xray_bot-0.1.4rc1-py3-none-any.whl.zip` & `tmp/xray_bot-0.1.4rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12334 bytes, number of entries: 12
+Zip file size: 12381 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      203 b- defN 23-Apr-23 01:52 xraybot/__init__.py
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-23 10:10 xraybot/__version__.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-24 03:42 xraybot/__version__.py
 -rw-r--r--  2.0 unx     4358 b- defN 23-Apr-21 11:02 xraybot/_context.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Apr-21 10:09 xraybot/_data.py
 -rw-r--r--  2.0 unx      192 b- defN 23-Apr-21 10:34 xraybot/_utils.py
 -rw-r--r--  2.0 unx    19127 b- defN 23-Apr-23 03:08 xraybot/_worker.py
--rw-r--r--  2.0 unx    20157 b- defN 23-Apr-23 02:52 xraybot/_xray_bot.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx      486 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      931 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/RECORD
-12 files, 47217 bytes uncompressed, 10780 bytes compressed:  77.2%
+-rw-r--r--  2.0 unx    20341 b- defN 23-Apr-24 03:29 xraybot/_xray_bot.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 03:43 xray_bot-0.1.4rc2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      486 b- defN 23-Apr-24 03:43 xray_bot-0.1.4rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 03:43 xray_bot-0.1.4rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 03:43 xray_bot-0.1.4rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      931 b- defN 23-Apr-24 03:43 xray_bot-0.1.4rc2.dist-info/RECORD
+12 files, 47401 bytes uncompressed, 10827 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xraybot/_worker.py
 Comment: 
 
 Filename: xraybot/_xray_bot.py
 Comment: 
 
-Filename: xray_bot-0.1.4rc1.dist-info/LICENSE
+Filename: xray_bot-0.1.4rc2.dist-info/LICENSE
 Comment: 
 
-Filename: xray_bot-0.1.4rc1.dist-info/METADATA
+Filename: xray_bot-0.1.4rc2.dist-info/METADATA
 Comment: 
 
-Filename: xray_bot-0.1.4rc1.dist-info/WHEEL
+Filename: xray_bot-0.1.4rc2.dist-info/WHEEL
 Comment: 
 
-Filename: xray_bot-0.1.4rc1.dist-info/top_level.txt
+Filename: xray_bot-0.1.4rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: xray_bot-0.1.4rc1.dist-info/RECORD
+Filename: xray_bot-0.1.4rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xraybot/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.4rc1"
+__version__ = "0.1.4rc2"
```

## xraybot/_xray_bot.py

```diff
@@ -58,14 +58,17 @@
     def configure_labels(self, labels: List[str]):
         self.config.configure_labels(labels)
 
     def get_xray_tests(self, filter_by_cf: bool = True) -> List[TestEntity]:
         logger.info(
             f"Start querying all xray tests for project: {self.context.project_key}"
         )
+        folder_id = self.worker_mgr.api_wrapper.automation_folder_id
+        assert folder_id is not None
+        # jql requires automation folder, need to make sure the folder exists
         jql = (
             f'project = "{self.context.project_key}" and type = "Test" and reporter = '
             f'"{self.context.jira_username}" '
             f'and status != "Obsolete" and issue in '
             f'testRepositoryFolderTests("{self.context.project_key}", '
             f'"{self.config.automation_folder_name}")'
         )
```

## Comparing `xray_bot-0.1.4rc1.dist-info/LICENSE` & `xray_bot-0.1.4rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xray_bot-0.1.4rc1.dist-info/RECORD` & `xray_bot-0.1.4rc2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 xraybot/__init__.py,sha256=9vptE2bh-sEH1jh9NFrm70D5vYw9-boQi9XgNA8_cn4,203
-xraybot/__version__.py,sha256=GIpwzbbPGQ9L-Oth25lm6mP4T9eA5Rwe9Ik85ZYTcz4,25
+xraybot/__version__.py,sha256=Cl8wC64wWewz9A4tJ455fws8cUNtM0L4CAC5GaLUIJQ,25
 xraybot/_context.py,sha256=9U4UnphDAvNTvi-WjjAhJ2IYOlmY3PlkLyoqIXxr24o,4358
 xraybot/_data.py,sha256=E4dsHZxyxioIqpc7I3c8TmNU8Kkj6JKZ6dKzO4Mrjb0,573
 xraybot/_utils.py,sha256=s7UwsTSNkSpDu73B-CeKaOjEXU8oQwDrF75FEhZAj_I,192
 xraybot/_worker.py,sha256=_gpmO4O98eNqDFQcXs-ggjjdOkNTXLDzlYNBkUdYHPs,19127
-xraybot/_xray_bot.py,sha256=9EAGIFDShB0Idt4CBwVDZCU0-AHzHAJPdZwJaY0pM4c,20157
-xray_bot-0.1.4rc1.dist-info/LICENSE,sha256=2V4UacA-K7TqPsdWQUP2it4zb9rJmDW5rW27r6Fho0U,1065
-xray_bot-0.1.4rc1.dist-info/METADATA,sha256=Ku_uoW8J_lne6jEzfoOGLXYjK-4k5vh9XQKhLQ1l18U,486
-xray_bot-0.1.4rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xray_bot-0.1.4rc1.dist-info/top_level.txt,sha256=xQlj4RDuEOf9bM5ryJNYButwxv-W_pXRvRl46gky_7Q,8
-xray_bot-0.1.4rc1.dist-info/RECORD,,
+xraybot/_xray_bot.py,sha256=BUQKaBEhHVIWzFl0xLWECcQAlhCFBSS5IpSPqPJ6AWw,20341
+xray_bot-0.1.4rc2.dist-info/LICENSE,sha256=2V4UacA-K7TqPsdWQUP2it4zb9rJmDW5rW27r6Fho0U,1065
+xray_bot-0.1.4rc2.dist-info/METADATA,sha256=-49Sjo138NuZx4UAoXNAyKPqvoscwfn716iF4T_VYEk,486
+xray_bot-0.1.4rc2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xray_bot-0.1.4rc2.dist-info/top_level.txt,sha256=xQlj4RDuEOf9bM5ryJNYButwxv-W_pXRvRl46gky_7Q,8
+xray_bot-0.1.4rc2.dist-info/RECORD,,
```

