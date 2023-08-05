# Comparing `tmp/shortgpt-0.1.1.tar.gz` & `tmp/shortgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortgpt-0.1.1.tar", last modified: Sat Aug  5 06:45:16 2023, max compression
+gzip compressed data, was "shortgpt-0.1.2.tar", last modified: Sat Aug  5 07:02:58 2023, max compression
```

## Comparing `shortgpt-0.1.1.tar` & `shortgpt-0.1.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.470000 shortgpt-0.1.1/
--rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    11354 2023-08-05 06:45:16.000000 shortgpt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 06:45:16.000000 shortgpt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-08-05 06:45:06.000000 shortgpt-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.530000 shortgpt-0.1.1/shortGPT/
--rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.1/shortGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.550000 shortgpt-0.1.1/shortGPT/api_utils/
--rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.1/shortGPT/api_utils/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/api_utils/eleven_api.py
--rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.1/shortGPT/api_utils/image_api.py
--rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/api_utils/pexels_api.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.580000 shortgpt-0.1.1/shortGPT/audio/
--rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.1/shortGPT/audio/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/audio/audio_duration.py
--rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/audio/audio_utils.py
--rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/audio/edge_voice_module.py
--rw-rw-rw-   0        0        0     1496 2023-08-05 06:24:20.000000 shortgpt-0.1.1/shortGPT/audio/eleven_voice_module.py
--rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.1/shortGPT/audio/voice_module.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.600000 shortgpt-0.1.1/shortGPT/config/
--rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.1/shortGPT/config/__init__.py
--rw-rw-rw-   0        0        0      715 2023-08-04 20:21:38.000000 shortgpt-0.1.1/shortGPT/config/api_db.py
--rw-rw-rw-   0        0        0    11429 2023-08-05 06:16:26.000000 shortgpt-0.1.1/shortGPT/config/asset_db.py
--rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/config/config.py
--rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/config/languages.py
--rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/config/path_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.630000 shortgpt-0.1.1/shortGPT/database/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.1/shortGPT/database/__init__.py
--rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/content_data_manager.py
--rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/content_database.py
--rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/database/db_document.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.660000 shortgpt-0.1.1/shortGPT/editing_framework/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.1/shortGPT/editing_framework/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/core_editing_engine.py
--rw-rw-rw-   0        0        0    11103 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.680000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:39:50.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/__init__.py
--rw-rw-rw-   0        0        0      374 2023-07-08 06:01:18.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_background_video.json
--rw-rw-rw-   0        0        0      289 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_background_voiceover.json
--rw-rw-rw-   0        0        0      182 2023-06-24 19:21:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/add_voiceover.json
--rw-rw-rw-   0        0        0      457 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/background_music.json
--rw-rw-rw-   0        0        0      553 2023-07-16 07:07:54.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json
--rw-rw-rw-   0        0        0      546 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/extract_audio.json
--rw-rw-rw-   0        0        0      350 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/insert_audio.json
--rw-rw-rw-   0        0        0      616 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption.json
--rw-rw-rw-   0        0        0      617 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic.json
--rw-rw-rw-   0        0        0      558 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json
--rw-rw-rw-   0        0        0      579 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_landscape.json
--rw-rw-rw-   0        0        0      404 2023-06-26 06:51:40.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_reddit_image.json
--rw-rw-rw-   0        0        0      686 2023-06-24 02:50:20.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_top_image.json
--rw-rw-rw-   0        0        0      512 2023-06-24 20:04:38.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_watermark.json
--rw-rw-rw-   0        0        0      592 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/subscribe_animation.json
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.710000 shortgpt-0.1.1/shortGPT/editing_framework/flows/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:39:56.000000 shortgpt-0.1.1/shortGPT/editing_framework/flows/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-07-03 07:06:58.000000 shortgpt-0.1.1/shortGPT/editing_framework/flows/build_reddit_image.json
--rw-rw-rw-   0        0        0     1107 2023-07-11 20:20:30.000000 shortgpt-0.1.1/shortGPT/editing_framework/rendering_logger.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.730000 shortgpt-0.1.1/shortGPT/editing_utils/
--rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.1/shortGPT/editing_utils/__init__.py
--rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_utils/captions.py
--rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.1/shortGPT/editing_utils/editing_images.py
--rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/editing_utils/handle_videos.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.760000 shortgpt-0.1.1/shortGPT/engine/
--rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.1/shortGPT/engine/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/abstract_content_engine.py
--rw-rw-rw-   0        0        0     8322 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_short_engine.py
--rw-rw-rw-   0        0        0     7831 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_translation_engine.py
--rw-rw-rw-   0        0        0     7801 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/content_video_engine.py
--rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.1/shortGPT/engine/facts_short_engine.py
--rw-rw-rw-   0        0        0     8283 2023-07-31 18:40:34.000000 shortgpt-0.1.1/shortGPT/engine/multi_language_translation_engine.py
--rw-rw-rw-   0        0        0     5730 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/engine/reddit_short_engine.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.780000 shortgpt-0.1.1/shortGPT/gpt/
--rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.1/shortGPT/gpt/__init__.py
--rw-rw-rw-   0        0        0      921 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/facts_gpt.py
--rw-rw-rw-   0        0        0     1275 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_chat_video.py
--rw-rw-rw-   0        0        0     1788 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_editing.py
--rw-rw-rw-   0        0        0      516 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_translate.py
--rw-rw-rw-   0        0        0     3502 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_utils.py
--rw-rw-rw-   0        0        0      389 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_voice.py
--rw-rw-rw-   0        0        0      806 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/gpt_yt.py
--rw-rw-rw-   0        0        0     2255 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/gpt/reddit_gpt.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.810000 shortgpt-0.1.1/shortGPT/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-08-05 06:34:46.000000 shortgpt-0.1.1/shortGPT/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      970 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_edit_script.yaml
--rw-rw-rw-   0        0        0      918 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_script.yaml
--rw-rw-rw-   0        0        0     3199 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_images.yaml
--rw-rw-rw-   0        0        0     1897 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_videos.yaml
--rw-rw-rw-   0        0        0     1629 2023-07-07 17:47:06.000000 shortgpt-0.1.1/shortGPT/prompt_templates/facts_generator.yaml
--rw-rw-rw-   0        0        0      342 2023-07-07 17:46:48.000000 shortgpt-0.1.1/shortGPT/prompt_templates/facts_subjects_generation.yaml
--rw-rw-rw-   0        0        0     1910 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_extract_question.yaml
--rw-rw-rw-   0        0        0      722 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_filter_realistic.yaml
--rw-rw-rw-   0        0        0     1657 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_question.yaml
--rw-rw-rw-   0        0        0     1604 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_script.yaml
--rw-rw-rw-   0        0        0     1160 2023-06-29 23:38:32.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_story_filter.yaml
--rw-rw-rw-   0        0        0      245 2023-07-07 06:42:50.000000 shortgpt-0.1.1/shortGPT/prompt_templates/reddit_username.yaml
--rw-rw-rw-   0        0        0      757 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/translate_content.yaml
--rw-rw-rw-   0        0        0      356 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/voice_identify_gender.yaml
--rw-rw-rw-   0        0        0      814 2023-07-28 20:38:42.000000 shortgpt-0.1.1/shortGPT/prompt_templates/yt_title_description.yaml
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.830000 shortgpt-0.1.1/shortGPT/tracking/
--rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.1/shortGPT/tracking/__init__.py
--rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.1/shortGPT/tracking/api_tracking.py
--rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.1/shortGPT/tracking/cost_analytics.py
-drwxrwxrwx   0        0        0        0 2023-08-05 06:45:14.860000 shortgpt-0.1.1/shortgpt.egg-info/
--rw-rw-rw-   0        0        0    11354 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 06:45:16.000000 shortgpt-0.1.1/shortgpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:56.820000 shortgpt-0.1.2/
+-rw-rw-rw-   0        0        0     2446 2023-07-28 20:38:40.000000 shortgpt-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    11354 2023-08-05 07:03:00.000000 shortgpt-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10523 2023-08-04 05:22:42.000000 shortgpt-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 07:03:00.000000 shortgpt-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-08-05 07:02:42.000000 shortgpt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:56.950000 shortgpt-0.1.2/shortGPT/
+-rw-rw-rw-   0        0        0      945 2023-06-25 07:31:22.000000 shortgpt-0.1.2/shortGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:56.970000 shortgpt-0.1.2/shortGPT/api_utils/
+-rw-rw-rw-   0        0        0       49 2023-06-16 06:17:04.000000 shortgpt-0.1.2/shortGPT/api_utils/__init__.py
+-rw-rw-rw-   0        0        0     2150 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/api_utils/eleven_api.py
+-rw-rw-rw-   0        0        0     1558 2023-06-21 03:55:24.000000 shortgpt-0.1.2/shortGPT/api_utils/image_api.py
+-rw-rw-rw-   0        0        0     2231 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/api_utils/pexels_api.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.000000 shortgpt-0.1.2/shortGPT/audio/
+-rw-rw-rw-   0        0        0       90 2023-06-17 09:33:20.000000 shortgpt-0.1.2/shortGPT/audio/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-07-31 18:40:34.000000 shortgpt-0.1.2/shortGPT/audio/audio_duration.py
+-rw-rw-rw-   0        0        0     3515 2023-07-31 18:40:34.000000 shortgpt-0.1.2/shortGPT/audio/audio_utils.py
+-rw-rw-rw-   0        0        0     1874 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/audio/edge_voice_module.py
+-rw-rw-rw-   0        0        0     1496 2023-08-05 06:24:20.000000 shortgpt-0.1.2/shortGPT/audio/eleven_voice_module.py
+-rw-rw-rw-   0        0        0      332 2023-07-05 20:41:30.000000 shortgpt-0.1.2/shortGPT/audio/voice_module.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.020000 shortgpt-0.1.2/shortGPT/config/
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:42:54.000000 shortgpt-0.1.2/shortGPT/config/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-08-04 20:21:38.000000 shortgpt-0.1.2/shortGPT/config/api_db.py
+-rw-rw-rw-   0        0        0    11429 2023-08-05 06:16:26.000000 shortgpt-0.1.2/shortGPT/config/asset_db.py
+-rw-rw-rw-   0        0        0     2065 2023-07-03 07:06:58.000000 shortgpt-0.1.2/shortGPT/config/config.py
+-rw-rw-rw-   0        0        0    11200 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/config/languages.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/config/path_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.050000 shortgpt-0.1.2/shortGPT/database/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.2/shortGPT/database/__init__.py
+-rw-rw-rw-   0        0        0      784 2023-07-31 18:40:34.000000 shortgpt-0.1.2/shortGPT/database/content_data_manager.py
+-rw-rw-rw-   0        0        0     1167 2023-07-31 18:40:34.000000 shortgpt-0.1.2/shortGPT/database/content_database.py
+-rw-rw-rw-   0        0        0     3914 2023-07-31 18:40:34.000000 shortgpt-0.1.2/shortGPT/database/db_document.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.070000 shortgpt-0.1.2/shortGPT/editing_framework/
+-rw-rw-rw-   0        0        0        0 2023-06-26 19:09:00.000000 shortgpt-0.1.2/shortGPT/editing_framework/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/core_editing_engine.py
+-rw-rw-rw-   0        0        0    11103 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.090000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:50.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-07-08 06:01:18.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/add_background_video.json
+-rw-rw-rw-   0        0        0      289 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/add_background_voiceover.json
+-rw-rw-rw-   0        0        0      182 2023-06-24 19:21:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/add_voiceover.json
+-rw-rw-rw-   0        0        0      457 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/background_music.json
+-rw-rw-rw-   0        0        0      553 2023-07-16 07:07:54.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json
+-rw-rw-rw-   0        0        0      546 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/extract_audio.json
+-rw-rw-rw-   0        0        0      350 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/insert_audio.json
+-rw-rw-rw-   0        0        0      616 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption.json
+-rw-rw-rw-   0        0        0      617 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_arabic.json
+-rw-rw-rw-   0        0        0      558 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json
+-rw-rw-rw-   0        0        0      579 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_landscape.json
+-rw-rw-rw-   0        0        0      404 2023-06-26 06:51:40.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/show_reddit_image.json
+-rw-rw-rw-   0        0        0      686 2023-06-24 02:50:20.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/show_top_image.json
+-rw-rw-rw-   0        0        0      512 2023-06-24 20:04:38.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/show_watermark.json
+-rw-rw-rw-   0        0        0      592 2023-07-03 07:06:58.000000 shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/subscribe_animation.json
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.130000 shortgpt-0.1.2/shortGPT/editing_framework/flows/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:39:56.000000 shortgpt-0.1.2/shortGPT/editing_framework/flows/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-07-03 07:06:58.000000 shortgpt-0.1.2/shortGPT/editing_framework/flows/build_reddit_image.json
+-rw-rw-rw-   0        0        0     1107 2023-07-11 20:20:30.000000 shortgpt-0.1.2/shortGPT/editing_framework/rendering_logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.160000 shortgpt-0.1.2/shortGPT/editing_utils/
+-rw-rw-rw-   0        0        0       52 2023-06-26 03:51:12.000000 shortgpt-0.1.2/shortGPT/editing_utils/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_utils/captions.py
+-rw-rw-rw-   0        0        0      781 2023-07-11 20:20:28.000000 shortgpt-0.1.2/shortGPT/editing_utils/editing_images.py
+-rw-rw-rw-   0        0        0     3423 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/editing_utils/handle_videos.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.200000 shortgpt-0.1.2/shortGPT/engine/
+-rw-rw-rw-   0        0        0       72 2023-07-08 06:01:18.000000 shortgpt-0.1.2/shortGPT/engine/__init__.py
+-rw-rw-rw-   0        0        0     4124 2023-08-05 06:59:58.000000 shortgpt-0.1.2/shortGPT/engine/abstract_content_engine.py
+-rw-rw-rw-   0        0        0     8375 2023-08-05 07:01:10.000000 shortgpt-0.1.2/shortGPT/engine/content_short_engine.py
+-rw-rw-rw-   0        0        0     7884 2023-08-05 07:01:08.000000 shortgpt-0.1.2/shortGPT/engine/content_translation_engine.py
+-rw-rw-rw-   0        0        0     7854 2023-08-05 07:01:14.000000 shortgpt-0.1.2/shortGPT/engine/content_video_engine.py
+-rw-rw-rw-   0        0        0     1023 2023-07-29 19:03:56.000000 shortgpt-0.1.2/shortGPT/engine/facts_short_engine.py
+-rw-rw-rw-   0        0        0     8336 2023-08-05 07:01:20.000000 shortgpt-0.1.2/shortGPT/engine/multi_language_translation_engine.py
+-rw-rw-rw-   0        0        0     5783 2023-08-05 07:01:24.000000 shortgpt-0.1.2/shortGPT/engine/reddit_short_engine.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.230000 shortgpt-0.1.2/shortGPT/gpt/
+-rw-rw-rw-   0        0        0       49 2023-06-14 21:37:36.000000 shortgpt-0.1.2/shortGPT/gpt/__init__.py
+-rw-rw-rw-   0        0        0      921 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/facts_gpt.py
+-rw-rw-rw-   0        0        0     1275 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_chat_video.py
+-rw-rw-rw-   0        0        0     1788 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_editing.py
+-rw-rw-rw-   0        0        0      516 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_translate.py
+-rw-rw-rw-   0        0        0     3502 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_utils.py
+-rw-rw-rw-   0        0        0      389 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_voice.py
+-rw-rw-rw-   0        0        0      806 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/gpt_yt.py
+-rw-rw-rw-   0        0        0     2255 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/gpt/reddit_gpt.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.260000 shortgpt-0.1.2/shortGPT/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-08-05 06:34:46.000000 shortgpt-0.1.2/shortGPT/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      970 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/chat_video_edit_script.yaml
+-rw-rw-rw-   0        0        0      918 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/chat_video_script.yaml
+-rw-rw-rw-   0        0        0     3199 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/editing_generate_images.yaml
+-rw-rw-rw-   0        0        0     1897 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/editing_generate_videos.yaml
+-rw-rw-rw-   0        0        0     1629 2023-07-07 17:47:06.000000 shortgpt-0.1.2/shortGPT/prompt_templates/facts_generator.yaml
+-rw-rw-rw-   0        0        0      342 2023-07-07 17:46:48.000000 shortgpt-0.1.2/shortGPT/prompt_templates/facts_subjects_generation.yaml
+-rw-rw-rw-   0        0        0     1910 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_extract_question.yaml
+-rw-rw-rw-   0        0        0      722 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_filter_realistic.yaml
+-rw-rw-rw-   0        0        0     1657 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_generate_question.yaml
+-rw-rw-rw-   0        0        0     1604 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_generate_script.yaml
+-rw-rw-rw-   0        0        0     1160 2023-06-29 23:38:32.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_story_filter.yaml
+-rw-rw-rw-   0        0        0      245 2023-07-07 06:42:50.000000 shortgpt-0.1.2/shortGPT/prompt_templates/reddit_username.yaml
+-rw-rw-rw-   0        0        0      757 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/translate_content.yaml
+-rw-rw-rw-   0        0        0      356 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/voice_identify_gender.yaml
+-rw-rw-rw-   0        0        0      814 2023-07-28 20:38:42.000000 shortgpt-0.1.2/shortGPT/prompt_templates/yt_title_description.yaml
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.280000 shortgpt-0.1.2/shortGPT/tracking/
+-rw-rw-rw-   0        0        0       26 2023-06-12 09:14:36.000000 shortgpt-0.1.2/shortGPT/tracking/__init__.py
+-rw-rw-rw-   0        0        0     1975 2023-07-02 23:56:10.000000 shortgpt-0.1.2/shortGPT/tracking/api_tracking.py
+-rw-rw-rw-   0        0        0     1693 2023-07-03 00:19:18.000000 shortgpt-0.1.2/shortGPT/tracking/cost_analytics.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:02:57.420000 shortgpt-0.1.2/shortgpt.egg-info/
+-rw-rw-rw-   0        0        0    11354 2023-08-05 07:02:58.000000 shortgpt-0.1.2/shortgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2023-08-05 07:02:58.000000 shortgpt-0.1.2/shortgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 07:02:58.000000 shortgpt-0.1.2/shortgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-08-05 07:02:58.000000 shortgpt-0.1.2/shortgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 07:02:58.000000 shortgpt-0.1.2/shortgpt.egg-info/top_level.txt
```

### Comparing `shortgpt-0.1.1/LICENSE` & `shortgpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/PKG-INFO` & `shortgpt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.1 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.2 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
```

### Comparing `shortgpt-0.1.1/README.md` & `shortgpt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/setup.py` & `shortgpt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Automating video and short content creation with AI'
 LONG_DESCRIPTION = 'A powerful tool for automating content creation. It simplifies video creation, footage sourcing, voiceover synthesis, and editing tasks.'
 
 
 setup(
     name="shortgpt",
     version=VERSION,
```

### Comparing `shortgpt-0.1.1/shortGPT/__init__.py` & `shortgpt-0.1.2/shortGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/api_utils/eleven_api.py` & `shortgpt-0.1.2/shortGPT/api_utils/eleven_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/api_utils/image_api.py` & `shortgpt-0.1.2/shortGPT/api_utils/image_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/api_utils/pexels_api.py` & `shortgpt-0.1.2/shortGPT/api_utils/pexels_api.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/audio/audio_duration.py` & `shortgpt-0.1.2/shortGPT/audio/audio_duration.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/audio/audio_utils.py` & `shortgpt-0.1.2/shortGPT/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/audio/edge_voice_module.py` & `shortgpt-0.1.2/shortGPT/audio/edge_voice_module.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/audio/eleven_voice_module.py` & `shortgpt-0.1.2/shortGPT/audio/eleven_voice_module.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/config/api_db.py` & `shortgpt-0.1.2/shortGPT/config/api_db.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/config/asset_db.py` & `shortgpt-0.1.2/shortGPT/config/asset_db.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/config/config.py` & `shortgpt-0.1.2/shortGPT/config/config.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/config/languages.py` & `shortgpt-0.1.2/shortGPT/config/languages.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/config/path_utils.py` & `shortgpt-0.1.2/shortGPT/config/path_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/database/content_data_manager.py` & `shortgpt-0.1.2/shortGPT/database/content_data_manager.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/database/content_database.py` & `shortgpt-0.1.2/shortGPT/database/content_database.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/database/db_document.py` & `shortgpt-0.1.2/shortGPT/database/db_document.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/core_editing_engine.py` & `shortgpt-0.1.2/shortGPT/editing_framework/core_editing_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_engine.py` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/crop_1920x1080_to_short.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/extract_audio.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/extract_audio.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_arabic.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_arabic_landscape.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/make_caption_landscape.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/make_caption_landscape.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_top_image.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/show_top_image.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/show_watermark.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/show_watermark.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/editing_steps/subscribe_animation.json` & `shortgpt-0.1.2/shortGPT/editing_framework/editing_steps/subscribe_animation.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/flows/build_reddit_image.json` & `shortgpt-0.1.2/shortGPT/editing_framework/flows/build_reddit_image.json`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_framework/rendering_logger.py` & `shortgpt-0.1.2/shortGPT/editing_framework/rendering_logger.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_utils/captions.py` & `shortgpt-0.1.2/shortGPT/editing_utils/captions.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_utils/editing_images.py` & `shortgpt-0.1.2/shortGPT/editing_utils/editing_images.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/editing_utils/handle_videos.py` & `shortgpt-0.1.2/shortGPT/editing_utils/handle_videos.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/engine/abstract_content_engine.py` & `shortgpt-0.1.2/shortGPT/engine/abstract_content_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
             self.dataManager = CONTENT_DB.createContentDataManager(content_type)
         self.id = str(self.dataManager._getId())
         self.initializeMagickAndFFMPEG()
         self.prepareEditingPaths()
         self._db_language = language.value
         self.voiceModule = voiceModule
         self.stepDict = {}
-        self.logger = lambda _: print(_)
+        self.default_logger = lambda _: print(_)
+        self.logger = self.default_logger
 
     def __getattr__(self, name):
         if name.startswith('_db_'):
             db_path = name[4:]  # remove '_db_' prefix
             cache_attr = '_' + name
             if not hasattr(self, cache_attr):
                 setattr(self, cache_attr, self.dataManager.get(db_path))
```

### Comparing `shortgpt-0.1.1/shortGPT/engine/content_short_engine.py` & `shortgpt-0.1.2/shortGPT/engine/content_short_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                                                           'set_time_end': timing[1]})
             if self._db_num_images:
                 for timing, image_url in self._db_timed_image_urls:
                     videoEditor.addEditingStep(EditingStep.SHOW_IMAGE, {'url': image_url,
                                                                         'set_time_start': timing[0],
                                                                         'set_time_end': timing[1]})
 
