# Comparing `tmp/wagtail-webstories-0.0.4.tar.gz` & `tmp/wagtail-webstories-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-webstories-0.0.4.tar", last modified: Thu May 27 10:59:41 2021, max compression
+gzip compressed data, was "wagtail-webstories-0.1.tar", last modified: Thu Jul 27 16:08:07 2023, max compression
```

## Comparing `wagtail-webstories-0.0.4.tar` & `wagtail-webstories-0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/
--rw-r--r--   0 matthew    (501) staff       (20)    11931 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/PKG-INFO
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)    11931 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     1114 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)      140 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       19 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/top_level.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)     1476 2020-11-10 16:43:11.000000 wagtail-webstories-0.0.4/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      508 2021-05-27 10:32:07.000000 wagtail-webstories-0.0.4/CHANGELOG.md
--rw-r--r--   0 matthew    (501) staff       (20)      146 2021-05-27 10:37:29.000000 wagtail-webstories-0.0.4/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     9278 2021-03-11 18:45:58.000000 wagtail-webstories-0.0.4/README.md
--rw-r--r--   0 matthew    (501) staff       (20)     1295 2021-05-27 10:59:37.000000 wagtail-webstories-0.0.4/setup.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/migrations/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2021-03-11 18:42:26.000000 wagtail-webstories-0.0.4/wagtail_webstories/migrations/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      440 2021-05-27 10:23:16.000000 wagtail-webstories-0.0.4/wagtail_webstories/migrations/0002_extend_url_hash.py
--rw-r--r--   0 matthew    (501) staff       (20)     1291 2021-03-11 18:42:26.000000 wagtail-webstories-0.0.4/wagtail_webstories/migrations/0001_initial.py
--rw-r--r--   0 matthew    (501) staff       (20)    19149 2021-05-27 10:17:11.000000 wagtail-webstories-0.0.4/wagtail_webstories/models.py
--rw-r--r--   0 matthew    (501) staff       (20)        0 2020-11-10 16:45:31.000000 wagtail-webstories-0.0.4/wagtail_webstories/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     1884 2020-12-07 21:05:43.000000 wagtail-webstories-0.0.4/wagtail_webstories/markup.py
--rw-r--r--   0 matthew    (501) staff       (20)      969 2020-11-19 16:23:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/forms.py
--rw-r--r--   0 matthew    (501) staff       (20)      645 2020-11-12 12:39:45.000000 wagtail-webstories-0.0.4/wagtail_webstories/wagtail_hooks.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/blocks/
--rw-r--r--   0 matthew    (501) staff       (20)      255 2021-03-11 18:42:26.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/blocks/external_story_embed_block.html
--rw-r--r--   0 matthew    (501) staff       (20)      412 2021-03-11 18:42:26.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/blocks/external_story_poster_link.html
--rw-r--r--   0 matthew    (501) staff       (20)      256 2020-11-18 18:13:49.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/blocks/story_embed_block.html
--rw-r--r--   0 matthew    (501) staff       (20)      411 2020-11-18 20:34:12.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/blocks/story_poster_link.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/admin/
--rw-r--r--   0 matthew    (501) staff       (20)     1178 2020-11-12 11:39:35.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/admin/import.html
--rw-r--r--   0 matthew    (501) staff       (20)     2341 2020-11-12 13:05:42.000000 wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/base_web_story_page.html
--rw-r--r--   0 matthew    (501) staff       (20)     4545 2021-03-11 18:42:26.000000 wagtail-webstories-0.0.4/wagtail_webstories/blocks.py
--rw-r--r--   0 matthew    (501) staff       (20)     3516 2021-03-02 18:08:19.000000 wagtail-webstories-0.0.4/wagtail_webstories/views.py
--rw-r--r--   0 matthew    (501) staff       (20)      170 2020-11-12 11:17:51.000000 wagtail-webstories-0.0.4/wagtail_webstories/admin_urls.py
--rw-r--r--   0 matthew    (501) staff       (20)       38 2021-05-27 10:59:41.000000 wagtail-webstories-0.0.4/setup.cfg
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.966258 wagtail-webstories-0.1/
+-rw-r--r--   0 matthew    (501) staff       (20)      674 2023-07-27 15:59:14.000000 wagtail-webstories-0.1/CHANGELOG.md
+-rw-r--r--   0 matthew    (501) staff       (20)     1476 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      146 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)    10161 2023-07-27 16:08:07.965725 wagtail-webstories-0.1/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     9286 2023-07-27 15:57:24.000000 wagtail-webstories-0.1/README.md
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2023-07-27 16:08:07.966354 wagtail-webstories-0.1/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1489 2023-07-27 15:59:30.000000 wagtail-webstories-0.1/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.954787 wagtail-webstories-0.1/wagtail_webstories/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      170 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/admin_urls.py
+-rw-r--r--   0 matthew    (501) staff       (20)      240 2023-07-27 15:21:52.000000 wagtail-webstories-0.1/wagtail_webstories/apps.py
+-rw-r--r--   0 matthew    (501) staff       (20)     4606 2023-07-27 16:07:14.000000 wagtail-webstories-0.1/wagtail_webstories/blocks.py
+-rw-r--r--   0 matthew    (501) staff       (20)      966 2023-07-27 15:21:52.000000 wagtail-webstories-0.1/wagtail_webstories/forms.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1884 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/markup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.960264 wagtail-webstories-0.1/wagtail_webstories/migrations/
+-rw-r--r--   0 matthew    (501) staff       (20)     1291 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/migrations/0001_initial.py
+-rw-r--r--   0 matthew    (501) staff       (20)      440 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/migrations/0002_extend_url_hash.py
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/migrations/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)    19067 2023-07-27 15:21:52.000000 wagtail-webstories-0.1/wagtail_webstories/models.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.944063 wagtail-webstories-0.1/wagtail_webstories/templates/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.960569 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.961068 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/admin/
+-rw-r--r--   0 matthew    (501) staff       (20)     1178 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/admin/import.html
+-rw-r--r--   0 matthew    (501) staff       (20)     2341 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/base_web_story_page.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.964794 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/blocks/
+-rw-r--r--   0 matthew    (501) staff       (20)      255 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/blocks/external_story_embed_block.html
+-rw-r--r--   0 matthew    (501) staff       (20)      412 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/blocks/external_story_poster_link.html
+-rw-r--r--   0 matthew    (501) staff       (20)      256 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/blocks/story_embed_block.html
+-rw-r--r--   0 matthew    (501) staff       (20)      411 2023-07-27 15:09:18.000000 wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/blocks/story_poster_link.html
+-rw-r--r--   0 matthew    (501) staff       (20)     3518 2023-07-27 15:21:52.000000 wagtail-webstories-0.1/wagtail_webstories/views.py
+-rw-r--r--   0 matthew    (501) staff       (20)      641 2023-07-27 15:21:52.000000 wagtail-webstories-0.1/wagtail_webstories/wagtail_hooks.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-27 16:08:07.958343 wagtail-webstories-0.1/wagtail_webstories.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)    10161 2023-07-27 16:08:07.000000 wagtail-webstories-0.1/wagtail_webstories.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     1141 2023-07-27 16:08:07.000000 wagtail-webstories-0.1/wagtail_webstories.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-07-27 16:08:07.000000 wagtail-webstories-0.1/wagtail_webstories.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      153 2023-07-27 16:08:07.000000 wagtail-webstories-0.1/wagtail_webstories.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       19 2023-07-27 16:08:07.000000 wagtail-webstories-0.1/wagtail_webstories.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtail-webstories-0.0.4/PKG-INFO` & `wagtail-webstories-0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,264 +1,269 @@
 Metadata-Version: 2.1
 Name: wagtail-webstories
