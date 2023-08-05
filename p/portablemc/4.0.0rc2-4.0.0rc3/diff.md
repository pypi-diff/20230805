# Comparing `tmp/portablemc-4.0.0rc2.tar.gz` & `tmp/portablemc-4.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portablemc-4.0.0rc2.tar", max compression
+gzip compressed data, was "portablemc-4.0.0rc3.tar", max compression
```

## Comparing `portablemc-4.0.0rc2.tar` & `portablemc-4.0.0rc3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-07-14 20:55:06.871777 portablemc-4.0.0rc2/LICENSE
--rw-r--r--   0        0        0    14683 2023-07-29 19:17:52.174139 portablemc-4.0.0rc2/README.md
--rw-r--r--   0        0        0      306 2023-07-29 21:27:01.773514 portablemc-4.0.0rc2/portablemc/__init__.py
--rw-r--r--   0        0        0      800 2023-07-14 20:55:06.888443 portablemc-4.0.0rc2/portablemc/__main__.py
--rw-r--r--   0        0        0    16930 2023-07-29 18:39:34.554294 portablemc-4.0.0rc2/portablemc/auth.py
--rw-r--r--   0        0        0    28713 2023-07-29 22:06:41.150534 portablemc-4.0.0rc2/portablemc/cli/__init__.py
--rw-r--r--   0        0        0    13780 2023-07-29 19:58:42.262680 portablemc-4.0.0rc2/portablemc/cli/lang.py
--rw-r--r--   0        0        0     9442 2023-07-29 20:10:30.949309 portablemc-4.0.0rc2/portablemc/cli/output.py
--rw-r--r--   0        0        0     7297 2023-07-29 19:06:02.641566 portablemc-4.0.0rc2/portablemc/cli/parse.py
--rw-r--r--   0        0        0     3034 2023-07-28 21:45:28.559579 portablemc-4.0.0rc2/portablemc/cli/util.py
--rw-r--r--   0        0        0    12222 2023-07-29 20:26:00.437021 portablemc-4.0.0rc2/portablemc/download.py
--rw-r--r--   0        0        0     5322 2023-07-29 16:13:33.741775 portablemc-4.0.0rc2/portablemc/fabric.py
--rw-r--r--   0        0        0    18738 2023-07-29 16:13:49.891610 portablemc-4.0.0rc2/portablemc/forge.py
--rw-r--r--   0        0        0     2373 2023-07-15 10:13:00.771725 portablemc-4.0.0rc2/portablemc/http.py
--rw-r--r--   0        0        0    75274 2023-07-29 21:36:43.490242 portablemc-4.0.0rc2/portablemc/standard.py
--rw-r--r--   0        0        0     5040 2023-07-23 13:48:34.873644 portablemc-4.0.0rc2/portablemc/util.py
--rw-r--r--   0        0        0      961 2023-07-30 10:28:46.744101 portablemc-4.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    15730 1970-01-01 00:00:00.000000 portablemc-4.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 20:55:06.871777 portablemc-4.0.0rc3/LICENSE
+-rw-r--r--   0        0        0    14805 2023-07-30 19:22:32.107153 portablemc-4.0.0rc3/README.md
+-rw-r--r--   0        0        0      306 2023-07-30 14:07:08.487761 portablemc-4.0.0rc3/portablemc/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-14 20:55:06.888443 portablemc-4.0.0rc3/portablemc/__main__.py
+-rw-r--r--   0        0        0    16930 2023-07-29 18:39:34.554294 portablemc-4.0.0rc3/portablemc/auth.py
+-rw-r--r--   0        0        0    28770 2023-07-30 15:55:28.233277 portablemc-4.0.0rc3/portablemc/cli/__init__.py
+-rw-r--r--   0        0        0    13878 2023-07-30 12:44:18.083445 portablemc-4.0.0rc3/portablemc/cli/lang.py
+-rw-r--r--   0        0        0     9442 2023-07-29 20:10:30.949309 portablemc-4.0.0rc3/portablemc/cli/output.py
+-rw-r--r--   0        0        0     7311 2023-07-30 11:54:39.099223 portablemc-4.0.0rc3/portablemc/cli/parse.py
+-rw-r--r--   0        0        0     3034 2023-07-28 21:45:28.559579 portablemc-4.0.0rc3/portablemc/cli/util.py
+-rw-r--r--   0        0        0    14122 2023-07-30 19:22:32.110486 portablemc-4.0.0rc3/portablemc/download.py
+-rw-r--r--   0        0        0     5322 2023-07-29 16:13:33.741775 portablemc-4.0.0rc3/portablemc/fabric.py
+-rw-r--r--   0        0        0    19253 2023-07-30 13:05:15.136092 portablemc-4.0.0rc3/portablemc/forge.py
+-rw-r--r--   0        0        0     2373 2023-07-15 10:13:00.771725 portablemc-4.0.0rc3/portablemc/http.py
+-rw-r--r--   0        0        0    75654 2023-07-30 15:55:14.820080 portablemc-4.0.0rc3/portablemc/standard.py
+-rw-r--r--   0        0        0     5040 2023-07-23 13:48:34.873644 portablemc-4.0.0rc3/portablemc/util.py
+-rw-r--r--   0        0        0      961 2023-07-30 14:07:01.287822 portablemc-4.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    15852 1970-01-01 00:00:00.000000 portablemc-4.0.0rc3/PKG-INFO
```

### Comparing `portablemc-4.0.0rc2/LICENSE` & `portablemc-4.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/README.md` & `portablemc-4.0.0rc3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Portable Minecraft Launcher
-A fast, reliable and cross-platform command line Minecraft launcher and API for developers.
-This launcher is compatible with the official Minecraft launcher' version specification.
+A fast, reliable and cross-platform command-line Minecraft launcher and API for developers.
+This launcher is compatible with the official Minecraft launcher's version specification.
 It also includes fast installation of common mod loaders such as Fabric, Forge and Quilt.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/portablemc?label=PyPI%20version&style=flat-square) &nbsp;![PyPI - Downloads](https://img.shields.io/pypi/dm/portablemc?label=PyPI%20downloads&style=flat-square)
 
 ![illustration](doc/assets/illustration.png)
 
 *This launcher is tested for Python 3.7, 3.8, 3.9, 3.10, 3.11.*
@@ -34,87 +34,91 @@
 use `pip3` instead of `pip` in order to run it on Python 3. You can also use 
 `python -m pip` if the `pip` command is not in the path and the python executable is.
 
 ```sh
 pip install --user portablemc
 ```
 
-It's recommended to keep `--user` because this allows to install the launcher for your
+It's recommended to keep `--user` because this installs the launcher for your
 current user only, it is implicit if you are not an administrator and if you are, it 
 allows not to modify other users' installations.
 
 After that, you can try to show the launcher help message using `portablemc` in your 
 terminal. If it fails, you should check that the scripts directory is in your user path
 environment variable. On Windows you have to search for a directory at 
 `%appdata%/Python/Python3X/Scripts` and add it to the user's environment variable `Path`. 
 On UNIX systems it's `~/.local/bin`.
 
 ## Commands
 Arguments are split between multiple commands. 
 For example `portablemc [global-args] <cmd> [args]`. 
-You can use `-h` argument to display help *(also works for every sub-commands)*.
+You can use `-h` argument to display help *(also works for every sub-command)*.
 
 By default the launcher will run any command from the OS standard `.minecraft` directory 
 ([check wiki for more information](https://minecraft.gamepedia.com/.minecraft)). You can
 change this directory using `--main-dir <path>` global argument.
 
 You may also need `--work-dir <path>` to change the directory where your saves, resource 
 packs and all "user-specific" content is stored. This can be useful if you have a shared 
 read-only main directory (`--main-dir`) and user-specific working directory (for example 
 in `.minecraft`, by default it's the location of your main directory). The launcher also
 stores cached version manifest and authentication database in the working directory.
 
-The two arguments `--main-dir` and `--work-dir` may or may not be used by sub commands, 
-but they are always valid to use, allowing you to define command alias for running
+The two arguments `--main-dir` and `--work-dir` may or may not be used by sub-commands, 
+but they are always valid to use, allowing you to define command aliases for running
 PortableMC.
 
 Another argument, `--timeout <seconds>` can be used to set a global timeout value that 
 will be used for all network connections.
 
 The general output format of the launcher can be changed using the `--output <mode>` with
 one of the following modes:
 - `human`: Human readable output, translated messages, formatted tables and tasks.
 - `human-color`: Default, same as `human` but with some color where relevant, like tasks 
-  states and game's logs.
+  states and game logs.
 - `machine`: Machine
 
 The verbosity of the launcher can be adjusted if you encounter issues, using multiple 
 `-v` arguments (usually `-v` through `-vvv`). It's very useful to maintainers when fixing 
 issues.
 
 ### Start Minecraft
 The first thing you may want to do is install and start Minecraft, to do so you can use
 the `portablemc start [args] [version]` command. This command will install every component
 needed by the version before launching it. If you provide no version, the latest release
-is started, but you can specify a specific version launch, or a version alias: `release`
-or `snapshot` for latest version of their type.
+is started, but you can specify a version to launch, or a version alias: `release`
+or `snapshot` for the latest version of their type.
 
-In addition to Mojang's vanilla versions, the launcher natively support common mod
-loaders such as **Fabric**, **Forge** and **Quilt**. To start such version, you can
+In addition to Mojang's vanilla versions, the launcher natively supports common mod
+loaders such as **Fabric**, **Forge** and **Quilt**. To start such versions, you can
 prefix the version with either `fabric:`, `forge:` or `quilt:` (or `vanilla:` to
-explicitly choose vanilla version).
+explicitly choose a vanilla version).
 Depending on the mod loader, the version you put after the colon is different:
 - For Fabric and Quilt, you can directly specify the vanilla version, optionally followed
-  by `:<loader_version>`.
+  by `:<loader_version>`:  
+  `fabric:1.20.1`  
+  `fabric:1.20.1:0.11.2`
 - For Forge, you can put either a vanilla game version, optionally followed by `-latest`
-  or `-recommended`, or `-<loader_version>`.
+  or `-recommended`, or `-<loader_version>`:  
+  `forge:1.20-latest`  
+  `forge:1.20-46.0.14`
 
 *You can search for versions using the [search command](#search-for-versions).*
 
 #### Authentication
 Online mode is supported by this launcher, use the `-l <email_or_username>` (`--login`)
 argument to log into your account *(login with a username is deprecated by Mojang)*. 
 If your session is not cached or no longer valid, the launcher will ask for the 
 password or open the Microsoft connection page.
 
 **By default**, this will authenticate you using the Microsoft authentication services,
-you can change that using `--auth-service` argument, for example with `yggdrasil` if
-you need to log into an old Mojang account (being phased out by Mojang).
+although you can change that using the `--auth-service` argument, for example with
+`yggdrasil` if you need to log into an old Mojang account (being phased out by Mojang).
 
-If you want to be asked for password on each authentication, you can use `-t
+If you want to be asked for password on each authentication, you can use `-t`
 (`--temp-login`). This has no effect if the session is already cached before that.
 
 You can also use `--auth-anonymize` in order to hide most of your email when printing 
 it to the terminal. For example, `foo.bar@gmail.com` will become `f*****r@g***l.com`,
 this is useful to avoid leaking it when recording or streaming.
 However, if you use this, make sure that you either use an alias or a variable with the
 `-l` argument, for exemple `-l $PMC_LOGIN`.
@@ -168,15 +172,15 @@
 `export MESA_GL_VERSION_OVERRIDE=4.5` 
 ([more info here](https://forum.winehq.org/viewtopic.php?f=8&t=34889)).
 
 In case with the above you still get an `error: GLSL 1.50 is not supported` you may also 
 try `export MESA_GLSL_VERSION_OVERRIDE=150`.
 
 #### Fix unsupported systems
-Some Mojang provided natives (.so, .dll, .dylib) might not be compatible with your system.
+Some Mojang-provided natives (.so, .dll, .dylib) might not be compatible with your system.
 To mitigate that, the launcher provides two arguments, `--exclude-lib` and `--include-bin`
 that can be provided multiples times each.
 
 With `--exclude-lib <artifact>[:[<version>][:<classifier>]]` you can exclude libraries 
 (.jar) from the game's classpath (and so of the downloads). If a classifier is given, it
 will match libs' classifiers that starts with itself, for example `lwjgl-glfw::natives`
 will match the library `lwjgl-glfw:3.3.1:natives-windows-x86`.
@@ -187,37 +191,37 @@
 Windows). For shared objects files (.so) that contains version numbers in the filename,
 these are discarded in the bin directory, for example 
 `/lib/libglfw.so.3 -> .minecraft/bin/<uuid>/libglfw.so`.
 
 These arguments can be used together to fix various issues (e.g. wrong libc being linked
 by the LWJGL-provided natives).
 
-*Note that these arguments are compatible, and executed after the `--lwjgl` argument.
+*Note that these arguments are compatible with, and executed after the `--lwjgl` argument.
 You must however ensure that excluded lib and included binaries are compatible.*
 
 #### Miscellaneous
-With `--dry`, the start command do not start the game, but install it.
+With `--dry`, the start command does not start the game, but simply installs it.
 
 With `--demo` you can enable the [demo mode](https://minecraft.gamepedia.com/Demo_mode) 
 of the game.  
 
 With `--resolution <width>x<height>` you can change the resolution of the game window.
 
-The two arguments `--disable-mp` (mp: multiplayer), `--disable-chat` respectively to 
-disable multiplayer button and disable in-game chat *(since 1.16)*.
+The two arguments `--disable-mp` (mp: multiplayer) and `--disable-chat` can respectively
+disable the multiplayer button and the in-game chat *(since 1.16)*.
 
 ### Search for versions
 The `portablemc search [-k <kind>] [version]` sub-command is used to search for versions. 
 By default, this command will search for official Mojang versions available to download, 
-you can instead search for many kind of versions using the `-k` (`--kind`) arguments:
+you can instead search for many kinds of versions using the `-k` (`--kind`) arguments:
 - `local`, show all installed versions.
-- `forge`, show all recommended and latest forge loader versions *(only 1.5.2 and 
+- `forge`, show all recommended and latest Forge loader versions *(only 1.5.2 and 
   onward can be started)*.
-- `fabric`, show all available fabric loader versions.
-- `quilt`, show all available quilt loader versions.
+- `fabric`, show all available Fabric loader versions.
+- `quilt`, show all available Quilt loader versions.
 
 The search string is optional, if not specified no filter is applied on the table shown.
 
 ### Authentication sessions
 Two subcommands allow you to store or logout of sessions: `portablemc login|logout <email_or_username>`.
 These subcommands don't prevent you from using the `-l` (`--login`) argument when starting
 the game, these are just here to manage the session storage.
```

### Comparing `portablemc-4.0.0rc2/portablemc/__main__.py` & `portablemc-4.0.0rc3/portablemc/__main__.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/auth.py` & `portablemc-4.0.0rc3/portablemc/auth.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/cli/__init__.py` & `portablemc-4.0.0rc3/portablemc/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,16 +373,16 @@
     except ForgeInstallError as error:
         ns.out.task("FAILED", f"start.forge.install_error.{error.code}")
         ns.out.finish()
 
     except DownloadError as error:
         ns.out.task("FAILED", None)
         ns.out.finish()
-        for entry, code in error.errors:
-            ns.out.task(None, "download.error", name=entry.name, message=_(f"download.error.{code}"))
+        for entry, code, _origin in error.errors:
+            ns.out.task(None, "download.error", name=entry.url, message=_(f"download.error.{code}"))
             ns.out.finish()
     
     sys.exit(EXIT_FAILURE)
 
 def cmd_start_handler(ns: StartNs, kind: str, parts: List[str]) -> Optional[Version]:
     """This function handles particular kind of versions. If this function successfully
     decodes, the corresponding version should be returned. The global version's format 
@@ -709,15 +709,15 @@
             else:
                 ns.out.task("OK", "start.forge.resolved", version=e.forge_version)
                 ns.out.finish()
 
         super().__init__({
             VersionLoadingEvent: lambda e: progress_task("start.version.loading", version=e.version),
             VersionFetchingEvent: lambda e: progress_task("start.version.fetching", version=e.version),
-            VersionLoadedEvent: lambda e: finish_task("start.version.loaded", version=e.version),
+            VersionLoadedEvent: lambda e: finish_task("start.version.loaded.fetched" if e.fetched else "start.version.loaded", version=e.version),
             FeaturesEvent: features,
             JvmLoadingEvent: lambda e: progress_task("start.jvm.loading"),
             JvmLoadedEvent: lambda e: finish_task(f"start.jvm.loaded.{e.kind}", version=e.version or ""),
             JarFoundEvent: lambda e: finish_task("start.jar.found"),
             AssetsResolveEvent: assets_resolve,
             LibrariesResolvingEvent: lambda e: progress_task("start.libraries.resolving"),
             LibrariesResolvedEvent: libraries_resolved,
```

### Comparing `portablemc-4.0.0rc2/portablemc/cli/lang.py` & `portablemc-4.0.0rc3/portablemc/cli/lang.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     :return: Translated message, or the key itself if not found.
     """
     return get_raw(key, kwargs)
 
 
 lang = {
     # Addons
-    "addon.import_error": "The addon '{addon}' has failed to build because some packages is missing:",
-    "addon.unknown_error": "The addon '{addon}' has failed to build for unknown reason:",
+    # "addon.import_error": "The addon '{addon}' has failed to build because some packages is missing:",
+    # "addon.unknown_error": "The addon '{addon}' has failed to build for unknown reason:",
     # Args root
     "args": "PortableMC is an easy to use portable Minecraft launcher in only one Python "
         "script! This single-script launcher is still compatible with the official "
         "(Mojang) Minecraft Launcher stored in .minecraft and use it.",
     "args.main_dir": "Set the main directory where libraries, assets and versions. "
         "This argument can be used or not by subcommand.",
     "args.work_dir": "Set the working directory where the game run and place for examples "
@@ -102,17 +102,17 @@
     "args.logout.microsoft": "Logout from a Microsoft account.",
     # Args show
     "args.show": "Show and debug various data.",
     "args.show.about": "Display authors, version and license of PortableMC.",
     "args.show.auth": "Debug the authentication database and supported services.",
     "args.show.lang": "Debug the language mappings used for messages translation.",
     # Args addon
-    "args.addon": "Addons management subcommands.",
-    "args.addon.list": "List addons.",
-    "args.addon.show": "Show an addon details.",
+    # "args.addon": "Addons management subcommands.",
+    # "args.addon.list": "List addons.",
+    # "args.addon.show": "Show an addon details.",
     # Common
     "echo": "{echo}",
     "cancelled": "Cancelled.",
     "keyboard_interrupt": "Keyboard interrupted.",
     # Common errors
     "error.os": "An unexpected OS error happened:",
     "error.socket": "This operation requires an operational network, but a socket error happened:",
@@ -127,28 +127,29 @@
     "search.loader_version": "Loader version",
     # Command logout
     "logout.yggdrasil.pending": "Logging out {email} from Mojang...",
     "logout.microsoft.pending": "Logging out {email} from Microsoft...",
     "logout.success": "Logged out {email}",
     "logout.unknown_session": "No session for {email}",
     # Command addon list
-    "addon.list.id": "ID ({count})",
-    "addon.list.version": "Version",
-    "addon.list.authors": "Authors",
+    # "addon.list.id": "ID ({count})",
+    # "addon.list.version": "Version",
+    # "addon.list.authors": "Authors",
     # Command addon show
-    "addon.show.not_found": "Addon '{addon}' not found.",
-    "addon.show.version": "Version: {version}",
-    "addon.show.authors": "Authors: {authors}",
-    "addon.show.description": "Description: {description}",
+    # "addon.show.not_found": "Addon '{addon}' not found.",
+    # "addon.show.version": "Version: {version}",
+    # "addon.show.authors": "Authors: {authors}",
+    # "addon.show.description": "Description: {description}",
     # Command start
     "start.version.invalid_id": "Invalid version id, expected: {expected}",
     "start.version.invalid_id_unknown_kind": "Invalid version id, unknown kind: {kind}.",
     "start.version.loading": "Loading version {version}... ",
     "start.version.fetching": "Fetching version {version}... ",
     "start.version.loaded": "Loaded version {version}",
+    "start.version.loaded.fetched": "Loaded version {version} (fetched)",
     "start.version.not_found": "Version {version} not found",
     "start.version.too_much_parents": "Too much parents while resolving versions.",
     "start.features": "Features: {features}",
     "start.jar.found": "Checked version jar",
     "start.jar.not_found": "Version jar not found",
     "start.assets.resolving": "Checking assets version {index_version}... ",
     "start.assets.resolved": "Checked {count} assets version {index_version}",
```

### Comparing `portablemc-4.0.0rc2/portablemc/cli/output.py` & `portablemc-4.0.0rc3/portablemc/cli/output.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/cli/parse.py` & `portablemc-4.0.0rc3/portablemc/cli/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 def register_subcommands(subparsers):
     register_search_arguments(subparsers.add_parser("search", help=_("args.search")))
     register_start_arguments(subparsers.add_parser("start", help=_("args.start")))
     register_login_arguments(subparsers.add_parser("login", help=_("args.login")))
     register_logout_arguments(subparsers.add_parser("logout", help=_("args.logout")))
     register_show_arguments(subparsers.add_parser("show", help=_("args.show")))
-    register_addon_arguments(subparsers.add_parser("addon", help=_("args.addon")))
+    # register_addon_arguments(subparsers.add_parser("addon", help=_("args.addon")))
 
 
 def register_search_arguments(parser: ArgumentParser):
     parser.add_argument("-k", "--kind", help=_("args.search.kind"), default="mojang", choices=get_search_kinds())
     parser.add_argument("input", nargs="?")
 
 
@@ -134,20 +134,20 @@
     subparsers = parser.add_subparsers(title="subcommands", dest="show_subcommand")
     subparsers.required = True
     subparsers.add_parser("about", help=_("args.show.about"))
     subparsers.add_parser("auth", help=_("args.show.auth"))
     subparsers.add_parser("lang", help=_("args.show.lang"))
 
 
-def register_addon_arguments(parser: ArgumentParser):
-    subparsers = parser.add_subparsers(title="subcommands", dest="addon_subcommand")
-    subparsers.required = True
-    subparsers.add_parser("list", help=_("args.addon.list"))
-    show_parser = subparsers.add_parser("show", help=_("args.addon.show"))
-    show_parser.add_argument("addon_id")
+# def register_addon_arguments(parser: ArgumentParser):
+#     subparsers = parser.add_subparsers(title="subcommands", dest="addon_subcommand")
+#     subparsers.required = True
+#     subparsers.add_parser("list", help=_("args.addon.list"))
+#     show_parser = subparsers.add_parser("show", help=_("args.addon.show"))
+#     show_parser.add_argument("addon_id")
 
 
 def new_help_formatter_class(max_help_position: int) -> Type[HelpFormatter]:
 
     class CustomHelpFormatter(HelpFormatter):
         def __init__(self, prog):
             super().__init__(prog, max_help_position=max_help_position)
```

### Comparing `portablemc-4.0.0rc2/portablemc/cli/util.py` & `portablemc-4.0.0rc3/portablemc/cli/util.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/download.py` & `portablemc-4.0.0rc3/portablemc/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Definition of the optimized download task.
 """
 
 from http.client import HTTPConnection, HTTPSConnection, HTTPException
+from queue import Queue, Empty
 from threading import Thread
 from pathlib import Path
-from queue import Queue
 import urllib.parse
 import hashlib
 import time
 
 from typing import Optional, Dict, List, Tuple, Union, Iterator
 
 
@@ -98,19 +98,20 @@
     """
 
     CONNECTION = "connection"
     NOT_FOUND = "not_found"
     INVALID_SIZE = "invalid_size"
     INVALID_SHA1 = "invalid_sha1"
 
-    __slots__ = "code",
+    __slots__ = "code", "origin"
 
-    def __init__(self, thread_id: int, entry: DownloadEntry, code: str) -> None:
+    def __init__(self, thread_id: int, entry: DownloadEntry, code: str, origin: Optional[Exception]) -> None:
         super().__init__(thread_id, entry)
         self.code = code
+        self.origin = origin
 
 
 class DownloadList:
     """ A download list.
     """
 
     __slots__ = "entries", "count", "size"
@@ -166,47 +167,85 @@
 
         threads: List[Thread] = []
 
         entries_queue = Queue()
         result_queue = Queue()
 
         for th_id in range(threads_count):
-            th = Thread(target=_download_thread, 
+            th = Thread(target=_download_thread_wrapper, 
                         args=(th_id, entries_queue, result_queue, partial_progress), 
                         daemon=True, 
                         name=f"Download Thread {th_id}")
             th.start()
             threads.append(th)
         
         result_count = 0
 
         for entry in self.entries:
             entries_queue.put(entry)
+
+        crash = None
         
         while result_count < entries_count:
+
             result = result_queue.get()
+            if isinstance(result, _DownloadThreadCrash):
+                crash = result
+                break
+
             if not isinstance(result, DownloadResultProgress) or result.done:
                 result_count += 1
+            
             yield result_count, result
 
         # Send 'threads_count' sentinels.
+        # We intentionally don't join thread because it takes some time for unknown 
+        # reason. And we don't care of these threads because these are daemon ones.
         for th_id in range(threads_count):
             entries_queue.put(None)
 
-        # We intentionally don't join thread because it takes some time for unknown 
-        # reason. And we don't care of these threads because these are daemon ones.
-        pass
+        if crash is not None:
+            raise ValueError(f"unexpected crash from thread {crash.thread_id}", crash.origin)
+
+
+class _DownloadThreadCrash:
+    """Unexpected exception happening in a thread, this is the result of a bad logic
+    from programmer.
+    """
+    __slots__ = "thread_id", "origin",
+    def __init__(self, thread_id: int, origin: Optional[Exception]) -> None:
+        self.thread_id = thread_id
+        self.origin = origin
+
+
+def _download_thread_wrapper(
+    thread_id: int, 
+    entries_queue: Queue,
+    result_queue: Queue,
+    partial_progress: bool
+) -> None:
+    """Wrapper for the download thread that basically ensures that any unexpected error
+    sends a signal (DownloadThreadCrash) to the master to signal the crash.
+    """
+    try:
+        _download_thread(thread_id, entries_queue, result_queue, partial_progress)
+    except Exception as e:
+        result_queue.put(_DownloadThreadCrash(thread_id, e))
+    except:
+        # Really bad error, should not happen, but do we ever know...
+        result_queue.put(_DownloadThreadCrash(thread_id, None))
+        raise
 
 
 def _download_thread(
     thread_id: int, 
     entries_queue: Queue,
     result_queue: Queue,
     partial_progress: bool
-):
+) -> None:
     """This function is internally used for multi-threaded download.
 
     :param entries_queue: Where entries to download are received.
     :param result_queue: Where threads send progress update.
     """
     
     # Cache for connections depending on host and https
@@ -233,67 +272,77 @@
         raw_entry: Optional[_DownloadEntry] = entries_queue.get()
 
         # None is a sentinel to stop the thread, it should be consumed ONCE.
         if raw_entry is None:
             break
 
         conn_key = (raw_entry.https, raw_entry.host)
-        conn = conn_cache.get(conn_key)
+        conn_type = HTTPSConnection if raw_entry.https else HTTPConnection
 
+        # Get connection from cache or create it.
+        conn = conn_cache.get(conn_key)
         if conn is None:
-            conn_type = HTTPSConnection if raw_entry.https else HTTPConnection
             conn = conn_cache[conn_key] = conn_type(raw_entry.host)
 
         entry = raw_entry.entry
         
         # Allow modifying this URL when redirections happen.
         # size_target = 0 if entry.size is None else entry.size
         
         last_error: Optional[str] = None
+        last_error_origin: Optional[Exception] = None
         try_num = 0
 
         while True:
 
             try_num += 1
             if try_num > max_try_count:
                 # Retrying implies that we have set an error.
                 assert last_error is not None
-                result_queue.put(DownloadResultError(thread_id, entry, last_error))
+                result_queue.put(DownloadResultError(thread_id, entry, last_error, last_error_origin))
                 break
             
             try:
                 conn.request("GET", entry.url)
                 res = conn.getresponse()
-            except (ConnectionError, OSError, HTTPException):
-                last_error = DownloadResultError.CONNECTION
-                continue
+            except (ConnectionError, OSError, HTTPException) as e:
 
-            if res.status == 301 or res.status == 302:
+                # On errors, we just throw away the old connection and create a new one.
+                # Raw but efficient way of resetting the potentially broken state...
+                conn.close()
+                conn = conn_cache[conn_key] = conn_type(raw_entry.host)
 
-                redirect_url = res.headers["location"]
-                redirect_entry = DownloadEntry(
-                    redirect_url, 
-                    entry.dst, 
-                    size=entry.size, 
-                    sha1=entry.sha1, 
-                    name=entry.name)
-                
-                entries_queue.put(_DownloadEntry.from_entry(redirect_entry))
-                break  # Abort on redirect
+                last_error = DownloadResultError.CONNECTION
+                last_error_origin = e
+                continue
 
-            elif res.status != 200:
+            if res.status != 200:
 
                 # This loop is used to skip all bytes in the stream, 
                 # and allow further request.
                 while res.readinto(buffer):
                     pass
 
+                if res.status == 301 or res.status == 302:
+
+                    redirect_url = res.headers["location"]
+                    redirect_entry = DownloadEntry(
+                        redirect_url, 
+                        entry.dst, 
+                        size=entry.size, 
+                        sha1=entry.sha1, 
+                        name=entry.name)
+                    
+                    entries_queue.put(_DownloadEntry.from_entry(redirect_entry))
+                    break  # Abort on redirect
+
+                # Any other non-200 code is considered not found and we retry...
                 last_error = DownloadResultError.NOT_FOUND
                 continue
-
+            
             sha1 = None if entry.sha1 is None else hashlib.sha1()
             size = 0
 
             entry.dst.parent.mkdir(parents=True, exist_ok=True)
             with entry.dst.open("wb") as dst_fp:
 
                 while True:
```

### Comparing `portablemc-4.0.0rc2/portablemc/fabric.py` & `portablemc-4.0.0rc3/portablemc/fabric.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/forge.py` & `portablemc-4.0.0rc3/portablemc/forge.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from io import BytesIO
 import subprocess
 import shutil
 import json
 import os
 
-from .standard import parse_download_entry, \
+from .standard import parse_download_entry, LIBRARIES_URL, \
     Context, VersionHandle, Version, Watcher, VersionNotFoundError
 
 from .util import calc_input_sha1, LibrarySpecifier
 from .http import http_request, HttpError
 
 from typing import Dict, Optional, List
 
@@ -191,25 +191,27 @@
                     if len(lib_artifact["url"]):
                         self._dl.add(parse_download_entry(lib_artifact, lib_path, "forge profile: /json/libraries/"), verify=True)
                     else:
                         # The lib should be stored inside the JAR file, under maven/ directory.
                         zip_extract_file(install_jar, f"maven/{lib_spec.file_path()}", lib_path)
 
                 # Just keep the 'client' values.
-                for data_key, data_val in install_profile["data"].items():
+                install_data = install_profile["data"]
+                if isinstance(install_data, dict):
+                    for data_key, data_val in install_data.items():
+
+                        data_val = str(data_val["client"])
+
+                        # Refer to a file inside the JAR file.
+                        if data_val.startswith("/"):
+                            dst_path = post_info.tmp_dir / data_val[1:]
+                            zip_extract_file(install_jar, data_val[1:], dst_path)
+                            data_val = str(dst_path)  # Replace by the path of extracted file.
 
-                    data_val = str(data_val["client"])
-
-                    # Refer to a file inside the JAR file.
-                    if data_val.startswith("/"):
-                        dst_path = post_info.tmp_dir / data_val[1:]
-                        zip_extract_file(install_jar, data_val[1:], dst_path)
-                        data_val = str(dst_path)  # Replace by the path of extracted file.
-
-                    post_info.variables[data_key] = data_val
+                        post_info.variables[data_key] = data_val
                 
                 self._forge_post_info = post_info
 
             else: 
 
                 # Forge versions before 1.12.2-14.23.5.2847
                 version.metadata = install_profile.get("versionInfo")
@@ -220,14 +222,19 @@
                 for version_lib in version.metadata["libraries"]:
                     if "serverreq" in version_lib:
                         del version_lib["serverreq"]
                     if "clientreq" in version_lib:
                         del version_lib["clientreq"]
                     if "checksums" in version_lib:
                         del version_lib["checksums"]
+                    # Older version uses to require libraries that are no longer installed
+                    # by parent versions, therefore it's required to add url if not 
+                    # provided, pointing to maven central repository, for downloading.
+                    if not version_lib.get("url"):
+                        version_lib["url"] = LIBRARIES_URL
                 
                 # Old version (<= 1.6.4) of forge are broken, even on official launcher.
                 # So we fix them by manually adding the correct inherited version.
                 if "inheritsFrom" not in version.metadata:
                     version.metadata["inheritsFrom"] = install_profile["install"]["minecraft"]
 
                 # For "old" installers, that have an "install" section.
```

### Comparing `portablemc-4.0.0rc2/portablemc/http.py` & `portablemc-4.0.0rc3/portablemc/http.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/portablemc/standard.py` & `portablemc-4.0.0rc3/portablemc/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,19 +339,21 @@
             if len(hierarchy) > 10:
                 raise TooMuchParentsError(hierarchy)
             
             watcher.handle(VersionLoadingEvent(version))
 
             # Get version instance and load/fetch is needed.
             handle = self.context.get_version(version)
+            fetched = False
             if not self._load_version(handle, watcher):
                 watcher.handle(VersionFetchingEvent(version))
                 self._fetch_version(handle, watcher)
+                fetched = True
             
-            watcher.handle(VersionLoadedEvent(version))
+            watcher.handle(VersionLoadedEvent(version, fetched))
 
             # Set the parent of the last version to the version being resolved.
             if len(hierarchy):
                 hierarchy[-1].parent = handle
             
             hierarchy.append(handle)
             version = handle.metadata.pop("inheritsFrom", None)
@@ -873,15 +875,15 @@
 
             jvm_manifest_file.parent.mkdir(parents=True, exist_ok=True)
             with jvm_manifest_file.open("wt") as jvm_manifest_fp:
                 json.dump(jvm_manifest, jvm_manifest_fp)
         
         # Special case for macOS because of weird directory structure.
         if minecraft_os == "osx":
-            self.jvm_path = jvm_dir.joinpath("jre.bundle/Contents/Home/bin/java")
+            self._jvm_path = jvm_dir.joinpath("jre.bundle/Contents/Home/bin/java")
         else:
             self._jvm_path = jvm_dir.joinpath("bin", jvm_bin_filename)
         
         # This key is custom and set just above in code.
         self._jvm_version = jvm_manifest.get("version")
 
         jvm_files = jvm_manifest.get("files")
@@ -957,15 +959,15 @@
                     result_count,
                     result.entry,
                     result.size,
                     result.speed,
                     result.done
                 ))
             elif isinstance(result, DownloadResultError):
-                errors.append((result.entry, result.code))
+                errors.append((result.entry, result.code, result.origin))
 
         # If errors are present, raise an error.
         if len(errors):
             raise DownloadError(errors)
         
         # Clear entries if successful, therefore multiple calls can be chained if
         # needed, without re-downloading the same files.
@@ -1255,17 +1257,20 @@
 
     def __init__(self, code: str) -> None:
         self.code = code
 
 class DownloadError(Exception):
     """Raised when the downloader failed to download some entries.
     """
-    def __init__(self, errors: List[Tuple[DownloadEntry, str]]) -> None:
-        super().__init__()
+    def __init__(self, errors: List[Tuple[DownloadEntry, str, Optional[Exception]]]) -> None:
+        super().__init__(errors)
         self.errors = errors
+    
+    def __repr__(self) -> str:
+        return f"<DownloadError {repr(self.errors)}>"
 
 
 class VersionEvent:
     """Base class for events regarding version.
     """
     __slots__ = "version",
     def __init__(self, version: str) -> None:
@@ -1278,14 +1283,18 @@
 class VersionFetchingEvent(VersionEvent):
     """Event triggered when a version is being fetched.
     """
 
 class VersionLoadedEvent(VersionEvent):
     """Event triggered when a version has been successfully loaded.
     """
+    __slots__ = "fetched",
+    def __init__(self, version: str, fetched: bool) -> None:
+        super().__init__(version)
+        self.fetched = fetched
 
 class FeaturesEvent:
     """Event triggered when features for the version has been computed. Only enabled 
     features are given as list of features.
     """
     __slots__ = "features",
     def __init__(self, features: List[str]) -> None:
@@ -1399,15 +1408,15 @@
 
                 if "Last-Modified" in res.headers:
                     self.data["last_modified"] = res.headers["Last-Modified"]
 
                 if self.cache_file is not None:
                     self.cache_file.parent.mkdir(parents=True, exist_ok=True)
                     with self.cache_file.open("wt") as cache_fp:
-                        json.dump(self.data, cache_fp, indent=2)
+                        json.dump(self.data, cache_fp)
 
             except HttpError as error:
                 res = error.res
                 if res.status == 304 and cache_data is not None:
                     self.data = cache_data
                 else:
                     raise
@@ -1536,15 +1545,15 @@
 
 class StreamRunner(StandardRunner):
     """A specialized implementation of `RunTask` which allows streaming the game's output
     logs. This implementation also provides parsing of log4j XML layouts for logs.
     """
     
     def process_create(self, args: List[str], work_dir: Path) -> Popen:
-        return Popen(args, cwd=work_dir, stdout=PIPE, stderr=STDOUT, bufsize=1, universal_newlines=True)
+        return Popen(args, cwd=work_dir, stdout=PIPE, stderr=STDOUT, bufsize=1, universal_newlines=True, encoding="utf-8", errors="replace")
 
     def process_wait(self, process: Popen) -> None:
 
         from threading import Thread
 
         thread = Thread(target=self.process_stream_thread, name="Minecraft Stream Thread", args=(process,))
         thread.start()
```

### Comparing `portablemc-4.0.0rc2/portablemc/util.py` & `portablemc-4.0.0rc3/portablemc/util.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc2/pyproject.toml` & `portablemc-4.0.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "portablemc"
-version = "4.0.0rc2"
+version = "4.0.0rc3"
 description = "PortableMC is a module that provides both an API for development of your custom launcher and an executable script to run PortableMC CLI."
 authors = ["Théo Rozier <contact@theorozier.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/mindstorm38/portablemc"
 repository = "https://github.com/mindstorm38/portablemc"
 documentation = "https://github.com/mindstorm38/portablemc"
```

### Comparing `portablemc-4.0.0rc2/PKG-INFO` & `portablemc-4.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portablemc
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: PortableMC is a module that provides both an API for development of your custom launcher and an executable script to run PortableMC CLI.
 Home-page: https://github.com/mindstorm38/portablemc
 License: GPL-3.0-only
 Keywords: minecraft,launcher,portable,cli
 Author: Théo Rozier
 Author-email: contact@theorozier.fr
 Requires-Python: >=3.7
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://github.com/mindstorm38/portablemc
 Project-URL: Repository, https://github.com/mindstorm38/portablemc
 Description-Content-Type: text/markdown
 
 # Portable Minecraft Launcher
-A fast, reliable and cross-platform command line Minecraft launcher and API for developers.
-This launcher is compatible with the official Minecraft launcher' version specification.
+A fast, reliable and cross-platform command-line Minecraft launcher and API for developers.
+This launcher is compatible with the official Minecraft launcher's version specification.
 It also includes fast installation of common mod loaders such as Fabric, Forge and Quilt.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/portablemc?label=PyPI%20version&style=flat-square) &nbsp;![PyPI - Downloads](https://img.shields.io/pypi/dm/portablemc?label=PyPI%20downloads&style=flat-square)
 
 ![illustration](doc/assets/illustration.png)
 
 *This launcher is tested for Python 3.7, 3.8, 3.9, 3.10, 3.11.*
@@ -57,87 +57,91 @@
 use `pip3` instead of `pip` in order to run it on Python 3. You can also use 
 `python -m pip` if the `pip` command is not in the path and the python executable is.
 
 ```sh
 pip install --user portablemc
 ```
 
-It's recommended to keep `--user` because this allows to install the launcher for your
+It's recommended to keep `--user` because this installs the launcher for your
 current user only, it is implicit if you are not an administrator and if you are, it 
 allows not to modify other users' installations.
 
 After that, you can try to show the launcher help message using `portablemc` in your 
 terminal. If it fails, you should check that the scripts directory is in your user path
 environment variable. On Windows you have to search for a directory at 
 `%appdata%/Python/Python3X/Scripts` and add it to the user's environment variable `Path`. 
 On UNIX systems it's `~/.local/bin`.
 
 ## Commands
 Arguments are split between multiple commands. 
 For example `portablemc [global-args] <cmd> [args]`. 
-You can use `-h` argument to display help *(also works for every sub-commands)*.
+You can use `-h` argument to display help *(also works for every sub-command)*.
 
 By default the launcher will run any command from the OS standard `.minecraft` directory 
 ([check wiki for more information](https://minecraft.gamepedia.com/.minecraft)). You can
 change this directory using `--main-dir <path>` global argument.
 
 You may also need `--work-dir <path>` to change the directory where your saves, resource 
 packs and all "user-specific" content is stored. This can be useful if you have a shared 
 read-only main directory (`--main-dir`) and user-specific working directory (for example 
 in `.minecraft`, by default it's the location of your main directory). The launcher also
 stores cached version manifest and authentication database in the working directory.
 
-The two arguments `--main-dir` and `--work-dir` may or may not be used by sub commands, 
-but they are always valid to use, allowing you to define command alias for running
+The two arguments `--main-dir` and `--work-dir` may or may not be used by sub-commands, 
+but they are always valid to use, allowing you to define command aliases for running
 PortableMC.
 
 Another argument, `--timeout <seconds>` can be used to set a global timeout value that 
 will be used for all network connections.
 
 The general output format of the launcher can be changed using the `--output <mode>` with
 one of the following modes:
 - `human`: Human readable output, translated messages, formatted tables and tasks.
 - `human-color`: Default, same as `human` but with some color where relevant, like tasks 
-  states and game's logs.
+  states and game logs.
 - `machine`: Machine
 
 The verbosity of the launcher can be adjusted if you encounter issues, using multiple 
 `-v` arguments (usually `-v` through `-vvv`). It's very useful to maintainers when fixing 
 issues.
 
 ### Start Minecraft
 The first thing you may want to do is install and start Minecraft, to do so you can use
 the `portablemc start [args] [version]` command. This command will install every component
 needed by the version before launching it. If you provide no version, the latest release
-is started, but you can specify a specific version launch, or a version alias: `release`
-or `snapshot` for latest version of their type.
+is started, but you can specify a version to launch, or a version alias: `release`
+or `snapshot` for the latest version of their type.
 
-In addition to Mojang's vanilla versions, the launcher natively support common mod
-loaders such as **Fabric**, **Forge** and **Quilt**. To start such version, you can
+In addition to Mojang's vanilla versions, the launcher natively supports common mod
+loaders such as **Fabric**, **Forge** and **Quilt**. To start such versions, you can
 prefix the version with either `fabric:`, `forge:` or `quilt:` (or `vanilla:` to
-explicitly choose vanilla version).
+explicitly choose a vanilla version).
 Depending on the mod loader, the version you put after the colon is different:
 - For Fabric and Quilt, you can directly specify the vanilla version, optionally followed
-  by `:<loader_version>`.
+  by `:<loader_version>`:  
+  `fabric:1.20.1`  
+  `fabric:1.20.1:0.11.2`
 - For Forge, you can put either a vanilla game version, optionally followed by `-latest`
-  or `-recommended`, or `-<loader_version>`.
+  or `-recommended`, or `-<loader_version>`:  
+  `forge:1.20-latest`  
+  `forge:1.20-46.0.14`
 
 *You can search for versions using the [search command](#search-for-versions).*
 
 #### Authentication
 Online mode is supported by this launcher, use the `-l <email_or_username>` (`--login`)
 argument to log into your account *(login with a username is deprecated by Mojang)*. 
 If your session is not cached or no longer valid, the launcher will ask for the 
 password or open the Microsoft connection page.
 
 **By default**, this will authenticate you using the Microsoft authentication services,
-you can change that using `--auth-service` argument, for example with `yggdrasil` if
-you need to log into an old Mojang account (being phased out by Mojang).
+although you can change that using the `--auth-service` argument, for example with
+`yggdrasil` if you need to log into an old Mojang account (being phased out by Mojang).
 
-If you want to be asked for password on each authentication, you can use `-t
+If you want to be asked for password on each authentication, you can use `-t`
 (`--temp-login`). This has no effect if the session is already cached before that.
 
 You can also use `--auth-anonymize` in order to hide most of your email when printing 
 it to the terminal. For example, `foo.bar@gmail.com` will become `f*****r@g***l.com`,
 this is useful to avoid leaking it when recording or streaming.
 However, if you use this, make sure that you either use an alias or a variable with the
 `-l` argument, for exemple `-l $PMC_LOGIN`.
@@ -191,15 +195,15 @@
 `export MESA_GL_VERSION_OVERRIDE=4.5` 
 ([more info here](https://forum.winehq.org/viewtopic.php?f=8&t=34889)).
 
 In case with the above you still get an `error: GLSL 1.50 is not supported` you may also 
 try `export MESA_GLSL_VERSION_OVERRIDE=150`.
 
 #### Fix unsupported systems
-Some Mojang provided natives (.so, .dll, .dylib) might not be compatible with your system.
+Some Mojang-provided natives (.so, .dll, .dylib) might not be compatible with your system.
 To mitigate that, the launcher provides two arguments, `--exclude-lib` and `--include-bin`
 that can be provided multiples times each.
 
 With `--exclude-lib <artifact>[:[<version>][:<classifier>]]` you can exclude libraries 
 (.jar) from the game's classpath (and so of the downloads). If a classifier is given, it
 will match libs' classifiers that starts with itself, for example `lwjgl-glfw::natives`
 will match the library `lwjgl-glfw:3.3.1:natives-windows-x86`.
@@ -210,37 +214,37 @@
 Windows). For shared objects files (.so) that contains version numbers in the filename,
 these are discarded in the bin directory, for example 
 `/lib/libglfw.so.3 -> .minecraft/bin/<uuid>/libglfw.so`.
 
 These arguments can be used together to fix various issues (e.g. wrong libc being linked
 by the LWJGL-provided natives).
 
-*Note that these arguments are compatible, and executed after the `--lwjgl` argument.
+*Note that these arguments are compatible with, and executed after the `--lwjgl` argument.
 You must however ensure that excluded lib and included binaries are compatible.*
 
 #### Miscellaneous
-With `--dry`, the start command do not start the game, but install it.
+With `--dry`, the start command does not start the game, but simply installs it.
 
 With `--demo` you can enable the [demo mode](https://minecraft.gamepedia.com/Demo_mode) 
 of the game.  
 
 With `--resolution <width>x<height>` you can change the resolution of the game window.
 
-The two arguments `--disable-mp` (mp: multiplayer), `--disable-chat` respectively to 
-disable multiplayer button and disable in-game chat *(since 1.16)*.
+The two arguments `--disable-mp` (mp: multiplayer) and `--disable-chat` can respectively
+disable the multiplayer button and the in-game chat *(since 1.16)*.
 
 ### Search for versions
 The `portablemc search [-k <kind>] [version]` sub-command is used to search for versions. 
 By default, this command will search for official Mojang versions available to download, 
-you can instead search for many kind of versions using the `-k` (`--kind`) arguments:
+you can instead search for many kinds of versions using the `-k` (`--kind`) arguments:
 - `local`, show all installed versions.
-- `forge`, show all recommended and latest forge loader versions *(only 1.5.2 and 
+- `forge`, show all recommended and latest Forge loader versions *(only 1.5.2 and 
   onward can be started)*.
-- `fabric`, show all available fabric loader versions.
-- `quilt`, show all available quilt loader versions.
+- `fabric`, show all available Fabric loader versions.
+- `quilt`, show all available Quilt loader versions.
 
 The search string is optional, if not specified no filter is applied on the table shown.
 
 ### Authentication sessions
 Two subcommands allow you to store or logout of sessions: `portablemc login|logout <email_or_username>`.
 These subcommands don't prevent you from using the `-l` (`--login`) argument when starting
 the game, these are just here to manage the session storage.
```