-            videoEditor.renderVideo(outputPath, logger=self.logger)
+            videoEditor.renderVideo(outputPath, logger= self.logger if self.logger is not self.default_logger else None)
 
         self._db_video_path = outputPath
 
     def _addYoutubeMetadata(self):
 
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
```

### Comparing `shortgpt-0.1.1/shortGPT/engine/content_translation_engine.py` & `shortgpt-0.1.2/shortGPT/engine/content_translation_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 caption_key = "LANDSCAPE" if is_landscape else "SHORT"
                 caption_key += "_ARABIC" if target_language == Language.ARABIC else ""
                 caption_type = getattr(EditingStep, f"ADD_CAPTION_{caption_key}")
                 editing_engine.addEditingStep(caption_type, {'text': text, "set_time_start": t1, "set_time_end": t2})
     
         self._db_video_path = self.dynamicAssetDir+"translated_content.mp4"
 
-        editing_engine.renderVideo(self._db_video_path, logger=self.logger)
+        editing_engine.renderVideo(self._db_video_path, logger= self.logger if self.logger is not self.default_logger else None)
     def _add_metadata(self):
         self.logger(f"5 / 5 - Saving translated video")
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', f"translated_content_to_{self._db_target_language}")
```

### Comparing `shortgpt-0.1.1/shortGPT/engine/content_video_engine.py` & `shortgpt-0.1.2/shortGPT/engine/content_video_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                 caption_type = EditingStep.ADD_CAPTION_LANDSCAPE_ARABIC if self._db_language == Language.ARABIC.value else EditingStep.ADD_CAPTION_LANDSCAPE
 
             for (t1, t2), text in self._db_timed_captions:
                 videoEditor.addEditingStep(caption_type, {'text': text.upper(),
                                                           'set_time_start': t1,
                                                           'set_time_end': t2})
 
