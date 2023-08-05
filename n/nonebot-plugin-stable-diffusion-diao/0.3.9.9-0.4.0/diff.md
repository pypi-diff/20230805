# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.9.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.9.tar", last modified: Wed Aug  2 13:56:48 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.0.tar", last modified: Sat Aug  5 04:23:19 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9.tar` & `nonebot_plugin_stable_diffusion_diao-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.9/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    28626 2023-08-02 13:53:01.656227 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6144 2023-07-30 13:05:57.372381 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16512 2023-08-02 09:53:22.132707 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     7604 2023-08-02 03:51:33.221327 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    20867 2023-08-02 06:41:43.576286 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    47854 2023-08-02 11:02:49.349205 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      724 2023-07-31 04:15:37.158867 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      728 2023-08-02 13:56:48.145180 nonebot_plugin_stable_diffusion_diao-0.3.9.9/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.0/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    28728 2023-08-05 02:07:47.982325 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6142 2023-08-03 14:38:58.225454 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    17343 2023-08-04 09:13:48.463075 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    21031 2023-08-05 02:04:53.047052 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    11786 2023-08-05 02:25:43.200082 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2724 2023-08-04 05:01:28.104471 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    47852 2023-08-05 02:25:45.537023 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      724 2023-07-31 04:15:37.158867 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      726 2023-08-05 04:23:19.480361 nonebot_plugin_stable_diffusion_diao-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import time
 import re
 import random
 import json
 import os
 import ast
 
+
 from collections import deque
+from copy import deepcopy
 import aiohttp
 from aiohttp.client_exceptions import ClientConnectorError, ClientOSError
 from argparse import Namespace
 from asyncio import get_running_loop
 from nonebot import get_bot, on_shell_command
 import aiofiles
 import traceback
@@ -76,22 +78,19 @@
                            type=str, help="更换模型", dest="model_index")
 aidraw_parser.add_argument("-match_off","-match-off",
                            action="store_true", help="关闭自动匹配", dest="match")
 aidraw_parser.add_argument("-sr_on", "-sr-on", "-sr",
                            action="store_true", help="图片生产后再次超分", dest="sr")
 aidraw_parser.add_argument("-td", "--tiled-diffusion",
                            action="store_true", help="使用tiled-diffusion来生成图片", dest="td")
