# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.4.0.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.0.tar", last modified: Sat Aug  5 04:23:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.0.1.tar", last modified: Sat Aug  5 06:16:44 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.tar` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.0/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    28728 2023-08-05 02:07:47.982325 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6142 2023-08-03 14:38:58.225454 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    17343 2023-08-04 09:13:48.463075 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    21031 2023-08-05 02:04:53.047052 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    11786 2023-08-05 02:25:43.200082 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2724 2023-08-04 05:01:28.104471 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    47852 2023-08-05 02:25:45.537023 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      724 2023-07-31 04:15:37.158867 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      726 2023-08-05 04:23:19.480361 nonebot_plugin_stable_diffusion_diao-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.0.1/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    28637 2023-08-05 06:13:30.218007 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6142 2023-08-03 14:38:58.225454 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    17343 2023-08-05 06:16:23.495307 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    20931 2023-08-05 06:16:35.081043 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    11921 2023-08-05 05:23:20.600432 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2724 2023-08-05 06:16:27.628128 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    47852 2023-08-05 06:16:29.349873 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6353 2023-08-05 06:16:09.106340 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0     1010 2023-08-05 06:14:11.260591 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-08-05 06:16:44.723306 nonebot_plugin_stable_diffusion_diao-0.4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import re
 import random
 import json
 import os
 import ast
 
-
 from collections import deque
 from copy import deepcopy
 import aiohttp
 from aiohttp.client_exceptions import ClientConnectorError, ClientOSError
 from argparse import Namespace
 from asyncio import get_running_loop
 from nonebot import get_bot, on_shell_command
@@ -177,16 +176,16 @@
                 message_id = message_data["message_id"]
                 loop = get_running_loop()
                 loop.call_later(
                     random.randint(30, 60),
                     lambda: loop.create_task(
                         bot.delete_msg(message_id=message_id)),
                 )
-        first_tag_list = [tag for tag in args.tags]
-        tags_list = tags_to_list(",".join(first_tag_list))
+        tags_str = await prepocess_tags(args.tags, False)
+        tags_list = tags_to_list(tags_str)
         if redis_client:
             if config.auto_match and args.match is False:
                 r = redis_client[1]
                 if r.exists("style"):
                     info_style = ""
                     style_list: list[bytes] = r.lrange("style", 0, -1)
                     style_list_: list[bytes] = r.lrange("user_style", 0, -1)
@@ -210,20 +209,15 @@
         fifo = AIDRAW(**vars(args), event=event)
         fifo.extra_info += info_style
         
         if fifo.backend_index is not None and isinstance(fifo.backend_index, int):
             fifo.backend_name = config.backend_name_list[fifo.backend_index]
         else:
             await fifo.load_balance_init()
-        tags = fifo.tags
-        if isinstance(tags, str):
-            tags_list = tags_to_list(tags)
-        else:
-            tags_list = tags
-        org_tag_list = tags_list
+        org_tag_list = fifo.tags
         org_list = deepcopy(tags_list)
         new_tags_list = []
         if args.match or not config.auto_match:
             pass
         elif redis_client:
             r2 = redis_client[1]
             try:
@@ -278,20 +272,21 @@
                         fifo.extra_info += "自动匹配到的模型过多\n已关闭自动匹配功能"
                         model_info = ""
                         raise RuntimeError("匹配到很多lora")
                     fifo.extra_info += f"{model_info}\n"
             except Exception as e:
                 logger.warning(str(traceback.print_exc()))
                 new_tags_list = []
+                tags_list = org_list
                 logger.warning(f"tag自动匹配失效,出现问题的: {tag}\n或者是prompt里自动匹配到的模型过多")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
-            tags_list: str = await prepocess_tags(tags_list)
+            tags_list: str = await prepocess_tags(tags_list, False, True)
         except Exception as e:
-            logger.debug(str(e))
+            logger.error(str(traceback.print_exc()))
             await aidraw.finish("tag处理失败!可能是翻译API错误, 请稍后重试, 或者使用英文重试")
         fifo.ntags = await prepocess_tags(fifo.ntags)
         pattern = re.compile(f"{htags}", re.IGNORECASE)
         h_words = ""
         if isinstance(event, PrivateMessageEvent):
             pass
         else:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     novelai_cd: int = 60  # 默认的cd
     novelai_group_cd: int = 3  # 默认的群共享cd
     novelai_on: bool = True  # 是否全局开启
     novelai_revoke: int = 0  # 是否自动撤回，该值不为0时，则为撤回时间
     novelai_random_ratio: bool = True  # 是否开启随机比例
     novelai_random_sampler: bool = False  # 是否开启随机采样器
     novelai_random_scale: bool = False  # 是否开启随机CFG
