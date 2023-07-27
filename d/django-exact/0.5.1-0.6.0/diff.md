# Comparing `tmp/django-exact-0.5.1.tar.gz` & `tmp/django-exact-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-exact-0.5.1.tar", last modified: Wed Sep 28 10:44:01 2022, max compression
+gzip compressed data, was "django-exact-0.6.0.tar", last modified: Thu Jul 27 09:13:02 2023, max compression
```

## Comparing `django-exact-0.5.1.tar` & `django-exact-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.737170 django-exact-0.5.1/
--rw-r--r--   0 maldn     (1000) users      (100)      150 2019-06-17 10:35:24.000000 django-exact-0.5.1/.editorconfig
--rw-r--r--   0 maldn     (1000) users      (100)      211 2017-02-23 11:03:30.000000 django-exact-0.5.1/.gitignore
--rw-r--r--   0 maldn     (1000) users      (100)      511 2022-09-28 10:37:48.000000 django-exact-0.5.1/CHANGELOG.md
--rw-r--r--   0 maldn     (1000) users      (100)     1085 2017-02-23 11:31:28.000000 django-exact-0.5.1/LICENSE.txt
--rw-r--r--   0 maldn     (1000) users      (100)       74 2017-05-09 10:02:48.000000 django-exact-0.5.1/MANIFEST.in
--rw-r--r--   0 maldn     (1000) users      (100)      297 2022-09-28 10:44:01.737170 django-exact-0.5.1/PKG-INFO
--rw-r--r--   0 maldn     (1000) users      (100)     2326 2018-09-21 13:59:58.000000 django-exact-0.5.1/README.md
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.737170 django-exact-0.5.1/django_exact.egg-info/
--rw-r--r--   0 maldn     (1000) users      (100)      297 2022-09-28 10:44:01.000000 django-exact-0.5.1/django_exact.egg-info/PKG-INFO
--rw-r--r--   0 maldn     (1000) users      (100)      516 2022-09-28 10:44:01.000000 django-exact-0.5.1/django_exact.egg-info/SOURCES.txt
--rw-r--r--   0 maldn     (1000) users      (100)        1 2022-09-28 10:44:01.000000 django-exact-0.5.1/django_exact.egg-info/dependency_links.txt
--rw-r--r--   0 maldn     (1000) users      (100)       24 2022-09-28 10:44:01.000000 django-exact-0.5.1/django_exact.egg-info/requires.txt
--rw-r--r--   0 maldn     (1000) users      (100)        6 2022-09-28 10:44:01.000000 django-exact-0.5.1/django_exact.egg-info/top_level.txt
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.737170 django-exact-0.5.1/exact/
--rw-r--r--   0 maldn     (1000) users      (100)        0 2017-02-23 11:00:54.000000 django-exact-0.5.1/exact/__init__.py
--rw-r--r--   0 maldn     (1000) users      (100)      698 2020-03-11 15:34:29.000000 django-exact-0.5.1/exact/admin.py
--rw-r--r--   0 maldn     (1000) users      (100)    11197 2022-01-07 12:33:23.000000 django-exact-0.5.1/exact/api.py
--rw-r--r--   0 maldn     (1000) users      (100)      214 2020-03-11 15:47:56.000000 django-exact-0.5.1/exact/app.py
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.737170 django-exact-0.5.1/exact/migrations/
--rw-r--r--   0 maldn     (1000) users      (100)     2415 2020-03-11 15:39:46.000000 django-exact-0.5.1/exact/migrations/0001_initial.py
--rw-r--r--   0 maldn     (1000) users      (100)        0 2017-02-23 11:00:54.000000 django-exact-0.5.1/exact/migrations/__init__.py
--rw-r--r--   0 maldn     (1000) users      (100)     2099 2020-03-11 15:34:29.000000 django-exact-0.5.1/exact/models.py
--rw-r--r--   0 maldn     (1000) users      (100)     1195 2020-03-11 15:34:29.000000 django-exact-0.5.1/exact/signals.py
--rw-r--r--   0 maldn     (1000) users      (100)     1491 2020-03-11 15:34:29.000000 django-exact-0.5.1/exact/storage.py
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.733170 django-exact-0.5.1/exact/templates/
-drwxr-xr-x   0 maldn     (1000) users      (100)        0 2022-09-28 10:44:01.737170 django-exact-0.5.1/exact/templates/exact/
--rw-r--r--   0 maldn     (1000) users      (100)      772 2017-04-06 13:29:52.000000 django-exact-0.5.1/exact/templates/exact/status.html
--rw-r--r--   0 maldn     (1000) users      (100)      283 2022-07-07 10:42:10.000000 django-exact-0.5.1/exact/urls.py
--rw-r--r--   0 maldn     (1000) users      (100)     2552 2020-03-11 15:39:03.000000 django-exact-0.5.1/exact/views.py
--rw-r--r--   0 maldn     (1000) users      (100)      104 2022-01-07 12:58:59.000000 django-exact-0.5.1/pyproject.toml
--rw-r--r--   0 maldn     (1000) users      (100)       38 2022-09-28 10:44:01.737170 django-exact-0.5.1/setup.cfg
--rw-r--r--   0 maldn     (1000) users      (100)     1225 2022-09-28 10:42:26.000000 django-exact-0.5.1/setup.py
--rw-r--r--   0 maldn     (1000) users      (100)       56 2017-02-23 10:59:51.000000 django-exact-0.5.1/tox.ini
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.746142 django-exact-0.6.0/
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     1086 2023-07-27 09:06:58.000000 django-exact-0.6.0/LICENSE.txt
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)       74 2021-08-31 10:34:19.000000 django-exact-0.6.0/MANIFEST.in
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      297 2023-07-27 09:13:02.742142 django-exact-0.6.0/PKG-INFO
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     2326 2021-08-31 10:34:19.000000 django-exact-0.6.0/README.md
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.742142 django-exact-0.6.0/django_exact.egg-info/
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      297 2023-07-27 09:13:02.000000 django-exact-0.6.0/django_exact.egg-info/PKG-INFO
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      519 2023-07-27 09:13:02.000000 django-exact-0.6.0/django_exact.egg-info/SOURCES.txt
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)        1 2023-07-27 09:13:02.000000 django-exact-0.6.0/django_exact.egg-info/dependency_links.txt
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)       24 2023-07-27 09:13:02.000000 django-exact-0.6.0/django_exact.egg-info/requires.txt
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)        6 2023-07-27 09:13:02.000000 django-exact-0.6.0/django_exact.egg-info/top_level.txt
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.742142 django-exact-0.6.0/exact/
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)        0 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/__init__.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      698 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/admin.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)    11430 2023-07-27 09:00:03.000000 django-exact-0.6.0/exact/api.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      214 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/app.py
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.742142 django-exact-0.6.0/exact/migrations/
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     2415 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/migrations/0001_initial.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      293 2023-07-27 09:00:03.000000 django-exact-0.6.0/exact/migrations/0002_remove_session_division.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)        0 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/migrations/__init__.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     2065 2023-07-27 09:00:03.000000 django-exact-0.6.0/exact/models.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     1195 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/signals.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     1491 2021-08-31 10:34:19.000000 django-exact-0.6.0/exact/storage.py
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.742142 django-exact-0.6.0/exact/templates/
+drwxrwxr-x   0 maldn     (1001) maldn     (1001)        0 2023-07-27 09:13:02.742142 django-exact-0.6.0/exact/templates/exact/
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      628 2023-07-27 09:00:03.000000 django-exact-0.6.0/exact/templates/exact/status.html
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      283 2022-08-29 09:54:04.000000 django-exact-0.6.0/exact/urls.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     2385 2023-07-27 09:00:03.000000 django-exact-0.6.0/exact/views.py
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)      104 2022-01-11 13:59:33.000000 django-exact-0.6.0/pyproject.toml
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)       38 2023-07-27 09:13:02.746142 django-exact-0.6.0/setup.cfg
+-rw-rw-r--   0 maldn     (1001) maldn     (1001)     1225 2023-07-27 09:06:58.000000 django-exact-0.6.0/setup.py
```

### Comparing `django-exact-0.5.1/LICENSE.txt` & `django-exact-0.6.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017 Malte Böhme, Affiliprint Deutschland GmbH
+Copyright (c) 2023 Malte Böhme, Affiliprint Deutschland GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `django-exact-0.5.1/README.md` & `django-exact-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-exact-0.5.1/django_exact.egg-info/SOURCES.txt` & `django-exact-0.6.0/django_exact.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-.editorconfig
-.gitignore
-CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-tox.ini
 django_exact.egg-info/PKG-INFO
 django_exact.egg-info/SOURCES.txt
 django_exact.egg-info/dependency_links.txt
 django_exact.egg-info/requires.txt
 django_exact.egg-info/top_level.txt
 exact/__init__.py
 exact/admin.py
@@ -18,9 +14,10 @@
 exact/app.py
 exact/models.py
 exact/signals.py
 exact/storage.py
 exact/urls.py
 exact/views.py
 exact/migrations/0001_initial.py
+exact/migrations/0002_remove_session_division.py
 exact/migrations/__init__.py
 exact/templates/exact/status.html
```

