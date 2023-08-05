# Comparing `tmp/telegram_menu-2.1.1.tar.gz` & `tmp/telegram_menu-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_menu-2.1.1.tar", last modified: Sun May  7 20:37:10 2023, max compression
+gzip compressed data, was "telegram_menu-2.1.2.tar", last modified: Sat Aug  5 09:42:10 2023, max compression
```

## Comparing `telegram_menu-2.1.1.tar` & `telegram_menu-2.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/
--rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.1.1/LICENSE
--rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7259 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6458 2023-05-07 00:10:58.000000 telegram_menu-2.1.1/README.md
--rw-rw-rw-   0        0        0      102 2023-05-07 20:32:35.000000 telegram_menu-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.962821 telegram_menu-2.1.1/telegram_menu/
--rw-rw-rw-   0        0        0     1008 2023-02-20 21:30:49.000000 telegram_menu-2.1.1/telegram_menu/__init__.py
--rw-rw-rw-   0        0        0     1139 2023-05-07 20:33:52.000000 telegram_menu-2.1.1/telegram_menu/_version.py
--rw-rw-rw-   0        0        0    10601 2023-05-06 04:59:21.000000 telegram_menu-2.1.1/telegram_menu/models.py
--rw-rw-rw-   0        0        0    30013 2023-05-07 20:32:17.000000 telegram_menu-2.1.1/telegram_menu/navigation.py
--rw-rw-rw-   0        0        0       63 2023-02-20 21:36:29.000000 telegram_menu-2.1.1/telegram_menu/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/telegram_menu.egg-info/
--rw-rw-rw-   0        0        0     7259 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.1.1/telegram_menu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-07 20:37:10.000000 telegram_menu-2.1.1/telegram_menu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 20:37:10.966310 telegram_menu-2.1.1/tests/
--rw-rw-rw-   0        0        0      713 2023-02-20 21:40:17.000000 telegram_menu-2.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1321 2023-02-20 21:30:49.000000 telegram_menu-2.1.1/tests/demo.py
--rw-rw-rw-   0        0        0    20858 2023-05-07 20:33:23.000000 telegram_menu-2.1.1/tests/test_connection.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:10.878637 telegram_menu-2.1.2/
+-rw-rw-rw-   0        0        0    35823 2021-12-12 22:30:43.000000 telegram_menu-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0       43 2021-12-12 22:30:43.000000 telegram_menu-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7259 2023-08-05 09:42:10.878637 telegram_menu-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6458 2023-05-07 00:10:58.000000 telegram_menu-2.1.2/README.md
+-rw-rw-rw-   0        0        0      102 2023-08-05 09:15:05.000000 telegram_menu-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:42:10.879638 telegram_menu-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2022-01-16 20:03:45.000000 telegram_menu-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:10.863317 telegram_menu-2.1.2/telegram_menu/
+-rw-rw-rw-   0        0        0     1008 2023-02-20 21:30:49.000000 telegram_menu-2.1.2/telegram_menu/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-08-05 09:14:06.000000 telegram_menu-2.1.2/telegram_menu/_version.py
+-rw-rw-rw-   0        0        0    10873 2023-08-05 09:36:47.000000 telegram_menu-2.1.2/telegram_menu/models.py
+-rw-rw-rw-   0        0        0    30847 2023-08-05 09:36:47.000000 telegram_menu-2.1.2/telegram_menu/navigation.py
+-rw-rw-rw-   0        0        0       63 2023-02-20 21:36:29.000000 telegram_menu-2.1.2/telegram_menu/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:10.872634 telegram_menu-2.1.2/telegram_menu.egg-info/
+-rw-rw-rw-   0        0        0     7259 2023-08-05 09:42:10.000000 telegram_menu-2.1.2/telegram_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-08-05 09:42:10.000000 telegram_menu-2.1.2/telegram_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:42:10.000000 telegram_menu-2.1.2/telegram_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-06 22:45:49.000000 telegram_menu-2.1.2/telegram_menu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-08-05 09:42:10.000000 telegram_menu-2.1.2/telegram_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-05 09:42:10.000000 telegram_menu-2.1.2/telegram_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:10.875529 telegram_menu-2.1.2/tests/
+-rw-rw-rw-   0        0        0      713 2023-02-20 21:40:17.000000 telegram_menu-2.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-02-20 21:30:49.000000 telegram_menu-2.1.2/tests/demo.py
+-rw-rw-rw-   0        0        0    21006 2023-08-05 09:39:30.000000 telegram_menu-2.1.2/tests/test_connection.py
```

### Comparing `telegram_menu-2.1.1/LICENSE` & `telegram_menu-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/PKG-INFO` & `telegram_menu-2.1.2/telegram_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telegram_menu
-Version: 2.1.1
+Name: telegram-menu
+Version: 2.1.2
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
```

### Comparing `telegram_menu-2.1.1/README.md` & `telegram_menu-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/setup.py` & `telegram_menu-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/telegram_menu/__init__.py` & `telegram_menu-2.1.2/telegram_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/telegram_menu/_version.py` & `telegram_menu-2.1.2/telegram_menu/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
 """Package description."""
 
 __title__ = "telegram_menu"
 __description__ = "A python library to generate navigation menus using Telegram Bot API."
 __url__ = "https://github.com/mevellea/telegram_menu"
 __raw_url__ = "https://raw.githubusercontent.com/mevellea/telegram_menu/master"
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 __author__ = "Armel Mevellec"
 __author_email__ = "mevellea@gmail.com"
 __license__ = "GNU GPLv3"
 __copyright__ = "Copyright 2020-2023 " + __author__