-Version: 0.0.4
+Version: 0.1
 Summary: AMP web story support for Wagtail
 Home-page: https://github.com/torchbox/wagtail-webstories/
 Author: Matt Westcott
 Author-email: matthew@torchbox.com
 License: BSD
-Description: # wagtail-webstories
-        
-        This package adds support for [AMP web stories](https://amp.dev/about/stories/) to Wagtail. Stories created elsewhere can be linked or embedded from their original URL locations, or imported as Wagtail pages, including optionally importing images and videos into the Wagtail media library.
-        
-        `wagtail-webstories` is compatible with Wagtail 2.5 and above.
-        
-        ## Installation
-        
-        Install with pip:
-        
-        ```bash
-        pip install wagtail-webstories
-        ```
-        
-        Add to INSTALLED_APPS:
-        
-        ```python
-        INSTALLED_APPS = [
-            # ...
-            'wagtail_webstories',
-            # ...
-        ]
-        ```
-        
-        Run migrations:
-        
-        ```bash
-        ./manage.py migrate
-        ```
-        
-        ## Embedding and linking external stories
-        
-        To embed a web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.ExternalStoryEmbedBlock` block type in your StreamField definition:
-        
-        ```python
-        from wagtail_webstories.blocks import StoryEmbedBlock
-        
-        class BlogPage(Page):
-            body = StreamField([
-                ('heading', blocks.CharBlock()),
-                ('paragraph', blocks.RichTextBlock()),
-                ('story_embed', ExternalStoryEmbedBlock()),
-            ])
-        ```
-        
-        This block allows the page author to provide the URL to an AMP web story, which will render on the front-end template (when using `{% include_block %}`) as an `<amp-story-player>` element; your template should include [the necessary scripts for rendering this](https://amp.dev/documentation/guides-and-tutorials/integrate/embed-stories/?format=stories#embed-amp-story-player), along with a CSS rule to specify appropriate dimensions:
-        
-        ```html
-            <script async src="https://cdn.ampproject.org/amp-story-player-v0.js"></script>
-            <link href="https://cdn.ampproject.org/amp-story-player-v0.css" rel="stylesheet" type="text/css">
-            <style>
-                amp-story-player { width: 360px; height: 600px; }
-            </style>
-        ```
-        
-        To include a link to a story rather than embedding it, `wagtail_webstories.blocks.ExternalStoryBlock` can be used in place of `ExternalStoryEmbedBlock`. The default template `wagtail_webstories/blocks/external_story_poster_link.html` outputs a 'card' rendering of the story using the story's poster image, to be used with the following CSS:
-        
-        ```css
-            .webstory-poster {
-                display: block; width: 300px; height: 400px; border-radius: 15px; background-size: cover; position: relative;
-            }
-            .webstory-poster .webstory-info {
-                position: absolute; bottom: 0; width: 100%; background-color: #ccc; color: black; border-bottom-left-radius: 15px; border-bottom-right-radius: 15px;
-            }
-            .webstory-poster .title {
-                font-size: 1.5em; padding: 10px;
-            }
-            .webstory-poster .publisher {
-                padding: 0 10px 20px 10px;
-            }
-            .webstory-poster .publisher img {
-                vertical-align: middle;
-            }
-        ```
-        
-        ## Embedding and linking external stories without StreamField
-        
-        External stories are handled through the model `wagtail_webstories.models.ExternalStory`. To obtain an ExternalStory instance for a given URL, use: `ExternalStory.get_for_url(story_url)`. The story's metadata is cached within the ExternalStory model to avoid having to re-fetch the story on every request - the available metadata fields are `url`, `title`, `publisher`, `publisher_logo_src`, `poster_portrait_src`, `poster_square_src` and `poster_landscape_src`.
-        
-        The StreamField block templates `wagtail_webstories/blocks/external_story_embed_block.html` and `wagtail_webstories/blocks/external_story_poster_link.html` can be used to render an ExternalStory object, by passing it as the variable `story`:
-        
-        ```python
-        # models.py
-        class BlogPostWithStoryPage(Page):
-            story_url = model.URLField(max_length=2048)
-        
-            def get_context(self, request):
-                context = super().get_context(request)
-                context['story_obj'] = ExternalStory.get_for_url(self.story_url)
-                return context
-        ```
-        
-        ```html+django
-        {# blog_post_with_story_page.html #}
-        
-        {% include "wagtail_webstories/blocks/external_story_embed_block.html" with story=story_obj %}
-        ```
-        
-        
-        ## Importing
-        
-        To allow stories to be imported as Wagtail pages, define a model that extends `wagtail_webstories.models.BaseWebStoryPage`:
-        
-        ```python
-        from wagtail_webstories.models import BaseWebStoryPage
-        
-        class StoryPage(BaseWebStoryPage):
-            pass
-        ```
-        
-        Alternatively, if your project has an existing base page class that all page types must inherit from (which would prevent the use of BaseWebStoryPage in addition to that base class), extend `wagtail_webstories.models.WebStoryPageMixin` and define `content_panels` and `promote_panels` to incorporate its panel definitions:
-        
-        ```python
-        from wagtail_webstories.models import WebStoryPageMixin
-        
-        class StoryPage(WebStoryPageMixin, BasePage):
-            content_panels = BasePage.content_panels + WebStoryPageMixin.web_story_content_panels
-            promote_panels = BasePage.promote_panels + WebStoryPageMixin.web_story_promote_panels
-        ```
-        
-        Now create a corresponding template that extends `wagtail_webstories/base_web_story_page.html`:
-        
-        ```html+django
-        {% extends "wagtail_webstories/base_web_story_page.html" %}
-        ```
-        
-        Define a setting `WAGTAIL_WEBSTORIES_IMPORT_MODEL` pointing to the page model to use:
-        
-        ```python
-        WAGTAIL_WEBSTORIES_IMPORT_MODEL = 'myapp.StoryPage'
-        ```
-        
-        This will now add a "Web stories" item to the Wagtail admin menu, allowing you to import stories by URL.
-        
-        
-        ## HTML cleaning
-        
-        By default, all HTML elements and attributes not permitted by the AMP web story specification will be stripped out on importing and saving. To disable this, set `WAGTAIL_WEBSTORIES_CLEAN_HTML` to False:
-        
-        ```python
-        WAGTAIL_WEBSTORIES_CLEAN_HTML = False
-        ```
-        
-        
-        ## Image importing
-        
-        By default, image references within imported stories are left at their original URLs. BaseWebStoryPage provides a method `import_images()` to fetch all referenced images and import them into the Wagtail image library, de-duplicating if they already exist. It is recommended that you call this from a `post_save` signal handler:
-        
-        ```python
-        # myapp/signals.py
-        
-        from django.db.models.signals import post_save
-        from django.dispatch import receiver
-        
-        from .models import StoryPage
-        
-        
-        @receiver(post_save, sender=StoryPage)
-        def import_story_images(sender, instance, **kwargs):
-            changed = instance.import_images()
-            if changed:
-                instance.save()
-        
-        
-        # myapp/apps.py
-        
-        from django.apps import AppConfig
-        
-        
-        class MyappConfig(AppConfig):
-            name = 'myapp'
-        
-            def ready(self):
-                import myapp.signals  # noqa
-        
-        
-        # myapp/__init__.py
-        
-        default_app_config = 'myapp.apps.MyappConfig'
-        ```
-        
-        Since importing images can be a time-consuming process, you may wish to offload the call to `import_images` to a background task using Celery or similar, to avoid this blocking a web server thread.
-        
-        To customise the creation of new images (e.g. to assign imported images to a particular collection, or to populate additional metadata fields on a custom image model), override the story page model's `_create_image` method:
-        
-        ```python
-        class StoryPage(BaseWebStoryPage):
-        
-            def _create_image(self, file, title=None):
-                image = super()._create_image(file, title=title)
-                image.copyright = "All rights reserved"
-                return image
-        ```
-        
-        ## Video importing
-        
-        If you have [wagtailmedia](https://pypi.org/project/wagtailmedia/) installed, you can similarly import videos into the local media library by calling `import_videos()`. The signal handler above then becomes:
-        
-        ```python
-        # myapp/signals.py
-        
-        @receiver(post_save, sender=StoryPage)
-        def import_story_images(sender, instance, **kwargs):
-            images_changed = instance.import_images()
-            videos_changed = instance.import_videos()
-            if images_changed or videos_changed:
-                instance.save()
-        ```
-        
-        ## Linking and embedding imported stories
-        
-        To embed or link an imported web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.StoryEmbedBlock` or `wagtail_webstories.blocks.StoryChooserBlock` block type in your StreamField definition. These work similarly to ExternalStoryEmbedBlock and ExternalStoryBlock, but provide the page author with a page chooser interface rather than a URL field.
-        
-        ```python
-        from wagtail_webstories.blocks import StoryEmbedBlock
-        
-        class BlogPage(Page):
-            body = StreamField([
-                ('heading', blocks.CharBlock()),
-                ('paragraph', blocks.RichTextBlock()),
-                ('local_story_embed', StoryEmbedBlock(target_model=StoryPage)),
-            ])
-        ```
-        
-        The `target_model` argument is optional - by default, any page type inheriting from BaseWebStoryPage can be chosen. As with ExternalStoryEmbedBlock and ExternalStoryBlock, your page template must contain the appropriate JavaScript or CSS include for rendering the block.
-        
-        The templates `wagtail_webstories/blocks/story_poster_link.html` and `wagtail_webstories/blocks/story_embed_block.html` expect a single variable `page` containing the story page instance, so these can also be used outside of StreamField:
-        
-        ```python
-        # models.py
-        class StoryIndexPage(Page):
-            def get_context(self, request):
-                context = super().get_context(request)
-                context['stories'] = StoryPage.objects.child_of(self).live().order_by('-first_published_at')
-                return context
-        ```
-        
-        ```html+django
-        {# story_index_page.html #}
-        {% for story in stories %}
-            {% include "wagtail_webstories/blocks/story_poster_link.html" with page=story %}
-        {% endfor %}
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# wagtail-webstories
+
+This package adds support for [AMP web stories](https://amp.dev/about/stories/) to Wagtail. Stories created elsewhere can be linked or embedded from their original URL locations, or imported as Wagtail pages, including optionally importing images and videos into the Wagtail media library.
+
+`wagtail-webstories` is compatible with Wagtail 4.1 and above.
+
+## Installation
+
+Install with pip:
+
+```bash
+pip install wagtail-webstories
+```
+
+Add to INSTALLED_APPS:
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'wagtail_webstories',
+    # ...
+]
+```
+
+Run migrations:
+
+```bash
+./manage.py migrate
+```
+
+## Embedding and linking external stories
+
+To embed a web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.ExternalStoryEmbedBlock` block type in your StreamField definition:
+
+```python
+from wagtail_webstories.blocks import ExternalStoryEmbedBlock
+
+class BlogPage(Page):
+    body = StreamField([
+        ('heading', blocks.CharBlock()),
+        ('paragraph', blocks.RichTextBlock()),
+        ('story_embed', ExternalStoryEmbedBlock()),
+    ])
+```
+
+This block allows the page author to provide the URL to an AMP web story, which will render on the front-end template (when using `{% include_block %}`) as an `<amp-story-player>` element; your template should include [the necessary scripts for rendering this](https://amp.dev/documentation/guides-and-tutorials/integrate/embed-stories/?format=stories#embed-amp-story-player), along with a CSS rule to specify appropriate dimensions:
+
+```html
+    <script async src="https://cdn.ampproject.org/amp-story-player-v0.js"></script>
+    <link href="https://cdn.ampproject.org/amp-story-player-v0.css" rel="stylesheet" type="text/css">
+    <style>
+        amp-story-player { width: 360px; height: 600px; }
+    </style>
+```
+
+To include a link to a story rather than embedding it, `wagtail_webstories.blocks.ExternalStoryBlock` can be used in place of `ExternalStoryEmbedBlock`. The default template `wagtail_webstories/blocks/external_story_poster_link.html` outputs a 'card' rendering of the story using the story's poster image, to be used with the following CSS:
+
+```css
+    .webstory-poster {
+        display: block; width: 300px; height: 400px; border-radius: 15px; background-size: cover; position: relative;
+    }
+    .webstory-poster .webstory-info {
+        position: absolute; bottom: 0; width: 100%; background-color: #ccc; color: black; border-bottom-left-radius: 15px; border-bottom-right-radius: 15px;
+    }
+    .webstory-poster .title {
+        font-size: 1.5em; padding: 10px;
+    }
+    .webstory-poster .publisher {
+        padding: 0 10px 20px 10px;
+    }
+    .webstory-poster .publisher img {
+        vertical-align: middle;
+    }
+```
+
+## Embedding and linking external stories without StreamField
+
+External stories are handled through the model `wagtail_webstories.models.ExternalStory`. To obtain an ExternalStory instance for a given URL, use: `ExternalStory.get_for_url(story_url)`. The story's metadata is cached within the ExternalStory model to avoid having to re-fetch the story on every request - the available metadata fields are `url`, `title`, `publisher`, `publisher_logo_src`, `poster_portrait_src`, `poster_square_src` and `poster_landscape_src`.
+
+The StreamField block templates `wagtail_webstories/blocks/external_story_embed_block.html` and `wagtail_webstories/blocks/external_story_poster_link.html` can be used to render an ExternalStory object, by passing it as the variable `story`:
+
+```python
+# models.py
+class BlogPostWithStoryPage(Page):
+    story_url = model.URLField(max_length=2048)
+
+    def get_context(self, request):
+        context = super().get_context(request)
+        context['story_obj'] = ExternalStory.get_for_url(self.story_url)
+        return context
+```
+
+```html+django
+{# blog_post_with_story_page.html #}
+
+{% include "wagtail_webstories/blocks/external_story_embed_block.html" with story=story_obj %}
+```
+
+
+## Importing
+
+To allow stories to be imported as Wagtail pages, define a model that extends `wagtail_webstories.models.BaseWebStoryPage`:
+
+```python
+from wagtail_webstories.models import BaseWebStoryPage
+
+class StoryPage(BaseWebStoryPage):
+    pass
+```
+
+Alternatively, if your project has an existing base page class that all page types must inherit from (which would prevent the use of BaseWebStoryPage in addition to that base class), extend `wagtail_webstories.models.WebStoryPageMixin` and define `content_panels` and `promote_panels` to incorporate its panel definitions:
+
+```python
+from wagtail_webstories.models import WebStoryPageMixin
+
+class StoryPage(WebStoryPageMixin, BasePage):
+    content_panels = BasePage.content_panels + WebStoryPageMixin.web_story_content_panels
+    promote_panels = BasePage.promote_panels + WebStoryPageMixin.web_story_promote_panels
+```
+
+Now create a corresponding template that extends `wagtail_webstories/base_web_story_page.html`:
+
+```html+django
+{% extends "wagtail_webstories/base_web_story_page.html" %}
+```
+
+Define a setting `WAGTAIL_WEBSTORIES_IMPORT_MODEL` pointing to the page model to use:
+
+```python
+WAGTAIL_WEBSTORIES_IMPORT_MODEL = 'myapp.StoryPage'
+```
+
+This will now add a "Web stories" item to the Wagtail admin menu, allowing you to import stories by URL.
+
+
+## HTML cleaning
+
+By default, all HTML elements and attributes not permitted by the AMP web story specification will be stripped out on importing and saving. To disable this, set `WAGTAIL_WEBSTORIES_CLEAN_HTML` to False:
+
+```python
+WAGTAIL_WEBSTORIES_CLEAN_HTML = False
+```
+
+
+## Image importing
+
+By default, image references within imported stories are left at their original URLs. BaseWebStoryPage provides a method `import_images()` to fetch all referenced images and import them into the Wagtail image library, de-duplicating if they already exist. It is recommended that you call this from a `post_save` signal handler:
+
+```python
+# myapp/signals.py
+
+from django.db.models.signals import post_save
+from django.dispatch import receiver
+
+from .models import StoryPage
+
+
+@receiver(post_save, sender=StoryPage)
+def import_story_images(sender, instance, **kwargs):
+    changed = instance.import_images()
+    if changed:
+        instance.save()
+
+
+# myapp/apps.py
+
+from django.apps import AppConfig
+
+
+class MyappConfig(AppConfig):
+    name = 'myapp'
+
+    def ready(self):
+        import myapp.signals  # noqa
+
+
+# myapp/__init__.py
+
+default_app_config = 'myapp.apps.MyappConfig'
+```
+
+Since importing images can be a time-consuming process, you may wish to offload the call to `import_images` to a background task using Celery or similar, to avoid this blocking a web server thread.
+
+To customise the creation of new images (e.g. to assign imported images to a particular collection, or to populate additional metadata fields on a custom image model), override the story page model's `_create_image` method:
+
+```python
+class StoryPage(BaseWebStoryPage):
+
+    def _create_image(self, file, title=None):
+        image = super()._create_image(file, title=title)
+        image.copyright = "All rights reserved"
+        return image
+```
+
+## Video importing
+
+If you have [wagtailmedia](https://pypi.org/project/wagtailmedia/) installed, you can similarly import videos into the local media library by calling `import_videos()`. The signal handler above then becomes:
+
+```python
+# myapp/signals.py
+
+@receiver(post_save, sender=StoryPage)
+def import_story_images(sender, instance, **kwargs):
+    images_changed = instance.import_images()
+    videos_changed = instance.import_videos()
+    if images_changed or videos_changed:
+        instance.save()
+```
+
+## Linking and embedding imported stories
+
+To embed or link an imported web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.StoryEmbedBlock` or `wagtail_webstories.blocks.StoryChooserBlock` block type in your StreamField definition. These work similarly to ExternalStoryEmbedBlock and ExternalStoryBlock, but provide the page author with a page chooser interface rather than a URL field.
+
+```python
+from wagtail_webstories.blocks import StoryEmbedBlock
+
+class BlogPage(Page):
+    body = StreamField([
+        ('heading', blocks.CharBlock()),
+        ('paragraph', blocks.RichTextBlock()),
+        ('local_story_embed', StoryEmbedBlock(target_model=StoryPage)),
+    ])
+```
+
+The `target_model` argument is optional - by default, any page type inheriting from BaseWebStoryPage can be chosen. As with ExternalStoryEmbedBlock and ExternalStoryBlock, your page template must contain the appropriate JavaScript or CSS include for rendering the block.
+
+The templates `wagtail_webstories/blocks/story_poster_link.html` and `wagtail_webstories/blocks/story_embed_block.html` expect a single variable `page` containing the story page instance, so these can also be used outside of StreamField:
+
+```python
+# models.py
+class StoryIndexPage(Page):
+    def get_context(self, request):
+        context = super().get_context(request)
+        context['stories'] = StoryPage.objects.child_of(self).live().order_by('-first_published_at')
+        return context
+```
+
+```html+django
+{# story_index_page.html #}
+{% for story in stories %}
+    {% include "wagtail_webstories/blocks/story_poster_link.html" with page=story %}
+{% endfor %}
+```
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories.egg-info/PKG-INFO` & `wagtail-webstories-0.1/wagtail_webstories.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,264 +1,269 @@
 Metadata-Version: 2.1
 Name: wagtail-webstories
-Version: 0.0.4
+Version: 0.1
 Summary: AMP web story support for Wagtail
 Home-page: https://github.com/torchbox/wagtail-webstories/
 Author: Matt Westcott
 Author-email: matthew@torchbox.com
 License: BSD
-Description: # wagtail-webstories
-        
-        This package adds support for [AMP web stories](https://amp.dev/about/stories/) to Wagtail. Stories created elsewhere can be linked or embedded from their original URL locations, or imported as Wagtail pages, including optionally importing images and videos into the Wagtail media library.
-        
-        `wagtail-webstories` is compatible with Wagtail 2.5 and above.
-        
-        ## Installation
-        
-        Install with pip:
-        
-        ```bash
-        pip install wagtail-webstories
-        ```
-        
-        Add to INSTALLED_APPS:
-        
-        ```python
-        INSTALLED_APPS = [
-            # ...
-            'wagtail_webstories',
-            # ...
-        ]
-        ```
-        
-        Run migrations:
-        
-        ```bash
-        ./manage.py migrate
-        ```
-        
-        ## Embedding and linking external stories
-        
-        To embed a web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.ExternalStoryEmbedBlock` block type in your StreamField definition:
-        
-        ```python
-        from wagtail_webstories.blocks import StoryEmbedBlock
-        
-        class BlogPage(Page):
-            body = StreamField([
-                ('heading', blocks.CharBlock()),
-                ('paragraph', blocks.RichTextBlock()),
-                ('story_embed', ExternalStoryEmbedBlock()),
-            ])
-        ```
-        
-        This block allows the page author to provide the URL to an AMP web story, which will render on the front-end template (when using `{% include_block %}`) as an `<amp-story-player>` element; your template should include [the necessary scripts for rendering this](https://amp.dev/documentation/guides-and-tutorials/integrate/embed-stories/?format=stories#embed-amp-story-player), along with a CSS rule to specify appropriate dimensions:
-        
-        ```html
-            <script async src="https://cdn.ampproject.org/amp-story-player-v0.js"></script>
-            <link href="https://cdn.ampproject.org/amp-story-player-v0.css" rel="stylesheet" type="text/css">
-            <style>
-                amp-story-player { width: 360px; height: 600px; }
-            </style>
-        ```
-        
-        To include a link to a story rather than embedding it, `wagtail_webstories.blocks.ExternalStoryBlock` can be used in place of `ExternalStoryEmbedBlock`. The default template `wagtail_webstories/blocks/external_story_poster_link.html` outputs a 'card' rendering of the story using the story's poster image, to be used with the following CSS:
-        
-        ```css
-            .webstory-poster {
-                display: block; width: 300px; height: 400px; border-radius: 15px; background-size: cover; position: relative;
-            }
-            .webstory-poster .webstory-info {
-                position: absolute; bottom: 0; width: 100%; background-color: #ccc; color: black; border-bottom-left-radius: 15px; border-bottom-right-radius: 15px;
-            }
-            .webstory-poster .title {
-                font-size: 1.5em; padding: 10px;
-            }
-            .webstory-poster .publisher {
-                padding: 0 10px 20px 10px;
-            }
-            .webstory-poster .publisher img {
-                vertical-align: middle;
-            }
-        ```
-        
-        ## Embedding and linking external stories without StreamField
-        
-        External stories are handled through the model `wagtail_webstories.models.ExternalStory`. To obtain an ExternalStory instance for a given URL, use: `ExternalStory.get_for_url(story_url)`. The story's metadata is cached within the ExternalStory model to avoid having to re-fetch the story on every request - the available metadata fields are `url`, `title`, `publisher`, `publisher_logo_src`, `poster_portrait_src`, `poster_square_src` and `poster_landscape_src`.
-        
-        The StreamField block templates `wagtail_webstories/blocks/external_story_embed_block.html` and `wagtail_webstories/blocks/external_story_poster_link.html` can be used to render an ExternalStory object, by passing it as the variable `story`:
-        
-        ```python
-        # models.py
-        class BlogPostWithStoryPage(Page):
-            story_url = model.URLField(max_length=2048)
-        
-            def get_context(self, request):
-                context = super().get_context(request)
-                context['story_obj'] = ExternalStory.get_for_url(self.story_url)
-                return context
-        ```
-        
-        ```html+django
-        {# blog_post_with_story_page.html #}
-        
-        {% include "wagtail_webstories/blocks/external_story_embed_block.html" with story=story_obj %}
-        ```
-        
-        
-        ## Importing
-        
-        To allow stories to be imported as Wagtail pages, define a model that extends `wagtail_webstories.models.BaseWebStoryPage`:
-        
-        ```python
-        from wagtail_webstories.models import BaseWebStoryPage
-        
-        class StoryPage(BaseWebStoryPage):
-            pass
-        ```
-        
-        Alternatively, if your project has an existing base page class that all page types must inherit from (which would prevent the use of BaseWebStoryPage in addition to that base class), extend `wagtail_webstories.models.WebStoryPageMixin` and define `content_panels` and `promote_panels` to incorporate its panel definitions:
-        
-        ```python
-        from wagtail_webstories.models import WebStoryPageMixin
-        
-        class StoryPage(WebStoryPageMixin, BasePage):
-            content_panels = BasePage.content_panels + WebStoryPageMixin.web_story_content_panels
-            promote_panels = BasePage.promote_panels + WebStoryPageMixin.web_story_promote_panels
-        ```
-        
-        Now create a corresponding template that extends `wagtail_webstories/base_web_story_page.html`:
-        
-        ```html+django
-        {% extends "wagtail_webstories/base_web_story_page.html" %}
-        ```
-        
-        Define a setting `WAGTAIL_WEBSTORIES_IMPORT_MODEL` pointing to the page model to use:
-        
-        ```python
-        WAGTAIL_WEBSTORIES_IMPORT_MODEL = 'myapp.StoryPage'
-        ```
-        
-        This will now add a "Web stories" item to the Wagtail admin menu, allowing you to import stories by URL.
-        
-        
-        ## HTML cleaning
-        
-        By default, all HTML elements and attributes not permitted by the AMP web story specification will be stripped out on importing and saving. To disable this, set `WAGTAIL_WEBSTORIES_CLEAN_HTML` to False:
-        
-        ```python
-        WAGTAIL_WEBSTORIES_CLEAN_HTML = False
-        ```
-        
-        
-        ## Image importing
-        
-        By default, image references within imported stories are left at their original URLs. BaseWebStoryPage provides a method `import_images()` to fetch all referenced images and import them into the Wagtail image library, de-duplicating if they already exist. It is recommended that you call this from a `post_save` signal handler:
-        
-        ```python
-        # myapp/signals.py
-        
-        from django.db.models.signals import post_save
-        from django.dispatch import receiver
-        
-        from .models import StoryPage
-        
-        
-        @receiver(post_save, sender=StoryPage)
-        def import_story_images(sender, instance, **kwargs):
-            changed = instance.import_images()
-            if changed:
-                instance.save()
-        
-        
-        # myapp/apps.py
-        
-        from django.apps import AppConfig
-        
-        
-        class MyappConfig(AppConfig):
-            name = 'myapp'
-        
-            def ready(self):
-                import myapp.signals  # noqa
-        
-        
-        # myapp/__init__.py
-        
-        default_app_config = 'myapp.apps.MyappConfig'
-        ```
-        
-        Since importing images can be a time-consuming process, you may wish to offload the call to `import_images` to a background task using Celery or similar, to avoid this blocking a web server thread.
-        
-        To customise the creation of new images (e.g. to assign imported images to a particular collection, or to populate additional metadata fields on a custom image model), override the story page model's `_create_image` method:
-        
-        ```python
-        class StoryPage(BaseWebStoryPage):
-        
-            def _create_image(self, file, title=None):
-                image = super()._create_image(file, title=title)
-                image.copyright = "All rights reserved"
-                return image
-        ```
-        
-        ## Video importing
-        
-        If you have [wagtailmedia](https://pypi.org/project/wagtailmedia/) installed, you can similarly import videos into the local media library by calling `import_videos()`. The signal handler above then becomes:
-        
-        ```python
-        # myapp/signals.py
-        
-        @receiver(post_save, sender=StoryPage)
-        def import_story_images(sender, instance, **kwargs):
-            images_changed = instance.import_images()
-            videos_changed = instance.import_videos()
-            if images_changed or videos_changed:
-                instance.save()
-        ```
-        
-        ## Linking and embedding imported stories
-        
-        To embed or link an imported web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.StoryEmbedBlock` or `wagtail_webstories.blocks.StoryChooserBlock` block type in your StreamField definition. These work similarly to ExternalStoryEmbedBlock and ExternalStoryBlock, but provide the page author with a page chooser interface rather than a URL field.
-        
-        ```python
-        from wagtail_webstories.blocks import StoryEmbedBlock
-        
-        class BlogPage(Page):
-            body = StreamField([
-                ('heading', blocks.CharBlock()),
-                ('paragraph', blocks.RichTextBlock()),
-                ('local_story_embed', StoryEmbedBlock(target_model=StoryPage)),
-            ])
-        ```
-        
-        The `target_model` argument is optional - by default, any page type inheriting from BaseWebStoryPage can be chosen. As with ExternalStoryEmbedBlock and ExternalStoryBlock, your page template must contain the appropriate JavaScript or CSS include for rendering the block.
-        
-        The templates `wagtail_webstories/blocks/story_poster_link.html` and `wagtail_webstories/blocks/story_embed_block.html` expect a single variable `page` containing the story page instance, so these can also be used outside of StreamField:
-        
-        ```python
-        # models.py
-        class StoryIndexPage(Page):
-            def get_context(self, request):
-                context = super().get_context(request)
-                context['stories'] = StoryPage.objects.child_of(self).live().order_by('-first_published_at')
-                return context
-        ```
-        
-        ```html+django
-        {# story_index_page.html #}
-        {% for story in stories %}
-            {% include "wagtail_webstories/blocks/story_poster_link.html" with page=story %}
-        {% endfor %}
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# wagtail-webstories
+
+This package adds support for [AMP web stories](https://amp.dev/about/stories/) to Wagtail. Stories created elsewhere can be linked or embedded from their original URL locations, or imported as Wagtail pages, including optionally importing images and videos into the Wagtail media library.
+
+`wagtail-webstories` is compatible with Wagtail 4.1 and above.
+
+## Installation
+
+Install with pip:
+
+```bash
+pip install wagtail-webstories
+```
+
+Add to INSTALLED_APPS:
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'wagtail_webstories',
+    # ...
+]
+```
+
+Run migrations:
+
+```bash
+./manage.py migrate
+```
+
+## Embedding and linking external stories
+
+To embed a web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.ExternalStoryEmbedBlock` block type in your StreamField definition:
+
+```python
+from wagtail_webstories.blocks import ExternalStoryEmbedBlock
+
+class BlogPage(Page):
+    body = StreamField([
+        ('heading', blocks.CharBlock()),
+        ('paragraph', blocks.RichTextBlock()),
+        ('story_embed', ExternalStoryEmbedBlock()),
+    ])
+```
+
+This block allows the page author to provide the URL to an AMP web story, which will render on the front-end template (when using `{% include_block %}`) as an `<amp-story-player>` element; your template should include [the necessary scripts for rendering this](https://amp.dev/documentation/guides-and-tutorials/integrate/embed-stories/?format=stories#embed-amp-story-player), along with a CSS rule to specify appropriate dimensions:
+
+```html
+    <script async src="https://cdn.ampproject.org/amp-story-player-v0.js"></script>
+    <link href="https://cdn.ampproject.org/amp-story-player-v0.css" rel="stylesheet" type="text/css">
+    <style>
+        amp-story-player { width: 360px; height: 600px; }
+    </style>
+```
+
+To include a link to a story rather than embedding it, `wagtail_webstories.blocks.ExternalStoryBlock` can be used in place of `ExternalStoryEmbedBlock`. The default template `wagtail_webstories/blocks/external_story_poster_link.html` outputs a 'card' rendering of the story using the story's poster image, to be used with the following CSS:
+
+```css
+    .webstory-poster {
+        display: block; width: 300px; height: 400px; border-radius: 15px; background-size: cover; position: relative;
+    }
+    .webstory-poster .webstory-info {
+        position: absolute; bottom: 0; width: 100%; background-color: #ccc; color: black; border-bottom-left-radius: 15px; border-bottom-right-radius: 15px;
+    }
+    .webstory-poster .title {
+        font-size: 1.5em; padding: 10px;
+    }
+    .webstory-poster .publisher {
+        padding: 0 10px 20px 10px;
+    }
+    .webstory-poster .publisher img {
+        vertical-align: middle;
+    }
+```
+
+## Embedding and linking external stories without StreamField
+
+External stories are handled through the model `wagtail_webstories.models.ExternalStory`. To obtain an ExternalStory instance for a given URL, use: `ExternalStory.get_for_url(story_url)`. The story's metadata is cached within the ExternalStory model to avoid having to re-fetch the story on every request - the available metadata fields are `url`, `title`, `publisher`, `publisher_logo_src`, `poster_portrait_src`, `poster_square_src` and `poster_landscape_src`.
+
+The StreamField block templates `wagtail_webstories/blocks/external_story_embed_block.html` and `wagtail_webstories/blocks/external_story_poster_link.html` can be used to render an ExternalStory object, by passing it as the variable `story`:
+
+```python
+# models.py
+class BlogPostWithStoryPage(Page):
+    story_url = model.URLField(max_length=2048)
+
+    def get_context(self, request):
+        context = super().get_context(request)
+        context['story_obj'] = ExternalStory.get_for_url(self.story_url)
+        return context
+```
+
+```html+django
+{# blog_post_with_story_page.html #}
+
+{% include "wagtail_webstories/blocks/external_story_embed_block.html" with story=story_obj %}
+```
+
+
+## Importing
+
+To allow stories to be imported as Wagtail pages, define a model that extends `wagtail_webstories.models.BaseWebStoryPage`:
+
+```python
+from wagtail_webstories.models import BaseWebStoryPage
+
+class StoryPage(BaseWebStoryPage):
+    pass
+```
+
+Alternatively, if your project has an existing base page class that all page types must inherit from (which would prevent the use of BaseWebStoryPage in addition to that base class), extend `wagtail_webstories.models.WebStoryPageMixin` and define `content_panels` and `promote_panels` to incorporate its panel definitions:
+
+```python
+from wagtail_webstories.models import WebStoryPageMixin
+
+class StoryPage(WebStoryPageMixin, BasePage):
+    content_panels = BasePage.content_panels + WebStoryPageMixin.web_story_content_panels
+    promote_panels = BasePage.promote_panels + WebStoryPageMixin.web_story_promote_panels
+```
+
+Now create a corresponding template that extends `wagtail_webstories/base_web_story_page.html`:
+
+```html+django
+{% extends "wagtail_webstories/base_web_story_page.html" %}
+```
+
+Define a setting `WAGTAIL_WEBSTORIES_IMPORT_MODEL` pointing to the page model to use:
+
+```python
+WAGTAIL_WEBSTORIES_IMPORT_MODEL = 'myapp.StoryPage'
+```
+
+This will now add a "Web stories" item to the Wagtail admin menu, allowing you to import stories by URL.
+
+
+## HTML cleaning
+
+By default, all HTML elements and attributes not permitted by the AMP web story specification will be stripped out on importing and saving. To disable this, set `WAGTAIL_WEBSTORIES_CLEAN_HTML` to False:
+
+```python
+WAGTAIL_WEBSTORIES_CLEAN_HTML = False
+```
+
+
+## Image importing
+
+By default, image references within imported stories are left at their original URLs. BaseWebStoryPage provides a method `import_images()` to fetch all referenced images and import them into the Wagtail image library, de-duplicating if they already exist. It is recommended that you call this from a `post_save` signal handler:
+
+```python
+# myapp/signals.py
+
+from django.db.models.signals import post_save
+from django.dispatch import receiver
+
+from .models import StoryPage
+
+
+@receiver(post_save, sender=StoryPage)
+def import_story_images(sender, instance, **kwargs):
+    changed = instance.import_images()
+    if changed:
+        instance.save()
+
+
+# myapp/apps.py
+
+from django.apps import AppConfig
+
+
+class MyappConfig(AppConfig):
+    name = 'myapp'
+
+    def ready(self):
+        import myapp.signals  # noqa
+
+
+# myapp/__init__.py
+
+default_app_config = 'myapp.apps.MyappConfig'
+```
+
+Since importing images can be a time-consuming process, you may wish to offload the call to `import_images` to a background task using Celery or similar, to avoid this blocking a web server thread.
+
+To customise the creation of new images (e.g. to assign imported images to a particular collection, or to populate additional metadata fields on a custom image model), override the story page model's `_create_image` method:
+
+```python
+class StoryPage(BaseWebStoryPage):
+
+    def _create_image(self, file, title=None):
+        image = super()._create_image(file, title=title)
+        image.copyright = "All rights reserved"
+        return image
+```
+
+## Video importing
+
+If you have [wagtailmedia](https://pypi.org/project/wagtailmedia/) installed, you can similarly import videos into the local media library by calling `import_videos()`. The signal handler above then becomes:
+
+```python
+# myapp/signals.py
+
+@receiver(post_save, sender=StoryPage)
+def import_story_images(sender, instance, **kwargs):
+    images_changed = instance.import_images()
+    videos_changed = instance.import_videos()
+    if images_changed or videos_changed:
+        instance.save()
+```
+
+## Linking and embedding imported stories
+
+To embed or link an imported web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.StoryEmbedBlock` or `wagtail_webstories.blocks.StoryChooserBlock` block type in your StreamField definition. These work similarly to ExternalStoryEmbedBlock and ExternalStoryBlock, but provide the page author with a page chooser interface rather than a URL field.
+
+```python
+from wagtail_webstories.blocks import StoryEmbedBlock
+
+class BlogPage(Page):
+    body = StreamField([
+        ('heading', blocks.CharBlock()),
+        ('paragraph', blocks.RichTextBlock()),
+        ('local_story_embed', StoryEmbedBlock(target_model=StoryPage)),
+    ])
+```
+
+The `target_model` argument is optional - by default, any page type inheriting from BaseWebStoryPage can be chosen. As with ExternalStoryEmbedBlock and ExternalStoryBlock, your page template must contain the appropriate JavaScript or CSS include for rendering the block.
+
+The templates `wagtail_webstories/blocks/story_poster_link.html` and `wagtail_webstories/blocks/story_embed_block.html` expect a single variable `page` containing the story page instance, so these can also be used outside of StreamField:
+
+```python
+# models.py
+class StoryIndexPage(Page):
+    def get_context(self, request):
+        context = super().get_context(request)
+        context['stories'] = StoryPage.objects.child_of(self).live().order_by('-first_published_at')
+        return context
+```
+
+```html+django
+{# story_index_page.html #}
+{% for story in stories %}
+    {% include "wagtail_webstories/blocks/story_poster_link.html" with page=story %}
+{% endfor %}
+```
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories.egg-info/SOURCES.txt` & `wagtail-webstories-0.1/wagtail_webstories.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 wagtail_webstories/__init__.py
 wagtail_webstories/admin_urls.py
+wagtail_webstories/apps.py
 wagtail_webstories/blocks.py
 wagtail_webstories/forms.py
 wagtail_webstories/markup.py
 wagtail_webstories/models.py
 wagtail_webstories/views.py
 wagtail_webstories/wagtail_hooks.py
 wagtail_webstories.egg-info/PKG-INFO
```

### Comparing `wagtail-webstories-0.0.4/LICENSE` & `wagtail-webstories-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-webstories-0.0.4/README.md` & `wagtail-webstories-0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # wagtail-webstories
 
 This package adds support for [AMP web stories](https://amp.dev/about/stories/) to Wagtail. Stories created elsewhere can be linked or embedded from their original URL locations, or imported as Wagtail pages, including optionally importing images and videos into the Wagtail media library.
 
-`wagtail-webstories` is compatible with Wagtail 2.5 and above.
+`wagtail-webstories` is compatible with Wagtail 4.1 and above.
 
 ## Installation
 
 Install with pip:
 
 ```bash
 pip install wagtail-webstories
@@ -29,15 +29,15 @@
 ```
 
 ## Embedding and linking external stories
 
 To embed a web story into a regular (non-AMP) StreamField-based page, include the `wagtail_webstories.blocks.ExternalStoryEmbedBlock` block type in your StreamField definition:
 
 ```python
-from wagtail_webstories.blocks import StoryEmbedBlock
+from wagtail_webstories.blocks import ExternalStoryEmbedBlock
 
 class BlogPage(Page):
     body = StreamField([
         ('heading', blocks.CharBlock()),
         ('paragraph', blocks.RichTextBlock()),
         ('story_embed', ExternalStoryEmbedBlock()),
     ])
```

### Comparing `wagtail-webstories-0.0.4/setup.py` & `wagtail-webstories-0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="wagtail-webstories",
-    version="0.0.4",
+    version="0.1",
     packages=find_packages(exclude=('tests', 'tests.*')),
     include_package_data=True,
     test_suite="tests",
     url="https://github.com/torchbox/wagtail-webstories/",
 
     author="Matt Westcott",
     author_email="matthew@torchbox.com",
@@ -17,27 +17,33 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Framework :: Wagtail :: 2",
+        "Framework :: Django",
+        "Framework :: Django :: 3",
+        "Framework :: Django :: 4",
+        "Framework :: Wagtail",
+        "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "Topic :: Internet :: WWW/HTTP",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
-        "webstories>=0.0.1,<0.1",
+        "wagtail>=4.1",
+        "webstories>=0.0.1,<1",
         "requests>=2.24.0,<3",
         "beautifulsoup4>=4.6,<5",
     ],
     extras_require={
         "testing": [
             "responses>=0.12,<1",
-            "Pillow>=4.0.0,<9.0.0",
-            "wagtailmedia>=0.6,<0.8",
+            "Pillow>=4.0.0,<10.0.0",
+            "wagtailmedia>=0.6,<0.15",
         ]
     },
     license="BSD",
 )
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/migrations/0001_initial.py` & `wagtail-webstories-0.1/wagtail_webstories/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/models.py` & `wagtail-webstories-0.1/wagtail_webstories/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import hashlib
 import json
 import os.path
+import requests
+
 from urllib.parse import urljoin, urlparse
 
 from bs4 import BeautifulSoup
 from django.apps import apps
 from django.core.exceptions import ValidationError
+from django.core.files.base import ContentFile, File
+from django.core.files.images import ImageFile
 from django.db import models
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
-import requests
-from wagtail.admin.edit_handlers import FieldPanel, MultiFieldPanel, StreamFieldPanel
-from wagtail.core.fields import StreamField
-from django.core.files.base import ContentFile, File
-from django.core.files.images import ImageFile
-from wagtail.core.models import Page, get_page_models
+
+from wagtail.admin.panels import FieldPanel, MultiFieldPanel
+from wagtail.fields import StreamField
 from wagtail.images import get_image_model_string
-from wagtail.images.edit_handlers import ImageChooserPanel
 from wagtail.images.models import Filter
+from wagtail.models import Page, get_page_models
+
 from webstories import Story
 
 from .blocks import PageBlock
 from .markup import AMPText
 
 
 # Retrieve the (possibly custom) image model. Can't use get_image_model as of Wagtail 2.11, as we
@@ -53,31 +55,31 @@
 
     original_url = models.URLField('Original URL', blank=True, max_length=2047)
 
     custom_css = models.TextField(blank=True)
 
     pages = StreamField([
         ('page', PageBlock()),
-    ])
+    ], use_json_field=True)
 
     web_story_content_panels = [
         FieldPanel('custom_css'),
-        StreamFieldPanel('pages'),
+        FieldPanel('pages'),
     ]
 
     web_story_promote_panels = [
         MultiFieldPanel([
             FieldPanel('publisher'),
-            ImageChooserPanel('publisher_logo'),
+            FieldPanel('publisher_logo'),
             FieldPanel('original_url'),
         ], heading="Publisher"),
         MultiFieldPanel([
-            ImageChooserPanel('poster_image'),
+            FieldPanel('poster_image'),
         ], heading="Poster"),
-    ]
+    ]        
 
     def clean(self):
         super().clean()
 
         errors = {}
         if not (self.publisher_logo or self.publisher_logo_src_original):
             errors['publisher_logo'] = _("A publisher logo must be provided.")
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/markup.py` & `wagtail-webstories-0.1/wagtail_webstories/markup.py`

 * *Files identical despite different names*

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/forms.py` & `wagtail-webstories-0.1/wagtail_webstories/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
+
 from wagtail.admin.widgets import AdminPageChooser
-from wagtail.core.models import Page
+from wagtail.models import Page
+
 
 class ImportStoryForm(forms.Form):
     source_url = forms.URLField(required=True)
     destination = forms.ModelChoiceField(
         required=True,
         queryset=Page.objects.all(),
         widget=AdminPageChooser(can_choose_root=True, user_perms='copy_to'),
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/wagtail_hooks.py` & `wagtail-webstories-0.1/wagtail_webstories/wagtail_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.conf import settings
-from django.urls import path, include, reverse
+from django.urls import include, path, reverse
+
+from wagtail import hooks
 from wagtail.admin.menu import MenuItem
-from wagtail.core import hooks
 
 from . import admin_urls
 
 if getattr(settings, 'WAGTAIL_WEBSTORIES_IMPORT_MODEL', None):
 
     @hooks.register('register_admin_urls')
     def register_admin_urls():
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/admin/import.html` & `wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/admin/import.html`

 * *Files identical despite different names*

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/templates/wagtail_webstories/base_web_story_page.html` & `wagtail-webstories-0.1/wagtail_webstories/templates/wagtail_webstories/base_web_story_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/blocks.py` & `wagtail-webstories-0.1/wagtail_webstories/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import requests
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext as _
-import requests
-from wagtail.core import blocks
+
+from wagtail import blocks
+
 from webstories import Story, StoryPage
 
 from .markup import AMPText
 
 
 class AMPCleanHTMLBlock(blocks.RawHTMLBlock):
     def clean(self, value):
@@ -71,36 +73,40 @@
     class Meta:
         template = 'wagtail_webstories/blocks/story_embed_block.html'
 
 
 class ExternalStoryBlock(blocks.URLBlock):
     def get_default(self):
         from .models import ExternalStory
+
         # Allow specifying the default as either an ExternalStory or a URL string (or None).
         if not self.meta.default:
             return None
         elif isinstance(self.meta.default, ExternalStory):
             return self.meta.default
         else:
             # assume default has been passed as a string
             return ExternalStory.get_for_url(self.meta.default)
 
     def to_python(self, value):
         from .models import ExternalStory
+
         # The JSON representation of an ExternalStoryBlock value is a URL string;
         # this should be converted to an ExternalStory instance (or None).
         if not value:
             return None
         else:
             return ExternalStory.get_for_url(value)
 
     def get_prep_value(self, value):
         # serialisable value should be a URL string
         if value is None:
             return ''
+        elif isinstance(value, str):
+            return value
         else:
             return value.url
 
     def value_for_form(self, value):
         # the value to be handled by the URLField is a plain URL string (or the empty string)
         if value is None:
             return ''
```

### Comparing `wagtail-webstories-0.0.4/wagtail_webstories/views.py` & `wagtail-webstories-0.1/wagtail_webstories/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import requests
+
 from urllib.parse import urljoin
 
 from django.apps import apps
 from django.conf import settings
 from django.template.response import TemplateResponse
 from django.shortcuts import redirect
 from django.utils.translation import gettext as _
-import requests
 from wagtail.admin import messages
+
 from webstories import Story
 
 from .forms import ImportStoryForm
 from .markup import AMPText
 
 def import_story(request):
     if request.method == 'POST':
```