-# aidraw_parser.add_argument("-hr_e",
-#                            action=float, help="重绘幅度", dest="hr_strength")
-# aidraw_parser.add_argument("-acs", "--activate_custom_scripts",
-#                            action=int, help="启动自定义脚本生图", dest="custom_scripts")
-# aidraw_parser.add_argument("-xyz",
-#                            action=str, help="xyz生图", dest="xyz_plot")
-# aidraw_parser.add_argument("-sc", "--script", "--scripts",
-#                            action=int, help="脚本生图", dest="scripts")
+aidraw_parser.add_argument("-acs", "--activate_custom_scripts",
+                           type=int, help="启动自定义脚本生图", dest="custom_scripts")
+aidraw_parser.add_argument("-xyz", type=str, help="xyz生图", dest="xyz_plot")
+aidraw_parser.add_argument("-sc", "--script", "--scripts",
+                           type=int, help="脚本生图", dest="scripts")
 # aidraw_parser.add_argument("-ef", "--eye_fix",
 #                            action="store_true", help="使用ad插件修复脸部", dest="eye_fix")
 
 
 async def get_message_at(data: str) -> int:
     '''
     获取at列表
@@ -138,18 +137,22 @@
     global bot_id
     bot_id = bot.self_id
     # 判断是否禁用，若没禁用，进入处理流程
     if await config.get_value(group_id, "on"):
         message = ""
         if config.novelai_daylimit and not await SUPERUSER(bot, event):
             left = await count(user_id, 1)
-            if left == -1:
+            if left < 0:
                 await aidraw.finish(f"今天你的次数不够了哦")
             else:
-                message = message + f"，今天你还能够生成{left}张"
+                if config.novelai_daylimit_type == 2:
+                    message_ = f"今天你还能画{left}秒"
+                else:
+                    message_ = f"，今天你还能够生成{left}张"
+                message += message_
         # 判断cd
         nowtime = time.time()
         if isinstance(event, GroupMessageEvent):
             deltatime_ = nowtime - cd.get(group_id, 0)
             gcd = int(config.novelai_group_cd)
             if deltatime_ < gcd:
                 await aidraw.finish(f"本群共享剩余CD为{gcd - int(deltatime_)}s")
@@ -213,14 +216,15 @@
             await fifo.load_balance_init()
         tags = fifo.tags
         if isinstance(tags, str):
             tags_list = tags_to_list(tags)
         else:
             tags_list = tags
         org_tag_list = tags_list
+        org_list = deepcopy(tags_list)
         new_tags_list = []
         if args.match or not config.auto_match:
             pass
         elif redis_client:
             r2 = redis_client[1]
             try:
                 tag = ""
@@ -266,21 +270,22 @@
                                 model_info_ += f"自动找到的嵌入式模型: {emb}, \n"
                                 model_info += model_info_
                                 logger.info(model_info_)
                                 tags_list.pop(org_tag_list.index(tag))
                                 break
                     if len(new_tags_list) >2:
                         new_tags_list = []
-                        tags_list = org_tag_list
+                        tags_list = org_list
                         fifo.extra_info += "自动匹配到的模型过多\n已关闭自动匹配功能"
                         model_info = ""
                         raise RuntimeError("匹配到很多lora")
                     fifo.extra_info += f"{model_info}\n"
             except Exception as e:
                 logger.warning(str(traceback.print_exc()))
+                new_tags_list = []
                 logger.warning(f"tag自动匹配失效,出现问题的: {tag}\n或者是prompt里自动匹配到的模型过多")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
             tags_list: str = await prepocess_tags(tags_list)
         except Exception as e:
             logger.debug(str(e))
             await aidraw.finish("tag处理失败!可能是翻译API错误, 请稍后重试, 或者使用英文重试")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     return user_session[user_id]
 
 
 @chatgpt.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     if config.novelai_daylimit and not await SUPERUSER(bot, event):
         left = await count(str(event.user_id), 1)
-        if left == -1:
+        if left < 0:
             await chatgpt.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     user_msg = msg.extract_plain_text().strip()
     to_openai = user_msg + "prompt"
     prompt = await get_user_session(event.get_session_id()).main(to_openai)
 
     await risk_control(
                     bot,
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1266,15 +1266,15 @@
         else:
             get_info = await bot.get_group_member_info(group_id=event.group_id, user_id=user_id)
             user_name = get_info["nickname"]
     else:
         user_name = message
     if config.novelai_daylimit and not await SUPERUSER(bot, event):
         left = await count(str(event.user_id), 1)
-        if left == -1:
+        if left < 0:
             await today_girl.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     img_url = None
     random_int_str = str(random.randint(0, 65535))
 
     at_id = await get_message_at(event.json())
     if at_id:
         img_url = f"https://q1.qlogo.cn/g?b=qq&nk={at_id}&s=640"
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 import ast
 
 import aiohttp
 from nonebot import get_driver
 from nonebot.log import logger
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageEvent, PrivateMessageEvent
+from nonebot.permission import SUPERUSER
 from nonebot import logger
 from datetime import datetime
-from ..config import config, redis_client
+from ..config import config, redis_client, superusers
 from ..utils import png2jpg, unload_and_reload, get_generate_info
 from ..utils.data import shapemap
 from ..utils.load_balance import sd_LoadBalance
+from ..extension.daylimit import count
 
 
 class AIDRAW_BASE:
     max_resolution: int = 16
     sampler: str
 
     def __init__(
@@ -45,14 +47,15 @@
         hiresfix_scale: float = None,
         event: MessageEvent = None,
         sr: bool = False,
         model_index: str = None,
         custom_scripts: int = None,
         scripts: int = None,
         td = None,
+        xyz_plot = None,
         **kwargs,
     ):
         """
         AI绘画的核心部分,将与服务器通信的过程包装起来,并方便扩展服务器类型
 
         :user_id: 用户id,必须
         :group_id: 群聊id,如果是私聊则应置为0,必须
@@ -137,14 +140,15 @@
         self.audit_info = ""
         self.sr = sr or config.novelai_SuperRes_generate
         self.model_index = model_index
         self.is_random_model = False
         self.custom_scripts = custom_scripts
         self.scripts = scripts
         self.td = td
+        self.xyz_plot = xyz_plot
         
         # 数值合法检查
         if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
         if self.noise < 0 or self.noise > 1:
@@ -304,14 +308,24 @@
                         backend_info["gpu"] = backend_dict
                     else:
                         backend_dict = {}
                         backend_info["gpu"] = {}
                         for i in list(config.novelai_backend_url_dict.keys()):
                             backend_dict[i] = 1
                             backend_info["gpu"] = backend_dict
+                    if config.novelai_daylimit and self.user_id not in superusers and config.novelai_daylimit_type == 2:
+                        if backend_info.get("spend_time"):
+                            counting = backend_info.get("spend_time")
+                        else:
+                            counting = {}
+                        org_spend_time = counting.get(self.user_id, 0)
+                        user_spend_time = org_spend_time + int(spend_time)
+                        counting[self.user_id] = user_spend_time
+                        backend_info["spend_time"] = counting
+                    self.extra_info += f"\n耗时{spend_time:.2f}秒\n"
                     r.set(day, str(backend_info))
             else:
                 filename = "data/novelai/day_limit_data.json"
                 if os.path.exists(filename):
                     async with aiofiles.open(filename, "r") as f:
                         json_ = await f.read()
                         json_ = json.loads(json_)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ..utils import get_generate_info
 from nonebot import logger
 from copy import deepcopy
 import json, aiofiles
 import asyncio
 import traceback
 import random
+import ast
 
 
 header = {
                 "content-type": "application/json",
                 "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",
 }
 
@@ -84,33 +85,52 @@
             from ..extension.sd_extra_api_func import sd
             model_dict = await sd(self.backend_index or config.backend_site_list.index(self.backend_site), True)
             self.model_index = self.model_index if self.model_index.isdigit() else await self.get_model_index(self.model_index, model_dict)
             if self.is_random_model:
                 from ..extension.sd_extra_api_func import sd
                 self.model_index = random.randint(1, len(list(model_dict.keys())))
             self.model = model_dict[int(self.model_index)]
-            parameters.update({"override_settings": {"sd_model_checkpoint": self.model}, 
-                               "override_settings_restore_afterwards": "true"}
-                            )
-
+            parameters.update(
+                {"override_settings": {"sd_model_checkpoint": self.model}, 
+                "override_settings_restore_afterwards": "true"}
+            )
         if self.img2img:
             if self.control_net["control_net"] and config.novelai_hr:
                 parameters.update(self.novelai_hr_payload)
             parameters.update({
                 "init_images": ["data:image/jpeg;base64,"+self.image],
                 "denoising_strength": self.strength,
             }
             ) 
         else:
             if config.novelai_hr and self.disable_hr is False:
                 parameters.update(self.novelai_hr_payload)
             else:
                 self.hiresfix = False
+        if self.xyz_plot:
+            input_str_replaced = self.xyz_plot.replace('""', 'None')
+            try:
+                xyz_list = ast.literal_eval('[' + input_str_replaced + ']')
+            except (SyntaxError, ValueError):
+                xyz_list = []
+            xyz_list = ["" if item is None else item for item in xyz_list]
+            parameters.update({"script_name": "x/y/z plot", "script_args": xyz_list})
+            # if "_" and "," in self.xyz_plot:
+            #     result = [config.scripts[0]["args"][i:i+3] for i in range(0, len(config.scripts[0]["args"]), 3)]
+            #     axes = self.xyz_plot.split(",")
+            #     args = axes.split("_")
+            #     result[0][0] = args[0]
+            #     args[0] = 
+
         if self.td or config.tiled_diffusion:
-            parameters.update({"alwayson_scripts": config.custom_scripts})
+            parameters.update({"alwayson_scripts": config.custom_scripts[0]})
+        if self.custom_scripts is not None:
+            parameters.update({"alwayson_scripts": config.custom_scripts[self.custom_scripts]})
+        if self.scripts is not None:
+            parameters.update({"script_name": config.scripts[self.scripts]["name"], "script_args": config.scripts[self.scripts]["args"]})
         if self.control_net["control_net"] == True and config.novelai_hr:
             if config.hr_off_when_cn:
                 parameters.update({"enable_hr": "false"})
             else:
                 org_scale = parameters["hr_scale"]
                 parameters.update({"hr_scale": org_scale * 0.75}) # control较吃显存, 高清修复倍率恢复为1.5
             del parameters["init_images"]
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 jsonpath = Path("data/novelai/config.json").resolve()
 lb_jsonpath = Path("data/novelai/load_balance.json").resolve()
 redis_client = None
 backend_emb, backend_lora = None, None
 
 nickname = list(get_driver().config.nickname)[0] if len(
     get_driver().config.nickname) else "nonebot-plugin-stable-diffusion-diao"
+superusers = list(get_driver().config.superusers)
 
 
 class Config(BaseSettings):
     # 服务器设置
     lb_jsonpath
     novelai_steps: int = None  # 默认步数
     novelai_command_start: set = {"绘画", "咏唱", "召唤", "约稿", "aidraw", "画", "绘图", "AI绘图", "ai绘图"}
@@ -36,14 +37,15 @@
     novelai_site: str = "la.iamdiao.lol:5938"
     # 后台设置
     novelai_save: int = 2  # 是否保存图片至本地,0为不保存，1保存，2同时保存追踪信息
     novelai_save_png: bool = False  # 是否保存为PNG格式
     novelai_paid: int = 3  # 0为禁用付费模式，1为点数制，2为不限制
     novelai_pure: bool = True  # 是否启用简洁返回模式（只返回图片，不返回tag等数据）
     novelai_limit: bool = False  # 是否开启限速
+    novelai_daylimit_type = 2  # 限制模式, 1为张数限制, 2为画图所用时间计算
     novelai_daylimit: int = 24  # 每日次数限制，0为禁用
     novelai_h: int = 2  # 是否允许H, 0为不允许, 1为删除屏蔽词, 2允许
     novelai_htype: int = 3  # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
     novelai_antireport: bool = True  # 玄学选项。开启后，合并消息内发送者将会显示为调用指令的人而不是bot
     novelai_max: int = 3  # 每次能够生成的最大数量
     # 允许生成的图片最大分辨率，对应(值)^2.默认为1024（即1024*1024）。如果服务器比较寄，建议改成640（640*640）或者根据能够承受的情况修改。naifu和novelai会分别限制最大长宽为1024
     # 可运行更改的设置
@@ -86,57 +88,60 @@
     个人使用第一种方法post显卡占用率反复横跳TAT 
     tips:使用/controlnet/txt2img会提示warning: consider using the '/sdapi/v1/txt2img' route with the 'alwayson_scripts' json property instead''' 
     novelai_size_org: int = 640  # 最大分辨率
     if novelai_hr:
         novelai_size: int = novelai_size_org
     else:
         novelai_size: int = novelai_size_org * novelai_hr_payload["hr_scale"]
