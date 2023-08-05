# Comparing `tmp/dragonion-0.1.0rc4-py3-none-any.whl.zip` & `tmp/dragonion-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37008 bytes, number of entries: 69
+Zip file size: 42676 bytes, number of entries: 71
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 dragonion/__init__.py
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 dragonion/__main__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dragonion/modules/cli/__init__.py
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 dragonion/modules/cli/main.py
 -rw-r--r--  2.0 unx       21 b- defN 80-Jan-01 00:00 dragonion/modules/tui/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/authentication/__init__.py
@@ -14,23 +14,25 @@
 -rw-r--r--  2.0 unx      789 b- defN 80-Jan-01 00:00 dragonion/modules/tui/authentication/widgets/inputs.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/__init__.py
 -rw-r--r--  2.0 unx      881 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/chat.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/__init__.py
--rw-r--r--  2.0 unx     1194 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/command.py
+-rw-r--r--  2.0 unx     1344 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/command.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/__init__.py
 -rw-r--r--  2.0 unx      574 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/avatar.py
--rw-r--r--  2.0 unx     1475 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py
--rw-r--r--  2.0 unx      626 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py
--rw-r--r--  2.0 unx     3158 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py
+-rw-r--r--  2.0 unx     1717 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py
+-rw-r--r--  2.0 unx      661 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py
+-rw-r--r--  2.0 unx      393 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/exit.py
+-rw-r--r--  2.0 unx     3594 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/__init__.py
 -rw-r--r--  2.0 unx      494 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/socket.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py
+-rw-r--r--  2.0 unx     2124 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py
+-rw-r--r--  2.0 unx      440 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/command/commands/room.py
 -rw-r--r--  2.0 unx      481 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/general.py
 -rw-r--r--  2.0 unx      649 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/handlers/input/message.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/tasks/__init__.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/tasks/socket_handler/__init__.py
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/__init__.py
 -rw-r--r--  2.0 unx      539 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/connect.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/disconnect.py
@@ -60,12 +62,12 @@
 -rw-r--r--  2.0 unx     2805 b- defN 80-Jan-01 00:00 dragonion/utils/core/dirs.py
 -rw-r--r--  2.0 unx      699 b- defN 80-Jan-01 00:00 dragonion/utils/core/emoji.py
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 dragonion/utils/onion/__init__.py
 -rw-r--r--  2.0 unx     1110 b- defN 80-Jan-01 00:00 dragonion/utils/onion/auth.py
 -rw-r--r--  2.0 unx     6796 b- defN 80-Jan-01 00:00 dragonion/utils/onion/onion.py
 -rw-r--r--  2.0 unx    10968 b- defN 80-Jan-01 00:00 dragonion/utils/onion/stem_process.py
 -rw-r--r--  2.0 unx     2365 b- defN 80-Jan-01 00:00 dragonion/utils/onion/tor_downloader.py
--rw-r--r--  2.0 unx     1631 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     7267 b- defN 16-Jan-01 00:00 dragonion-0.1.0rc4.dist-info/RECORD
-69 files, 71267 bytes uncompressed, 24762 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx    29302 b- defN 80-Jan-01 00:00 dragonion-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dragonion-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dragonion-1.0.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     7512 b- defN 16-Jan-01 00:00 dragonion-1.0.0.dist-info/RECORD
+71 files, 101134 bytes uncompressed, 30014 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -66,26 +66,32 @@
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py
 Comment: 
 
+Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/exit.py
+Comment: 
+
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/__init__.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/socket.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py
 Comment: 
 
+Filename: dragonion/modules/tui/chat/utils/handlers/input/command/commands/room.py
+Comment: 
+
 Filename: dragonion/modules/tui/chat/utils/handlers/input/general.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/handlers/input/message.py
 Comment: 
 
 Filename: dragonion/modules/tui/chat/utils/tasks/__init__.py
@@ -189,20 +195,20 @@
 
 Filename: dragonion/utils/onion/stem_process.py
 Comment: 
 
 Filename: dragonion/utils/onion/tor_downloader.py
 Comment: 
 
-Filename: dragonion-0.1.0rc4.dist-info/METADATA
+Filename: dragonion-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: dragonion-0.1.0rc4.dist-info/WHEEL
+Filename: dragonion-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: dragonion-0.1.0rc4.dist-info/entry_points.txt
+Filename: dragonion-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dragonion-0.1.0rc4.dist-info/RECORD
+Filename: dragonion-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dragonion/modules/tui/chat/utils/handlers/input/command/command.py

```diff
@@ -1,12 +1,14 @@
 from .commands.join import join_command
 from .commands.connect import connect_command
 from .commands.disconnect import disconnect_command
 from .commands.help import help_command
 from .commands.avatar import avatar_command
+from .commands.room import room_command
+from .commands.exit import exit_command
 
 from textual.widgets import Static
 
 
 async def not_found_command(_: list):
     from dragonion.modules.tui import app
 
@@ -20,15 +22,17 @@
 
     try:
         result = await ({
             '/help': help_command,
             '/join': join_command,
             '/connect': connect_command,
             '/disconnect': disconnect_command,
-            '/avatar': avatar_command
+            '/avatar': avatar_command,
+            '/room': room_command,
+            '/exit': exit_command
         }.get(command, not_found_command)(args))
     except Exception as e:
         result = f'{e.__class__}: {e}'
 
     if result is not None:
         from dragonion.modules.tui import app
         app.query_one('MessagesContainer').mount_scroll(Static(
```

## dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py

```diff
@@ -1,14 +1,16 @@
 from textual.widgets import Static
 
 from dragonion.utils.onion import Onion
 from dragonion.utils.onion.auth import create_service_auth
 
 from .helpers import socket
 
+from socks import GeneralProxyError
+
 
 async def connect_command(command_args: list):
     if command_args:
         return 'this command doesn\'t accepts any arguments'
 
     from dragonion.modules.tui import app
 
@@ -37,12 +39,18 @@
 
     container.mount_scroll(
         Static(
             'Connecting socket...',
             classes='onion_setup_logs'
         )
     )
-    socket.connect()
+
+    try:
+        socket.connect()
+    except GeneralProxyError:
+        container.write(f'Cannot reach service, it may be turned off or you have '
+                        f'irrelevant id-key pair (auth file)')
+        return
 
     container.mount_scroll(Static(f'[green]Connected[/] to onion and authenticated '
                                   f'on {app.user_storage.host}'))
     container.query('.onion_setup_logs').remove()
```

## dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py

```diff
@@ -10,12 +10,13 @@
     container = app.query_one('MessagesContainer')
 
     if app.user_storage.websocket:
         container.write('[green]Disconnecting from room...[/]')
         await app.user_storage.websocket.close()
         await app.user_storage.websocket.wait_closed()
         app.user_storage.sock.close()
+        app.user_storage.keys = {}
 
     if onion := app.user_storage.onion:
         onion.cleanup()
 
     container.mount_scroll(Static("Disconnected \n"))
```

## dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py

```diff
@@ -52,14 +52,25 @@
             short_description='Set avatar',
             long_description='Will generate random avatar if no symbol specified '
                              'or will set your avatar to specified symbol',
             args_description={
                 'symbol': 'Must be exactly 1 character or not specified, avatar will '
                           'be set to this character.'
             }
+        ),
+        'room': CommandHelp(
+            short_description='Get users',
+            long_description='Will return list of users in your room (you will be in'
+                             'list also)',
+            args_description=None
+        ),
+        'exit': CommandHelp(
+            short_description='Exit chat',
+            long_description='Closes connection and leaves application',
+            args_description=None
         )
     }
 
     if command_args:
         help_ = commands.get(command_args[0])
         if help_ is None:
             return f'command {command_args[0]} doesn\'t exist'
```

## dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py

```diff
@@ -20,15 +20,21 @@
 
     if app.user_storage.websocket:
         log.write('[green]Disconnecting from room...[/]')
         await app.user_storage.websocket.close()
         await app.user_storage.websocket.wait_closed()
         app.user_storage.sock.close()
         from .helpers import socket
-        socket.connect()
+        from socks import GeneralProxyError
+        try:
+            socket.connect()
+        except GeneralProxyError:
+            log.write(f'Cannot reach service, it may be turned off or you have '
+                      f'irrelevant id-key pair (auth file)')
+            return
 
     log.write(f'[green]Connecting to {command_args[0]}...')
     app.user_storage.websocket = await websockets.client.connect(
         f'ws://{app.user_storage.host}:80/{command_args[0]}',
         sock=app.user_storage.sock
     )
     await app.user_storage.websocket.send(
@@ -42,13 +48,13 @@
     connection_message = WebMessage.from_json(await app.user_storage.websocket.recv())
 
     if connection_message.type == "error":
         log.write(
             f'[red]Error connecting to room[/]: {connection_message.error_message}'
         )
     elif connection_message.type == "connect_answer":
-        app.user_storage.keys |= connection_message.connected_users
+        app.user_storage.keys = connection_message.connected_users
         asyncio.create_task(handle_websocket())
     else:
         log.write(
             f'Received unknown answer {connection_message.type}: {connection_message}'
         )
```

## Comparing `dragonion-0.1.0rc4.dist-info/RECORD` & `dragonion-1.0.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 dragonion/modules/tui/authentication/widgets/inputs.py,sha256=u1vpoOFcQBI9LgeZZ7MfJvcY-HKFv3YBrpVl7aO6_2I,789
 dragonion/modules/tui/chat/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/chat.py,sha256=lzHrsOH07bgECDWRaxf8XDGqF1K6rqsTKCWlkPF1SOo,881
 dragonion/modules/tui/chat/utils/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/handlers/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/handlers/input/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/handlers/input/command/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
