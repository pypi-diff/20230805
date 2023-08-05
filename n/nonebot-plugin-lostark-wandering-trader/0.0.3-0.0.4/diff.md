# Comparing `tmp/nonebot_plugin_lostark_wandering_trader-0.0.3.tar.gz` & `tmp/nonebot_plugin_lostark_wandering_trader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.3.tar", last modified: Wed Aug  2 07:29:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_lostark_wandering_trader-0.0.4.tar", last modified: Sat Aug  5 12:40:29 2023, max compression
```

## Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3.tar` & `nonebot_plugin_lostark_wandering_trader-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/
--rw-r--r--   0 gongmin    (501) staff       (20)     5203 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/PKG-INFO
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader/
--rw-r--r--   0 gongmin    (501) staff       (20)      216 2023-08-02 03:29:55.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader/config.py
--rw-r--r--   0 gongmin    (501) staff       (20)     7473 2023-08-02 07:03:50.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader/__init__.py
--rw-r--r--   0 gongmin    (501) staff       (20)     3531 2023-08-02 07:16:54.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/README.md
--rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-02 07:28:47.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/setup.py
--rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/setup.cfg
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/
--rw-r--r--   0 gongmin    (501) staff       (20)     5203 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)      434 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
--rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
--rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-02 07:29:05.000000 nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.002961 nonebot_plugin_lostark_wandering_trader-0.0.4/
+-rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 12:40:29.002827 nonebot_plugin_lostark_wandering_trader-0.0.4/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/README.md
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.001511 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/
+-rw-r--r--   0 gongmin    (501) staff       (20)    10132 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/__init__.py
+-rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/config.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.002537 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/
+-rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)      449 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      764 2023-08-05 12:37:32.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/pyproject.toml
+-rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-05 12:40:29.003014 nonebot_plugin_lostark_wandering_trader-0.0.4/setup.cfg
+-rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-05 12:37:42.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_lostark_wandering_trader
-Version: 0.0.3
+Version: 0.0.4
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description: 
@@ -87,14 +87,31 @@
         
         ### TRADER__TIME
         
         - 类型: `int`
         - 默认: `1`
         - 说明: 检测流浪商人位置结果间隔时间
         
+        ### TRADER__RARITY
+        
+        - 类型: `list`
+        - 默认值: `[]`
+        - 说明: 需要通告的卡牌的稀有度，如果不填或是空，则默认会将 Rare 稀有度包括 Rare 以上的卡牌都通告
+          - Rare : 蓝色
+          - Epic : 紫色
+          - Legendary : 橙色
+        
+        ### TRADER__SEND_TYPE
+        
+        - 类型: `list`
+        - 默认值: `[]`
+        - 说明: 需要通告的内容，如果不填或是空，则默认会将卡牌以及橙色的礼物都通告
+          - Card : 卡牌
+          - Rapport : 礼物
+        
         ### TRADER__SERVER_ID
         
         - 类型: `int`
         - 默认: `14`
         - 说明：服务器对应的id（参考如下）：
           - 先锋服务器（亚克拉西亚）: 1
           - 先锋服务器（先锋体验服）: 2
@@ -130,14 +147,15 @@
         配置文件示例（默认模板）
         
         ```dotenv
         TRADER__USER_IDS=[12345678,87654321]
         TRADER__GROUP_IDS=[12345678,87654321]
         TRADER__TIME=1
         TRADER__SERVER_ID=14
