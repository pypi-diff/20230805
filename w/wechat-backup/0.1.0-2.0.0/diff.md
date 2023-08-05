# Comparing `tmp/wechat_backup-0.1.0.tar.gz` & `tmp/wechat_backup-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wechat_backup-0.1.0.tar", max compression
+gzip compressed data, was "wechat_backup-2.0.0.tar", max compression
```

## Comparing `wechat_backup-0.1.0.tar` & `wechat_backup-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rwxr-xr-x   0        0        0      305 2023-04-02 15:48:51.935723 wechat_backup-0.1.0/README.md
--rwxr-xr-x   0        0        0      618 2023-04-04 13:16:04.714063 wechat_backup-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-04-01 04:43:38.737613 wechat_backup-0.1.0/src/wechat_backup/__init__.py
--rwxr-xr-x   0        0        0     1021 2023-04-04 12:26:01.002410 wechat_backup-0.1.0/src/wechat_backup/__main__.py
--rwxr-xr-x   0        0        0      180 2023-04-04 12:41:17.238338 wechat_backup-0.1.0/src/wechat_backup/command/__init__.py
--rwxr-xr-x   0        0        0     1440 2023-04-04 12:26:18.407179 wechat_backup-0.1.0/src/wechat_backup/command/extract_contacts.py
--rwxr-xr-x   0        0        0      742 2023-04-04 12:40:03.594322 wechat_backup-0.1.0/src/wechat_backup/command/extract_messages.py
--rwxr-xr-x   0        0        0     1856 2023-04-04 09:40:02.267918 wechat_backup-0.1.0/src/wechat_backup/contact.py
--rwxr-xr-x   0        0        0      243 2023-04-04 12:54:42.325251 wechat_backup-0.1.0/src/wechat_backup/context.py
--rwxr-xr-x   0        0        0      965 2023-04-04 11:58:37.891640 wechat_backup-0.1.0/src/wechat_backup/helper.py
--rwxr-xr-x   0        0        0        0 2023-04-01 04:43:38.758610 wechat_backup-0.1.0/src/wechat_backup/message/__init__.py
--rwxr-xr-x   0        0        0     7921 2023-04-04 13:11:49.619828 wechat_backup-0.1.0/src/wechat_backup/message/parser.py
--rwxr-xr-x   0        0        0     3714 2023-04-04 13:13:09.559443 wechat_backup-0.1.0/src/wechat_backup/message/typing.py
--rwxr-xr-x   0        0        0        0 2023-04-04 12:25:08.477757 wechat_backup-0.1.0/src/wechat_backup/platform/__init__.py
--rwxr-xr-x   0        0        0      138 2023-04-01 04:43:38.770610 wechat_backup-0.1.0/src/wechat_backup/platform/android/__init__.py
--rwxr-xr-x   0        0        0     3764 2023-04-01 04:43:38.772610 wechat_backup-0.1.0/src/wechat_backup/platform/android/contact.py
--rwxr-xr-x   0        0        0      538 2023-04-01 04:43:38.774610 wechat_backup-0.1.0/src/wechat_backup/platform/android/context.py
--rwxr-xr-x   0        0        0     4896 2023-04-01 04:43:38.777225 wechat_backup-0.1.0/src/wechat_backup/platform/android/message.py
--rwxr-xr-x   0        0        0      126 2023-04-04 12:43:36.097001 wechat_backup-0.1.0/src/wechat_backup/platform/ios/__init__.py
--rwxr-xr-x   0        0        0     4582 2023-04-04 12:25:37.116021 wechat_backup-0.1.0/src/wechat_backup/platform/ios/contact.py
--rwxr-xr-x   0        0        0      789 2023-04-04 12:54:58.237595 wechat_backup-0.1.0/src/wechat_backup/platform/ios/context.py
--rwxr-xr-x   0        0        0     6982 2023-04-04 13:12:42.529116 wechat_backup-0.1.0/src/wechat_backup/platform/ios/message.py
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 wechat_backup-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-08-05 06:21:59.225750 wechat_backup-2.0.0/COPYING
+-rw-r--r--   0        0        0      686 2023-08-05 18:36:16.434904 wechat_backup-2.0.0/README.md
+-rw-r--r--   0        0        0     1373 2023-08-05 18:41:46.132982 wechat_backup-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-08-05 06:21:59.233774 wechat_backup-2.0.0/src/wechat_backup/__init__.py
+-rw-r--r--   0        0        0     1243 2023-08-05 18:06:21.938516 wechat_backup-2.0.0/src/wechat_backup/__main__.py
+-rw-r--r--   0        0        0      180 2023-08-05 18:04:29.059320 wechat_backup-2.0.0/src/wechat_backup/commands/__init__.py
+-rw-r--r--   0        0        0     1468 2023-08-05 18:12:08.295450 wechat_backup-2.0.0/src/wechat_backup/commands/extract_contacts.py
+-rw-r--r--   0        0        0      771 2023-08-05 18:16:30.575045 wechat_backup-2.0.0/src/wechat_backup/commands/extract_messages.py
+-rw-r--r--   0        0        0     1856 2023-08-05 06:21:59.235778 wechat_backup-2.0.0/src/wechat_backup/contact.py
+-rw-r--r--   0        0        0      243 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/context.py
+-rw-r--r--   0        0        0      959 2023-08-05 18:33:05.361835 wechat_backup-2.0.0/src/wechat_backup/helper.py
+-rw-r--r--   0        0        0        0 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/message/__init__.py
+-rw-r--r--   0        0        0     7760 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/message/parser.py
+-rw-r--r--   0        0        0     3575 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/message/typing.py
+-rw-r--r--   0        0        0        0 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/__init__.py
+-rw-r--r--   0        0        0      138 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/android/__init__.py
+-rw-r--r--   0        0        0     3764 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/android/contact.py
+-rw-r--r--   0        0        0      538 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/android/context.py
+-rw-r--r--   0        0        0     4896 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/android/message.py
+-rw-r--r--   0        0        0      126 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/ios/__init__.py
+-rw-r--r--   0        0        0     4582 2023-08-05 06:21:59.235820 wechat_backup-2.0.0/src/wechat_backup/platform/ios/contact.py
+-rw-r--r--   0        0        0      928 2023-08-05 18:28:45.560243 wechat_backup-2.0.0/src/wechat_backup/platform/ios/context.py
+-rw-r--r--   0        0        0     6773 2023-08-05 18:32:29.916668 wechat_backup-2.0.0/src/wechat_backup/platform/ios/message.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 wechat_backup-2.0.0/PKG-INFO
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/__main__.py` & `wechat_backup-2.0.0/src/wechat_backup/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 import importlib
 import configparser
 from pathlib import Path
 
 import click
 
