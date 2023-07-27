# Comparing `tmp/tikapi-3.1.22.tar.gz` & `tmp/tikapi-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikapi-3.1.22.tar", last modified: Fri Jun  9 14:15:02 2023, max compression
+gzip compressed data, was "tikapi-3.1.3.tar", last modified: Thu Jul 27 16:25:12 2023, max compression
```

## Comparing `tikapi-3.1.22.tar` & `tikapi-3.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.109197 tikapi-3.1.22/
--rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.22/MANIFEST.in
--rw-rw-rw-   0        0        0     1861 2023-06-09 14:15:02.109197 tikapi-3.1.22/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.22/README.md
--rw-rw-rw-   0        0        0      121 2023-06-09 14:15:02.109197 tikapi-3.1.22/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-06-09 14:14:47.000000 tikapi-3.1.22/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.103197 tikapi-3.1.22/tikapi/
--rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.22/tikapi/__init__.py
--rw-rw-rw-   0        0        0    64951 2023-06-09 14:13:46.000000 tikapi-3.1.22/tikapi/api.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:15:02.108198 tikapi-3.1.22/tikapi.egg-info/
--rw-rw-rw-   0        0        0     1861 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.22/tikapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 14:15:02.000000 tikapi-3.1.22/tikapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.753670 tikapi-3.1.3/
+-rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1860 2023-07-27 16:25:12.753670 tikapi-3.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.3/README.md
+-rw-rw-rw-   0        0        0      121 2023-07-27 16:25:12.754671 tikapi-3.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-07-27 13:38:19.000000 tikapi-3.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.748669 tikapi-3.1.3/tikapi/
+-rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.3/tikapi/__init__.py
+-rw-rw-rw-   0        0        0    86591 2023-07-27 16:23:25.000000 tikapi-3.1.3/tikapi/api.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.752670 tikapi-3.1.3/tikapi.egg-info/
+-rw-rw-rw-   0        0        0     1860 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.3/tikapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/top_level.txt
```

### Comparing `tikapi-3.1.22/PKG-INFO` & `tikapi-3.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.22
+Version: 3.1.3
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