-            videoEditor.renderVideo(outputPath, logger=self.logger)
+            videoEditor.renderVideo(outputPath, logger= self.logger if self.logger is not self.default_logger else None)
 
         self._db_video_path = outputPath
 
     def _addMetadata(self):
 
         self._db_yt_title, self._db_yt_description = gpt_yt.generate_title_description_dict(self._db_script)
```

### Comparing `shortgpt-0.1.1/shortGPT/engine/facts_short_engine.py` & `shortgpt-0.1.2/shortGPT/engine/facts_short_engine.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/engine/multi_language_translation_engine.py` & `shortgpt-0.1.2/shortGPT/engine/multi_language_translation_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 caption_key = "LANDSCAPE" if is_landscape else "SHORT"
                 caption_key += "_ARABIC" if target_language == Language.ARABIC else ""
                 caption_type = getattr(EditingStep, f"ADD_CAPTION_{caption_key}")
                 editing_engine.addEditingStep(caption_type, {'text': text, "set_time_start": t1, "set_time_end": t2})
     
         self._db_video_path = self.dynamicAssetDir+"translated_content.mp4"
 
-        editing_engine.renderVideo(self._db_video_path, logger=self.logger)
+        editing_engine.renderVideo(self._db_video_path, logger= self.logger if self.logger is not self.default_logger else None)
 
     def _add_metadata(self):
         self.logger(f"5 / 5 - Saving translated video")
         now = datetime.datetime.now()
         date_str = now.strftime("%Y-%m-%d_%H-%M-%S")
         newFileName = f"videos/{date_str} - " + \
             re.sub(r"[^a-zA-Z0-9 '\n\.]", '', f"translated_content_to_{self._db_target_language}")