-from wechat_backup.command import command_group
+from wechat_backup import __version__
+from wechat_backup.commands import command_group
+
+
+def print_version(ctx: click.Context, _, value: str):
+    if not value or ctx.resilient_parsing:
+        return
+
+    click.echo(__version__)
+    ctx.exit()
 
 
 @click.group(commands=command_group)
-@click.option('--profile', help='Profile in configurations to use.', type=str, required=False, default='default')
-@click.option('--config-file', help='Path of configuration file.', type=click.Path(exists=True, dir_okay=False), required=False, default=Path.home().joinpath('.wechat-backup', 'config.ini'))
+@click.option('--version', help='Show version information.', is_flag=True, callback=print_version, expose_value=False, is_eager=True)
+@click.option('-p', '--profile', help='Profile to load from configurations.', default='default')
 @click.pass_context
-def cli(ctx: click.Context, profile: str, config_file: Path):
-    """A command-line tool to extract user data from WeChat backup files."""
+def cli(ctx: click.Context, profile: str):
+    """A command-line tool to help user manage data in WeChat backup files."""
 
     ctx.ensure_object(dict)
 
-    parser = configparser.ConfigParser()
-    parser.read(Path(config_file))
-    config = {k: v for k, v in parser.items(section=profile)}
+    profile_file = Path.home() / '.wechat-backup/profiles.ini'
+
+    if not profile_file.exists():
+        ctx.fail('Profile file not found')
+
+    config = configparser.ConfigParser()
+    config.read(profile_file)
 
-    ctx.obj['platform_module'] = importlib.import_module(f'wechat_backup.platform.{config["platform"]}')
-    ctx.obj['context'] = ctx.obj['platform_module'].context.new_context(config)
+    ctx.obj['profile'] = dict(config.items(section=profile))
+    ctx.obj['platform_module'] = importlib.import_module(f'wechat_backup.platform.{ctx.obj["profile"]["platform"]}')
 
 
 if __name__ == '__main__':
