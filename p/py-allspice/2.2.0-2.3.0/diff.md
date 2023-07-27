# Comparing `tmp/py-allspice-2.2.0.tar.gz` & `tmp/py-allspice-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-allspice-2.2.0.tar", last modified: Thu Jul 20 20:07:05 2023, max compression
+gzip compressed data, was "py-allspice-2.3.0.tar", last modified: Thu Jul 27 16:52:22 2023, max compression
```

## Comparing `py-allspice-2.2.0.tar` & `py-allspice-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 20:06:48.000000 py-allspice-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-20 20:07:05.506049 py-allspice-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-20 20:06:48.000000 py-allspice-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.502049 py-allspice-2.2.0/allspice/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/allspice.py
--rw-r--r--   0 runner    (1001) docker     (123)    58771 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/ratelimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:07:05.506049 py-allspice-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 20:06:54.000000 py-allspice-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api_longtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api_ratelimiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:22.758330 py-allspice-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 16:52:13.000000 py-allspice-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 16:52:22.754330 py-allspice-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-27 16:52:13.000000 py-allspice-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:22.754330 py-allspice-2.3.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58902 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:22.754330 py-allspice-2.3.0/allspice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-27 16:52:13.000000 py-allspice-2.3.0/allspice/utils/bom_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:22.754330 py-allspice-2.3.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 16:52:22.000000 py-allspice-2.3.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-27 16:52:22.000000 py-allspice-2.3.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:52:22.000000 py-allspice-2.3.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 16:52:22.000000 py-allspice-2.3.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 16:52:22.000000 py-allspice-2.3.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:52:22.758330 py-allspice-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 16:52:15.000000 py-allspice-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:52:22.754330 py-allspice-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-07-27 16:52:13.000000 py-allspice-2.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-27 16:52:13.000000 py-allspice-2.3.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-27 16:52:13.000000 py-allspice-2.3.0/tests/test_api_ratelimiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-27 16:52:13.000000 py-allspice-2.3.0/tests/test_utils.py
```

### Comparing `py-allspice-2.2.0/LICENSE` & `py-allspice-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/PKG-INFO` & `py-allspice-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.2.0
+Version: 2.3.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/Langenfeld/py-gitea
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py-allspice-2.2.0/README.md` & `py-allspice-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/allspice/__init__.py` & `py-allspice-2.3.0/allspice/__init__.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/allspice/allspice.py` & `py-allspice-2.3.0/allspice/allspice.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/allspice/apiobject.py` & `py-allspice-2.3.0/allspice/apiobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,31 +407,31 @@
             owner: str,
             name: str,
     ) -> Repository:
         return cls._request(allspice_client, {"owner": owner, "name": name})
 
     @classmethod
     def search(
-        cls, 
+        cls,
         allspice_client: 'AllSpice',
         query: Optional[str] = None,
         topic: bool = False,
         include_description: bool = False,
         user: Optional[User] = None,
         owner_to_prioritize: Union[User, Organization, None] = None,
     ) -> list[Repository]:
         """
         Search for repositories.
 
-        See https://hub.allspice.io/api/swagger#/repository/repoSearch 
+        See https://hub.allspice.io/api/swagger#/repository/repoSearch
 
         :param query: The query string to search for
-        :param topic: If true, the query string will only be matched against the 
+        :param topic: If true, the query string will only be matched against the
             repository's topic.
-        :param include_description: If true, the query string will be matched 
+        :param include_description: If true, the query string will be matched
             against the repository's description as well.
         :param user: If specified, only repositories that this user owns or
             contributes to will be searched.
         :param owner_to_prioritize: If specified, repositories owned by the
             given entity will be prioritized in the search.
         :returns: All repositories matching the query. If there are many
             repositories matching this query, this may take some time.
@@ -448,15 +448,15 @@
         if user is not None:
             params["user"] = user.id
         if owner_to_prioritize is not None:
             params["owner_to_prioritize"] = owner_to_prioritize.id
 
         responses = allspice_client.requests_get_paginated(cls.REPO_SEARCH, params=params)
 
-        return [Repository.parse_response(allspice_client, response) 
+        return [Repository.parse_response(allspice_client, response)
                 for response in responses]
 
 
     _patchable_fields = {
         "allow_manual_merge",
         "allow_merge_commits",
         "allow_rebase",
@@ -971,24 +971,24 @@
         return self.allspice_client.requests_get(url)["topics"]
 
 
     def add_topic(self, topic: str):
         """
         Adds a topic to the repository.
 
