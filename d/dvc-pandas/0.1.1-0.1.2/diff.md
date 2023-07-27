# Comparing `tmp/dvc-pandas-0.1.1.tar.gz` & `tmp/dvc-pandas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-pandas-0.1.1.tar", last modified: Wed Jul 26 16:43:25 2023, max compression
+gzip compressed data, was "dvc-pandas-0.1.2.tar", last modified: Thu Jul 27 17:22:37 2023, max compression
```

## Comparing `dvc-pandas-0.1.1.tar` & `dvc-pandas-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/
--rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/LICENSE
--rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/README.md
--rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.1/pyproject.toml
--rw-rw-r--   0 jey       (1000) jey       (1000)     1025 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/setup.cfg
--rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/setup.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/dvc_pandas/
--rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.1/src/dvc_pandas/__init__.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-07-26 16:41:53.000000 dvc-pandas-0.1.1/src/dvc_pandas/dataset.py
--rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.1/src/dvc_pandas/dvc.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.1/src/dvc_pandas/git.py
--rw-rw-r--   0 jey       (1000) jey       (1000)    13396 2023-07-26 16:38:54.000000 dvc-pandas-0.1.1/src/dvc_pandas/repository.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/
--rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)      366 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       91 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/requires.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/LICENSE
+-rw-rw-r--   0 jey       (1000) jey       (1000)      593 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/README.md
+-rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.2/pyproject.toml
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1025 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/setup.cfg
+-rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/setup.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/dvc_pandas/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.2/src/dvc_pandas/__init__.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-07-26 16:41:53.000000 dvc-pandas-0.1.2/src/dvc_pandas/dataset.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.2/src/dvc_pandas/dvc.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.2/src/dvc_pandas/git.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)    14041 2023-07-27 16:44:40.000000 dvc-pandas-0.1.2/src/dvc_pandas/repository.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      593 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)      366 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       91 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/requires.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/top_level.txt
```

### Comparing `dvc-pandas-0.1.1/LICENSE` & `dvc-pandas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.1/PKG-INFO` & `dvc-pandas-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
+
+
```

### Comparing `dvc-pandas-0.1.1/setup.cfg` & `dvc-pandas-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvc-pandas
-version = 0.1.1
+version = 0.1.2
 author = Bernhard Bliem
 author_email = bernhard.bliem@kausal.tech
 description = Wrapper for DVC and git to easily fetch Pandas dataframes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kausaltech/dvc-pandas
 project_urls =
```

### Comparing `dvc-pandas-0.1.1/src/dvc_pandas/dataset.py` & `dvc-pandas-0.1.2/src/dvc_pandas/dataset.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.1/src/dvc_pandas/git.py` & `dvc-pandas-0.1.2/src/dvc_pandas/git.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.1/src/dvc_pandas/repository.py` & `dvc-pandas-0.1.2/src/dvc_pandas/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,17 +209,22 @@
         origin = self.git_repo.remote()
         origin.fetch()
         for remote_ref in origin.refs:
             if remote_ref.remote_head in ('master', 'main'):
                 break
         else:
             raise KeyError("No 'master' or 'main' branch found for origin")
-        ref: git.Head = getattr(self.git_repo.heads, remote_ref.remote_head)
-        ref.set_commit(remote_ref.commit)
-        ref.checkout()
+
+        if self.git_repo.head.commit == remote_ref.commit:
+            self.log_info("Already up-to-date")
+            return
+
+        if not self.git_repo.is_ancestor(self.git_repo.head.commit, remote_ref.commit):
+            raise Exception("Current HEAD is not an ancestor of origin/%s" % (remote_ref.remote_head))
+        self.git_repo.head.reset(remote_ref, index=True, working_tree=True)
 
     @ensure_repo_lock
     def push_dataset(self, dataset: Dataset):
         """
         Add the given dataset as a parquet file to DVC, create a commit and push it.
 
         Updates the git repository first. If something goes wrong, restores the repository and all files to the state
@@ -230,26 +235,30 @@
         """
         if self.dataset_stage:
             raise ValueError("push_dataset was called with nonempty stage.")
         if self.read_only:
             raise ValueError("push_dataset was called while repository is read-only.")
 
         self.pull_datasets()
+
+        prev_head = self.git_repo.head.commit
+
         parquet_path = self.repo_dir / (dataset.identifier + '.parquet')
         self.add(dataset)
         try:
             self.push()
         except Exception:
             # Restore original data
-            # git reset --hard origin/master
-            logger.debug("Hard-reset master branch to origin/master")
-            self.git_repo.head.reset('origin/master', index=True, working_tree=True)
+            self.git_repo.head.reset(prev_head, index=True, working_tree=True)
 
-            logger.debug(f"Checkout {parquet_path} from DVC")
-            self.dvc_repo.checkout(str(parquet_path), force=True)
+            tree = self.git_repo.head.commit.tree
+            dvc_file = dataset.identifier + '.parquet.dvc'
+            if dvc_file in tree:
+                logger.debug(f"Checkout {parquet_path} from DVC")
+                self.dvc_repo.checkout(str(parquet_path), force=True)
 
             # Remove rolled back stuff that may be left on the remote
             # self.dvc_repo.gc(all_commits=True, cloud=True, remote=self.dvc_remote)
             # TODO: Before reinstating the previous line, make sure gc doesn't delete blobs for which we don't have
             # a git commit because our git repository is outdated.
             raise
         finally:
@@ -269,15 +278,14 @@
         self.dataset_stage.append(DatasetStageItem(dataset))
 
     @ensure_repo_lock
     def push(self):
         """Upload, commit and push the staged files and clear the stage."""
         if self.read_only:
             raise ValueError("add was called while repository is read-only.")
-
         for stage_item in self.dataset_stage:
             path = self.repo_dir / (stage_item.identifier + '.parquet')
 
             # Remove old .dvc file (if it exists) and replace it with a new one
             dvc_file_path = path.parent / (path.name + '.dvc')
             if dvc_file_path.exists():
                 logger.debug(f"Remove file {dvc_file_path} from DVC")
@@ -297,15 +305,20 @@
             self.dvc_repo.push(str(dvc_file_path), remote=self.dvc_remote)
 
         # Commit and push
         if self._need_commit():
             identifiers = [stage_item.identifier for stage_item in self.dataset_stage]
             commit_message = f"Update {', '.join(identifiers)}"
             logger.debug(f"Create commit: {commit_message}")
-            self.git_repo.index.commit(commit_message)
+            commit = self.git_repo.index.commit(commit_message)
+            assert len(commit.parents) == 1
+            diff_index = commit.parents[0].diff(commit)
+            for diff in diff_index:
+                if diff.change_type not in ('A', 'M'):
+                    raise Exception("Invalid changes in the git commit (only additions and modifications allowed)")
             logger.debug("Push to git repository")
             git_push(self.git_repo)
         else:
             logger.debug("No commit needed")
 
         self.dataset_stage = []
```

### Comparing `dvc-pandas-0.1.1/src/dvc_pandas.egg-info/PKG-INFO` & `dvc-pandas-0.1.2/src/dvc_pandas.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
+
+
```

