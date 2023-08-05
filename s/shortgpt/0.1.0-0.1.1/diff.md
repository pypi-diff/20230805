# Comparing `tmp/shortgpt-0.1.0.tar.gz` & `tmp/shortgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortgpt-0.1.0.tar", last modified: Fri Aug  4 20:10:46 2023, max compression
+gzip compressed data, was "shortgpt-0.1.1.tar", last modified: Sat Aug  5 06:45:16 2023, max compression
```

## Comparing `shortgpt-0.1.0.tar` & `shortgpt-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.620000 shortgpt-0.1.0/
--rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    11354 2023-08-04 20:10:48.000000 shortgpt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 20:10:48.000000 shortgpt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1680 2023-08-04 20:08:30.000000 shortgpt-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.730000 shortgpt-0.1.0/shortGPT/
--rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.0/shortGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.760000 shortgpt-0.1.0/shortGPT/api_utils/
--rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.0/shortGPT/api_utils/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/api_utils/eleven_api.py
--rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.0/shortGPT/api_utils/image_api.py
--rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/api_utils/pexels_api.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.780000 shortgpt-0.1.0/shortGPT/audio/
--rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.0/shortGPT/audio/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/audio/audio_duration.py
--rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/audio/audio_utils.py
--rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/audio/edge_voice_module.py
--rw-rw-rw-   0        0        0     1490 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/audio/eleven_voice_module.py
--rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.0/shortGPT/audio/voice_module.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.810000 shortgpt-0.1.0/shortGPT/config/
--rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.0/shortGPT/config/__init__.py
--rw-rw-rw-   0        0        0      409 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/config/api_db.py
--rw-rw-rw-   0        0        0    11356 2023-08-04 19:58:00.000000 shortgpt-0.1.0/shortGPT/config/asset_db.py
--rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.0/shortGPT/config/config.py
--rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/config/languages.py
--rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/config/path_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.830000 shortgpt-0.1.0/shortGPT/database/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.0/shortGPT/database/__init__.py
--rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/database/content_data_manager.py
--rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/database/content_database.py
--rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/database/db_document.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.860000 shortgpt-0.1.0/shortGPT/editing_utils/
--rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.0/shortGPT/editing_utils/__init__.py
--rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/editing_utils/captions.py
--rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.0/shortGPT/editing_utils/editing_images.py
--rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/editing_utils/handle_videos.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.890000 shortgpt-0.1.0/shortGPT/engine/
--rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.0/shortGPT/engine/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/engine/abstract_content_engine.py
--rw-rw-rw-   0        0        0     8322 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/engine/content_short_engine.py
--rw-rw-rw-   0        0        0     7831 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/engine/content_translation_engine.py
--rw-rw-rw-   0        0        0     7801 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/engine/content_video_engine.py
--rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.0/shortGPT/engine/facts_short_engine.py
--rw-rw-rw-   0        0        0     8283 2023-07-31 18:40:34.000000 shortgpt-0.1.0/shortGPT/engine/multi_language_translation_engine.py
--rw-rw-rw-   0        0        0     5730 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/engine/reddit_short_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.910000 shortgpt-0.1.0/shortGPT/gpt/
--rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.0/shortGPT/gpt/__init__.py
--rw-rw-rw-   0        0        0      921 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/facts_gpt.py
--rw-rw-rw-   0        0        0     1275 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_chat_video.py
--rw-rw-rw-   0        0        0     1788 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_editing.py
--rw-rw-rw-   0        0        0      516 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_translate.py
--rw-rw-rw-   0        0        0     3502 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_utils.py
--rw-rw-rw-   0        0        0      389 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_voice.py
--rw-rw-rw-   0        0        0      806 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/gpt_yt.py
--rw-rw-rw-   0        0        0     2255 2023-07-28 20:38:42.000000 shortgpt-0.1.0/shortGPT/gpt/reddit_gpt.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.930000 shortgpt-0.1.0/shortGPT/tracking/
--rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.0/shortGPT/tracking/__init__.py
--rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.0/shortGPT/tracking/api_tracking.py
--rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.0/shortGPT/tracking/cost_analytics.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:10:45.950000 shortgpt-0.1.0/shortgpt.egg-info/
--rw-rw-rw-   0        0        0    11354 2023-08-04 20:10:46.000000 shortgpt-0.1.0/shortgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-08-04 20:10:46.000000 shortgpt-0.1.0/shortgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 20:10:46.000000 shortgpt-0.1.0/shortgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      199 2023-08-04 20:10:46.000000 shortgpt-0.1.0/shortgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 20:10:46.000000 shortgpt-0.1.0/shortgpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.470000 shortgpt-0.1.1/
+-rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    11354 2023-08-05 06:45:16.000000 shortgpt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 06:45:16.000000 shortgpt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-08-05 06:45:06.000000 shortgpt-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.530000 shortgpt-0.1.1/shortGPT/
+-rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.1/shortGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.550000 shortgpt-0.1.1/shortGPT/api_utils/
+-rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.1/shortGPT/api_utils/__init__.py
+-rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/api_utils/eleven_api.py
+-rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.1/shortGPT/api_utils/image_api.py
+-rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/api_utils/pexels_api.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.580000 shortgpt-0.1.1/shortGPT/audio/
+-rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.1/shortGPT/audio/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/audio/audio_duration.py
+-rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/audio/audio_utils.py
+-rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/audio/edge_voice_module.py
+-rw-rw-rw-   0        0        0     1496 2023-08-05 06:24:20.000000 shortgpt-0.1.1/shortGPT/audio/eleven_voice_module.py
+-rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.1/shortGPT/audio/voice_module.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.600000 shortgpt-0.1.1/shortGPT/config/
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.1/shortGPT/config/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-08-04 20:21:38.000000 shortgpt-0.1.1/shortGPT/config/api_db.py
+-rw-rw-rw-   0        0        0    11429 2023-08-05 06:16:26.000000 shortgpt-0.1.1/shortGPT/config/asset_db.py
+-rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/config/config.py
+-rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/config/languages.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/config/path_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.630000 shortgpt-0.1.1/shortGPT/database/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.1/shortGPT/database/__init__.py
+-rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/content_data_manager.py
+-rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/content_database.py
+-rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/db_document.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.660000 shortgpt-0.1.1/shortGPT/editing_framework/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.1/shortGPT/editing_framework/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/core_editing_engine.py
+-rw-rw-rw-   0        0        0    11103 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.680000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:50.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-07-08 06:01:18.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_background_video.json
+-rw-rw-rw-   0        0        0      289 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_background_voiceover.json
+-rw-rw-rw-   0        0        0      182 2023-06-24 19:21:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_voiceover.json
+-rw-rw-rw-   0        0        0      457 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/background_music.json
+-rw-rw-rw-   0        0        0      553 2023-07-16 07:07:54.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json
+-rw-rw-rw-   0        0        0      546 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/extract_audio.json
+-rw-rw-rw-   0        0        0      350 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/insert_audio.json
+-rw-rw-rw-   0        0        0      616 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption.json
+-rw-rw-rw-   0        0        0      617 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic.json
+-rw-rw-rw-   0        0        0      558 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json
+-rw-rw-rw-   0        0        0      579 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_landscape.json
+-rw-rw-rw-   0        0        0      404 2023-06-26 06:51:40.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_reddit_image.json
+-rw-rw-rw-   0        0        0      686 2023-06-24 02:50:20.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_top_image.json
+-rw-rw-rw-   0        0        0      512 2023-06-24 20:04:38.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_watermark.json
+-rw-rw-rw-   0        0        0      592 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/subscribe_animation.json
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.710000 shortgpt-0.1.1/shortGPT/editing_framework/flows/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:56.000000 shortgpt-0.1.1/shortGPT/editing_framework/flows/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/editing_framework/flows/build_reddit_image.json
+-rw-rw-rw-   0        0        0     1107 2023-07-11 20:20:30.000000 shortgpt-0.1.1/shortGPT/editing_framework/rendering_logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.730000 shortgpt-0.1.1/shortGPT/editing_utils/
+-rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.1/shortGPT/editing_utils/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_utils/captions.py
+-rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.1/shortGPT/editing_utils/editing_images.py
+-rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_utils/handle_videos.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.760000 shortgpt-0.1.1/shortGPT/engine/
+-rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.1/shortGPT/engine/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/abstract_content_engine.py
+-rw-rw-rw-   0        0        0     8322 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_short_engine.py
+-rw-rw-rw-   0        0        0     7831 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_translation_engine.py
+-rw-rw-rw-   0        0        0     7801 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_video_engine.py
+-rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.1/shortGPT/engine/facts_short_engine.py
+-rw-rw-rw-   0        0        0     8283 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/multi_language_translation_engine.py
+-rw-rw-rw-   0        0        0     5730 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/engine/reddit_short_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.780000 shortgpt-0.1.1/shortGPT/gpt/
+-rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.1/shortGPT/gpt/__init__.py
+-rw-rw-rw-   0        0        0      921 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/facts_gpt.py
+-rw-rw-rw-   0        0        0     1275 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_chat_video.py
+-rw-rw-rw-   0        0        0     1788 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_editing.py
+-rw-rw-rw-   0        0        0      516 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_translate.py
+-rw-rw-rw-   0        0        0     3502 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_utils.py
+-rw-rw-rw-   0        0        0      389 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_voice.py
+-rw-rw-rw-   0        0        0      806 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_yt.py
+-rw-rw-rw-   0        0        0     2255 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/reddit_gpt.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.810000 shortgpt-0.1.1/shortGPT/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:34:46.000000 shortgpt-0.1.1/shortGPT/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      970 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_edit_script.yaml
+-rw-rw-rw-   0        0        0      918 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_script.yaml
+-rw-rw-rw-   0        0        0     3199 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_images.yaml
+-rw-rw-rw-   0        0        0     1897 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_videos.yaml
+-rw-rw-rw-   0        0        0     1629 2023-07-07 17:47:06.000000 shortgpt-0.1.1/shortGPT/prompt_templates/facts_generator.yaml
+-rw-rw-rw-   0        0        0      342 2023-07-07 17:46:48.000000 shortgpt-0.1.1/shortGPT/prompt_templates/facts_subjects_generation.yaml
+-rw-rw-rw-   0        0        0     1910 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_extract_question.yaml
+-rw-rw-rw-   0        0        0      722 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_filter_realistic.yaml
+-rw-rw-rw-   0        0        0     1657 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_question.yaml
+-rw-rw-rw-   0        0        0     1604 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_script.yaml
+-rw-rw-rw-   0        0        0     1160 2023-06-29 23:38:32.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_story_filter.yaml
+-rw-rw-rw-   0        0        0      245 2023-07-07 06:42:50.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_username.yaml
+-rw-rw-rw-   0        0        0      757 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/translate_content.yaml
+-rw-rw-rw-   0        0        0      356 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/voice_identify_gender.yaml
+-rw-rw-rw-   0        0        0      814 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/yt_title_description.yaml
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.830000 shortgpt-0.1.1/shortGPT/tracking/
+-rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.1/shortGPT/tracking/__init__.py
+-rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.1/shortGPT/tracking/api_tracking.py
+-rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.1/shortGPT/tracking/cost_analytics.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.860000 shortgpt-0.1.1/shortgpt.egg-info/
+-rw-rw-rw-   0        0        0    11354 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/top_level.txt
```

### Comparing `shortgpt-0.1.0/LICENSE` & `shortgpt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/PKG-INFO` & `shortgpt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.0 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.1 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
```

### Comparing `shortgpt-0.1.0/README.md` & `shortgpt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/setup.py` & `shortgpt-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,46 +3,45 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Automating video and short content creation with AI'
 LONG_DESCRIPTION = 'A powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.'
 
 
 setup(
     name="shortgpt",
     version=VERSION,
     author="RayVentura",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
+    package_data={'': ['*.yaml', '*.json']},    # This will include all yaml files in package
     install_requires=[
         'ffmpeg', 
         'python-dotenv', 
-        'gradio',
         'openai', 
         'tiktoken',
         'tinydb',
         'tinymongo',
         'proglog',
         'yt-dlp',
         'torch',
         'whisper-timestamped',
         'torchaudio',
         'pillow==9.0.0',
         'protobuf==3.20.0',
         'edge-tts',
         'moviepy==1.0.3',
-        'termcolor',
         'progress',
         'questionary',
     ],
     keywords=['python', 'video', 'content creation', 'AI', 'automation', 'editing', 'voiceover synthesis', 'video captions', 'asset sourcing', 'tinyDB'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `shortgpt-0.1.0/shortGPT/__init__.py` & `shortgpt-0.1.1/shortGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/api_utils/eleven_api.py` & `shortgpt-0.1.1/shortGPT/api_utils/eleven_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/api_utils/image_api.py` & `shortgpt-0.1.1/shortGPT/api_utils/image_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/api_utils/pexels_api.py` & `shortgpt-0.1.1/shortGPT/api_utils/pexels_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/audio/audio_duration.py` & `shortgpt-0.1.1/shortGPT/audio/audio_duration.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/audio/audio_utils.py` & `shortgpt-0.1.1/shortGPT/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/audio/edge_voice_module.py` & `shortgpt-0.1.1/shortGPT/audio/edge_voice_module.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/audio/eleven_voice_module.py` & `shortgpt-0.1.1/shortGPT/audio/eleven_voice_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from shortGPT.api_utils.eleven_api import ElevenLabsAPI
 from shortGPT.audio.voice_module import VoiceModule
 
 
 class ElevenLabsVoiceModule(VoiceModule):
-    def __init__(self, api_key, voiceName, checkElevenCredits):
+    def __init__(self, api_key, voiceName, checkElevenCredits=False):
         self.api_key = api_key
         self.voiceName = voiceName
         self.remaining_credits = None
         self.eleven_labs_api = ElevenLabsAPI(self.api_key)
         self.update_usage()
         if checkElevenCredits and self.get_remaining_characters() < 1200:
             raise Exception(f"Your ElevenLabs API KEY doesn't have enough credits ({self.remaining_credits} character remaining). Minimum required: 1200 characters (equivalent to a 45sec short)")
```

### Comparing `shortgpt-0.1.0/shortGPT/config/asset_db.py` & `shortgpt-0.1.1/shortGPT/config/asset_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import base64
 import re
 import shutil
 import time
 from datetime import datetime
 from pathlib import Path
-
+import enum
 import pandas as pd
 
 from shortGPT.audio.audio_utils import downloadYoutubeAudio, get_asset_duration
 from shortGPT.database.db_document import TinyMongoDocument
 
 AUDIO_EXTENSIONS = {".mp3", ".m4a", ".wav", ".flac", ".aac", ".ogg", ".wma", ".opus"}
 IMAGE_EXTENSIONS = {".jpg", ".jpeg", ".png", ".gif", ".bmp", ".svg", ".webp"}
 VIDEO_EXTENSIONS = {".mp4", ".mkv", ".flv", ".avi", ".mov", ".wmv", ".webm", ".m4v"}
 TEMPLATE_ASSETS_DB_PATH = '.database/template_asset_db.json'
 ASSETS_DB_PATH = '.database/asset_db.json'
 
+class AssetType(enum.Enum):
+    VIDEO = "video"
+    AUDIO = "audio"
+    IMAGE = "image"
+    BACKGROUND_MUSIC = "background music"
+    BACKGROUND_VIDEO = "background video"
+    OTHER = "other"
 
 class AssetDatabase:
     """
     Class for managing assets, both local and remote.
     The class provides methods to add, remove, get and sync assets.
     It uses a MongoDB-like database to store information about the assets.
     """
 
     if not Path(ASSETS_DB_PATH).exists() and Path(TEMPLATE_ASSETS_DB_PATH).exists():
         shutil.copy(TEMPLATE_ASSETS_DB_PATH, ASSETS_DB_PATH)
 
     local_assets = TinyMongoDocument("asset_db", "asset_collection", "local_assets", create=True)
     remote_assets = TinyMongoDocument("asset_db", "asset_collection", "remote_assets", create=True)
 
-    @classmethod
-    def _update_timestamp_and_get(cls, asset_type, key):
-        asset = asset_type._get(key)
-        asset['ts'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        asset_type._save({key: asset})
-        return asset
 
     @classmethod
     def asset_exists(cls, name: str) -> bool:
         return name in cls.local_assets._get() or name in cls.remote_assets._get()
 
     @classmethod
-    def add_local_asset(cls, name: str, asset_type: str, path: str):
+    def add_local_asset(cls, name: str, asset_type: AssetType, path: str):
         cls.local_assets._save({
             name: {
-                "type": asset_type,
+                "type": asset_type.value,
                 "path": path,
                 "ts": datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             }
         })
 
     @classmethod
-    def add_remote_asset(cls, name: str, asset_type: str, url: str):
+    def add_remote_asset(cls, name: str, asset_type: AssetType, url: str):
         cls.remote_assets._save({
             name: {
-                "type": asset_type,
+                "type": asset_type.value,
                 "url": url,
                 "ts": datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             }
         })
 
     @classmethod
     def remove_asset(cls, name: str):
@@ -82,15 +83,15 @@
                              'ts': asset.get('ts')
                              })
         if source is None or source == 'youtube':
             for key, asset in cls.remote_assets._get().items():
                 data.append({'name': key,
                             'type': asset['type'],
                              'link': asset['url'],
-                             'source': 'youtube',
+                             'source': 'youtube' if 'youtube' in asset['url'] else 'internet',
                              'ts': asset.get('ts')
                              })
 
         df = pd.DataFrame(data)
         if (not df.empty):
             df.sort_values(by='ts', ascending=False, inplace=True)
             return df.drop(columns='ts')
@@ -166,25 +167,25 @@
         Add a local asset to the database from a file path.
 
         Args:
             path (Path): Path to the asset.
         """
         file_ext = path.suffix
         if file_ext in AUDIO_EXTENSIONS:
-            asset_type = 'audio'
+            asset_type = AssetType.AUDIO
         elif file_ext in IMAGE_EXTENSIONS:
-            asset_type = 'image'
+            asset_type = AssetType.IMAGE
         elif file_ext in VIDEO_EXTENSIONS:
-            asset_type = 'video'
+            asset_type = AssetType.VIDEO
         else:
-            asset_type = 'other'
+            asset_type = AssetType.OTHER
         cls.local_assets._save({
             path.stem: {
                 "path": str(path),
-                "type": asset_type,
+                "type": asset_type.value,
                 "ts": datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             }
         })
 
     @classmethod
     def _update_local_asset_timestamp_and_get_link(cls, key: str) -> str:
         """
```

### Comparing `shortgpt-0.1.0/shortGPT/config/config.py` & `shortgpt-0.1.1/shortGPT/config/config.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/config/languages.py` & `shortgpt-0.1.1/shortGPT/config/languages.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/config/path_utils.py` & `shortgpt-0.1.1/shortGPT/config/path_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/database/content_data_manager.py` & `shortgpt-0.1.1/shortGPT/database/content_data_manager.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/database/content_database.py` & `shortgpt-0.1.1/shortGPT/database/content_database.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/database/db_document.py` & `shortgpt-0.1.1/shortGPT/database/db_document.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/editing_utils/captions.py` & `shortgpt-0.1.1/shortGPT/editing_utils/captions.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/editing_utils/editing_images.py` & `shortgpt-0.1.1/shortGPT/editing_utils/editing_images.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/editing_utils/handle_videos.py` & `shortgpt-0.1.1/shortGPT/editing_utils/handle_videos.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/abstract_content_engine.py` & `shortgpt-0.1.1/shortGPT/engine/abstract_content_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/content_short_engine.py` & `shortgpt-0.1.1/shortGPT/engine/content_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/content_translation_engine.py` & `shortgpt-0.1.1/shortGPT/engine/content_translation_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/content_video_engine.py` & `shortgpt-0.1.1/shortGPT/engine/content_video_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/facts_short_engine.py` & `shortgpt-0.1.1/shortGPT/engine/facts_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/multi_language_translation_engine.py` & `shortgpt-0.1.1/shortGPT/engine/multi_language_translation_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/engine/reddit_short_engine.py` & `shortgpt-0.1.1/shortGPT/engine/reddit_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/facts_gpt.py` & `shortgpt-0.1.1/shortGPT/gpt/facts_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/gpt_chat_video.py` & `shortgpt-0.1.1/shortGPT/gpt/gpt_chat_video.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/gpt_editing.py` & `shortgpt-0.1.1/shortGPT/gpt/gpt_editing.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/gpt_translate.py` & `shortgpt-0.1.1/shortGPT/gpt/gpt_translate.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/gpt_utils.py` & `shortgpt-0.1.1/shortGPT/gpt/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/gpt_yt.py` & `shortgpt-0.1.1/shortGPT/gpt/gpt_yt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/gpt/reddit_gpt.py` & `shortgpt-0.1.1/shortGPT/gpt/reddit_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/tracking/api_tracking.py` & `shortgpt-0.1.1/shortGPT/tracking/api_tracking.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortGPT/tracking/cost_analytics.py` & `shortgpt-0.1.1/shortGPT/tracking/cost_analytics.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.0/shortgpt.egg-info/PKG-INFO` & `shortgpt-0.1.1/shortgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automating video and short content creation with AI
 Author: RayVentura
 Author-email: 
 Keywords: python,video,content creation,AI,automation,editing,voiceover synthesis,video captions,asset sourcing,tinyDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.0 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.1 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
```