### Comparing `tikapi-3.1.22/README.md` & `tikapi-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.22/setup.py` & `tikapi-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 INSTALL_REQUIRES = [
    'requests',
 ]
 
 setup(
     name='tikapi',
-    version='3.1.22',
+    version='3.1.3',
     description='TikAPI | TikTok Unofficial API',
     long_description_content_type="text/markdown",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     license='TikAPI',
     author='TikAPI',
     author_email='contact@tikapi.io',
     url='https://www.tikapi.io',
```

### Comparing `tikapi-3.1.22/tikapi/__init__.py` & `tikapi-3.1.3/tikapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.22/tikapi/api.py` & `tikapi-3.1.3/tikapi/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -509,14 +509,46 @@
 			'''
 				Get video information 
 			'''
 			
 			return wrap({"path":"/public/video","help":"Get video information","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.video")(id=id, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
+		def relatedPosts(cls, video_id: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get related posts 
+			'''
+			
+			return wrap({"path":"/public/related_posts","help":"Get related posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"video_id":{"help":"The video ID from which to get related posts. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.relatedPosts")(video_id=video_id, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
+		def playlists(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get an user playlists 
+			'''
+			count = None if count is cls.playlists.__defaults__[1] else count
+			return wrap({"path":"/public/playlists","help":"Get an user playlists","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.playlists")(secUid=secUid, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
+		def playlistItems(cls, playlist_id = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get a playlist items 
+			'''
+			count = None if count is cls.playlistItems.__defaults__[1] else count
+			return wrap({"path":"/public/playlist/items","help":"Get a playlist items","params":{"playlist_id":{"validate":"^[0-9]+$","required":True,"example":"6948562344666532614","help":"The playlist ID."},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.playlistItems")(playlist_id=playlist_id, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
+		def exploreCategory(cls, category_id = None, count: int = Default(30), country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get explore posts by category 
+			'''
+			count = None if count is cls.exploreCategory.__defaults__[1] else count
+			return wrap({"path":"/public/explore/category","help":"Get explore posts by category","comment":"The following categories are supported:<br/><br/>\n\t\t\t\"Comedy & Drama\": 1,<br/>\n\t\t\t\"Dance & Music\": 2,<br/>\n\t\t\t\"Relationships\": 3,<br/>\n\t\t\t\"Nature & Pets\": 4,<br/>\n\t\t\t\"Lifestyle\": 5,<br/>\n\t\t\t\"Society\": 6,<br/>\n\t\t\t\"Fashion\": 7,<br/>\n\t\t\t\"Entertainment\": 8,<br/>\n\t\t\t\"Informative\": 10,<br/>\n\t\t\t\"Sports & Outdoors\": 11,<br/>\n\t\t\t\"Auto & Vehicle\": 12,","params":{"category_id":{"validate":"^[0-9]+$","required":True,"example":"1","help":"The category ID."},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"}},"$other":{"openapi":{"hide":True,"fields":{"x-new":True,"x-beta":True}}},"method":"GET"}, cls.__get_options__(), "Public.exploreCategory")(category_id=category_id, count=count, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
 		def hashtag(cls, id: str = None, name: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get hashtag posts 
 			'''
 			count = None if count is cls.hashtag.__defaults__[2] else count
 			return wrap({"help":"Get hashtag posts","comment":"Your first request should be using the hashtag `name` parameter, then the following requests should be using the `id` parameter which you have stored from the first request (returned in response `challengeInfo > challenge > id`). <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/hashtag","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The hashtag ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","example":"4655293"},"name":{"type":"string","help":"The hashtag name"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.hashtag")(id=id, name=name, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
@@ -665,14 +697,54 @@
 			'''
 				Get liked posts 
 			'''
 			count = None if count is cls.likes.__defaults__[0] else count
 			return wrap({"help":"Get liked posts","comment":"Get current user liked posts, or someone elses by providing the `secUid` parameter.","path":"/user/likes","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["explore"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.likes")(count=count, secUid=secUid, cursor=cursor, **otherParams)
 	
 		@classmethod
+		def followingPosts(cls, count: int = Default(30), cursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get following posts 
+			'''
+			count = None if count is cls.followingPosts.__defaults__[0] else count
+			return wrap({"path":"/user/following_posts","help":"Get following posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["explore"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.followingPosts")(count=count, cursor=cursor, **otherParams)
+	
+		@classmethod
+		def relatedPosts(cls, video_id: str = None, **otherParams) -> APIResponse:
+			'''
+				Get related posts 
+			'''
+			
+			return wrap({"path":"/user/related_posts","help":"Get related posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"video_id":{"help":"The video ID from which to get related posts. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["explore"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.relatedPosts")(video_id=video_id, **otherParams)
+	
+		@classmethod
+		def savedPosts(cls, count: int = Default(30), cursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get saved posts 
+			'''
+			count = None if count is cls.savedPosts.__defaults__[0] else count
+			return wrap({"path":"/user/saved","help":"Get saved posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["view_collections"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.savedPosts")(count=count, cursor=cursor, **otherParams)
+	
+		@classmethod
+		def playlists(cls, secUid: str = None, count: int = Default(30), cursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get user playlists 
+			'''
+			count = None if count is cls.playlists.__defaults__[1] else count
+			return wrap({"path":"/user/playlists","help":"Get user playlists","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":False},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["view_collections"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.playlists")(secUid=secUid, count=count, cursor=cursor, **otherParams)
+	
+		@classmethod
+		def playlistItems(cls, playlist_id = None, count: int = Default(30), cursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get a playlist items 
+			'''
+			count = None if count is cls.playlistItems.__defaults__[1] else count
+			return wrap({"path":"/user/playlist/items","help":"Get a playlist items","params":{"playlist_id":{"validate":"^[0-9]+$","required":True,"example":"6948562344666532614","help":"The playlist ID."},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["view_collections"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.playlistItems")(playlist_id=playlist_id, count=count, cursor=cursor, **otherParams)
+	
+		@classmethod
 		def explore(cls, count: int = Default(30), **otherParams) -> APIResponse:
 			'''
 				Get trending posts 
 			'''
 			count = None if count is cls.explore.__defaults__[0] else count
 			return wrap({"help":"Get trending posts","comment":"Get current user recommended posts from the *For You* section.","path":"/user/explore","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["explore"]}]}}},"method":"GET"}, cls.__get_options__(), "UserPosts.explore")(count=count, **otherParams)
 	
@@ -698,14 +770,76 @@
 				Unlike a video 
 			'''
 			
 			return wrap({"help":"Unlike a video","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n","path":"/user/unlike","method":"POST","enctype":"json","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["media_actions"]}]}}}}, cls.__get_options__(), "UserPosts.unlike")(media_id=media_id, **otherParams)
 	
 		comments = Rests.UserPostsComments
 	Rests.UserPosts = UserPosts
+	class UserConversationRequests(Rests.BaseClass):
+		'''
+			ConversationRequests Endpoints Category 
+		'''
+
+		__options__ = {"headers":{},"params":{"accountKey":{"name":"X-ACCOUNT-KEY","required":True,"help":"The Account Key is required","location":"headers","validate":"^[a-zA-Z0-9]{10,}$","example":"DemoAccountKeyTokenSeHYGXDfd4SFD320Sc39Asd0Sc39A","$initsOnly":True}},"values":{},"$other":{"openapi":{"fields":{"parameters":[],"responses":{},"tags":["Messages"],"security":[{"apiKey":[],"accountKey":["conversation_requests"]}],"x-new":True}}}}
+
+		def __new__(self, **values) -> 'UserConversationRequests':
+			'''
+				Initialize new 'UserConversationRequests' instance with default values & options
+			'''
+			return super().__new__(self, **values)
+
+		@classmethod
+		def set(self, **values) -> 'UserConversationRequests':
+			'''
+				Method is only available for the root category.
+				Set default values & options for 'UserConversationRequests'
+			'''
+			return super().set(**values)
+	
+		@classmethod
+		def conversations(cls, nextCursor: int = None, **otherParams) -> APIResponse:
+			'''
+				Get user conversation requests 
+			'''
+			
+			return wrap({"path":"/user/conversations/requests","help":"Get user conversation requests","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\nGet a list of current user conversations requests including the latest message.","params":{"nextCursor":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "UserConversationRequests.conversations")(nextCursor=nextCursor, **otherParams)
+	
+		@classmethod
+		def messages(cls, conversation_id = None, conversation_short_id = None, **otherParams) -> APIResponse:
+			'''
+				Get a conversation request messages 
+			'''
+			
+			return wrap({"path":"/user/messages/requests","help":"Get a conversation request messages","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\nGet the messages of a conversation in the requests tab (generally there is a 3 message limit).","params":{"conversation_id":{"help":"The conversation ID","required":True,"example":"0:1:684574219823284956:69402435203845897564"},"conversation_short_id":{"help":"The additional conversation short ID","required":True,"example":"6940245147502654884"}},"method":"GET"}, cls.__get_options__(), "UserConversationRequests.messages")(conversation_id=conversation_id, conversation_short_id=conversation_short_id, **otherParams)
+	
+		@classmethod
+		def markRead(cls, conversation_id = None, conversation_short_id = None, **otherParams) -> APIResponse:
+			'''
+				Mark a requests conversation as read 
+			'''
+			
+			return wrap({"path":"/user/conversations/requests/mark_read","help":"Mark a requests conversation as read","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\n","params":{"conversation_id":{"help":"The conversation ID","required":True,"example":"0:1:684574219823284956:69402435203845897564"},"conversation_short_id":{"help":"The additional conversation short ID","required":True,"example":"6940245147502654884"}},"$other":{"openapi":{"hide":True}},"method":"GET"}, cls.__get_options__(), "UserConversationRequests.markRead")(conversation_id=conversation_id, conversation_short_id=conversation_short_id, **otherParams)
+	
+		@classmethod
+		def delete(cls, conversation_id = None, conversation_short_id = None, **otherParams) -> APIResponse:
+			'''
+				Delete a conversation request 
+			'''
+			
+			return wrap({"path":"/user/conversations/requests/delete","help":"Delete a conversation request","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\n","params":{"conversation_id":{"help":"The conversation ID","required":True,"example":"0:1:684574219823284956:69402435203845897564"},"conversation_short_id":{"help":"The additional conversation short ID","required":True,"example":"6940245147502654884"}},"method":"GET"}, cls.__get_options__(), "UserConversationRequests.delete")(conversation_id=conversation_id, conversation_short_id=conversation_short_id, **otherParams)
+	
+		@classmethod
+		def accept(cls, conversation_id = None, conversation_short_id = None, user_id: str = None, **otherParams) -> APIResponse:
+			'''
+				Accept a conversation request 
+			'''
+			
+			return wrap({"path":"/user/conversations/requests/accept","help":"Accept a conversation request","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\n","params":{"conversation_id":{"help":"The conversation ID","required":True,"example":"0:1:684574219823284956:69402435203845897564"},"conversation_short_id":{"help":"The additional conversation short ID","required":True,"example":"6940245147502654884"},"user_id":{"help":"The sender ID.","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"method":"GET"}, cls.__get_options__(), "UserConversationRequests.accept")(conversation_id=conversation_id, conversation_short_id=conversation_short_id, user_id=user_id, **otherParams)
+	
+	Rests.UserConversationRequests = UserConversationRequests
 	class UserLive(Rests.BaseClass):
 		'''
 			Live Endpoints Category 
 		'''
 
 		__options__ = {"headers":{},"params":{"accountKey":{"name":"X-ACCOUNT-KEY","required":True,"help":"The Account Key is required","location":"headers","validate":"^[a-zA-Z0-9]{10,}$","example":"DemoAccountKeyTokenSeHYGXDfd4SFD320Sc39Asd0Sc39A","$initsOnly":True}},"values":{},"$other":{"openapi":{"fields":{"parameters":[],"responses":{},"tags":["Live"],"security":[{"apiKey":[],"accountKey":["live"]}]}}}}
 
@@ -797,15 +931,47 @@
 	
 		@classmethod
 		def transactionHistory(cls, page = None, count = None, **otherParams) -> APIResponse:
 			'''
 				Get coin transactions history 
 			'''
 			
-			return wrap({"help":"Get coin transactions history","path":"/user/wallet/transactions","params":{"page":{"help":"The list page number","example":1},"count":{"help":"The items limit per page","example":12}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_profile"]}]}}},"method":"GET"}, cls.__get_options__(), "UserLive.transactionHistory")(page=page, count=count, **otherParams)
+			return wrap({"help":"Get coin transactions history","path":"/user/wallet/transactions","params":{"page":{"help":"The list page number","example":1},"count":{"help":"The items limit per page","example":12}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_coins"]}]}}},"method":"GET"}, cls.__get_options__(), "UserLive.transactionHistory")(page=page, count=count, **otherParams)
+	
+		@classmethod
+		def search(cls, query: str = None, cursor: int = None, **otherParams) -> APIResponse:
+			'''
+				Search live videos 
+			'''
+			
+			return wrap({"help":"Search live videos","path":"/user/search/live","params":{"query":{"type":"string","example":"lilyachty","required":True,"help":"The search keyword"},"cursor":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "UserLive.search")(query=query, cursor=cursor, **otherParams)
+	
+		@classmethod
+		def analytics(cls, days: int = Default(7), **otherParams) -> APIResponse:
+			'''
+				Get live analytics 
+			'''
+			days = None if days is cls.analytics.__defaults__[0] else days
+			return wrap({"help":"Get live analytics","path":"/user/live/analytics","params":{"days":{"default":7,"help":"The days time frame for the analytics data","validate":"^[0-9]+$","type":"number"}},"$other":{"openapi":{"fields":{"x-new":True,"security":[{"apiKey":[],"accountKey":["view_analytics"]}]}}},"method":"GET"}, cls.__get_options__(), "UserLive.analytics")(days=days, **otherParams)
+	
+		@classmethod
+		def list(cls, count: int = Default(30), offset: int = None, sort: int = None, **otherParams) -> APIResponse:
+			'''
+				Get live videos list 
+			'''
+			count = None if count is cls.list.__defaults__[0] else count
+			return wrap({"help":"Get live videos list","path":"/user/live/list","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"offset":{"help":"The starting offset of items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"},"sort":{"help":"Sort results by ascending (1) or descending (0). Default is descending (0).","in":[0,1],"default":0,"type":"number","example":1}},"$other":{"openapi":{"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "UserLive.list")(count=count, offset=offset, sort=sort, **otherParams)
+	
+		@classmethod
+		def details(cls, room_id: str = None, **otherParams) -> APIResponse:
+			'''
+				Get a live video details 
+			'''
+			
+			return wrap({"help":"Get a live video details","path":"/user/live/detail","params":{"room_id":{"help":"The Live room ID.","type":"string","example":"7112492061034646278","required":True}},"$other":{"openapi":{"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "UserLive.details")(room_id=room_id, **otherParams)
 	
 	Rests.UserLive = UserLive
 	class User(Rests.BaseClass):
 		'''
 			The user endpoints require an `accountKey` 
 		'''
 
@@ -844,55 +1010,71 @@
 		@classmethod
 		def notifications(cls, filter: str = Default("all"), count: int = Default(30), max_time = None, min_time = None, **otherParams) -> APIResponse:
 			'''
 				Get notifications 
 			'''
 			filter = None if filter is cls.notifications.__defaults__[0] else filter
 			count = None if count is cls.notifications.__defaults__[1] else count
-			return wrap({"help":"Get notifications","comment":"Get current user recent notifications.<br><br>*Note: Some notifications are limited by TikTok.*","path":"/user/notifications","params":{"filter":{"default":"all","help":"Filter notifications by type","type":"string","in":["all","likes","comments","mentions","followers"]},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"max_time":{"name":"max_time","help":"Returned in every response, should be included in the next request for iteration.","validate":"^[0-9]+$"},"min_time":{"help":"Returned in every response, should be included in the next request for iteration.","name":"min_time","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_profile"]}],"tags":["Profile"]}}},"method":"GET"}, cls.__get_options__(), "User.notifications")(filter=filter, count=count, max_time=max_time, min_time=min_time, **otherParams)
+			return wrap({"help":"Get notifications","comment":"Get current user recent notifications.<br><br>*Note: Some notifications are limited by TikTok.*","path":"/user/notifications","params":{"filter":{"default":"all","help":"Filter notifications by type","type":"string","in":["all","likes","comments","mentions","followers"]},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"max_time":{"name":"max_time","help":"Returned in every response, should be included in the next request for iteration.","validate":"^[0-9]+$"},"min_time":{"help":"Returned in every response, should be included in the next request for iteration.","name":"min_time","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_notifications"]}],"tags":["Profile"]}}},"method":"GET"}, cls.__get_options__(), "User.notifications")(filter=filter, count=count, max_time=max_time, min_time=min_time, **otherParams)
 	
 		@classmethod
 		def analytics(cls, type: str = None, days: int = Default(7), media_id = None, **otherParams) -> APIResponse:
 			'''
 				Get analytics 
 			'''
 			days = None if days is cls.analytics.__defaults__[1] else days
-			return wrap({"help":"Get analytics","comment":"Get analytics for business or creator accounts","path":"/creator/analytics/{type}","params":{"type":{"required":True,"in":["overview","content","video","followers","live"],"type":"string","help":"The analytics type","example":"overview","location":"path"},"days":{"default":7,"help":"The days time frame of analytics data","validate":"^[0-9]+$","type":"number"},"media_id":{"help":"Required only for **video** type analytics, otherwise don't include.","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_profile"]}],"tags":["Profile"]}}},"method":"GET"}, cls.__get_options__(), "User.analytics")(type=type, days=days, media_id=media_id, **otherParams)
+			return wrap({"help":"Get analytics","comment":"Get analytics for business or creator accounts","path":"/creator/analytics/{type}","params":{"type":{"required":True,"in":["overview","content","video","followers","live"],"type":"string","help":"The analytics type","example":"overview","location":"path"},"days":{"default":7,"help":"The days time frame for the analytics data","validate":"^[0-9]+$","type":"number"},"media_id":{"help":"Required only for **video** type analytics, otherwise don't include.","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_profile"]}],"tags":["Profile"]}}},"method":"GET"}, cls.__get_options__(), "User.analytics")(type=type, days=days, media_id=media_id, **otherParams)
 	
 		@classmethod
 		def verify(cls, **otherParams) -> APIResponse:
 			'''
 				Check session 
 			'''
 			
 			return wrap({"help":"Check session","comment":"Check if the current user's session is valid. Auto-removes the user if it's invalid. <br><br>*Note: The session is automatically checked, though you can still manually call this endpoint if you are having issues with a user.*","path":"/user/session/check","$other":{"openapi":{"fields":{"security":[{"apiKey":[],"accountKey":["view_profile"]}],"tags":["Profile"],"responses":{"428":{"$ref":"./error_responses/428.yaml"}}}}},"method":"GET","params":{}}, cls.__get_options__(), "User.verify")(**otherParams)
 	
 		@classmethod
-		def following(cls, count: int = Default(30), cursor: int = None, **otherParams) -> APIResponse:
+		def followingV1(cls, count: int = Default(30), cursor: int = None, **otherParams) -> APIResponse:
 			'''
 				Get following list 
 			'''
-			count = None if count is cls.following.__defaults__[0] else count
-			return wrap({"help":"Get following list","comment":"Get current user's following list","path":"/user/following","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{"fields":{"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["view_profile"]}]}}},"method":"GET"}, cls.__get_options__(), "User.following")(count=count, cursor=cursor, **otherParams)
+			count = None if count is cls.followingV1.__defaults__[0] else count
+			return wrap({"help":"Get following list","comment":"Get current user's following list","path":"/user/following/v1","params":{"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{"hide":True,"fields":{"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["view_followers"]}]}}},"method":"GET"}, cls.__get_options__(), "User.followingV1")(count=count, cursor=cursor, **otherParams)
+	
+		@classmethod
+		def following(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get following list 
+			'''
+			count = None if count is cls.following.__defaults__[1] else count
+			return wrap({"help":"Get following list","comment":"Get current user following list (or a friends by specifying the secUid).","path":"/user/following","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{"fields":{"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["view_followers"]}]}}},"method":"GET"}, cls.__get_options__(), "User.following")(secUid=secUid, count=count, nextCursor=nextCursor, **otherParams)
+	
+		@classmethod
+		def followers(cls, secUid: str = None, count: int = Default(30), nextCursor: str = None, **otherParams) -> APIResponse:
+			'''
+				Get followers list 
+			'''
+			count = None if count is cls.followers.__defaults__[1] else count
+			return wrap({"help":"Get followers list","comment":"Get current user followers list (or a friends by specifying the secUid).","path":"/user/followers","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{"fields":{"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["view_followers"]}]}}},"method":"GET"}, cls.__get_options__(), "User.followers")(secUid=secUid, count=count, nextCursor=nextCursor, **otherParams)
 	
 		@classmethod
 		def follow(cls, username: str = None, secUid: str = None, user_id: str = None, **otherParams) -> APIResponse:
 			'''
 				Follow an user 
 			'''
 			
-			return wrap({"help":"Follow an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/follow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.follow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
+			return wrap({"help":"Follow an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/follow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.follow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
 	
 		@classmethod
 		def unfollow(cls, username: str = None, secUid: str = None, user_id: str = None, **otherParams) -> APIResponse:
 			'''
 				Unfollows an user 
 			'''
 			
-			return wrap({"help":"Unfollows an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/unfollow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.unfollow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
+			return wrap({"help":"Unfollows an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/unfollow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.unfollow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
 	
 		posts = Rests.UserPosts
 		@classmethod
 		def conversations(cls, nextCursor: int = None, **otherParams) -> APIResponse:
 			'''
 				Get user conversations 
 			'''
@@ -911,14 +1093,15 @@
 		def sendMessage(cls, text: str = None, conversation_id: str = None, conversation_short_id: str = None, ticket: str = None, **otherParams) -> APIResponse:
 			'''
 				Send a message 
 			'''
 			
 			return wrap({"path":"/user/message/send","help":"Send a message","comment":"**Premium**<img title='Only Business and Enterprise subscriptions can access this\nendpoint' style='margin-bottom: -3px;cursor: help;'\nsrc='/assets/img/star.png' width='18px'><br/>\n*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n","method":"POST","params":{"text":{"required":True,"type":"string","help":"The message text","example":"Hey! How you doing?"},"conversation_id":{"help":"The conversation ID","required":True,"type":"string","example":"0:1:684574219823284956:69402435203845897564"},"conversation_short_id":{"help":"The additional conversation short ID (TikTok uses two different ID's for some reason)","required":True,"type":"string","example":"6940245147502654884"},"ticket":{"help":"The conversation ticket","required":True,"type":"string","example":"3M8IlBpABq00h2aNB1B5JJ2ne0DTnGLLAFjGQQGMf4BKWJxEYxf7RAE0KaD2EjkQkWiJalT4xj36JGWa1ZmQg7SgQfHLoXffNFYLkIJhe1HVyiPXitoxWFyuzlX1xvBCYhZxkQALHE4gx9AaXBPEZjks7jC"}},"$other":{"openapi":{"fields":{"tags":["Messages"],"security":[{"apiKey":[],"accountKey":["send_messages"]}]}}}}, cls.__get_options__(), "User.sendMessage")(text=text, conversation_id=conversation_id, conversation_short_id=conversation_short_id, ticket=ticket, **otherParams)
 	
+		conversationRequests = Rests.UserConversationRequests
 		live = Rests.UserLive
 	Rests.User = User
 	class API(Rests.BaseClass):
 		
 
 		__options__ = {}
```

### Comparing `tikapi-3.1.22/tikapi.egg-info/PKG-INFO` & `tikapi-3.1.3/tikapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.22
+Version: 3.1.3
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

