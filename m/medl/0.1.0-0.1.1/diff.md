# Comparing `tmp/medl-0.1.0.tar.gz` & `tmp/medl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medl-0.1.0.tar", max compression
+gzip compressed data, was "medl-0.1.1.tar", max compression
```

## Comparing `medl-0.1.0.tar` & `medl-0.1.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1087 2023-07-26 13:16:25.684059 medl-0.1.0/LICENSE
--rw-r--r--   0        0        0      285 2023-07-26 13:16:25.684059 medl-0.1.0/README.md
--rw-r--r--   0        0        0      293 2023-07-26 13:16:25.684059 medl-0.1.0/medl/__init__.py
--rw-r--r--   0        0        0      420 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/__init__.py
--rw-r--r--   0        0        0      219 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/__init__.py
--rw-r--r--   0        0        0      154 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/init/__init__.py
--rw-r--r--   0        0        0      160 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/init/ffmpeg_initializer.py
--rw-r--r--   0        0        0      289 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/init/folder_initializer.py
--rw-r--r--   0        0        0      243 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/initializer.py
--rw-r--r--   0        0        0      717 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/log_formatter.py
--rw-r--r--   0        0        0     2729 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/logger.py
--rw-r--r--   0        0        0      340 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/classes/options_manager.py
--rw-r--r--   0        0        0       90 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/consts/__init__.py
--rw-r--r--   0        0        0      169 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/consts/paths.py
--rw-r--r--   0        0        0      109 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/data/__init__.py
--rw-r--r--   0        0        0      846 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/data/medl_options.py
--rw-r--r--   0        0        0     2243 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/data/song_data.py
--rw-r--r--   0        0        0       71 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/di/__init__.py
--rw-r--r--   0        0        0      643 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/di/dependency_injection.py
--rw-r--r--   0        0        0       71 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/exceptions/__init__.py
--rw-r--r--   0        0        0      147 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/exceptions/medl_exception.py
--rw-r--r--   0        0        0      202 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/interfaces/__init__.py
--rw-r--r--   0        0        0      134 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/interfaces/base_initializer.py
--rw-r--r--   0        0        0      444 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/interfaces/base_logger.py
--rw-r--r--   0        0        0      265 2023-07-26 13:16:25.684059 medl-0.1.0/medl/common/interfaces/base_options_manager.py
--rw-r--r--   0        0        0      266 2023-07-26 13:16:25.684059 medl-0.1.0/medl/dependency_injection.py
--rw-r--r--   0        0        0      157 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/__init__.py
--rw-r--r--   0        0        0      987 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/__init__.py
--rw-r--r--   0        0        0      591 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/__init__.py
--rw-r--r--   0        0        0      832 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/download_url_finder.py
--rw-r--r--   0        0        0     1145 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/lyrics_fetcher.py
--rw-r--r--   0        0        0      981 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/metadata_embedder.py
--rw-r--r--   0        0        0     1637 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/metadata_fetcher.py
--rw-r--r--   0        0        0      735 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/post_download_handler.py
--rw-r--r--   0        0        0     1176 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/pre_download_handler.py
--rw-r--r--   0        0        0     1242 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/track_converter.py
--rw-r--r--   0        0        0      899 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/handlers/track_downloader.py
--rw-r--r--   0        0        0      544 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/__init__.py
--rw-r--r--   0        0        0      789 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/download_url_finder_logger.py
--rw-r--r--   0        0        0      726 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/lyrics_fetcher_logger.py
--rw-r--r--   0        0        0      824 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/metadata_embedder_logger.py
--rw-r--r--   0        0        0      781 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/metadata_fetcher_logger.py
--rw-r--r--   0        0        0      758 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/track_converter_logger.py
--rw-r--r--   0        0        0      818 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/loggers/track_downloader_logger.py
--rw-r--r--   0        0        0     3037 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/music_toolbox.py
--rw-r--r--   0        0        0      259 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/tools/__init__.py
--rw-r--r--   0        0        0     1358 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/tools/downloader.py
--rw-r--r--   0        0        0     2219 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/tools/ffmpeg_converter.py
--rw-r--r--   0        0        0     1042 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/tools/parallelizer.py
--rw-r--r--   0        0        0      933 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/classes/tools/path_formatter.py
--rw-r--r--   0        0        0       68 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/data/__init__.py
--rw-r--r--   0        0        0      160 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/data/download_info.py
--rw-r--r--   0        0        0      188 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/di/__init__.py
--rw-r--r--   0        0        0      654 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/di/dependency_injector.py
--rw-r--r--   0        0        0     1428 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/di/handler_injector.py
--rw-r--r--   0        0        0     1291 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/di/logger_injector.py
--rw-r--r--   0        0        0      741 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/di/tool_injector.py
--rw-r--r--   0        0        0     1164 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/__init__.py
--rw-r--r--   0        0        0      421 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/base_music_toolbox.py
--rw-r--r--   0        0        0      695 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/__init__.py
--rw-r--r--   0        0        0      223 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_download_url_finder.py
--rw-r--r--   0        0        0      213 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_lyrics_fetcher.py
--rw-r--r--   0        0        0      271 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_metadata_embedder.py
--rw-r--r--   0        0        0      282 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_metadata_fetcher.py
--rw-r--r--   0        0        0      223 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_post_download_handler.py
--rw-r--r--   0        0        0      221 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_pre_download_handler.py
--rw-r--r--   0        0        0      312 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_track_converter.py
--rw-r--r--   0        0        0      288 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/handlers/base_track_downloader.py
--rw-r--r--   0        0        0      622 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/__init__.py
--rw-r--r--   0        0        0      356 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_download_url_finder_logger.py
--rw-r--r--   0        0        0      349 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_lyrics_fetcher_logger.py
--rw-r--r--   0        0        0      374 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_metadata_embedder_logger.py
--rw-r--r--   0        0        0      434 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_metadata_fetcher_logger.py
--rw-r--r--   0        0        0      382 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_track_converter_logger.py
--rw-r--r--   0        0        0      406 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/loggers/base_track_downloader_logger.py
--rw-r--r--   0        0        0      311 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/tools/__init__.py
--rw-r--r--   0        0        0      194 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/tools/base_downloader.py
--rw-r--r--   0        0        0      207 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/tools/base_ffmpeg_converter.py
--rw-r--r--   0        0        0      256 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/tools/base_parallelizer.py
--rw-r--r--   0        0        0      220 2023-07-26 13:16:25.684059 medl-0.1.0/medl/main/interfaces/tools/base_path_formatter.py
--rw-r--r--   0        0        0        0 2023-07-26 13:16:25.684059 medl-0.1.0/medl/py.typed
--rw-r--r--   0        0        0      828 2023-07-26 13:16:25.684059 medl-0.1.0/medl/test.py
--rw-r--r--   0        0        0     1394 2023-07-26 13:16:25.684059 medl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 medl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-27 19:11:55.270328 medl-0.1.1/LICENSE
+-rw-r--r--   0        0        0      285 2023-07-27 19:11:55.270328 medl-0.1.1/README.md
+-rw-r--r--   0        0        0      293 2023-07-27 19:11:55.270328 medl-0.1.1/medl/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/init/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/init/ffmpeg_initializer.py
+-rw-r--r--   0        0        0      289 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/init/folder_initializer.py
+-rw-r--r--   0        0        0      243 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/initializer.py
+-rw-r--r--   0        0        0      717 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/log_formatter.py
+-rw-r--r--   0        0        0     2729 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/logger.py
+-rw-r--r--   0        0        0      340 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/classes/options_manager.py
+-rw-r--r--   0        0        0       90 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/consts/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/consts/paths.py
+-rw-r--r--   0        0        0      109 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/data/__init__.py
+-rw-r--r--   0        0        0      846 2023-07-27 19:11:55.270328 medl-0.1.1/medl/common/data/medl_options.py
+-rw-r--r--   0        0        0     2243 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/data/song_data.py
+-rw-r--r--   0        0        0       71 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/di/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/di/dependency_injection.py
+-rw-r--r--   0        0        0       71 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      147 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/exceptions/medl_exception.py
+-rw-r--r--   0        0        0      202 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/interfaces/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/interfaces/base_initializer.py
+-rw-r--r--   0        0        0      444 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/interfaces/base_logger.py
+-rw-r--r--   0        0        0      265 2023-07-27 19:11:55.274328 medl-0.1.1/medl/common/interfaces/base_options_manager.py
+-rw-r--r--   0        0        0      266 2023-07-27 19:11:55.274328 medl-0.1.1/medl/dependency_injection.py
+-rw-r--r--   0        0        0      157 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/__init__.py
+-rw-r--r--   0        0        0      987 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/__init__.py
+-rw-r--r--   0        0        0      591 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/download_url_finder.py
+-rw-r--r--   0        0        0     1145 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/lyrics_fetcher.py
+-rw-r--r--   0        0        0      981 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/metadata_embedder.py
+-rw-r--r--   0        0        0     1637 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/metadata_fetcher.py
+-rw-r--r--   0        0        0      735 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/post_download_handler.py
+-rw-r--r--   0        0        0     1176 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/pre_download_handler.py
+-rw-r--r--   0        0        0     1242 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/track_converter.py
+-rw-r--r--   0        0        0      899 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/handlers/track_downloader.py
+-rw-r--r--   0        0        0      544 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/download_url_finder_logger.py
+-rw-r--r--   0        0        0      726 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/lyrics_fetcher_logger.py
+-rw-r--r--   0        0        0      824 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/metadata_embedder_logger.py
+-rw-r--r--   0        0        0      781 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/metadata_fetcher_logger.py
+-rw-r--r--   0        0        0      758 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/track_converter_logger.py
+-rw-r--r--   0        0        0      818 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/loggers/track_downloader_logger.py
+-rw-r--r--   0        0        0     3037 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/music_toolbox.py
+-rw-r--r--   0        0        0      259 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/tools/__init__.py
+-rw-r--r--   0        0        0     1358 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/tools/downloader.py
+-rw-r--r--   0        0        0     2219 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/tools/ffmpeg_converter.py
+-rw-r--r--   0        0        0     1042 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/tools/parallelizer.py
+-rw-r--r--   0        0        0      933 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/classes/tools/path_formatter.py
+-rw-r--r--   0        0        0       68 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/data/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/data/download_info.py
+-rw-r--r--   0        0        0      188 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/di/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/di/dependency_injector.py
+-rw-r--r--   0        0        0     1428 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/di/handler_injector.py
+-rw-r--r--   0        0        0     1291 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/di/logger_injector.py
+-rw-r--r--   0        0        0      741 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/di/tool_injector.py
+-rw-r--r--   0        0        0     1164 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/base_music_toolbox.py
+-rw-r--r--   0        0        0      695 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_download_url_finder.py
+-rw-r--r--   0        0        0      213 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_lyrics_fetcher.py
+-rw-r--r--   0        0        0      271 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_metadata_embedder.py
+-rw-r--r--   0        0        0      282 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_metadata_fetcher.py
+-rw-r--r--   0        0        0      223 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_post_download_handler.py
+-rw-r--r--   0        0        0      221 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_pre_download_handler.py
+-rw-r--r--   0        0        0      312 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_track_converter.py
+-rw-r--r--   0        0        0      288 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/handlers/base_track_downloader.py
+-rw-r--r--   0        0        0      622 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/__init__.py
+-rw-r--r--   0        0        0      356 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_download_url_finder_logger.py
+-rw-r--r--   0        0        0      349 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_lyrics_fetcher_logger.py
+-rw-r--r--   0        0        0      374 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_metadata_embedder_logger.py
+-rw-r--r--   0        0        0      434 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_metadata_fetcher_logger.py
+-rw-r--r--   0        0        0      382 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_track_converter_logger.py
+-rw-r--r--   0        0        0      406 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/loggers/base_track_downloader_logger.py
+-rw-r--r--   0        0        0      311 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/tools/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/tools/base_downloader.py
+-rw-r--r--   0        0        0      207 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/tools/base_ffmpeg_converter.py
+-rw-r--r--   0        0        0      256 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/tools/base_parallelizer.py
+-rw-r--r--   0        0        0      220 2023-07-27 19:11:55.274328 medl-0.1.1/medl/main/interfaces/tools/base_path_formatter.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:11:55.274328 medl-0.1.1/medl/py.typed
+-rw-r--r--   0        0        0      828 2023-07-27 19:11:55.274328 medl-0.1.1/medl/test.py
+-rw-r--r--   0        0        0     1394 2023-07-27 19:11:55.274328 medl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 medl-0.1.1/PKG-INFO
```

### Comparing `medl-0.1.0/LICENSE` & `medl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/common/classes/log_formatter.py` & `medl-0.1.1/medl/common/classes/log_formatter.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/common/classes/logger.py` & `medl-0.1.1/medl/common/classes/logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/common/data/medl_options.py` & `medl-0.1.1/medl/common/data/medl_options.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/common/data/song_data.py` & `medl-0.1.1/medl/common/data/song_data.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/common/di/dependency_injection.py` & `medl-0.1.1/medl/common/di/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/__init__.py` & `medl-0.1.1/medl/main/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/__init__.py` & `medl-0.1.1/medl/main/classes/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/download_url_finder.py` & `medl-0.1.1/medl/main/classes/handlers/download_url_finder.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/lyrics_fetcher.py` & `medl-0.1.1/medl/main/classes/handlers/lyrics_fetcher.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/metadata_embedder.py` & `medl-0.1.1/medl/main/classes/handlers/metadata_embedder.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/metadata_fetcher.py` & `medl-0.1.1/medl/main/classes/handlers/metadata_fetcher.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/post_download_handler.py` & `medl-0.1.1/medl/main/classes/handlers/post_download_handler.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/pre_download_handler.py` & `medl-0.1.1/medl/main/classes/handlers/pre_download_handler.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/track_converter.py` & `medl-0.1.1/medl/main/classes/handlers/track_converter.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/handlers/track_downloader.py` & `medl-0.1.1/medl/main/classes/handlers/track_downloader.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/__init__.py` & `medl-0.1.1/medl/main/classes/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/download_url_finder_logger.py` & `medl-0.1.1/medl/main/classes/loggers/download_url_finder_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/lyrics_fetcher_logger.py` & `medl-0.1.1/medl/main/classes/loggers/lyrics_fetcher_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/metadata_embedder_logger.py` & `medl-0.1.1/medl/main/classes/loggers/metadata_embedder_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/metadata_fetcher_logger.py` & `medl-0.1.1/medl/main/classes/loggers/metadata_fetcher_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/track_converter_logger.py` & `medl-0.1.1/medl/main/classes/loggers/track_converter_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/loggers/track_downloader_logger.py` & `medl-0.1.1/medl/main/classes/loggers/track_downloader_logger.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/music_toolbox.py` & `medl-0.1.1/medl/main/classes/music_toolbox.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/tools/downloader.py` & `medl-0.1.1/medl/main/classes/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/tools/ffmpeg_converter.py` & `medl-0.1.1/medl/main/classes/tools/ffmpeg_converter.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/classes/tools/parallelizer.py` & `medl-0.1.1/medl/main/classes/tools/parallelizer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         options = options_manager.get_options()
 
         self._loop: asyncio.AbstractEventLoop = (
             asyncio.new_event_loop()
             if sys.platform != "win32"
             else asyncio.ProactorEventLoop()
         )