+        TRADER__RARITY=["Rare","Epic","Legendary"]
         ```
         
         ## 说明
         
         数据来源：https://www.emrpg.com
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot_plugin_lostark_wandering_trader Version:
-0.0.3 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.4 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
@@ -22,16 +22,23 @@
 éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### TRADER__USER_IDS -
 ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çQQå·ï¼éè¦æ¯å¥½åï¼ ### TRADER__GROUP_IDS
 - ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çç¾¤å·ï¼éè¦å¨ç¾¤éï¼ ### TRADER__TIME -
 ç±»å: `int` - é»è®¤: `1` - è¯´æ:
-æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__SERVER_ID - ç±»å:
-`int` - é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
+æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__RARITY - ç±»å: `list`
+- é»è®¤å¼: `[]` - è¯´æ:
+éè¦éåçå¡ççç¨æåº¦ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°
+Rare ç¨æåº¦åæ¬ Rare ä»¥ä¸çå¡çé½éå - Rare : èè² - Epic :
+ç´«è² - Legendary : æ©è² ### TRADER__SEND_TYPE - ç±»å: `list` - é»è®¤å¼:
+`[]` - è¯´æ:
+éè¦éåçåå®¹ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°å¡çä»¥åæ©è²çç¤¼ç©é½éå
+- Card : å¡ç - Rapport : ç¤¼ç© ### TRADER__SERVER_ID - ç±»å: `int` -
+é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
 åéæå¡å¨ï¼äºåæè¥¿äºï¼: 1 - åéæå¡å¨ï¼åéä½éªæï¼:
 2 - å¢ä½©æ©ï¼å¢ç¹å°ï¼: 3 - å¢ä½©æ©ï¼å®å¿è°·ï¼: 4 -
 å¢ä½©æ©ï¼å¦®å¨èï¼: 5 - å¢ä½©æ©ï¼å¡ä¸¹ï¼: 6 -
 å¢ä½©æ©ï¼å¸éå®ï¼: 7 - å¢ä½©æ©ï¼æ©å¯å¯ï¼: 12 -
 å¢ä½©æ©ï¼å¡å¡ï¼: 13 - å¢ä½©æ©ï¼è¾å¼æ ¼é·æ¯ï¼: 14 -
 å¢ä½©æ©ï¼çº³è¥¿å°¼å°ï¼: 15 - å¢ä½©æ©ï¼å¯è¨å°ï¼: 16 -
 å¢ä½©æ©ï¼æ´ææ´å°ï¼: 17 - å¢ä½©æ©ï¼åºåèµé¡¿ï¼: 19 -
@@ -41,11 +48,12 @@
 å¡æ°æ´æ¯ï¼å¯å ï¼: 29 - å¡æ°æ´æ¯ï¼å¡éï¼: 30 -
 æ®ç½ææ¸©ï¼ææåï¼: 31 - æ®ç½ææ¸©ï¼é¿å¸è±ä¿®å¾·ï¼: 32 -
 æ®ç½ææ¸©ï¼è¾ä¼¦ï¼: 33 - æ®ç½ææ¸©ï¼é¿è´¾å¨ï¼: 34 -
 æ®ç½ææ¸©ï¼è¨æ²ï¼: 35 - æ®ç½ææ¸©ï¼å¡é¨ï¼: 36 -
 æ®ç½ææ¸©ï¼é¿é»å°ï¼: 37 - æ®ç½ææ¸©ï¼é¸èä¹åï¼: 38
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv TRADER__USER_IDS=
 [12345678,87654321] TRADER__GROUP_IDS=[12345678,87654321] TRADER__TIME=1
-TRADER__SERVER_ID=14 ``` ## è¯´æ æ°æ®æ¥æºï¼https://www.emrpg.com
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8,<4.0 Description-Content-Type: text/markdown
+TRADER__SERVER_ID=14 TRADER__RARITY=["Rare","Epic","Legendary"] ``` ## è¯´æ
+æ°æ®æ¥æºï¼https://www.emrpg.com Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8,<4.0
+Description-Content-Type: text/markdown
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader/__init__.py` & `nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment
 from nonebot import on_keyword, require, get_bot, get_bots, get_driver
 from httpx import Response, AsyncClient
 import datetime
+import time
 from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     name="命运方舟流浪商人卡牌刷新提示",
     description="国服命运方舟流浪商人稀有史诗传说卡牌刷新提示",
     usage="nb plugin install nonebot_plugin_lostark_wandering_trader",
     type="application",
@@ -18,19 +19,28 @@
     supported_adapters={"~onebot.v11"},
 )
 
 require("nonebot_plugin_apscheduler")
 
 from nonebot_plugin_apscheduler import scheduler
 
-plugin_config = Config.parse_obj(get_driver().config).trader
-
+try:
+    plugin_config = Config.parse_obj(get_driver().config).trader.dict()
+except:
+    plugin_config = {
+        'user_ids': [],
+        'group_ids': [],
+        'time': 1,
+        'server_id': 6,
+        'rarity': [],
+    }
+    
 notice_data = []
 
-@scheduler.scheduled_job("cron", minute=f"*/{plugin_config.time}", id="check_trader")
+@scheduler.scheduled_job("cron", minute=f"*/{plugin_config.get('time')}", id="check_trader")
 async def check_trader():
     global notice_data
     bots = get_bots().values()
     if len(notice_data) == 0:
         for bot in bots:
             notice_data.append([])
     for index,bot in enumerate(bots):
@@ -40,52 +50,91 @@
 
         date = datetime.datetime.now().date().isoformat()
         time_start = datetime.datetime.strptime( date + ' ' + hour + ':30:00', '%Y-%m-%d %H:%M:%S')
         time_one = datetime.datetime.strptime( date + ' ' + hour + ':35:00', '%Y-%m-%d %H:%M:%S')
         time_two = datetime.datetime.strptime( date + ' ' + hour + ':55:00', '%Y-%m-%d %H:%M:%S')
 
         response = ''
-
+        
         if now < time_two and now > time_one:
             result = await get_detail(int(time_start.timestamp()))
             if len(result) != 0:
                 for item in result:
                     can_notice = True
                     for notice in notice_data[index]:
-                        nid = notice.get('id', '')
-                        id = item.get('id', '')
+                        nid = notice.get('locationId', '')
+                        id = item.get('locationId', '')
                         if nid == id:
                             can_notice = False
                     if can_notice:
                         card = item.get('_card', {})
+                        rapport = item.get('_rapport', {})
                         rarity = card.get('rarity', '')
-                        if rarity == 'Epic' or rarity == 'Legendary' or rarity == 'Rare':
-                            location = item.get('_location', {})
-                            lname = location.get('name', '')
+                        rarity_array = []
+                        send_type_array = []
+                        if len(plugin_config.get('send_type')) == 0:
+                            send_type_array = ['card', 'rapport']
+                        else:
+                            send_type_array = plugin_config.get('send_type')
+                        if len(plugin_config.get('rarity')) == 0:
+                            rarity_array = ['Epic', 'Legendary', 'Rare']
+                        else:
+                            rarity_array = plugin_config.get('rarity')
+                        confirm = False
+                        for rItem in rarity_array:
+                            if rItem == rarity and "card" in send_type_array:
+                                confirm = True
+                        location = item.get('_location', {})
+                        image = location.get('snapshot', '')
+                        lname = location.get('name', '')
+                        member = item.get('_member', {})
+                        username = member.get('username', '未知人士')
+                        if confirm:
                             cname = card.get('name', '')
-                            image = location.get('snapshot', '')
-                            response = lname + f' 出{cname}了！' + f'稀有度为{rarity}'
-                            for qq in plugin_config.user_ids:
+                            response = lname + f' 出{cname}了！' + f'稀有度为{rarity}' + f' 提报人: {username}'
+                            for qq in plugin_config.get('user_ids'):
                                 await bot.call_api('send_private_msg', **{
                                     'user_id': qq,
                                     'message': response
                                 })
+                            for group in plugin_config.get('group_ids'):
+                                await bot.call_api('send_group_msg', **{
+                                    'group_id': group,
+                                    'message': response
+                                })
+                            time.sleep(1)
+                        rapport_confirm = False
+                        if rapport.get('rarity') == 'Legendary' and "rapport" in send_type_array:
+                            rapport_confirm = True
+                        if rapport_confirm:
+                            rname = rapport.get('name', '')
+                            response = lname + f' 出{rname}了！' + '稀有度为传说' + f' 提报人: {username}'
+                            for qq in plugin_config.get('user_ids'):
                                 await bot.call_api('send_private_msg', **{
                                     'user_id': qq,
-                                    'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
+                                    'message': response
                                 })
-                            for group in plugin_config.group_ids:
+                            for group in plugin_config.get('group_ids'):
                                 await bot.call_api('send_group_msg', **{
                                     'group_id': group,
                                     'message': response
                                 })
+                            time.sleep(1)
+                        if confirm or rapport_confirm:
+                            for qq in plugin_config.get('user_ids'):
+                                await bot.call_api('send_private_msg', **{
+                                    'user_id': qq,
+                                    'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
+                                })
+                            for group in plugin_config.get('group_ids'):
                                 await bot.call_api('send_group_msg', **{
                                     'group_id': group,
                                     'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
                                 })
+                            time.sleep(1)
                 notice_data[index] = result
         else:
             notice_data[index] = []
             
 
 trader = on_keyword({"下一个商人"}, priority=1)
 
@@ -95,30 +144,38 @@
         'X-Ajax': '1',
         'Cookie': 'acw_tc=707c9fc716906220300653664e550e283e11113d450a6e9e21bb7af38e99ab; UBtd_671d_saltkey=l3nfa1If; UBtd_671d_lastvisit=1690618430; UBtd_671d_sid=w61IJF; UBtd_671d_lastact=1690623811%09plugin.php%09; UBtd_671d_sid=O3zbk8; UBtd_671d_lastact=1690799529%09plugin.php%09',
         'User-Agent': 'Apifox/1.0.0 (https://apifox.com)',
         'Accept': '*/*',
         'Host': 'www.emrpg.com',
         'Connection': 'keep-alive'
         }
-        res = await client.get(f"https://www.emrpg.com/plugin.php?displayAt={displayAt}&fromServer=lostarkcn&serverId={plugin_config.server_id}&uri=merchants/active&_pipes=withCard,withRapport,withLocation,withMember&id=tj_emrpg", headers=headers)
-        result = res.json().get('data' , [])
+        result = []
+        try:
+            res = await client.get(f"https://www.emrpg.com/plugin.php?displayAt={displayAt}&fromServer=lostarkcn&serverId={plugin_config.get('server_id')}&uri=merchants/active&_pipes=withCard,withRapport,withLocation,withMember&id=tj_emrpg", headers=headers)
+            result = res.json().get('data' , [])
+        except:
+            result = []
         return result
 
 async def get_data():
     async with AsyncClient() as client:
         headers = {
         'X-Ajax': '1',
         'Cookie': 'acw_tc=707c9fc716906220300653664e550e283e11113d450a6e9e21bb7af38e99ab; UBtd_671d_saltkey=l3nfa1If; UBtd_671d_lastvisit=1690618430; UBtd_671d_sid=Z6bM50; UBtd_671d_sendmail=1; UBtd_671d_lastact=1690622038%09plugin.php%09; UBtd_671d_saltkey=AMcqaqQh; UBtd_671d_lastvisit=1690616006; UBtd_671d_sid=PeEjTE; UBtd_671d_lastact=1690622255%09plugin.php%09; acw_tc=76b20f6b16906221102315601e4147a5e05cf53f9b496a18f9a8670e71ca6d',
         'User-Agent': 'Apifox/1.0.0 (https://apifox.com)',
         'Accept': '*/*',
         'Host': 'www.emrpg.com',
         'Connection': 'keep-alive'
         }
-        res = await client.get(f"https://www.emrpg.com/plugin.php?fromServer=lostarkcn&serverId={plugin_config.server_id}&uri=merchants/list&id=tj_emrpg", headers=headers)
-        result = res.json().get('data' , [])
+        result = []
+        try:
+            res = await client.get(f"https://www.emrpg.com/plugin.php?fromServer=lostarkcn&serverId={plugin_config.get('server_id')}&uri=merchants/list&id=tj_emrpg", headers=headers)
+            result = res.json().get('data' , [])
+        except:
+            result = []
         return result
 
 
 @trader.handle()
 async def _(matcher: Matcher, event: MessageEvent):
     now = datetime.datetime.now()
     hour = str(now.hour)
@@ -145,9 +202,7 @@
                 #     response = response + item.get('region', '未知地区') + '的' + item.get('name', '未知商人') + '\n'
                 # else:
                 #     response = response + item.get('region', '未知地区') + '的' + item.get('name', '未知商人')
             response = response + 'by: EmiyaGm'
         else:
             response = '暂无数据'
     await trader.finish(response)
-
-
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3/README.md` & `nonebot_plugin_lostark_wandering_trader-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,31 @@
 
 ### TRADER__TIME
 
 - 类型: `int`
 - 默认: `1`
 - 说明: 检测流浪商人位置结果间隔时间
 
+### TRADER__RARITY
+
+- 类型: `list`
+- 默认值: `[]`
+- 说明: 需要通告的卡牌的稀有度，如果不填或是空，则默认会将 Rare 稀有度包括 Rare 以上的卡牌都通告
+  - Rare : 蓝色
+  - Epic : 紫色
+  - Legendary : 橙色
+
+### TRADER__SEND_TYPE
+
+- 类型: `list`
+- 默认值: `[]`
+- 说明: 需要通告的内容，如果不填或是空，则默认会将卡牌以及橙色的礼物都通告
+  - Card : 卡牌
+  - Rapport : 礼物
+
 ### TRADER__SERVER_ID
 
 - 类型: `int`
 - 默认: `14`
 - 说明：服务器对应的id（参考如下）：
   - 先锋服务器（亚克拉西亚）: 1
   - 先锋服务器（先锋体验服）: 2
@@ -120,12 +137,13 @@
 配置文件示例（默认模板）
 
 ```dotenv
 TRADER__USER_IDS=[12345678,87654321]
 TRADER__GROUP_IDS=[12345678,87654321]
 TRADER__TIME=1
 TRADER__SERVER_ID=14
