# Comparing `tmp/hikari_core-0.9.0.6.tar.gz` & `tmp/hikari_core-0.9.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.9.0.6.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.7.tar", max compression
```

## Comparing `hikari_core-0.9.0.6.tar` & `hikari_core-0.9.0.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     5180 2023-07-28 09:08:18.103258 hikari_core-0.9.0.6/hikari_core/__init__.py
--rw-r--r--   0        0        0    13284 2023-07-28 09:48:16.899560 hikari_core-0.9.0.6/hikari_core/analyze.py
--rw-r--r--   0        0        0     3861 2023-07-28 09:35:38.013387 hikari_core-0.9.0.6/hikari_core/command_select.py
--rw-r--r--   0        0        0     1800 2023-07-28 08:57:45.614961 hikari_core-0.9.0.6/hikari_core/config.py
--rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.6/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.6/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.6/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.6/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.6/hikari_core/game/help.py
--rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.6/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.6/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.6/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.6/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.6/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.6/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.6/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.6/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.6/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.6/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.6/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.6/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.6/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.6/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.6/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.6/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0    11651 2023-07-28 09:51:36.928109 hikari_core-0.9.0.6/hikari_core/moudle/wws_real_game.py
--rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.6/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.6/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.6/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.6/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-07-28 09:52:33.662113 hikari_core-0.9.0.6/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     3783 2023-07-28 09:52:33.969133 hikari_core-0.9.0.6/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5166 2023-07-28 09:52:34.018963 hikari_core-0.9.0.6/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-07-28 09:52:34.035610 hikari_core-0.9.0.6/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7310 2023-07-28 09:52:34.343749 hikari_core-0.9.0.6/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-07-28 09:52:34.381775 hikari_core-0.9.0.6/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-07-28 09:52:34.662703 hikari_core-0.9.0.6/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28156 2023-07-28 09:52:34.709757 hikari_core-0.9.0.6/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    28083 2023-07-28 09:52:34.738553 hikari_core-0.9.0.6/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-07-28 09:52:34.775878 hikari_core-0.9.0.6/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-07-28 09:52:34.811824 hikari_core-0.9.0.6/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21441 2023-07-28 09:52:34.873514 hikari_core-0.9.0.6/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-07-28 09:52:34.910943 hikari_core-0.9.0.6/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-07-28 09:52:34.940249 hikari_core-0.9.0.6/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.6/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.6/LICENSE
--rw-r--r--   0        0        0     1572 2023-07-28 09:52:51.769766 hikari_core-0.9.0.6/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.6/README.md
--rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.6/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5180 2023-07-28 09:08:18.103258 hikari_core-0.9.0.7/hikari_core/__init__.py
+-rw-r--r--   0        0        0    13320 2023-08-05 20:09:19.643906 hikari_core-0.9.0.7/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3976 2023-07-28 12:15:42.694292 hikari_core-0.9.0.7/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1800 2023-07-31 09:41:01.730296 hikari_core-0.9.0.7/hikari_core/config.py
+-rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.7/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.7/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.7/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.7/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.7/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.7/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.7/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.7/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.7/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.7/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.7/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.7/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.7/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.7/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.7/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.7/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.7/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.7/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.7/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.7/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.7/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0    11651 2023-07-28 09:51:36.928109 hikari_core-0.9.0.7/hikari_core/moudle/wws_real_game.py
+-rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.7/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     3552 2023-07-28 12:15:00.805096 hikari_core-0.9.0.7/hikari_core/moudle/wws_recents.py
+-rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.7/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.7/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.7/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-08-05 20:12:34.736007 hikari_core-0.9.0.7/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-08-05 20:12:34.949453 hikari_core-0.9.0.7/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-08-05 20:12:34.968142 hikari_core-0.9.0.7/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-08-05 20:12:34.983769 hikari_core-0.9.0.7/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-08-05 20:12:35.002399 hikari_core-0.9.0.7/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-08-05 20:12:35.020594 hikari_core-0.9.0.7/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-08-05 20:12:35.038336 hikari_core-0.9.0.7/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-08-05 20:12:35.057062 hikari_core-0.9.0.7/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28083 2023-08-05 20:12:35.076435 hikari_core-0.9.0.7/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-08-05 20:12:35.095167 hikari_core-0.9.0.7/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-08-05 20:12:35.116875 hikari_core-0.9.0.7/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-08-05 20:12:35.144355 hikari_core-0.9.0.7/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-08-05 20:12:35.162258 hikari_core-0.9.0.7/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-08-05 20:12:35.181909 hikari_core-0.9.0.7/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.7/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.7/LICENSE
+-rw-r--r--   0        0        0     1572 2023-08-05 20:13:36.642446 hikari_core-0.9.0.7/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.7/README.md
+-rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.7/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.7/PKG-INFO
```

### Comparing `hikari_core-0.9.0.6/hikari_core/__init__.py` & `hikari_core-0.9.0.7/hikari_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/analyze.py` & `hikari_core-0.9.0.7/hikari_core/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 return hikari.error('请发送wws help查看帮助')
             if random.randint(1, 1000) == 1:
                 return hikari.error('一天到晚惦记你那b水表，就nm离谱')
             hikari.Input.Command_Text = html.unescape(str(hikari.Input.Command_Text)).strip()
             hikari = await extract_with_special_name(hikari)
             hikari.Function, hikari.Input.Command_List = await select_command(hikari.Input.Command_List)
             if hikari.Input.AccountName:
-                hikari.Input.Command_List.append(hikari.Input.AccountName)
+                hikari.Input.Command_List.insert(len(hikari.Input.Command_List) - 1, hikari.Input.AccountName)
             hikari = await extract_with_me_or_at(hikari)
             hikari = await extract_with_function(hikari)
         return hikari
     except Exception:
         logger.error(traceback.format_exc())
         return hikari.error('解析指令时发生错误，请确认输入参数无误')
```

### Comparing `hikari_core-0.9.0.6/hikari_core/command_select.py` & `hikari_core-0.9.0.7/hikari_core/command_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .moudle.publicAPI import get_ship_name
 from .moudle.wws_bind import change_BindInfo, delete_BindInfo, get_BindInfo, set_BindInfo, set_special_BindInfo
 
 # from .moudle.wws_clan import get_ClanInfo
 from .moudle.wws_info import get_AccountInfo
 from .moudle.wws_real_game import add_listen_list, delete_listen_list, get_diff_ship, get_listen_list
 from .moudle.wws_recent import get_RecentInfo
+from .moudle.wws_recents import get_RecentsInfo
 
 # from .moudle.wws_record import get_record
 from .moudle.wws_ship_info import get_ShipInfo
 from .moudle.wws_ship_recent import get_ShipRecent
 from .moudle.wws_shiprank import get_ShipRank
 
 
@@ -38,14 +39,15 @@
 first_command_list = [  # 同指令中越长的匹配词越靠前
     command(('切换绑定', '更换绑定', '更改绑定'), change_BindInfo),
     command(('查询绑定', '绑定查询', '绑定列表', '查绑定'), get_BindInfo),
     command(('删除绑定',), delete_BindInfo),
     command(('特殊绑定',), set_special_BindInfo),
     command(('ship.rank', 'rank'), get_ShipRank),
     command(('bind', '绑定', 'set'), set_BindInfo),
+    command(('recents', '单场近期'), None, get_RecentsInfo),
     command(('recent', '近期'), None, get_RecentInfo),
     command(('ship', '单船'), None, get_ShipInfo),
     # command(("record", "历史记录"), None, get_record),
     # command(("clan", "军团", "公会", "工会"), None, get_ClanInfo),
     # command(("随机表情包",), get_Random_Ocr_Pic),
     command(('roll', '随机'), roll_ship),
     command(('sx', '扫雪'), get_sx_info),
```

### Comparing `hikari_core-0.9.0.6/hikari_core/config.py` & `hikari_core-0.9.0.7/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/data_source.py` & `hikari_core-0.9.0.7/hikari_core/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/game/ban_search.py` & `hikari_core-0.9.0.7/hikari_core/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/game/box_check.py` & `hikari_core-0.9.0.7/hikari_core/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/game/help.py` & `hikari_core-0.9.0.7/hikari_core/game/help.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/game/roll.py` & `hikari_core-0.9.0.7/hikari_core/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/game/sx.py` & `hikari_core-0.9.0.7/hikari_core/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0.7/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0.7/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0.7/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0.7/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0.7/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0.7/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0.7/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/model.py` & `hikari_core-0.9.0.7/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0.7/hikari_core/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_bind.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_real_game.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_real_game.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_ship_info.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_ship_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_ship_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/moudle/wws_shiprank.py` & `hikari_core-0.9.0.7/hikari_core/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/bind-list.html` & `hikari_core-0.9.0.7/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0.7/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0.7/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0.7/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/hikari_core/utils.py` & `hikari_core-0.9.0.7/hikari_core/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/LICENSE` & `hikari_core-0.9.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.6/pyproject.toml` & `hikari_core-0.9.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.9.0.6"
+version = "0.9.0.7"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
```

### Comparing `hikari_core-0.9.0.6/setup.py` & `hikari_core-0.9.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.9.0.6',
+    'version': '0.9.0.7',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-0.9.0.6/PKG-INFO` & `hikari_core-0.9.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.9.0.6
+Version: 0.9.0.7
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