```

### Comparing `shortgpt-0.1.1/shortGPT/engine/reddit_short_engine.py` & `shortgpt-0.1.2/shortGPT/engine/reddit_short_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,11 +94,11 @@
                                                                      'set_time_end': timing[1]})
             if self._db_num_images:
                 for timing, image_url in self._db_timed_image_urls:
                     videoEditor.addEditingStep(EditingStep.SHOW_IMAGE, {'url': image_url,
                                                                         'set_time_start': timing[0],
                                                                         'set_time_end': timing[1]})
 
-            videoEditor.renderVideo(outputPath, logger=self.logger)
+            videoEditor.renderVideo(outputPath, logger= self.logger if self.logger is not self.default_logger else None)
 
         self._db_video_path = outputPath
```

### Comparing `shortgpt-0.1.1/shortGPT/gpt/facts_gpt.py` & `shortgpt-0.1.2/shortGPT/gpt/facts_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/gpt_chat_video.py` & `shortgpt-0.1.2/shortGPT/gpt/gpt_chat_video.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/gpt_editing.py` & `shortgpt-0.1.2/shortGPT/gpt/gpt_editing.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/gpt_translate.py` & `shortgpt-0.1.2/shortGPT/gpt/gpt_translate.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/gpt_utils.py` & `shortgpt-0.1.2/shortGPT/gpt/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/gpt_yt.py` & `shortgpt-0.1.2/shortGPT/gpt/gpt_yt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/gpt/reddit_gpt.py` & `shortgpt-0.1.2/shortGPT/gpt/reddit_gpt.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_edit_script.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/chat_video_edit_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/chat_video_script.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/chat_video_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_images.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/editing_generate_images.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/editing_generate_videos.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/editing_generate_videos.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/facts_generator.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/facts_generator.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/reddit_extract_question.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/reddit_extract_question.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/reddit_filter_realistic.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/reddit_filter_realistic.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_question.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/reddit_generate_question.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/reddit_generate_script.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/reddit_generate_script.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/reddit_story_filter.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/reddit_story_filter.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/translate_content.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/translate_content.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/prompt_templates/yt_title_description.yaml` & `shortgpt-0.1.2/shortGPT/prompt_templates/yt_title_description.yaml`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/tracking/api_tracking.py` & `shortgpt-0.1.2/shortGPT/tracking/api_tracking.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortGPT/tracking/cost_analytics.py` & `shortgpt-0.1.2/shortGPT/tracking/cost_analytics.py`

 * *Files identical despite different names*

### Comparing `shortgpt-0.1.1/shortgpt.egg-info/PKG-INFO` & `shortgpt-0.1.2/shortgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortgpt
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: shortgpt Version: 0.1.1 Summary: Automating video
+Metadata-Version: 2.1 Name: shortgpt Version: 0.1.2 Summary: Automating video
 and short content creation with AI Author: RayVentura Author-email: Keywords:
 python,video,content creation,AI,automation,editing,voiceover synthesis,video
 captions,asset sourcing,tinyDB Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Description-Content-Type: text/markdown License-File:
```

### Comparing `shortgpt-0.1.1/shortgpt.egg-info/SOURCES.txt` & `shortgpt-0.1.2/shortgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