+TRADER__RARITY=["Rare","Epic","Legendary"]
 ```
 
 ## 说明
 
 数据来源：https://www.emrpg.com
```

#### html2text {}

```diff
@@ -16,16 +16,23 @@
 éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### TRADER__USER_IDS -
 ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çQQå·ï¼éè¦æ¯å¥½åï¼ ### TRADER__GROUP_IDS
 - ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çç¾¤å·ï¼éè¦å¨ç¾¤éï¼ ### TRADER__TIME -
 ç±»å: `int` - é»è®¤: `1` - è¯´æ:
-æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__SERVER_ID - ç±»å:
-`int` - é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
+æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__RARITY - ç±»å: `list`
+- é»è®¤å¼: `[]` - è¯´æ:
+éè¦éåçå¡ççç¨æåº¦ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°
+Rare ç¨æåº¦åæ¬ Rare ä»¥ä¸çå¡çé½éå - Rare : èè² - Epic :
+ç´«è² - Legendary : æ©è² ### TRADER__SEND_TYPE - ç±»å: `list` - é»è®¤å¼:
+`[]` - è¯´æ:
+éè¦éåçåå®¹ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°å¡çä»¥åæ©è²çç¤¼ç©é½éå
+- Card : å¡ç - Rapport : ç¤¼ç© ### TRADER__SERVER_ID - ç±»å: `int` -
+é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
 åéæå¡å¨ï¼äºåæè¥¿äºï¼: 1 - åéæå¡å¨ï¼åéä½éªæï¼:
 2 - å¢ä½©æ©ï¼å¢ç¹å°ï¼: 3 - å¢ä½©æ©ï¼å®å¿è°·ï¼: 4 -
 å¢ä½©æ©ï¼å¦®å¨èï¼: 5 - å¢ä½©æ©ï¼å¡ä¸¹ï¼: 6 -
 å¢ä½©æ©ï¼å¸éå®ï¼: 7 - å¢ä½©æ©ï¼æ©å¯å¯ï¼: 12 -
 å¢ä½©æ©ï¼å¡å¡ï¼: 13 - å¢ä½©æ©ï¼è¾å¼æ ¼é·æ¯ï¼: 14 -
 å¢ä½©æ©ï¼çº³è¥¿å°¼å°ï¼: 15 - å¢ä½©æ©ï¼å¯è¨å°ï¼: 16 -
 å¢ä½©æ©ï¼æ´ææ´å°ï¼: 17 - å¢ä½©æ©ï¼åºåèµé¡¿ï¼: 19 -
@@ -35,8 +42,9 @@
 å¡æ°æ´æ¯ï¼å¯å ï¼: 29 - å¡æ°æ´æ¯ï¼å¡éï¼: 30 -
 æ®ç½ææ¸©ï¼ææåï¼: 31 - æ®ç½ææ¸©ï¼é¿å¸è±ä¿®å¾·ï¼: 32 -
 æ®ç½ææ¸©ï¼è¾ä¼¦ï¼: 33 - æ®ç½ææ¸©ï¼é¿è´¾å¨ï¼: 34 -
 æ®ç½ææ¸©ï¼è¨æ²ï¼: 35 - æ®ç½ææ¸©ï¼å¡é¨ï¼: 36 -
 æ®ç½ææ¸©ï¼é¿é»å°ï¼: 37 - æ®ç½ææ¸©ï¼é¸èä¹åï¼: 38
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv TRADER__USER_IDS=
 [12345678,87654321] TRADER__GROUP_IDS=[12345678,87654321] TRADER__TIME=1
-TRADER__SERVER_ID=14 ``` ## è¯´æ æ°æ®æ¥æºï¼https://www.emrpg.com
+TRADER__SERVER_ID=14 TRADER__RARITY=["Rare","Epic","Legendary"] ``` ## è¯´æ
+æ°æ®æ¥æºï¼https://www.emrpg.com
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3/setup.py` & `nonebot_plugin_lostark_wandering_trader-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "NoneBot lostark cn wandering trader plugin"
 
 setuptools.setup(
     name="nonebot_plugin_lostark_wandering_trader",
-    version="0.0.3",
+    version="0.0.4",
     author="EmiyaGm",
     author_email="464723943@qq.com",
     description="NoneBot lostark cn wandering trader plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
     project_urls={
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.3/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-lostark-wandering-trader
-Version: 0.0.3
+Version: 0.0.4
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description: 
@@ -87,14 +87,31 @@
         
         ### TRADER__TIME
         
         - 类型: `int`
         - 默认: `1`
         - 说明: 检测流浪商人位置结果间隔时间
         
+        ### TRADER__RARITY
+        
+        - 类型: `list`
+        - 默认值: `[]`
+        - 说明: 需要通告的卡牌的稀有度，如果不填或是空，则默认会将 Rare 稀有度包括 Rare 以上的卡牌都通告
+          - Rare : 蓝色
+          - Epic : 紫色
+          - Legendary : 橙色
+        
+        ### TRADER__SEND_TYPE
+        
+        - 类型: `list`
+        - 默认值: `[]`
+        - 说明: 需要通告的内容，如果不填或是空，则默认会将卡牌以及橙色的礼物都通告
+          - Card : 卡牌
+          - Rapport : 礼物
+        
         ### TRADER__SERVER_ID
         
         - 类型: `int`
         - 默认: `14`
         - 说明：服务器对应的id（参考如下）：
           - 先锋服务器（亚克拉西亚）: 1
           - 先锋服务器（先锋体验服）: 2
@@ -130,14 +147,15 @@
         配置文件示例（默认模板）
         
         ```dotenv
         TRADER__USER_IDS=[12345678,87654321]
         TRADER__GROUP_IDS=[12345678,87654321]
         TRADER__TIME=1
         TRADER__SERVER_ID=14