```

### Comparing `telegram_menu-2.1.1/telegram_menu/models.py` & `telegram_menu-2.1.2/telegram_menu/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     """Button type enumeration."""
 
     NOTIFICATION = auto()
     MESSAGE = auto()
     PICTURE = auto()
     STICKER = auto()
     POLL = auto()
+    LINK = auto()
 
 
 @dataclass
 class MenuButton:
     """Base button class, wrapper for label with callback.
 
     Args:
@@ -240,17 +241,21 @@
         for row in self.keyboard:
             if not self.input_field and row:
                 self.input_field = row[0].label
             button_array: List[InlineKeyboardButton] = []
             for btn in row:
                 lbl = f"{self.label}.{btn.label}"
                 if btn.web_app_url and validators.url(btn.web_app_url):
-                    button_array.append(
-                        InlineKeyboardButton(text=btn.label, web_app=WebAppInfo(url=btn.web_app_url), callback_data=lbl)
-                    )
+                    if btn.btype == ButtonType.LINK:
+                        button_array.append(InlineKeyboardButton(text=btn.label, url=btn.web_app_url))
+                    else:
+                        # do not use callback_data as it is not supported
+                        button_array.append(
+                            InlineKeyboardButton(text=btn.label, web_app=WebAppInfo(url=btn.web_app_url))
+                        )
                 else:
                     button_array.append(InlineKeyboardButton(text=btn.label, callback_data=lbl))
             keyboard_buttons.append(button_array)
         return InlineKeyboardMarkup(inline_keyboard=keyboard_buttons)
 
     def is_alive(self) -> None:
         """Update message timestamp."""
```

### Comparing `telegram_menu-2.1.1/telegram_menu/navigation.py` & `telegram_menu-2.1.2/telegram_menu/navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         self.application.add_handler(MessageHandler(telegram.ext.filters.TEXT, self._button_select_callback))
         self.application.add_handler(
             MessageHandler(telegram.ext.filters.StatusUpdate.WEB_APP_DATA, self._button_webapp_callback)
         )
         self.application.add_handler(CallbackQueryHandler(self._button_inline_select_callback))
         self.application.add_handler(telegram.ext.PollAnswerHandler(self._poll_answer))
         self.application.add_error_handler(self._msg_error_handler)
+        self.application.add_handler(MessageHandler(telegram.ext.filters.LOCATION, self._get_location_handler))
 
     def start(
         self,
         start_message_class: Type[BaseMessage],
         start_message_args: Optional[List[Any]] = None,
         polling: bool = True,
         navigation_handler_class: Optional[Type[NavigationHandler]] = None,
@@ -142,14 +143,21 @@
     def get_session(self, chat_id: int = 0) -> Optional[NavigationHandler]:
         """Get session from list."""
         sessions = [x for x in self.sessions if chat_id in (x.chat_id, 0)]
         if not sessions:
             return None
         return sessions[0]
 
+    async def _get_location_handler(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
+        if update.effective_chat is None or update.message is None or update.message.location is None:
+            raise NavigationException("Incorrect session, location can't be updated")
+        session = self.get_session(update.effective_chat.id)
+        if session is not None:
+            session.location = update.message.location
+
     async def _button_select_callback(self, update: Update, context: CallbackContext[BT, UD, CD, BD]) -> None:
         """Menu message main entry point."""
         if update.effective_chat is None or update.message is None:
             raise NavigationException("Chat object was not created")
         session = self.get_session(update.effective_chat.id)
         if session is None:
             await self._send_start_message(update, context)
@@ -241,14 +249,15 @@
         self._poll: Optional[Message] = None
         self._poll_callback: Optional[TypeCallback] = None
 
         self.scheduler = scheduler
         self.chat_id = chat.id
         self.user_name = chat.first_name
         self.poll_name = f"poll_{self.user_name}"
+        self.location: Optional[telegram.Location] = None
 
         logger.info(f"Opening chat with user {self.user_name}")
 
         self._menu_queue: List[BaseMessage] = []  # list of menus selected by user
         self._message_queue: List[BaseMessage] = []  # list of application messages sent
 
         # check if messages have expired every MESSAGE_CHECK_TIMEOUT seconds
@@ -441,28 +450,31 @@
                 if btn.callback.inlined:
                     msg_id = await self._send_app_message(btn.callback, label, context)
                     if btn.callback.home_after:
                         msg_id = await self.goto_home(context)
                 else:
                     msg_id = await self.goto_menu(btn.callback, context)
             elif btn.callback is not None and hasattr(btn.callback, "__call__"):
-                await call_function_EAFP(btn.callback, context)
+                if btn.args is not None:
+                    await call_function_EAFP(btn.callback, context, btn.args)
+                else:
+                    await call_function_EAFP(btn.callback, context)
             return msg_id
 
         # label does not match any sub-menu, just process the user input
         await self.capture_user_input(label, context)
         return None
 
     async def capture_user_input(self, label: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> None:
         """Process the user input in the last message updated."""
         last_menu_message = self._menu_queue[-1]
         if self._message_queue:
-            last_app_message = self._message_queue[-1]
-            if last_app_message.time_alive > last_menu_message.time_alive:
-                last_menu_message = last_app_message
+            for last_app_message in self._message_queue[::-1]:
+                if last_app_message.time_alive > last_menu_message.time_alive:
+                    last_menu_message = last_app_message
         await last_menu_message.text_input(label, context)
 
     async def app_message_webapp_callback(self, webapp_data: str, button_text: str) -> None:
         """Execute the callback associated to this webapp."""
         last_menu = self._menu_queue[-1]
         webapp_message = next(iter(y for x in last_menu.keyboard for y in x if y.label == button_text), None)
         if webapp_message is not None and callable(webapp_message.callback):
@@ -577,14 +589,15 @@
         try:
             return await self._bot.send_photo(
                 chat_id=self.chat_id,
                 photo=picture_obj,
                 caption=caption,
                 reply_markup=keyboard,
                 disable_notification=not notification,
+                parse_mode=ParseMode.HTML,
             )
         except telegram.error.BadRequest as error:
             logger.error(f"Failed to send picture {picture_path}: {error}")
         return None
 
     async def send_sticker(self, sticker_path: str, notification: bool = True) -> Optional[telegram.Message]:
         """Send a picture."""
```

### Comparing `telegram_menu-2.1.1/telegram_menu.egg-info/PKG-INFO` & `telegram_menu-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telegram-menu
-Version: 2.1.1
+Name: telegram_menu
+Version: 2.1.2
 Summary: A python library to generate navigation menus using Telegram Bot API.
 Home-page: https://github.com/mevellea/telegram_menu
 Author: Armel Mevellec
 Author-email: mevellea@gmail.com
 License: GNU GPLv3
 Keywords: telegram
 Platform: any
```

### Comparing `telegram_menu-2.1.1/tests/__init__.py` & `telegram_menu-2.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/tests/demo.py` & `telegram_menu-2.1.2/tests/demo.py`

 * *Files identical despite different names*

### Comparing `telegram_menu-2.1.1/tests/test_connection.py` & `telegram_menu-2.1.2/tests/test_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 from telegram import InlineKeyboardMarkup, Message, ReplyKeyboardMarkup
 
 try:
     from typing_extensions import TypedDict
 except ImportError:
     from typing import TypedDict
 
+from telegram.ext._callbackcontext import CallbackContext
+from telegram.ext._utils.types import BD, BT, CD, UD
+
 import telegram_menu
 from telegram_menu import BaseMessage, ButtonType, MenuButton, NavigationHandler, TelegramMenuSession
 from telegram_menu._version import __raw_url__
 
 KeyboardContent = List[Union[str, List[str]]]
 UpdateCallback = Union[Callable[[Any], None], Coroutine[Any, Any, None]]
 KeyboardTester = TypedDict("KeyboardTester", {"buttons": int, "output": List[int]})
@@ -191,18 +194,18 @@
         if edited:
             self.is_alive()
 
     def update(self) -> str:
         """Update message content."""
         return "Third message"
 
-    async def text_input(self, text: str) -> None:
+    async def text_input(self, text: str, context: Optional[CallbackContext[BT, UD, CD, BD]] = None) -> None:
         """Process text received."""
-        msg_id = await self.navigation.select_menu_button("Action")
-        await self.navigation.delete_message(message_id=msg_id)
+        logging.info(f"Text received: {text}")
+        await self.navigation.select_menu_button("Action")
 
 
 class SecondMenuMessage(BaseMessage):
     """Second example of menu."""
 
     LABEL = "second_message"
```

