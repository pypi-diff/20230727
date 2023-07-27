# Comparing `tmp/aquarium-python-api-2.0.6.tar.gz` & `tmp/aquarium-python-api-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.6.tar", last modified: Mon Jun 12 16:10:51 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.8.tar", last modified: Thu Jul 27 15:14:25 2023, max compression
```

## Comparing `aquarium-python-api-2.0.6.tar` & `aquarium-python-api-2.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.116188 aquarium-python-api-2.0.6/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.6/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-12 16:10:51.116544 aquarium-python-api-2.0.6/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.6/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.089125 aquarium-python-api-2.0.6/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.6/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.6/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.6/aquarium/auth.py
--rw-r--r--   0 yann       (501) staff       (20)     3541 2023-06-06 16:57:13.000000 aquarium-python-api-2.0.6/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.6/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.6/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.6/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    27598 2023-06-12 15:25:14.000000 aquarium-python-api-2.0.6/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.110702 aquarium-python-api-2.0.6/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.6/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.6/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.6/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.6/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.6/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.6/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.6/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.6/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4345 2023-06-05 10:38:49.000000 aquarium-python-api-2.0.6/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.6/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.6/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.6/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.115712 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-12 16:10:51.118658 aquarium-python-api-2.0.6/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.6/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-07-27 15:14:25.672978 aquarium-python-api-2.0.8/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.8/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-07-27 15:14:25.673502 aquarium-python-api-2.0.8/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.8/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-07-27 15:14:25.655217 aquarium-python-api-2.0.8/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.8/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.8/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.8/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3541 2023-06-06 16:57:13.000000 aquarium-python-api-2.0.8/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.8/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.8/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.8/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    27300 2023-07-27 15:11:50.000000 aquarium-python-api-2.0.8/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-07-27 15:14:25.668004 aquarium-python-api-2.0.8/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.8/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.8/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.8/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.8/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.8/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.8/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.8/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.8/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     6309 2023-06-28 11:02:05.000000 aquarium-python-api-2.0.8/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.8/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.8/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.8/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-07-27 15:14:25.672359 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-07-27 15:14:25.000000 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      703 2023-07-27 15:14:25.000000 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-07-27 15:14:25.000000 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-07-27 15:14:25.000000 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-07-27 15:14:25.000000 aquarium-python-api-2.0.8/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-07-27 15:14:25.674938 aquarium-python-api-2.0.8/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.8/setup.py
```

### Comparing `aquarium-python-api-2.0.6/LICENSE.md` & `aquarium-python-api-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/PKG-INFO` & `aquarium-python-api-2.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.6
+Version: 2.0.8
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.6/README.md` & `aquarium-python-api-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/__init__.py` & `aquarium-python-api-2.0.8/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/aquarium.py` & `aquarium-python-api-2.0.8/aquarium/aquarium.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/edge.py` & `aquarium-python-api-2.0.8/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/element.py` & `aquarium-python-api-2.0.8/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/entity.py` & `aquarium-python-api-2.0.8/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/exceptions.py` & `aquarium-python-api-2.0.8/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/item.py` & `aquarium-python-api-2.0.8/aquarium/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,39 +324,32 @@
         result = [self.parent.cast(data) for data in result]
         return result
 
     def get_permissions(self, sort=None, populate=False, offset=0, limit=50, depth=1, includeMembers=False):
         """
         Gets the permissions of the item
 
-        .. warning::
-            We are improving the behavior of depth and includeMembers parameters.
-            Feel free to reach our support if you have any questions.
-
         :param      sort:  Sort participants with a meshQL expression. Example: 'item.data.name ASC'
         :type       sort:  boolean, optional
         :param      populate:  Populate with User object
         :type       populate:  boolean, optional
         :param      offset:  Number of skipped items. Used for pagination
         :type       offset:  integer, optional
         :param      limit:  Maximum limit of returned items
         :type       limit:  integer, optional
-        :param      depth:  Get deeper participants.
-        :type       depth:  integer, optional
         :param      includeMembers:  Include members of the current item
         :type       includeMembers:  boolean, optional
 
         :returns:   List of edge and user
         :rtype:     list
         """
         params = dict(
             populate=populate,
             offset=offset,
             limit=limit,
-            depth=depth,
             includeMembers=includeMembers
         )
 
         if sort != None:
             params['sort'] = sort
 
         jsonify(params)
```

### Comparing `aquarium-python-api-2.0.6/aquarium/items/asset.py` & `aquarium-python-api-2.0.8/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/organisation.py` & `aquarium-python-api-2.0.8/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/playlist.py` & `aquarium-python-api-2.0.8/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/project.py` & `aquarium-python-api-2.0.8/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/task.py` & `aquarium-python-api-2.0.8/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/template.py` & `aquarium-python-api-2.0.8/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/items/user.py` & `aquarium-python-api-2.0.8/aquarium/items/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -125,7 +125,87 @@
                 "AND (<($Child, 5)- item._key == '{0}' AND path.vertices[*].type NONE == 'User')".format(project_key))
 
         query.append(")")
 
         result = self.traverse(meshql=' '.join(query))
         result = [self.parent.element(data) for data in result]
         return result
+
+    def promote_as_admin(self):
+        """
+        Promote the user as admin.
+
+        .. tip::
+            Admin users can
+                - administrate items
+                - access administrative panel
+
+        :returns:   Membership edge object
+        :rtype:     dict
+        """
+
+        domain = self.parent.usergroup('domain')
+        domain.add_user(self._key)
+
+    def promote_as_super_admin(self):
+        """
+        Promote the user as super admin.
+
+        .. tip::
+            Super admin users can
+                - add/remove licenses, users and files
+                - administrate items
+                - access administrative panel
+
+        :returns:   A dict with the {user: participant, edge: the created permission edge}
+        :rtype:     dict
+        """
+
+        domain = self.parent.usergroup('domain')
+
+        try:
+            domain.add_user(self._key)
+        except:
+            pass
+
+        return domain.create_permission(self._key, 'rwsadtlug', False)
+
+    def demote(self):
+        """
+        Remove admin and super admin privilege.
+
+        :returns:   None
+        """
+
+        domain = self.parent.usergroup('domain')
+
+        try:
+            domain.remove_user(self._key)
+            domain.remove_participant(self._key)
+        except:
+            pass
+
+    def get_admin_status(self):
+        """
+        Return user admin status (None, 'admin' or 'super admin')
+
+        :returns: Admin status of the user
+        :rtype: None or 'admin' or 'super admin'
+        """
+
+        status = None
+
+        domain = self.parent.usergroup('domain')
+        members = domain.get_users()
+
+        if (any([m for m in members if m._key == self._key])):
+                status = 'admin'
+
+        if status is not None:
+            domain_permissions = domain.get_permissions()
+            if (any([p for p in domain_permissions if p.user._key == self._key])):
+                status = 'super_admin'
+
+
+        return status
+
+
```

### Comparing `aquarium-python-api-2.0.6/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.8/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/tools.py` & `aquarium-python-api-2.0.8/aquarium/tools.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium/utils.py` & `aquarium-python-api-2.0.8/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.8/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.6
+Version: 2.0.8
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.6/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.8/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.6/setup.cfg` & `aquarium-python-api-2.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.0.6
+version = 2.0.8
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