-    custom_scripts = {  # 自定义脚本此功能就可以使用webui上才能调用的插件, 需要自己去抓包
-    "Tiled Diffusion": {
-        "args": [True, "MultiDiffusion", False, True, 1024, 1024, 96, 96, 48, 1, "None", 2, False, 10, 1, []]
-    },
-    "Tiled VAE": {
-        "args": [True, 1536, 96, False, True, True]
-    },
-    "ADetailer": {
-        "args": [
-        True, 
+    custom_scripts = [{
+        "Tiled Diffusion": {
+            "args": [True, "MultiDiffusion", False, True, 1024, 1024, 96, 96, 48, 1, "None", 2, False, 10, 1, []]}
+        ,
+        "Tiled VAE": {
+            "args": [True, 1536, 96, False, True, True]
+        }
+        },
         {
-    "ad_model": "mediapipe_face_mesh_eyes_only",
-    "ad_prompt": "",
-    "ad_negative_prompt": "",
-    "ad_confidence": 0.1,
-    "ad_mask_min_ratio": 0,
-    "ad_mask_max_ratio": 1,
-    "ad_x_offset": 0,
-    "ad_y_offset": 0,
-    "ad_dilate_erode": 4,
-    "ad_mask_merge_invert": "None",
-    "ad_mask_blur": 4,
-    "ad_denoising_strength": 0.4,
-    "ad_inpaint_only_masked": True,
-    "ad_inpaint_only_masked_padding": 32,
-    "ad_use_inpaint_width_height": False,
-    "ad_inpaint_width": 512,
-    "ad_inpaint_height": 512,
-    "ad_use_steps": False,
-    "ad_steps": 28,
-    "ad_use_cfg_scale": False,
-    "ad_cfg_scale": 7,
-    "ad_use_sampler": False,
-    "ad_sampler": "Euler a",
-    "ad_use_noise_multiplier": False,
-    "ad_noise_multiplier": 1,
-    "ad_use_clip_skip": False,
-    "ad_clip_skip": 1,
-    "ad_restore_face": False
-                }
-            ]
+        "ADetailer": {
+            "args": [
+            True, 
+            {
+        "ad_model": "mediapipe_face_mesh_eyes_only",
+        "ad_prompt": "",
+        "ad_negative_prompt": "",
+        "ad_confidence": 0.1,
+        "ad_mask_min_ratio": 0,
+        "ad_mask_max_ratio": 1,
+        "ad_x_offset": 0,
+        "ad_y_offset": 0,
+        "ad_dilate_erode": 4,
+        "ad_mask_merge_invert": "None",
+        "ad_mask_blur": 4,
+        "ad_denoising_strength": 0.4,
+        "ad_inpaint_only_masked": True,
+        "ad_inpaint_only_masked_padding": 32,
+        "ad_use_inpaint_width_height": False,
+        "ad_inpaint_width": 512,
+        "ad_inpaint_height": 512,
+        "ad_use_steps": False,
+        "ad_steps": 28,
+        "ad_use_cfg_scale": False,
+        "ad_cfg_scale": 7,
+        "ad_use_sampler": False,
+        "ad_sampler": "Euler a",
+        "ad_use_noise_multiplier": False,
+        "ad_noise_multiplier": 1,
+        "ad_use_clip_skip": False,
+        "ad_clip_skip": 1,
+        "ad_restore_face": False
+                    }
+                ]
+            }
         }
-    }
+    ]
     scripts = [{"name": "x/y/z plot", "args": [9, "", ["DDIM", "Euler a", "Euler"], 0, "", "", 0, "", ""]}]
     novelai_ControlNet_payload: list = [
         {
             "alwayson_scripts": {
             "controlnet": {
             "args": [
                 {
@@ -189,15 +194,14 @@
     is_redis_enable = True  # 是否启动redis, 启动redis以获得更多功能
     auto_match = True  # 是否自动匹配
     hr_off_when_cn = True  # 使用controlnet功能的时候关闭高清修复
     backend_name_list = []
     backend_site_list = []
     only_super_user = True  # 只有超级用户才能永久更换模型, 雕雕没有小号来测试了, 悲
     tiled_diffusion = False  # 使用tiled-diffusion来生成图片
-    enable_scripts = False  # 是否启动custom_scripts中设置的自定义脚本
     save_img = True  # 是否保存图片(API侧)
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files 12% similar despite different names*

```diff
@@ -125,14 +125,22 @@
 预设maid,red_eye,white_hair -n "女仆" -u "负面提示词"  # 添加名为女仆的预设正面提示词为"maid,red_eye,white_hair"
 预设 -f "女仆"  # 查找名为女仆的预设
 预设 -d "女仆"  # 删除名为女仆的预设
 # 绘图女仆  插件检测到 "女仆" 即自动等于  绘图maid,red_eye,white_hair
 释放显存0
 # 字面含义, 为1号后端释放显存并且重载模型
 ```
+```
+随机出图
+# 随机一个模型画一张图,也可以 随机出图miku来指定prompt
+刷新模型
+# 刷新所有后端的lora和大模型
+终止生成1
+终止指定后端的生成任务
+```
 # 绘画功能详解 🖼️
 ## 基础使用方法 😊
 <div style="background-color:rgba(12, 0, 0, 0.5);">&nbsp</div>
 ```text
 基础使用方法, 使用.aidraw开头
 [{config.novelai_command_start}]也是可以的
 带上图片即可图生图, 带上 -cn 参数启动controlnet以图生图功能
@@ -249,14 +257,27 @@
 -hr 1.5
 # 绘画 -hr 1.5
 设置高清修复倍率为1.5
 ```
 ```text
 本张图片绘图完成后进行再次超分
 -sr
+使用 Tiled Diffusion 进行绘图, 降低显存使用, 已经低分辨率出大图
+-td
+```
+```
+绘制xyz表格
+-xyz 请严格按照以下格式
+绘画reimu -xyz '9, "", ("DDIM", "Euler a", "Euler"), 4, "8, 12, 20", "", 0, "", ""' -sd 1 
+分为三段, 分别为xyz轴, 每条轴3个参数
+第一位为数字, 为脚本索引(请去webui看, 或者使用获取脚本命令来查看)0为不使用本条轴
+第二位为字符串, 具体如何使用请查看webui, 例如步数, prompt等是手动填写参数, 故填写第二个参数, 例如步数
+第三位为元组, 当此项参数为可以由webui自动填写的时候填写, 例如采样器
+以上命令解释为
+绘画 x轴为采样器(第一位为9)轴, y轴为步数(第一位为4)轴的xyz图标, 不使用z轴(第一位为0)
 ```
 ### 最后, 送你一个示例
 <div style="background-color:rgba(255, 0, 0, 0.5);">&nbsp</div>
 ```text
 绘画 plaid_skirt,looking back ，bare shoulders -t 20 -sd 0 -sp UniPC -c 8 -b 3 -u nsfw
 ```
 <table><tr><td bgcolor=pink>画3张使用UniPC采样器, 步数20步, 服从度7, 不希望出现nsfw(不适宜内容)的图, 使用1号后端进行工作</td></tr></table>
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import json
 from ..config import config, redis_client
 import aiofiles
 import ast
 from datetime import datetime
-
+from nonebot import logger
 
 
 async def count(user: str, num) -> int:
+    mutil = 1 if config.novelai_daylimit_type == 1 else 20
     current_date = datetime.now().date()
     day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
     json_data = {"date": day, "count": {}}
     gpu = {}
     for backend in config.backend_name_list:
         gpu[backend] = 0
     json_data["gpu"] = gpu
@@ -19,23 +20,35 @@
         r = redis_client[2]
         if r.exists(day):
             json_data = r.get(day)
             json_data = json_data.decode("utf-8")
             json_data = ast.literal_eval(json_data)
         else:
             r.set(day, str(json_data))
+        if config.novelai_daylimit_type == 2:
+            if json_data.get("spend_time"):
+                spend_time_ditc = json_data.get("spend_time")
+            else:
+                spend_time_ditc = {}
+            total_spend_time = spend_time_ditc.get(user, 0)
+            if total_spend_time > config.novelai_daylimit * mutil:
+                return -1
         data = json_data["count"]
         count: int = data.get(user, 0) + num
-        if count > config.novelai_daylimit:
-            return -1
+        if config.novelai_daylimit_type == 1:
+            if count > config.novelai_daylimit:
+                return -1
         else:
             data[user] = count
             json_data["count"] = data
             r.set(day, str(json_data))
-            return config.novelai_daylimit-count
+            if config.novelai_daylimit_type == 1:
+                return config.novelai_daylimit - count
+            else:
+                return config.novelai_daylimit * mutil - total_spend_time
     else:
         filename = "data/novelai/day_limit_data.json"
         
         async def save_data(data):
             async with aiofiles.open(filename, "w") as file:
                 await file.write(json.dumps(data))
 
@@ -54,8 +67,8 @@
         count: int = data.get(user, 0) + num
         if count > config.novelai_daylimit:
             return -1
         else:
             data[user] = count
             json_data["count"] = data
             await save_data(json_data)
-            return config.novelai_daylimit-count
+            return config.novelai_daylimit * mutil - count
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,15 @@
     pass
 
 
 @control_net.got("net", "你的图图呢？")
 async def _(event: MessageEvent, bot: Bot, tag: str = ArgPlainText("tag"), msg: Message = Arg("net")):
     if config.novelai_daylimit and not await SUPERUSER(bot, event):
         left = await count(str(event.user_id), 2)
-        if left == -1:
+        if left < 0:
             await control_net.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     await func_init(event)
     start = time.time()
     tags_en = None
     reply= event.reply
     await bot.send(event=event, message=f"control_net以图生图中")
     if msg[0].type == "image":
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.4.0/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.9/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.9"
+version = "0.4.0"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