-        See https://hub.allspice.io/api/swagger#/repository/repoAddTopic 
+        See https://hub.allspice.io/api/swagger#/repository/repoAddTopic
 
         :param topic: The topic to add. Topic names must consist only of
             lowercase letters, numnbers and dashes (-), and cannot start with
             dashes. Topic names also must be under 35 characters long.
         """
 
         url = self.REPO_ADD_TOPIC.format(
-            owner=self.owner.username, 
-            repo=self.name, 
+            owner=self.owner.username,
+            repo=self.name,
             topic=topic
         )
         self.allspice_client.requests_put(url)
 
 
 
     def delete(self):
@@ -1544,16 +1544,20 @@
         self._commit(args)
 
     def add_user(self, user: User):
         """https://hub.allspice.io/api/swagger#/organization/orgAddTeamMember"""
         url = f"/teams/{self.id}/members/{user.login}"
         self.allspice_client.requests_put(url)
 
-    def add_repo(self, org: Organization, repo: Repository):
-        self.allspice_client.requests_put(Team.ADD_REPO % (self.id, org, repo.name))
+    def add_repo(self, org: Organization, repo: Union[Repository, str]):
+        if isinstance(repo, Repository):
+            repo_name = repo.name
+        else:
+            repo_name = repo
+        self.allspice_client.requests_put(Team.ADD_REPO % (self.id, org.username, repo_name))
 
     def get_members(self):
         """ Get all users assigned to the team. """
         results = self.allspice_client.requests_get(Team.GET_MEMBERS % self.id)
         return [User.parse_response(self.allspice_client, result) for result in results]
 
     def get_repos(self):
```

### Comparing `py-allspice-2.2.0/allspice/baseapiobject.py` & `py-allspice-2.3.0/allspice/baseapiobject.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/allspice/exceptions.py` & `py-allspice-2.3.0/allspice/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/allspice/ratelimiter.py` & `py-allspice-2.3.0/allspice/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/py_allspice.egg-info/PKG-INFO` & `py-allspice-2.3.0/py_allspice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.2.0
+Version: 2.3.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/Langenfeld/py-gitea
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py-allspice-2.2.0/setup.py` & `py-allspice-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='py-allspice',
-    version='2.2.0',
+    version='2.3.0',
     description='A python wrapper for the AllSpice Hub API',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='AllSpice, Inc.',
     author_email='maintainers@allspice.io',
```

### Comparing `py-allspice-2.2.0/tests/test_api.py` & `py-allspice-2.3.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,14 +319,31 @@
 def test_create_team(instance):
     org = Organization.request(instance, test_org)
     team = instance.create_team(org, test_team, "descr")
     assert team.name == test_team
     assert team.description == "descr"
     assert team.organization == org
 
+def test_add_repo_to_team(instance):
+    org = Organization.request(instance, test_org)
+    team = org.get_team(test_team)
+    repository = Repository.request(instance, test_org, test_repo)
+
+    # First with name
+    team.add_repo(org, test_repo)
+    assert test_repo in [repo.name for repo in team.get_repos()]
+
+    team.delete()
+
+    team = instance.create_team(org, test_team, "descr")
+    # Then with object
+    team.add_repo(org, repository)
+    assert test_repo in [repo.name for repo in team.get_repos()]
+
+
 def test_create_team_without_units_map(instance):
     org = Organization.request(instance, test_org)
     team = instance.create_team(org, test_team + "1", "descr")
     permission = team.permission
     assert set(team.units_map.keys()) == set(team.units)
     assert list(team.units_map.values()) == [permission] * len(team.units)
```

### Comparing `py-allspice-2.2.0/tests/test_api_longtests.py` & `py-allspice-2.3.0/tests/test_api_longtests.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.2.0/tests/test_api_ratelimiting.py` & `py-allspice-2.3.0/tests/test_api_ratelimiting.py`

 * *Files identical despite different names*