-    cli()
+    cli(obj={})  # pylint: disable=no-value-for-parameter
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/command/extract_contacts.py` & `wechat_backup-2.0.0/src/wechat_backup/commands/extract_contacts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import json
-
 import click
-
 from wechat_backup.contact import assemble_friend, assemble_official_account, assemble_microprogram, assemble_chatroom
 from wechat_backup.helper import EntityJSONEncoder
 
 
 @click.command('extract-contacts')
-@click.option('--type', 'contact_type', help='Type of contacts', type=click.Choice(['friend', 'official', 'microprogram', 'chatroom']), required=True, default='friend')
+@click.option('-t', '--type', 'contact_type', help='Type of contacts', type=click.Choice(['friend', 'official', 'microprogram', 'chatroom']), default='friend')
 @click.pass_context
 def extract_contacts_command(ctx: click.Context, contact_type: str):
-    """Extract contacts."""
+    """Extract WeChat contacts."""
 
     platform_module = ctx.obj['platform_module']
-    context = ctx.obj['context']
+    context = platform_module.context.new_context(ctx.obj['profile'])
 
     def assemble_friend_wrapper(record: dict):
         return assemble_friend(record=record, labels=platform_module.contact.load_contact_labels(context=context))
 
     assemblers = {
         'friend': assemble_friend_wrapper,
         'official': assemble_official_account,
@@ -28,11 +26,11 @@
     loaders = {
         'friend': platform_module.contact.load_friends,
         'official': platform_module.contact.load_official_accounts,
         'microprogram': platform_module.contact.load_microprograms,
         'chatroom': platform_module.contact.load_chatrooms
     }
 
-    click.echo(json.dumps([
+    print(json.dumps([
         assemblers[contact_type](record=record)
         for record in loaders[contact_type](context=context)
     ], indent=4, ensure_ascii=False, cls=EntityJSONEncoder))
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/command/extract_messages.py` & `wechat_backup-2.0.0/src/wechat_backup/commands/extract_messages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import json
-
 import click
-
 from wechat_backup.message.parser import assemble_message
 from wechat_backup.helper import EntityJSONEncoder
 
 
 @click.command('extract-messages')
-@click.option('--conversation-id', help='Conversation of messages', type=str, required=True)
+@click.option('-i', '--conversation-id', help='Conversation of messages.', required=True)
 @click.pass_context
 def extract_messages_command(ctx: click.Context, conversation_id: str):
-    """Extract messages by conversation."""
+    """Extract messages of a conversation."""
 
     platform_module = ctx.obj['platform_module']
-    context = ctx.obj['context']
+    context = platform_module.context.new_context(ctx.obj['profile'])
 
-    click.echo(json.dumps([
+    print(json.dumps([
         assemble_message(record=record, context=context)
         for record in platform_module.message.load_messages(context=context, conversation_id=conversation_id)
     ], indent=4, ensure_ascii=False, cls=EntityJSONEncoder))
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/contact.py` & `wechat_backup-2.0.0/src/wechat_backup/contact.py`

 * *Files identical despite different names*

### Comparing `wechat_backup-0.1.0/src/wechat_backup/helper.py` & `wechat_backup-2.0.0/src/wechat_backup/helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import hashlib
 import sqlite3
 from json import JSONEncoder
-from enum import Enum
 from datetime import datetime
 from dataclasses import is_dataclass
-from typing import List
+from enum import Enum
 
 
 def sqlite_connect(path: str) -> sqlite3.Connection:
-    def dict_factory(cursor: sqlite3.Cursor, row: List) -> dict:
-        return {col[0]: row[i] for i, col in enumerate(cursor.description)}
+    def dict_factory(cursor, row) -> dict:
+        d = {}
+        for i, col in enumerate(cursor.description):
+            d[col[0]] = row[i]
+        return d
 
     conn = sqlite3.connect(path)
     conn.row_factory = dict_factory
 
     return conn
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/message/parser.py` & `wechat_backup-2.0.0/src/wechat_backup/message/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-import xml.etree.ElementTree as ET
+from lxml import etree
 from .typing import *
 from wechat_backup.context import WechatContext, WechatPlatform
 
 _CONTENT_PARSERS = {}
 _APPMSG_PARSERS = {}
 
 
@@ -124,15 +124,15 @@
 def parse_content_system(record: dict, context: WechatContext):
     return SystemContent.content_type, SystemContent(text=record['content'])
 
 
 # noinspection PyUnusedLocal
 @content_parser(type=WechatMessageType.NameCard)
 def parse_content_name_card(record: dict, context: WechatContext):
-    node = ET.fromstring(record['content']).find('.')
+    node = etree.fromstring(record['content']).xpath('/msg')[0]
 
     username = node.attrib['username']
 
     return NameCardContent.content_type, NameCardContent(
         user_id=username,
         nickname=node.attrib['nickname'],
         province=node.attrib['province'],
@@ -140,110 +140,103 @@
         gender=NameCardContent.Gender(int(node.attrib['sex']))
     )
 
 
 # noinspection PyUnusedLocal
 @content_parser(type=WechatMessageType.Location)
 def parse_content_location(record: dict, context: WechatContext):
-    node = ET.fromstring(record['content']).find('./location')
+    node = etree.fromstring(record['content']).xpath('/msg/location')[0]
 
     return LocationContent.content_type, LocationContent(
         latitude=float(node.attrib['x']),
         longitude=float(node.attrib['y']),
         address=node.attrib['label'],
         label=node.attrib['poiname']
     )
 
 
 @content_parser(type=WechatMessageType.Application)
 def parse_content_application(record: dict, context: WechatContext):
-    app_type = WechatAppmsgType(int(ET.fromstring(record['content']).find('./appmsg/type').text))
+    app_type = WechatAppmsgType(int(etree.fromstring(record['content']).xpath('/msg/appmsg/type')[0].text))
 
     if context.platform not in _APPMSG_PARSERS.keys() or app_type not in _APPMSG_PARSERS[context.platform].keys():
         platform = WechatPlatform.All
     else:
         platform = context.platform
 
     return _APPMSG_PARSERS[platform][app_type](record=record, context=context)
 
 
 # noinspection PyUnusedLocal
 @appmsg_parser(type=WechatAppmsgType.Text)
 def parse_appmsg_text(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
 
     return TextContent.content_type, TextContent(
-        text=appmsg.find('./title').text,
+        text=appmsg.xpath('title')[0].text,
     )
 
 
 # noinspection PyUnusedLocal
 @appmsg_parser(type=WechatAppmsgType.MoneyPacket)
 def parse_appmsg_money_packet(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
-    wcpayinfo = appmsg.find('./wcpayinfo')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
+    wcpayinfo = appmsg.xpath('wcpayinfo')[0]
 
     return MoneyPacketContent.content_type, MoneyPacketContent(
         payment_info=MoneyPacketContent.PaymentInfo(
-            icon_url=wcpayinfo.find('./iconurl').text,
-            receiver_title=wcpayinfo.find('./receivertitle').text,
-            receiver_description=wcpayinfo.find('./receiverdes').text,
-            sender_title=wcpayinfo.find('./sendertitle').text,
-            sender_description=wcpayinfo.find('./senderdes').text,
-            scene_id=int(wcpayinfo.find('./sceneid').text),
-            scene_description=wcpayinfo.find('./senderdes').text
+            icon_url=wcpayinfo.xpath('iconurl')[0].text,
+            receiver_title=wcpayinfo.xpath('receivertitle')[0].text,
+            receiver_description=wcpayinfo.xpath('receiverdes')[0].text,
+            sender_title=wcpayinfo.xpath('sendertitle')[0].text,
+            sender_description=wcpayinfo.xpath('senderdes')[0].text,
+            scene_id=int(wcpayinfo.xpath('sceneid')[0].text),
+            scene_description=wcpayinfo.xpath('senderdes')[0].text
         ),
-        title=appmsg.find('./title').text,
-        description=appmsg.find('./des').text
+        title=appmsg.xpath('title')[0].text,
+        description=appmsg.xpath('des')[0].text
     )
 
 
 # noinspection PyUnusedLocal
 @appmsg_parser(type=WechatAppmsgType.Transfer)
 def parse_appmsg_transfer(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
-    wcpayinfo = appmsg.find('./wcpayinfo')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
+    wcpayinfo = appmsg.xpath('wcpayinfo')[0]
 
     # noinspection PyCallByClass
     return TransferContent.content_type, TransferContent(
         payment_info=TransferContent.PaymentInfo(
-            subtype=int(wcpayinfo.find('./paysubtype').text),
-            description=wcpayinfo.find('./feedesc').text,
-            transfer_id=wcpayinfo.find('./transferid').text,
-            transfer_time=int(wcpayinfo.find('./begintransfertime').text),
-            expire_time=int(wcpayinfo.find('./invalidtime').text),
-            memo=wcpayinfo.find('./pay_memo').text,
+            subtype=int(wcpayinfo.xpath('paysubtype')[0].text),
+            description=wcpayinfo.xpath('feedesc')[0].text,
+            transfer_id=wcpayinfo.xpath('transferid')[0].text,
+            transfer_time=int(wcpayinfo.xpath('begintransfertime')[0].text),
+            expire_time=int(wcpayinfo.xpath('invalidtime')[0].text),
+            memo=wcpayinfo.xpath('pay_memo')[0].text,
         ),
-        title=appmsg.find('./title').text,
-        description=appmsg.find('./des').text
+        title=appmsg.xpath('title')[0].text,
+        description=appmsg.xpath('des')[0].text
     )
 
 
 # noinspection PyUnusedLocal
 @appmsg_parser(type=WechatAppmsgType.LocationShare)
 def parse_appmsg_location_share(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
 
-    return LocationShareContent.content_type, LocationShareContent(title=appmsg.find('./title').text)
+    return LocationShareContent.content_type, LocationShareContent(title=appmsg.xpath('title')[0].text)
 
 
 @appmsg_parser(type=WechatAppmsgType.Emoji)
 def parse_appmsg_emoji(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
-    md5 = appmsg.find('./appattach/emoticonmd5').text
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
+    md5 = appmsg.xpath('appattach/emoticonmd5')[0].text
 
     path = '%s/%s.gif' % (context.emoji_cache, md5)
 
     if not os.path.exists(path):
         sys.stderr.write('[WARNING] No emoji found for "%s".\n' % md5)
         path = 'emoji://%s' % md5
 
     return EmojiContent.content_type, EmojiContent(
         file_path=path
     )
-
-
-@appmsg_parser(type=WechatAppmsgType.Reference)
-def parse_appmsg_reference(record: dict, context: WechatContext):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
-
-    return ReferenceContent.content_type, ReferenceContent(text=appmsg.find('./title').text)
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/message/typing.py` & `wechat_backup-2.0.0/src/wechat_backup/message/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     Link = 'link'
     Music = 'music'
     Attachment = 'attachment'
     MoneyPacket = 'money-packet'
     Transfer = 'transfer'
     LocationShare = 'location-share'
     VoIP = 'voip'
-    Reference = 'reference'
     System = 'system'
 
 
 @dataclass
 class Message:
     conversation_id: str
     sent_at: datetime
@@ -120,15 +119,14 @@
 
     class VoIPType(Enum):
         Unknown = -1
         Video = 0
         Audio = 1
 
     class VoIPStatus(Enum):
-        Unknown = 2
         Answered = 4
         Cancelled = 5
 
     type: VoIPType
     status: VoIPStatus
     duration: int
 
@@ -196,12 +194,7 @@
 
 
 @dataclass
 class LocationShareContent:
     content_type = MessageType.LocationShare
 
     title: str
-
-
-@dataclass
-class ReferenceContent(TextContent):
-    content_type = MessageType.Reference
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/android/contact.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/android/contact.py`

 * *Files identical despite different names*

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/android/context.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/android/context.py`

 * *Files identical despite different names*

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/android/message.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/android/message.py`

 * *Files identical despite different names*

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/ios/contact.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/ios/contact.py`

 * *Files identical despite different names*

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/ios/context.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/ios/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import sqlite3
+import os.path
 from dataclasses import dataclass
+from glob import glob
 from typing import List
-from pathlib import Path
 
 from wechat_backup.context import WechatPlatform, WechatContext
 from wechat_backup.helper import sqlite_connect
 
 
 @dataclass
 class WechatContextIos(WechatContext):
     doc_dir: str
     contact_db: sqlite3.Connection
+    mm_db: sqlite3.Connection
     message_db: List[sqlite3.Connection]
 
 
-def new_context(config: dict):
-    db_dir = Path(config["doc_dir"], 'DB')
-
+def new_context(profile: dict):
     return WechatContextIos(
         platform=WechatPlatform.iOS,
-        user_id=config['user_id'],
-        emoji_cache=config['emoji_cache'],
-        doc_dir=config['doc_dir'],
-        message_db=list(map(lambda f: sqlite_connect(f), db_dir.glob('message_*.sqlite'))),
-        contact_db=sqlite_connect(str(db_dir.joinpath('WCDB_Contact.sqlite')))
+        user_id=profile['user_id'],
+        doc_dir=profile['doc_dir'],
+        message_db=[sqlite_connect(db_file) for db_file in glob(f'{os.path.join(profile["doc_dir"], "DB")}/message_*.sqlite')],
+        mm_db=sqlite_connect(os.path.join(profile['doc_dir'], 'DB', 'MM.sqlite')),
+        contact_db=sqlite_connect(os.path.join(profile['doc_dir'], 'DB', 'WCDB_Contact.sqlite')),
+        emoji_cache=profile['emoji_cache']
     )
```

### Comparing `wechat_backup-0.1.0/src/wechat_backup/platform/ios/message.py` & `wechat_backup-2.0.0/src/wechat_backup/platform/ios/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-import os
-import sys
 import sqlite3
-import xml.etree.ElementTree as ET
-
 from typing import Iterable
-from .context import WechatContextIos
-from wechat_backup.helper import md5_utf8, path_or_none
-from wechat_backup.message.parser import content_parser, appmsg_parser, WechatMessageType, WechatAppmsgType
-from wechat_backup.message.parser import AttachmentContent, EmojiContent, ImageContent, LinkContent, MusicContent, VoiceContent, VideoContent, VoIPContent
+from typing import List
 
+from wechat_backup.helper import md5_utf8, path_or_none
+from wechat_backup.message.parser import *
 from wechat_backup.context import WechatPlatform
+from .context import WechatContextIos
 
 
-def find_message_db(message_db: Iterable[sqlite3.Connection], table_name: str) -> sqlite3.Connection:
-    sql = "SELECT COUNT(*) AS C FROM sqlite_schema WHERE tbl_name = ?"
-
-    for db in message_db:
-        if db.execute(sql, (table_name,)).fetchone()['C'] > 0:
+def find_message_db(table_name: str, db_list: List[sqlite3.Connection]):
+    for db in db_list:
+        row = db.cursor().execute("SELECT COUNT(*) AS C FROM sqlite_master WHERE type = 'table' AND name = ?", (table_name,)).fetchone()
+        if row['C'] > 0:
             return db
 
-    raise ValueError(f'Table "{table_name}" not found in any message databases.')
-
 
 def load_messages(context: WechatContextIos, conversation_id: str) -> Iterable[dict]:
-    table_name = f'Chat_{md5_utf8(conversation_id)}'
+    table_name = 'Chat_%s' % md5_utf8(conversation_id)
+
+    db = find_message_db(table_name, context.message_db)
 
     sql = f'''
             SELECT
                 '{conversation_id}' AS conversation_id,
                 Type AS type,
                 NOT Des AS is_send,
                 CreateTime AS sent_at,
                 Message AS content,
 
                 MesLocalID
             FROM {table_name}
             ORDER BY CreateTime
             '''
 
-    return find_message_db(context.message_db, table_name).cursor().execute(sql).fetchall()
+    return db.cursor().execute(sql).fetchall()
 
 
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.Image)
 def parse_content_image(record: dict, context: WechatContextIos):
     doc_dir = context.doc_dir
     prefix = '%s/Img/%s' % (doc_dir, md5_utf8(record['conversation_id']))
 
@@ -53,68 +48,68 @@
     )
 
 
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.Voice)
 def parse_content_voice(record: dict, context: WechatContextIos):
     prefix = '%s/Audio/%s' % (context.doc_dir, md5_utf8(record['conversation_id']))
 
-    node = ET.fromstring(record['content']).find('./voicemsg')
+    node = etree.fromstring(record['content']).xpath('/msg/voicemsg')[0]
 
     return VoiceContent.content_type, VoiceContent(
         file_path=path_or_none('%s/%d.aud' % (prefix, record['MesLocalID'])),
         duration=int(node.attrib['voicelength'])
     )
 
 
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.Video)
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.WechatVideo)
 def parse_content_video(record: dict, context: WechatContextIos):
-    node = ET.fromstring(record['content']).find('./videomsg')
+    node = etree.fromstring(record['content']).xpath('/msg/videomsg')[0]
 
     return VideoContent.content_type, VideoContent(
         file_path=path_or_none('%s/Video/%s/%d.mp4' % (context.doc_dir, md5_utf8(record['conversation_id']), record['MesLocalID'])),
         duration=int(node.attrib['playlength']),
         thumbnail_path=path_or_none('%s/Video/%s/%d.video_thum' % (context.doc_dir, md5_utf8(record['conversation_id']), record['MesLocalID']))
     )
 
 
 # noinspection PyUnusedLocal
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.VoIP)
 def parse_content_voip(record: dict, context: WechatContextIos):
-    node = ET.fromstring('<root>%s</root>' % record['content']).find('.')
-    status = VoIPContent.VoIPStatus(int(node.find('voipinvitemsg/status').text))
+    node = etree.fromstring('<root>%s</root>' % record['content']).xpath('/root')[0]
+    status = VoIPContent.VoIPStatus(int(node.xpath('voipinvitemsg/status')[0].text))
 
     return VoIPContent.content_type, VoIPContent(
-        type=VoIPContent.VoIPType(int(node.find('voipinvitemsg/invitetype').text)),
+        type=VoIPContent.VoIPType(int(node.xpath('voipinvitemsg/invitetype')[0].text)),
         status=status,
-        duration=int(node.find('voiplocalinfo/duration').text) if status == VoIPContent.VoIPStatus.Answered else 0
+        duration=int(node.xpath('voiplocalinfo/duration')[0].text) if status == VoIPContent.VoIPStatus.Answered else 0
     )
 
 
 @content_parser(platform=WechatPlatform.iOS, type=WechatMessageType.Emoji)
 def parse_content_emoji(record: dict, context: WechatContextIos):
-    md5 = ET.fromstring(record['content']).find('./emoji').attrib['md5']
+    md5 = etree.fromstring(record['content']).xpath('/msg/emoji')[0].attrib['md5']
 
     path = '%s/%s.gif' % (context.emoji_cache, md5)
 
     if not os.path.exists(path):
         sys.stderr.write('[WARNING] No emoji found for "%s".\n' % md5)
         path = 'emoji://%s' % md5
 
     return EmojiContent.content_type, EmojiContent(file_path=path)
 
 
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Attachment)
 def parse_appmsg_attachment(record: dict, context: WechatContextIos):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
-    file_ext = appmsg.find('./appattach/fileext').text
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
+    file_ext = appmsg.xpath('/msg/appmsg/appattach/fileext')[0].text
 
     # noinspection PyArgumentList
     return AttachmentContent.content_type, AttachmentContent(
-        title=appmsg.find('title').text,
+        title=appmsg.xpath('title')[0].text,
         file_path=path_or_none('%s/OpenData/%s/%d.%s' % (context.doc_dir, md5_utf8(record['conversation_id']), record['MesLocalID'], file_ext))
     )
 
 
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Video)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Game)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.EmojiSet)
@@ -122,20 +117,20 @@
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.MicroprogramLink)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.GiftCard)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Coupon)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.ChatHistory)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.FavorChatHistory)
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Link)
 def parse_appmsg_link(record: dict, context: WechatContextIos):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
 
     return LinkContent.content_type, LinkContent(
-        title=appmsg.find('title').text,
-        description=appmsg.find('des').text,
-        url=appmsg.find('url').text,
+        title=appmsg.xpath('title')[0].text,
+        description=appmsg.xpath('des')[0].text,
+        url=appmsg.xpath('url')[0].text,
         thumbnail_path=path_or_none('%s/OpenData/%s/%d.pic_thum' % (context.doc_dir, md5_utf8(record['conversation_id']), record['MesLocalID']))
     )
 
 
 @appmsg_parser(platform=WechatPlatform.iOS, type=WechatAppmsgType.Image)
 def parse_appmsg_image(record: dict, context: WechatContextIos):
     # noinspection PyTypeChecker
@@ -145,14 +140,14 @@
         high_definition_path=None
     )
 
 
 # noinspection PyUnusedLocal
 @appmsg_parser(type=WechatAppmsgType.Music)
 def parse_appmsg_music(record: dict, context: WechatContextIos):
-    appmsg = ET.fromstring(record['content']).find('./appmsg')
+    appmsg = etree.fromstring(record['content']).xpath('/msg/appmsg')[0]
 
     # noinspection PyArgumentList
     return MusicContent.content_type, MusicContent(
-        data_url=appmsg.find('dataurl').text,
+        data_url=appmsg.xpath('dataurl')[0].text,
         **parse_appmsg_link(record=record, context=context)[1].__dict__
     )
```