### Comparing `django-exact-0.5.1/exact/admin.py` & `django-exact-0.6.0/exact/admin.py`

 * *Files identical despite different names*

### Comparing `django-exact-0.5.1/exact/api.py` & `django-exact-0.6.0/exact/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 	@property
 	def limits_reached(self):
 		if self.limits and (self.limits["daily_remaining"] == 0 or self.limits["minutely_remaining"] == 0):
 			return True
 		return False
 
 
+class ExactAuthException(ExactException):
+	pass
+
+
 class DoesNotExist(Exception):
 	pass
 
 
 class MultipleObjectsReturned(Exception):
 	pass
 
@@ -144,16 +148,21 @@
 	DoesNotExist = DoesNotExist
 	MultipleObjectsReturned = MultipleObjectsReturned
 	# this is only for benchmarking
 	# exact needs ~5.5 seconds to open a https connection
 	# so reusing it speeds things up a lot. (~200ms per call)
 	_REUSE_SESSION = True
 
-	def __init__(self):
-		s, created = Session.objects.get_or_create(**EXACT_SETTINGS)
+	def __init__(self, division=None):
+		if division is None:
+			division = EXACT_SETTINGS["division"]
+		self.division = division
+
+		session_kwargs = {k: v for k, v in EXACT_SETTINGS.items() if k != "division"}
+		s, created = Session.objects.get_or_create(**session_kwargs)
 		self.session = s
 
 		retry_strategy = Retry(
 			total=5,
 			backoff_factor=10,
 			status_forcelist=[429],
 			method_whitelist=["GET", "POST", "PUT"]
@@ -193,15 +202,15 @@
 		# this is also the only request which is not "application/json"
 		prepped.headers["Content-Type"] = "application/x-www-form-urlencoded"
 
 		logger.debug("sending request: %s" % prepped.url)
 		response = self.requests_session.send(prepped)
 		if response.status_code != 200:
 			msg = "unexpected response while getting/refreshing token: %s" % response.text
-			raise ExactException(msg, response)
+			raise ExactAuthException(msg, response)
 		decoded = response.json()
 		self.session.access_token = decoded["access_token"]
 		self.session.refresh_token = decoded["refresh_token"]
 		# TODO: use access_expiry to avoid an unnecessary request if we know we will need to re-auth
 		self.session.access_expiry = int(time.time()) + int(decoded["expires_in"])
 		self.session.save()
 		# add new token to default headers
@@ -235,15 +244,15 @@
 			self.requests_session.headers.update({
 				"Accept": "application/json",
 				"Authorization": "Bearer %s" % self.session.access_token,
 				"Content-Type": "application/json",
 				"Prefer": "return=representation",
 			})
 
-		url = "%s/v1/%s/%s" % (self.session.api_url, self.session.division, resource)
+		url = "%s/v1/%s/%s" % (self.session.api_url, self.division, resource)
 		request = Request(method, url, data=data, params=params)
 		prepped = self.requests_session.prepare_request(request)
 
 		logger.debug("sending request: %s" % prepped.url)
 		response = self.requests_session.send(prepped)
 		if response.status_code == 401:
 			self.refresh_token()
```

### Comparing `django-exact-0.5.1/exact/migrations/0001_initial.py` & `django-exact-0.6.0/exact/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-exact-0.5.1/exact/models.py` & `django-exact-0.6.0/exact/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 class Session(models.Model):
 	api_url = models.URLField(_("API base URL"), help_text=_("E.g https://start.exactonline.nl/api"))
 	client_id = models.CharField(max_length=255, help_text=_("Your OAuth2/Exact App client ID"))
 	client_secret = models.CharField(max_length=255, help_text=_("Your OAuth2/Exact App client secret"))
 	redirect_uri = models.URLField(_("OAuth2 redirect URI"), help_text=_("Callback URL on your server. https://example.com/exact/authenticate"))
-	division = models.IntegerField()
 
 	access_expiry = models.IntegerField(blank=True, null=True)
 	access_token = models.TextField(blank=True, null=True)
 	refresh_token = models.TextField(blank=True, null=True)
 	authorization_code = models.TextField(blank=True, null=True)
```

### Comparing `django-exact-0.5.1/exact/signals.py` & `django-exact-0.6.0/exact/signals.py`

 * *Files identical despite different names*

### Comparing `django-exact-0.5.1/exact/storage.py` & `django-exact-0.6.0/exact/storage.py`

 * *Files identical despite different names*

### Comparing `django-exact-0.5.1/exact/templates/exact/status.html` & `django-exact-0.6.0/exact/templates/exact/status.html`

 * *Files 18% similar despite different names*

```diff
@@ -7,25 +7,15 @@
 <body>
 <div>API took {{ dt }}</div>
 <div>API user details:</div>
 <ul>
 	{% for k,v in api_user.items %}
 		{% if k == "__metadata" %}
 		{% elif k == "ThumbnailPicture" %}
-			<img src="data:image/jpg;base64, {{ v }}"/>
-		{% else %}
-			<li>{{ k }}: {{ v }}</li>
-		{% endif %}
-	{% endfor %}
-</ul>
-
-<div>Division:</div>
-<ul>
-	{% for k,v in division.items %}
-		{% if k == "__metadata" %}
+			{% if v %}<img src="data:image/jpg;base64, {{ v }}"/>{% endif %}
 		{% else %}
 			<li>{{ k }}: {{ v }}</li>
 		{% endif %}
 	{% endfor %}
 </ul>
 
 <div>Webhooks:</div>
```

#### html2text {}

```diff
@@ -1,15 +1,12 @@
 API took {{ dt }}
 API user details:
     * {% for k,v in api_user.items %} {% if k == "__metadata" %} {% elif k ==
-      "ThumbnailPicture" %} [data:image/jpg;base64, {{ v }}] {% else %}
-    * {{ k }}: {{ v }}
-    * {% endif %} {% endfor %}
-Division:
-    * {% for k,v in division.items %} {% if k == "__metadata" %} {% else %}
+      "ThumbnailPicture" %} {% if v %}[data:image/jpg;base64, {{ v }}]{% endif
+      %} {% else %}
     * {{ k }}: {{ v }}
     * {% endif %} {% endfor %}
 Webhooks:
 {% for webhook in webhooks %}
     * {% for k,v in webhook.items %}
     * {{ k }}: {{ v }}
     * {% endfor %}