-        self._semaphore: asyncio.Semaphore = asyncio.Semaphore(options.threads)
-
         asyncio.set_event_loop(self._loop)
 
+        self._semaphore: asyncio.Semaphore = asyncio.Semaphore(options.threads)
+
     def run_in_parallel(self, method: Callable[[T], U], arguments: List[T]) -> List[U]:
         async def method_with_semaphore(arg: T):
             async with self._semaphore:
                 return await self._loop.run_in_executor(None, method, arg)
 
         tasks = [method_with_semaphore(arg) for arg in arguments]
         results = list(self._loop.run_until_complete(asyncio.gather(*tasks)))
```

### Comparing `medl-0.1.0/medl/main/classes/tools/path_formatter.py` & `medl-0.1.1/medl/main/classes/tools/path_formatter.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/di/dependency_injector.py` & `medl-0.1.1/medl/main/di/dependency_injector.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/di/handler_injector.py` & `medl-0.1.1/medl/main/di/handler_injector.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/di/logger_injector.py` & `medl-0.1.1/medl/main/di/logger_injector.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/di/tool_injector.py` & `medl-0.1.1/medl/main/di/tool_injector.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/interfaces/__init__.py` & `medl-0.1.1/medl/main/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/interfaces/handlers/__init__.py` & `medl-0.1.1/medl/main/interfaces/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/main/interfaces/loggers/__init__.py` & `medl-0.1.1/medl/main/interfaces/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/medl/test.py` & `medl-0.1.1/medl/test.py`

 * *Files identical despite different names*

### Comparing `medl-0.1.0/pyproject.toml` & `medl-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Medl"
-version = "0.1.0"
+version = "0.1.1"
 description = "Music Explorer and DownLoader"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "medl"}]
 
 keywords = ["medl", "music", "python", "metadata", "spotify", "youtube", "youtube music"]
```

### Comparing `medl-0.1.0/PKG-INFO` & `medl-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Music Explorer and DownLoader
 Home-page: https://github.com/Billuc/Medl
 License: MIT
 Keywords: medl,music,python,metadata,spotify,youtube,youtube music
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
```