-dragonion/modules/tui/chat/utils/handlers/input/command/command.py,sha256=UhErIxm8rgF9uQzFBItw2lbK0io54_DcAHvNAwAZDUo,1194
+dragonion/modules/tui/chat/utils/handlers/input/command/command.py,sha256=w0VbAxIDYLltAFzNoM9emREmnQwp4pg8yXyhy5DPqw4,1344
 dragonion/modules/tui/chat/utils/handlers/input/command/commands/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/handlers/input/command/commands/avatar.py,sha256=p3TsCc7-4IQ_RiFUwXmSz4OkZSIjo7YiIC-IdwG9d1s,574
-dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py,sha256=w4ITQZJeCk1NjD20PIkDlwldadgF5m-uQEzsQjPdDmQ,1475
-dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py,sha256=vPTWRt5xqsweGxBHv3CaXqLpQ_oKMPEcsHrpQZCjPlU,626
-dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py,sha256=ACaH6yexRbkgrNiUu1MnPhSqKqhUArlRANeRJP6uD3w,3158
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/connect.py,sha256=jzJ08KzX3qK_uKFTOseWsUYrDC6_VvvEt9XxpdN1EMQ,1717
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/disconnect.py,sha256=BENnH96XmEcV5iJ7_qmn1z4ZUPETvBQsFyUiCXzc-jI,661
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/exit.py,sha256=cDA4kIc9jc8857c3_yA6LO8R_8rtU7eYIY64KkDkBPI,393
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/help.py,sha256=yhJM0axCER-dt-WMTuSo-dtG9L7YXl4_b1s5agB8ltE,3594
 dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/handlers/input/command/commands/helpers/socket.py,sha256=11EutftWMC4nVERq4PJiN-E-0DGNyYHRznCwq7EqT88,494
-dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py,sha256=2n4dEd5_KutOERWPyXGhz3TI7x2fhjIK18A7jbCWc80,1869
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/join.py,sha256=R84WAxwVz8R3_WQPT1NmKQllqq6wdvC8H6xzVHYKUjE,2124
+dragonion/modules/tui/chat/utils/handlers/input/command/commands/room.py,sha256=i_3DIpT8KO8xN28inWHaJ_TGfZnL-rH3WRl_yr50W3Q,440
 dragonion/modules/tui/chat/utils/handlers/input/general.py,sha256=6eX6dv3-BpUY-Coi9hjq0zaVIjB9gUa-Xa3L_ZDNCW4,481
 dragonion/modules/tui/chat/utils/handlers/input/message.py,sha256=BKGefnDayLT_iq7Jwou4sHegKM3qUEUMVPHW7crd6-E,649
 dragonion/modules/tui/chat/utils/tasks/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/tasks/socket_handler/__init__.py,sha256=n1bnYdeb_bNDBKASWGywTRa0Ne9hMAkal3AuVZJgovI,5
 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/__init__.py,sha256=CN3pLZENjt70T3R75PQFrdi9vOZTT4qY7blrZddjICU,192
 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/connect.py,sha256=gvkFFpc-PAyDxaLCl2dkc45pgmNWVNIwHThnT6u3rlk,539
 dragonion/modules/tui/chat/utils/tasks/socket_handler/handlers/disconnect.py,sha256=k8pk8zCZqyoMCvNbWcfJNeRjw-Sft-hdDSguRiPnwvI,457
@@ -59,11 +61,11 @@
 dragonion/utils/core/dirs.py,sha256=M_7bjY6_Em8ICbfcNc-AZPhIz4s2t6KLBvBeURIz3wY,2805
 dragonion/utils/core/emoji.py,sha256=ojZx_hL50wBlpq6Zip-Y23c_q-ljrQKXtmscK4jyoY8,699
 dragonion/utils/onion/__init__.py,sha256=gQajsInd9Xh0QMplPYSpOVDs7f3HAajOqF2G1pg6TfQ,52
 dragonion/utils/onion/auth.py,sha256=2762A-N1elA0G-JTxkknEwkmWY2UvGX7bGGRrxEheEw,1110
 dragonion/utils/onion/onion.py,sha256=OifJcBEZHZYmuWNw4Clu1qct2VTE471wnLzD9Jdc4Po,6796
 dragonion/utils/onion/stem_process.py,sha256=0QB6ErA1pO4I1aIPkyoRDqpTjcZQkCjHjbsao-cX7JY,10968
 dragonion/utils/onion/tor_downloader.py,sha256=XXJepwjwPvrwxvTA4dIPmmqYQLXaIk6SCs7po5ikpHA,2365
-dragonion-0.1.0rc4.dist-info/METADATA,sha256=4mjzknXSJY55DHa_N3pyX1QYA6azkUao1J9UC-JedeE,1631
-dragonion-0.1.0rc4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-dragonion-0.1.0rc4.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
-dragonion-0.1.0rc4.dist-info/RECORD,,
+dragonion-1.0.0.dist-info/METADATA,sha256=WaP6K3TeQeCzKps2VhJTwqbM7v-Uf1upz3BdsWEHACM,29302
+dragonion-1.0.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+dragonion-1.0.0.dist-info/entry_points.txt,sha256=JVx0FGUdz6RQu1_M4biP7bmduOt6v6Bl8wnAnGZZ9BQ,44
+dragonion-1.0.0.dist-info/RECORD,,
```

