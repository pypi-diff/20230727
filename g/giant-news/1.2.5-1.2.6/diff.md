# Comparing `tmp/giant_news-1.2.5.tar.gz` & `tmp/giant_news-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_news-1.2.5.tar", max compression
+gzip compressed data, was "giant_news-1.2.6.tar", max compression
```

## Comparing `giant_news-1.2.5.tar` & `giant_news-1.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1069 2022-04-25 13:43:34.356732 giant_news-1.2.5/LICENSE
--rw-r--r--   0        0        0     6113 2022-07-05 09:12:47.069243 giant_news-1.2.5/README.md
--rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/__init__.py
--rw-r--r--   0        0        0     2370 2023-02-16 15:33:36.055680 giant_news-1.2.5/giant_news/admin.py
--rw-r--r--   0        0        0      134 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/apps.py
--rw-r--r--   0        0        0      472 2023-07-26 12:43:20.643209 giant_news-1.2.5/giant_news/cms_apps.py
--rw-r--r--   0        0        0     1424 2023-02-16 15:33:26.271588 giant_news-1.2.5/giant_news/cms_plugins.py
--rw-r--r--   0        0        0     1537 2023-02-16 15:33:26.271588 giant_news-1.2.5/giant_news/forms.py
--rw-r--r--   0        0        0     4599 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/migrations/0001_initial.py
--rw-r--r--   0        0        0     2455 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py
--rw-r--r--   0        0        0      674 2022-07-05 07:36:44.035564 giant_news-1.2.5/giant_news/migrations/0003_alter_article_content.py
--rw-r--r--   0        0        0      789 2022-07-05 07:36:44.035564 giant_news-1.2.5/giant_news/migrations/0004_auto_20220601_0915.py
--rw-r--r--   0        0        0      772 2023-02-16 15:33:36.055680 giant_news-1.2.5/giant_news/migrations/0005_auto_20220912_0459.py
--rw-r--r--   0        0        0     3280 2023-07-26 12:43:20.643209 giant_news-1.2.5/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py
--rw-r--r--   0        0        0      618 2023-07-26 12:43:20.643209 giant_news-1.2.5/giant_news/migrations/0007_relatedarticleplugin_title.py
--rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/migrations/__init__.py
--rw-r--r--   0        0        0       60 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/models/__init__.py
--rw-r--r--   0        0        0     4580 2023-07-27 14:15:25.797223 giant_news-1.2.5/giant_news/models/article.py
--rw-r--r--   0        0        0     3154 2023-07-26 12:43:20.643209 giant_news-1.2.5/giant_news/models/plugin.py
--rw-r--r--   0        0        0      377 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/sitemaps.py
--rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/templates/base.html
--rw-r--r--   0        0        0      621 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/templates/news/detail.html
--rw-r--r--   0        0        0     2184 2022-07-05 07:36:44.035564 giant_news-1.2.5/giant_news/templates/news/index.html
--rw-r--r--   0        0        0     1421 2023-07-26 12:43:20.643209 giant_news-1.2.5/giant_news/templates/plugins/related_articles/container.html
--rw-r--r--   0        0        0      663 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/templates/plugins/related_articles/item.html
--rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/tests/__init__.py
--rw-r--r--   0        0        0      272 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/tests/test_cms_apps.py
--rw-r--r--   0        0        0     2157 2023-02-16 15:33:26.271588 giant_news-1.2.5/giant_news/tests/test_forms.py
--rw-r--r--   0        0        0     1382 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/tests/test_models.py
--rw-r--r--   0        0        0     2245 2023-02-16 15:33:26.271588 giant_news-1.2.5/giant_news/tests/test_views.py
--rw-r--r--   0        0        0      150 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/tests/urls.py
--rw-r--r--   0        0        0      239 2022-04-25 13:43:34.356732 giant_news-1.2.5/giant_news/urls.py
--rw-r--r--   0        0        0     1423 2023-02-16 15:33:26.271588 giant_news-1.2.5/giant_news/views.py
--rw-r--r--   0        0        0     1426 2023-07-27 14:15:25.797223 giant_news-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 giant_news-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-04-25 13:43:34.356732 giant_news-1.2.6/LICENSE
+-rw-r--r--   0        0        0     6113 2022-07-05 09:12:47.069243 giant_news-1.2.6/README.md
+-rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/__init__.py
+-rw-r--r--   0        0        0     2370 2023-02-16 15:33:36.055680 giant_news-1.2.6/giant_news/admin.py
+-rw-r--r--   0        0        0      134 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/apps.py
+-rw-r--r--   0        0        0      472 2023-07-26 12:43:20.643209 giant_news-1.2.6/giant_news/cms_apps.py
+-rw-r--r--   0        0        0     1424 2023-02-16 15:33:26.271588 giant_news-1.2.6/giant_news/cms_plugins.py
+-rw-r--r--   0        0        0     1537 2023-02-16 15:33:26.271588 giant_news-1.2.6/giant_news/forms.py
+-rw-r--r--   0        0        0     4599 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2455 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py
+-rw-r--r--   0        0        0      674 2022-07-05 07:36:44.035564 giant_news-1.2.6/giant_news/migrations/0003_alter_article_content.py
+-rw-r--r--   0        0        0      789 2022-07-05 07:36:44.035564 giant_news-1.2.6/giant_news/migrations/0004_auto_20220601_0915.py
+-rw-r--r--   0        0        0      772 2023-02-16 15:33:36.055680 giant_news-1.2.6/giant_news/migrations/0005_auto_20220912_0459.py
+-rw-r--r--   0        0        0     3280 2023-07-26 12:43:20.643209 giant_news-1.2.6/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py
+-rw-r--r--   0        0        0      618 2023-07-26 12:43:20.643209 giant_news-1.2.6/giant_news/migrations/0007_relatedarticleplugin_title.py
+-rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/models/__init__.py
+-rw-r--r--   0        0        0     4586 2023-07-27 14:42:17.542098 giant_news-1.2.6/giant_news/models/article.py
+-rw-r--r--   0        0        0     3154 2023-07-26 12:43:20.643209 giant_news-1.2.6/giant_news/models/plugin.py
+-rw-r--r--   0        0        0      377 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/sitemaps.py
+-rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/templates/base.html
+-rw-r--r--   0        0        0      621 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/templates/news/detail.html
+-rw-r--r--   0        0        0     2184 2022-07-05 07:36:44.035564 giant_news-1.2.6/giant_news/templates/news/index.html
+-rw-r--r--   0        0        0     1421 2023-07-26 12:43:20.643209 giant_news-1.2.6/giant_news/templates/plugins/related_articles/container.html
+-rw-r--r--   0        0        0      663 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/templates/plugins/related_articles/item.html
+-rw-r--r--   0        0        0        0 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/tests/__init__.py
+-rw-r--r--   0        0        0      272 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/tests/test_cms_apps.py
+-rw-r--r--   0        0        0     2157 2023-02-16 15:33:26.271588 giant_news-1.2.6/giant_news/tests/test_forms.py
+-rw-r--r--   0        0        0     1382 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/tests/test_models.py
+-rw-r--r--   0        0        0     2245 2023-02-16 15:33:26.271588 giant_news-1.2.6/giant_news/tests/test_views.py
+-rw-r--r--   0        0        0      150 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/tests/urls.py
+-rw-r--r--   0        0        0      239 2022-04-25 13:43:34.356732 giant_news-1.2.6/giant_news/urls.py
+-rw-r--r--   0        0        0     1423 2023-02-16 15:33:26.271588 giant_news-1.2.6/giant_news/views.py
+-rw-r--r--   0        0        0     1426 2023-07-27 14:44:57.030200 giant_news-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 giant_news-1.2.6/PKG-INFO
```

### Comparing `giant_news-1.2.5/LICENSE` & `giant_news-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/README.md` & `giant_news-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/admin.py` & `giant_news-1.2.6/giant_news/admin.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/cms_plugins.py` & `giant_news-1.2.6/giant_news/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/forms.py` & `giant_news-1.2.6/giant_news/forms.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0001_initial.py` & `giant_news-1.2.6/giant_news/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py` & `giant_news-1.2.6/giant_news/migrations/0002_relatedarticlecardplugin_relatedarticleplugin.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0003_alter_article_content.py` & `giant_news-1.2.6/giant_news/migrations/0003_alter_article_content.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0004_auto_20220601_0915.py` & `giant_news-1.2.6/giant_news/migrations/0004_auto_20220601_0915.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0005_auto_20220912_0459.py` & `giant_news-1.2.6/giant_news/migrations/0005_auto_20220912_0459.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py` & `giant_news-1.2.6/giant_news/migrations/0006_alter_article_author_alter_article_category_and_more.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/migrations/0007_relatedarticleplugin_title.py` & `giant_news-1.2.6/giant_news/migrations/0007_relatedarticleplugin_title.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/models/article.py` & `giant_news-1.2.6/giant_news/models/article.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return f"{self.title} article by {self.author}"
 
     def save(self, *args, **kwargs):
         """
         Override save method so we can store the plugin text
         """
         if self.content:
-            self.plugin_text = self.plain_text
+            self.plugin_text = self.rich_plugin_text
         super().save(*args, **kwargs)
 
     def get_absolute_url(self):
         """
         Builds the url for the article object
         """
         return reverse("news:detail", kwargs={"slug": self.slug})
```

### Comparing `giant_news-1.2.5/giant_news/models/plugin.py` & `giant_news-1.2.6/giant_news/models/plugin.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/templates/news/detail.html` & `giant_news-1.2.6/giant_news/templates/news/detail.html`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/templates/news/index.html` & `giant_news-1.2.6/giant_news/templates/news/index.html`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/templates/plugins/related_articles/container.html` & `giant_news-1.2.6/giant_news/templates/plugins/related_articles/container.html`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/templates/plugins/related_articles/item.html` & `giant_news-1.2.6/giant_news/templates/plugins/related_articles/item.html`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/tests/test_forms.py` & `giant_news-1.2.6/giant_news/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/tests/test_models.py` & `giant_news-1.2.6/giant_news/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/tests/test_views.py` & `giant_news-1.2.6/giant_news/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/giant_news/views.py` & `giant_news-1.2.6/giant_news/views.py`

 * *Files identical despite different names*

### Comparing `giant_news-1.2.5/pyproject.toml` & `giant_news-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-news"
-version = "1.2.5"
+version = "1.2.6"
 description = "A small reusable package that adds a News app to a project"
 authors = ["Will-Hoey <will.hoey@giantdigital.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-news"
 repository = "https://github.com/giantmade/giant-news"
 keywords = ["giant_news", "app"]
```

### Comparing `giant_news-1.2.5/PKG-INFO` & `giant_news-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-news
-Version: 1.2.5
+Version: 1.2.6
 Summary: A small reusable package that adds a News app to a project
 Home-page: https://github.com/giantmade/giant-news
 License: MIT
 Keywords: giant_news,app
 Author: Will-Hoey
 Author-email: will.hoey@giantdigital.co.uk
 Requires-Python: >=3.9,<4.0
```