```

### Comparing `django-exact-0.5.1/exact/views.py` & `django-exact-0.6.0/exact/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,19 +52,14 @@
 		start = datetime.now()
 		# eval generator to force a possible re-auth
 		ctx["webhooks"] = list(self.api.filter("webhooks/WebhookSubscriptions"))
 
 		response = self.api.raw("GET", "/v1/current/Me", params={"$select": "FullName,Email,ThumbnailPicture"})
 		ctx["api_user"] = response.json()["d"]["results"][0]
 
-		ctx["division"] = self.api.get(
-			"hrm/Divisions",
-			filter_string="Code eq %d" % self.api.session.division,
-			select="Code,CustomerName,Description,Country"
-		)
 		ctx["dt"] = datetime.now() - start
 		return ctx
 
 
 @csrf_exempt
 def webhook(request):
 	# TODO: show how to validate request
```

### Comparing `django-exact-0.5.1/setup.py` & `django-exact-0.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 setup(
 	name='django-exact',
 
 	# Versions should comply with PEP440.  For a discussion on single-sourcing
 	# the version across setup.py and the project code, see
 	# https://packaging.python.org/en/latest/single_source_version.html
-	version='0.5.1',
+	version='0.6.0',
 
 	description='API Wrapper and Django app for Exact Online',
 	# long_description='',
 
 	# The project's main homepage.
 	url='https://github.com/affiliprint/django-exact',
```