+        TRADER__RARITY=["Rare","Epic","Legendary"]
         ```
         
         ## 说明
         
         数据来源：https://www.emrpg.com
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-lostark-wandering-trader Version:
-0.0.3 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.4 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
@@ -22,16 +22,23 @@
 éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### TRADER__USER_IDS -
 ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çQQå·ï¼éè¦æ¯å¥½åï¼ ### TRADER__GROUP_IDS
 - ç±»åï¼`list` - é»è®¤å¼ï¼`[]` -
 è¯´æï¼éè¦åééç¥çç¾¤å·ï¼éè¦å¨ç¾¤éï¼ ### TRADER__TIME -
 ç±»å: `int` - é»è®¤: `1` - è¯´æ:
-æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__SERVER_ID - ç±»å:
-`int` - é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
+æ£æµæµæµªåäººä½ç½®ç»æé´éæ¶é´ ### TRADER__RARITY - ç±»å: `list`
+- é»è®¤å¼: `[]` - è¯´æ:
+éè¦éåçå¡ççç¨æåº¦ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°
+Rare ç¨æåº¦åæ¬ Rare ä»¥ä¸çå¡çé½éå - Rare : èè² - Epic :
+ç´«è² - Legendary : æ©è² ### TRADER__SEND_TYPE - ç±»å: `list` - é»è®¤å¼:
+`[]` - è¯´æ:
+éè¦éåçåå®¹ï¼å¦æä¸å¡«ææ¯ç©ºï¼åé»è®¤ä¼å°å¡çä»¥åæ©è²çç¤¼ç©é½éå
+- Card : å¡ç - Rapport : ç¤¼ç© ### TRADER__SERVER_ID - ç±»å: `int` -
+é»è®¤: `14` - è¯´æï¼æå¡å¨å¯¹åºçidï¼åèå¦ä¸ï¼ï¼ -
 åéæå¡å¨ï¼äºåæè¥¿äºï¼: 1 - åéæå¡å¨ï¼åéä½éªæï¼:
 2 - å¢ä½©æ©ï¼å¢ç¹å°ï¼: 3 - å¢ä½©æ©ï¼å®å¿è°·ï¼: 4 -
 å¢ä½©æ©ï¼å¦®å¨èï¼: 5 - å¢ä½©æ©ï¼å¡ä¸¹ï¼: 6 -
 å¢ä½©æ©ï¼å¸éå®ï¼: 7 - å¢ä½©æ©ï¼æ©å¯å¯ï¼: 12 -
 å¢ä½©æ©ï¼å¡å¡ï¼: 13 - å¢ä½©æ©ï¼è¾å¼æ ¼é·æ¯ï¼: 14 -
 å¢ä½©æ©ï¼çº³è¥¿å°¼å°ï¼: 15 - å¢ä½©æ©ï¼å¯è¨å°ï¼: 16 -
 å¢ä½©æ©ï¼æ´ææ´å°ï¼: 17 - å¢ä½©æ©ï¼åºåèµé¡¿ï¼: 19 -
@@ -41,11 +48,12 @@
 å¡æ°æ´æ¯ï¼å¯å ï¼: 29 - å¡æ°æ´æ¯ï¼å¡éï¼: 30 -
 æ®ç½ææ¸©ï¼ææåï¼: 31 - æ®ç½ææ¸©ï¼é¿å¸è±ä¿®å¾·ï¼: 32 -
 æ®ç½ææ¸©ï¼è¾ä¼¦ï¼: 33 - æ®ç½ææ¸©ï¼é¿è´¾å¨ï¼: 34 -
 æ®ç½ææ¸©ï¼è¨æ²ï¼: 35 - æ®ç½ææ¸©ï¼å¡é¨ï¼: 36 -
 æ®ç½ææ¸©ï¼é¿é»å°ï¼: 37 - æ®ç½ææ¸©ï¼é¸èä¹åï¼: 38
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv TRADER__USER_IDS=
 [12345678,87654321] TRADER__GROUP_IDS=[12345678,87654321] TRADER__TIME=1
-TRADER__SERVER_ID=14 ``` ## è¯´æ æ°æ®æ¥æºï¼https://www.emrpg.com
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8,<4.0 Description-Content-Type: text/markdown
+TRADER__SERVER_ID=14 TRADER__RARITY=["Rare","Epic","Legendary"] ``` ## è¯´æ
+æ°æ®æ¥æºï¼https://www.emrpg.com Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8,<4.0
+Description-Content-Type: text/markdown
```

