# Comparing `tmp/vlcsync-0.2.0.tar.gz` & `tmp/vlcsync-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlcsync-0.2.0.tar", max compression
+gzip compressed data, was "vlcsync-0.2.1.tar", max compression
```

## Comparing `vlcsync-0.2.0.tar` & `vlcsync-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2022-04-29 00:02:43.380289 vlcsync-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     3063 2022-11-04 23:31:32.379868 vlcsync-0.2.0/README.md
--rw-r--r--   0        0        0     1092 2022-11-04 23:29:50.924255 vlcsync-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-27 21:36:53.816975 vlcsync-0.2.0/vlcsync/__init__.py
--rw-r--r--   0        0        0     1382 2022-11-04 23:29:50.968253 vlcsync-0.2.0/vlcsync/cli.py
--rw-r--r--   0        0        0      883 2022-11-04 23:29:50.972252 vlcsync-0.2.0/vlcsync/cli_utils.py
--rwxr-xr-x   0        0        0      303 2022-11-04 23:29:50.992251 vlcsync-0.2.0/vlcsync/main.py
--rw-r--r--   0        0        0     2503 2022-11-04 23:29:51.000251 vlcsync-0.2.0/vlcsync/syncer.py
--rw-r--r--   0        0        0     5856 2022-11-04 23:29:51.008251 vlcsync-0.2.0/vlcsync/vlc.py
--rw-r--r--   0        0        0     2662 2022-11-04 23:29:51.008251 vlcsync-0.2.0/vlcsync/vlc_finder.py
--rw-r--r--   0        0        0     1850 2022-11-04 23:29:51.008251 vlcsync-0.2.0/vlcsync/vlc_socket.py
--rw-r--r--   0        0        0     2442 2022-11-04 23:29:51.008251 vlcsync-0.2.0/vlcsync/vlc_state.py
--rw-r--r--   0        0        0     3993 2022-11-05 00:14:47.164321 vlcsync-0.2.0/setup.py
--rw-r--r--   0        0        0     4120 2022-11-05 00:14:47.164756 vlcsync-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-04-29 00:02:43.380289 vlcsync-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     3064 2023-08-05 01:06:01.048897 vlcsync-0.2.1/README.md
+-rw-r--r--   0        0        0     1092 2023-08-05 01:09:54.347326 vlcsync-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-27 21:36:53.816975 vlcsync-0.2.1/vlcsync/__init__.py
+-rw-r--r--   0        0        0     1382 2023-08-05 01:09:54.347326 vlcsync-0.2.1/vlcsync/cli.py
+-rw-r--r--   0        0        0      883 2022-11-05 00:49:33.486641 vlcsync-0.2.1/vlcsync/cli_utils.py
+-rwxr-xr-x   0        0        0      303 2022-11-04 23:29:50.992251 vlcsync-0.2.1/vlcsync/main.py
+-rw-r--r--   0        0        0     2503 2023-08-05 00:47:05.227453 vlcsync-0.2.1/vlcsync/syncer.py
+-rw-r--r--   0        0        0     5856 2023-08-05 00:47:05.227453 vlcsync-0.2.1/vlcsync/vlc.py
+-rw-r--r--   0        0        0     2727 2023-08-05 01:09:54.347326 vlcsync-0.2.1/vlcsync/vlc_finder.py
+-rw-r--r--   0        0        0     1850 2022-11-04 23:29:51.008251 vlcsync-0.2.1/vlcsync/vlc_socket.py
+-rw-r--r--   0        0        0     2442 2023-08-05 00:47:05.227453 vlcsync-0.2.1/vlcsync/vlc_state.py
+-rw-r--r--   0        0        0     3994 2023-08-05 01:11:33.840380 vlcsync-0.2.1/setup.py
+-rw-r--r--   0        0        0     4121 2023-08-05 01:11:33.840838 vlcsync-0.2.1/PKG-INFO
```

### Comparing `vlcsync-0.2.0/LICENSE.md` & `vlcsync-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/README.md` & `vlcsync-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,22 @@
   - Linux (Ubuntu 20.04)
   - Windows 7 (32-bit)
   - Windows 10 (64-bit)
 
 ## Alternatives
 
 - [vlc](https://www.videolan.org/vlc/index.ru.html) 
-    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reeason)
+    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reason)
     - Open additional media. Seems feature broken in vlc 3 (also afaik limited only 2 streams)  
 - [Syncplay](https://github.com/Syncplay/syncplay) - very promised, but little [complicated](https://github.com/Syncplay/syncplay/discussions/463) for sync different videos
 - [bino](https://bino3d.org/) - working, very strange controls, file dialog not working and only fullscreen
 - [gridplayer](https://github.com/vzhd1701/gridplayer) - low fps by some reason
 - [mpv](https://github.com/mpv-player/mpv) - with [mixing multiple videos](https://superuser.com/a/1325668/1272472) in one window. Unfortunally does not support multiple screens
 - [AVPlayer](http://www.awesomevideoplayer.com/) - only Win, macOS, up to 4 videos in free version
 
 ## Contributing
 
 Any thoughts, ideas and contributions welcome!
 
-Special thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>
+A special thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>
 
 Enjoy!
```

### Comparing `vlcsync-0.2.0/pyproject.toml` & `vlcsync-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vlcsync"
-version = "0.2.0"
+version = "0.2.1"
 description = "Utility for synchronize multiple instances of VLC. Supports seek, play and pause. "
 authors = ["mrkeuz <mrkeuz@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mrkeuz/vlcsync/"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `vlcsync-0.2.0/vlcsync/cli.py` & `vlcsync-0.2.1/vlcsync/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import click
 
 from vlcsync.cli_utils import parse_url
 from vlcsync.syncer import AppConfig, Syncer
 from vlcsync.vlc_finder import print_exc
 from vlcsync.vlc_state import VlcId
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 @click.command
 @click.version_option(__version__)
 @click.option("--rc-host",
               'rc_host_list',
               help='Additional players (can be multiple).',
```

### Comparing `vlcsync-0.2.0/vlcsync/cli_utils.py` & `vlcsync-0.2.1/vlcsync/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/vlcsync/syncer.py` & `vlcsync-0.2.1/vlcsync/syncer.py`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/vlcsync/vlc.py` & `vlcsync-0.2.1/vlcsync/vlc.py`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/vlcsync/vlc_finder.py` & `vlcsync-0.2.1/vlcsync/vlc_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,23 +71,23 @@
 
         # noinspection PyUnreachableCode
         return None
 
     @functools.lru_cache(maxsize=1024)
     def is_vlc(self, proc: Process):
         with skip_on_error():
-            return proc.name() == 'vlc' or self.vlc_cmdline(proc)
+            return proc.name() is not None and proc.name().lower() == 'vlc' or self.vlc_cmdline(proc)
 
         # noinspection PyUnreachableCode
         return False
 
     @staticmethod
     def vlc_cmdline(proc) -> bool:
         for part in proc.cmdline():
-            if 'vlc' in part:
+            if part is not None and 'vlc' in part.lower():
                 return True
         return False
 
 
 def print_exc():
     print("-" * 60)
     print("Exception in user code: ")
```

### Comparing `vlcsync-0.2.0/vlcsync/vlc_socket.py` & `vlcsync-0.2.1/vlcsync/vlc_socket.py`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/vlcsync/vlc_state.py` & `vlcsync-0.2.1/vlcsync/vlc_state.py`

 * *Files identical despite different names*

### Comparing `vlcsync-0.2.0/setup.py` & `vlcsync-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['cached-property', 'click>=8.1.3,<9.0.0', 'loguru', 'psutil']
 
 entry_points = \
 {'console_scripts': ['vlcsync = vlcsync.main:main']}
 
 setup_kwargs = {
     'name': 'vlcsync',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Utility for synchronize multiple instances of VLC. Supports seek, play and pause. ',
-    'long_description': 'VLC Sync\n========\n\nUtility for synchronize multiple instances of VLC. Supports seek, play and pause. \n  \n\n#### Motivation\n\nStrongly inspired by F1 streams with extra driver tracking data streams. Did [not find](#alternatives) reasonable alternative for Linux for playing several videos synchronously. So decided to write my own solution.\n\n## Install\n\n```shell\npip3 install -U vlcsync\n```\n\nor \n\n- Download [binary release](https://github.com/mrkeuz/vlcsync/releases) for Windows 7/10  \n  NOTE: On some systems there are false positive Antivirus warnings [issues](https://github.com/mrkeuz/vlcsync/issues/1).\n  In this case use [alternative way](./docs/install.md#windows-detailed-instructions) to install.   \n\n## Run\n\n`Vlc` players should open with `--rc-host 127.0.0.42` option OR configured properly from gui (see [how configure vlc](./docs/vlc_setup.md)) \n\n```shell\n\n# Run vlc players \n$ vlc --rc-host 127.0.0.42 SomeMedia1.mkv &\n$ vlc --rc-host 127.0.0.42 SomeMedia2.mkv &\n$ vlc --rc-host 127.0.0.42 SomeMedia3.mkv &\n\n# vlcsync will monitor and syncing all players\n$ vlcsync\n\n# Started from version 0.2.0\n\n# For control remote vlc instances, \n# remote port should be open and rc interface listen on 0.0.0.0\n$ vlcsync --rc-host 192.168.1.100:12345 --rc-host 192.168.1.50:54321\n\n# For disable local discovery (only remote instances)\n$ vlcsync --no-local-discovery --rc-host 192.168.1.100:12345\n\n# For help and see all options\n$ vlcsync --help\n```\n\n## Awesome \n\nAwesome [use-case](./docs/awesome.md) ideas\n\n## Demo\n\n![vlcsync](./docs/vlcsync.gif)\n\n## Limitations \n\n- Frame-to-frame sync NOT provided. `vlc` does not have precise controlling via `rc` interface out of box. \n  Difference between videos can be **up to ~0.5 seconds** in worst case. Especially when playing from network share, \n  due buffering time and network latency.\n\n- Currently, tested only on:\n  - Linux (Ubuntu 20.04)\n  - Windows 7 (32-bit)\n  - Windows 10 (64-bit)\n\n## Alternatives\n\n- [vlc](https://www.videolan.org/vlc/index.ru.html) \n    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reeason)\n    - Open additional media. Seems feature broken in vlc 3 (also afaik limited only 2 streams)  \n- [Syncplay](https://github.com/Syncplay/syncplay) - very promised, but little [complicated](https://github.com/Syncplay/syncplay/discussions/463) for sync different videos\n- [bino](https://bino3d.org/) - working, very strange controls, file dialog not working and only fullscreen\n- [gridplayer](https://github.com/vzhd1701/gridplayer) - low fps by some reason\n- [mpv](https://github.com/mpv-player/mpv) - with [mixing multiple videos](https://superuser.com/a/1325668/1272472) in one window. Unfortunally does not support multiple screens\n- [AVPlayer](http://www.awesomevideoplayer.com/) - only Win, macOS, up to 4 videos in free version\n\n## Contributing\n\nAny thoughts, ideas and contributions welcome!\n\nSpecial thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>\n\nEnjoy!\n',
+    'long_description': 'VLC Sync\n========\n\nUtility for synchronize multiple instances of VLC. Supports seek, play and pause. \n  \n\n#### Motivation\n\nStrongly inspired by F1 streams with extra driver tracking data streams. Did [not find](#alternatives) reasonable alternative for Linux for playing several videos synchronously. So decided to write my own solution.\n\n## Install\n\n```shell\npip3 install -U vlcsync\n```\n\nor \n\n- Download [binary release](https://github.com/mrkeuz/vlcsync/releases) for Windows 7/10  \n  NOTE: On some systems there are false positive Antivirus warnings [issues](https://github.com/mrkeuz/vlcsync/issues/1).\n  In this case use [alternative way](./docs/install.md#windows-detailed-instructions) to install.   \n\n## Run\n\n`Vlc` players should open with `--rc-host 127.0.0.42` option OR configured properly from gui (see [how configure vlc](./docs/vlc_setup.md)) \n\n```shell\n\n# Run vlc players \n$ vlc --rc-host 127.0.0.42 SomeMedia1.mkv &\n$ vlc --rc-host 127.0.0.42 SomeMedia2.mkv &\n$ vlc --rc-host 127.0.0.42 SomeMedia3.mkv &\n\n# vlcsync will monitor and syncing all players\n$ vlcsync\n\n# Started from version 0.2.0\n\n# For control remote vlc instances, \n# remote port should be open and rc interface listen on 0.0.0.0\n$ vlcsync --rc-host 192.168.1.100:12345 --rc-host 192.168.1.50:54321\n\n# For disable local discovery (only remote instances)\n$ vlcsync --no-local-discovery --rc-host 192.168.1.100:12345\n\n# For help and see all options\n$ vlcsync --help\n```\n\n## Awesome \n\nAwesome [use-case](./docs/awesome.md) ideas\n\n## Demo\n\n![vlcsync](./docs/vlcsync.gif)\n\n## Limitations \n\n- Frame-to-frame sync NOT provided. `vlc` does not have precise controlling via `rc` interface out of box. \n  Difference between videos can be **up to ~0.5 seconds** in worst case. Especially when playing from network share, \n  due buffering time and network latency.\n\n- Currently, tested only on:\n  - Linux (Ubuntu 20.04)\n  - Windows 7 (32-bit)\n  - Windows 10 (64-bit)\n\n## Alternatives\n\n- [vlc](https://www.videolan.org/vlc/index.ru.html) \n    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reason)\n    - Open additional media. Seems feature broken in vlc 3 (also afaik limited only 2 streams)  \n- [Syncplay](https://github.com/Syncplay/syncplay) - very promised, but little [complicated](https://github.com/Syncplay/syncplay/discussions/463) for sync different videos\n- [bino](https://bino3d.org/) - working, very strange controls, file dialog not working and only fullscreen\n- [gridplayer](https://github.com/vzhd1701/gridplayer) - low fps by some reason\n- [mpv](https://github.com/mpv-player/mpv) - with [mixing multiple videos](https://superuser.com/a/1325668/1272472) in one window. Unfortunally does not support multiple screens\n- [AVPlayer](http://www.awesomevideoplayer.com/) - only Win, macOS, up to 4 videos in free version\n\n## Contributing\n\nAny thoughts, ideas and contributions welcome!\n\nA special thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>\n\nEnjoy!\n',
     'author': 'mrkeuz',
     'author_email': 'mrkeuz@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mrkeuz/vlcsync/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vlcsync-0.2.0/PKG-INFO` & `vlcsync-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlcsync
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility for synchronize multiple instances of VLC. Supports seek, play and pause. 
 Home-page: https://github.com/mrkeuz/vlcsync/
 License: MIT
 Author: mrkeuz
 Author-email: mrkeuz@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -93,23 +93,23 @@
   - Linux (Ubuntu 20.04)
   - Windows 7 (32-bit)
   - Windows 10 (64-bit)
 
 ## Alternatives
 
 - [vlc](https://www.videolan.org/vlc/index.ru.html) 
-    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reeason)
+    - There is a [netsync](https://wiki.videolan.org/Documentation:Modules/netsync/) but seem only master-slave (tried, but not working by some reason)
     - Open additional media. Seems feature broken in vlc 3 (also afaik limited only 2 streams)  
 - [Syncplay](https://github.com/Syncplay/syncplay) - very promised, but little [complicated](https://github.com/Syncplay/syncplay/discussions/463) for sync different videos
 - [bino](https://bino3d.org/) - working, very strange controls, file dialog not working and only fullscreen
 - [gridplayer](https://github.com/vzhd1701/gridplayer) - low fps by some reason
 - [mpv](https://github.com/mpv-player/mpv) - with [mixing multiple videos](https://superuser.com/a/1325668/1272472) in one window. Unfortunally does not support multiple screens
 - [AVPlayer](http://www.awesomevideoplayer.com/) - only Win, macOS, up to 4 videos in free version
 
 ## Contributing
 
 Any thoughts, ideas and contributions welcome!
 
-Special thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>
+A special thanks to **KorDen32** for inspiration! <img src="./docs/F1.svg" alt="F1" width="45"/>
 
 Enjoy!
```