-    novelai_random_ratio_list: list =  [("p", 0.55), ("s", 0.1), ("l", 0.2), ("uw", 0.05), ("uwp", 0.1)] # 随机图片比例
-    novelai_random_sampler_list = [("Euler a", 0.35), ("DDIM", 0.3), ("DPM++ 2S a Karras", 0.05), ("DPM++ 2M Karras", 0.3)]
-    novelai_random_scale_list = [(3, 0.05), (4, 0.2), (5, 0.05), (6, 0.4), (7, 0.1), (8, 0.18), (9, 0.02)]
+    novelai_random_ratio_list: list =  [("p", 0.7), ("s", 0.1), ("l", 0.1), ("uw", 0.05), ("uwp", 0.05)] # 随机图片比例
+    novelai_random_sampler_list = [("Euler a", 0.9), ("DDIM", 0.1)]
+    novelai_random_scale_list = [(5, 0.4), (6, 0.4), (7, 0.2)]
     novelai_load_balance: bool = True  # 负载均衡, 使用前请先将队列限速关闭, 目前只支持stable-diffusion-webui, 所以目前只支持novelai_mode = "sd" 时可用, 目前已知问题, 很短很短时间内疯狂画图的话无法均匀分配任务
     novelai_load_balance_mode: int = 1  # 负载均衡模式, 1为随机, 2为加权随机选择
     novelai_load_balance_weight: list = []  # 设置列表, 列表长度为你的后端数量, 数值为随机权重, 例[0.2, 0.5, 0.3]
     novelai_backend_url_dict: dict = {"雕雕的后端": "la.iamdiao.lol:5938", "雕雕的后端2": "la.iamdiao.lol:1521"} # 你能用到的后端, 键为名称, 值为url, 例:backend_url_dict = {"NVIDIA P102-100": "192.168.5.197:7860","NVIDIA CMP 40HX": "127.0.0.1:7860"
     novelai_sampler: str = None  # 默认采样器,不写的话默认Euler a, Euler a系画人物可能比较好点, DDIM系, 如UniPC画出来的背景比较丰富, DPM系采样器一般速度较慢, 请你自己尝试(以上为个人感觉
     novelai_hr: bool = True  # 是否启动高清修复
     novelai_hr_scale: float = 1.5  # 高清修复放大比例
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     resp_data = await bot.get_login_info()
     bot_qq = resp_data["user_id"]
     url = await get_url()
     markdown = f'''
 <div style="background-color:rgba(255, 0, 0, 0.5);">&nbsp</div>
 # 我是群Ai绘画{nickname}
 ### 快速画图: 绘画 白发,红色眼睛
+### 请注意!!! 请用英文双引号把tags括起来 绘画"pink hair, red eye" 否则在带空格的情况下可能会意外解析
 <img width="300" src="https://q1.qlogo.cn/g?b=qq&nk={bot_qq}&s=640"/> 这是我主人QQ{superuser_list[0]}捏<img width="300" src="https://q1.qlogo.cn/g?b=qq&nk={superuser_list[0]}&s=640"/>
 <div style="background-color:rgba(255, 0, 0, 0.5);">&nbsp</div>
 ## 以下是功能捏 "#"井号是备注!请忽略它!😡
 ### 群管理功能  🥰
 发送 绘画设置 四个字查看本群绘画设置, 只有管理员和群主能更改设置
 <div style="background-color:rgba(12, 0, 0, 0.5);">&nbsp</div>
 ```text
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import re
 from ..extension.translation import translate
+from nonebot import logger
+from copy import deepcopy
 
 
-async def prepocess_tags(tags: list[str], translation=True):
-    tags: str = "".join([i+"," for i in tags if isinstance(i,str)])
-    # 去除CQ码
-    tags = re.sub("\[CQ[^\s]*?]", "", tags)
-    # 检测中文
-    taglist = tags.split(",")
-    if not translation:
-        return ','.join(taglist)
+async def trans(taglist):
+    tag_str = ",".join(taglist)
     tagzh = ""
     tags_ = ""
     for i in taglist:
-        if re.search('[\u4e00-\u9fa5]', tags):
+        if re.search('[\u4e00-\u9fa5]', tag_str):
             tagzh += f"{i},"
         else:
             tags_ += f"{i},"
     if tagzh:
         tags_en = await translate(tagzh, "en")
         if tags_en == tagzh:
             return ""
         else:
             tags_ += tags_en
     return tags_
+
+
+async def prepocess_tags(tags: list[str], translation=True, only_trans=False):
+    if only_trans:
+        trans_result = await trans(tags)
+        return trans_result
+    tags: str = "".join([i+" " for i in tags if isinstance(i,str)])
+    # 去除CQ码
+    tags = re.sub("\[CQ[^\s]*?]", "", tags)
+    # 检测中文
+    taglist = tags.split(",")
+    if not translation:
+        return ','.join(taglist)
+    tags_str = await trans(tags)
+    return tags_str
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.4.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.4.0"
+version = "0.4.0.1"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

