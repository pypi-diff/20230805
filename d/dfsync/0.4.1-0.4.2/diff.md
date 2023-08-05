# Comparing `tmp/dfsync-0.4.1.tar.gz` & `tmp/dfsync-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsync-0.4.1.tar", max compression
+gzip compressed data, was "dfsync-0.4.2.tar", max compression
```

## Comparing `dfsync-0.4.1.tar` & `dfsync-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.1/dfsync/__init__.py
--rw-r--r--   0        0        0       64 2021-04-06 10:05:47.000000 dfsync-0.4.1/dfsync/backends/__init__.py
--rw-r--r--   0        0        0    23995 2023-04-03 16:24:42.000000 dfsync-0.4.1/dfsync/backends/kube.py
--rwxr-xr-x   0        0        0     1928 2022-09-10 10:08:34.000000 dfsync-0.4.1/dfsync/backends/kube_exec.py
--rw-r--r--   0        0        0     5473 2023-07-31 21:29:22.099082 dfsync-0.4.1/dfsync/backends/rsync.py
--rw-r--r--   0        0        0     3617 2023-07-31 19:01:18.508583 dfsync-0.4.1/dfsync/char_ui.py
--rw-r--r--   0        0        0     1334 2022-10-21 04:03:26.000000 dfsync-0.4.1/dfsync/chcli.py
--rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.1/dfsync/check_dns.py
--rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.1/dfsync/cli.py
--rw-r--r--   0        0        0     2381 2023-06-19 07:28:44.923993 dfsync-0.4.1/dfsync/config.py
--rw-r--r--   0        0        0     2389 2023-07-31 22:35:43.410956 dfsync-0.4.1/dfsync/distribution.py
--rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.1/dfsync/exp.py
--rw-r--r--   0        0        0     7155 2023-08-03 09:59:21.618826 dfsync-0.4.1/dfsync/filters.py
--rw-r--r--   0        0        0     1094 2023-05-20 11:19:56.000000 dfsync-0.4.1/dfsync/generate.py
--rw-r--r--   0        0        0     4543 2023-06-17 23:21:49.780512 dfsync-0.4.1/dfsync/kube_credentials.py
--rw-r--r--   0        0        0      679 2023-07-31 20:23:04.492784 dfsync-0.4.1/dfsync/lib.py
--rw-r--r--   0        0        0    10870 2023-07-31 20:25:25.957594 dfsync-0.4.1/dfsync/monitor.py
--rw-r--r--   0        0        0      725 2023-07-08 13:02:10.410286 dfsync-0.4.1/dfsync/pycode/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-20 10:16:55.000000 dfsync-0.4.1/dfsync/pycode/bpe.py
--rw-r--r--   0        0        0     3641 2023-05-18 09:12:53.000000 dfsync-0.4.1/dfsync/pycode/generate_data.py
--rw-r--r--   0        0        0     2121 2023-05-20 11:12:31.000000 dfsync-0.4.1/dfsync/pycode/generate_docstring.py
--rw-r--r--   0        0        0     5869 2023-05-20 13:52:38.000000 dfsync-0.4.1/dfsync/pycode/generate_expansion.py
--rw-r--r--   0        0        0     3088 2023-05-20 11:12:48.000000 dfsync-0.4.1/dfsync/pycode/generate_func.py
--rw-r--r--   0        0        0      540 2023-05-16 17:24:44.000000 dfsync-0.4.1/dfsync/pycode/generate_pytest.py
--rw-r--r--   0        0        0     1822 2023-07-08 13:05:08.349161 dfsync-0.4.1/dfsync/pycode/oai.py
--rw-r--r--   0        0        0     2674 2023-06-02 11:17:40.000000 dfsync-0.4.1/dfsync/pycode/prompts.py
--rw-r--r--   0        0        0      212 2023-07-08 13:05:57.874746 dfsync-0.4.1/dfsync/pycode/search.py
--rw-r--r--   0        0        0     1830 2023-05-18 09:18:10.000000 dfsync-0.4.1/dfsync/pycode/test_generate_data.py
--rw-r--r--   0        0        0     4879 2023-05-20 08:26:16.000000 dfsync-0.4.1/dfsync/pycode/tokens.py
--rw-r--r--   0        0        0     3193 2023-05-20 11:11:17.000000 dfsync-0.4.1/dfsync/pycode/util.py
--rw-r--r--   0        0        0     4269 2023-07-26 02:24:53.086605 dfsync-0.4.1/dfsync/scrape_anm.py
--rw-r--r--   0        0        0      982 2023-07-26 01:41:23.893303 dfsync-0.4.1/dfsync/scrape_reord.py
--rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.1/dfsync/transactions.py
--rw-r--r--   0        0        0      630 2023-08-03 15:01:26.464929 dfsync-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 dfsync-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.2/dfsync/__init__.py
+-rw-r--r--   0        0        0       64 2021-04-06 10:05:47.000000 dfsync-0.4.2/dfsync/backends/__init__.py
+-rw-r--r--   0        0        0    23995 2023-04-03 16:24:42.000000 dfsync-0.4.2/dfsync/backends/kube.py
+-rwxr-xr-x   0        0        0     2168 2023-08-05 13:32:35.365088 dfsync-0.4.2/dfsync/backends/kube_exec.py
+-rw-r--r--   0        0        0     9741 2023-08-05 13:53:45.136201 dfsync-0.4.2/dfsync/backends/rsync.py
+-rw-r--r--   0        0        0     3617 2023-07-31 19:01:18.508583 dfsync-0.4.2/dfsync/char_ui.py
+-rw-r--r--   0        0        0     1334 2022-10-21 04:03:26.000000 dfsync-0.4.2/dfsync/chcli.py
+-rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.2/dfsync/check_dns.py
+-rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.2/dfsync/cli.py
+-rw-r--r--   0        0        0     2381 2023-06-19 07:28:44.923993 dfsync-0.4.2/dfsync/config.py
+-rw-r--r--   0        0        0     2389 2023-07-31 22:35:43.410956 dfsync-0.4.2/dfsync/distribution.py
+-rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.2/dfsync/exp.py
+-rw-r--r--   0        0        0     7193 2023-08-05 10:09:42.805988 dfsync-0.4.2/dfsync/filters.py
+-rw-r--r--   0        0        0     1094 2023-05-20 11:19:56.000000 dfsync-0.4.2/dfsync/generate.py
+-rw-r--r--   0        0        0     4543 2023-06-17 23:21:49.780512 dfsync-0.4.2/dfsync/kube_credentials.py
+-rw-r--r--   0        0        0     1059 2023-08-05 04:10:44.479647 dfsync-0.4.2/dfsync/lib.py
+-rw-r--r--   0        0        0    13657 2023-08-05 14:09:03.736723 dfsync-0.4.2/dfsync/monitor.py
+-rw-r--r--   0        0        0      725 2023-07-08 13:02:10.410286 dfsync-0.4.2/dfsync/pycode/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-20 10:16:55.000000 dfsync-0.4.2/dfsync/pycode/bpe.py
+-rw-r--r--   0        0        0     3641 2023-05-18 09:12:53.000000 dfsync-0.4.2/dfsync/pycode/generate_data.py
+-rw-r--r--   0        0        0     2121 2023-05-20 11:12:31.000000 dfsync-0.4.2/dfsync/pycode/generate_docstring.py
+-rw-r--r--   0        0        0     5869 2023-05-20 13:52:38.000000 dfsync-0.4.2/dfsync/pycode/generate_expansion.py
+-rw-r--r--   0        0        0     3088 2023-05-20 11:12:48.000000 dfsync-0.4.2/dfsync/pycode/generate_func.py
+-rw-r--r--   0        0        0      540 2023-05-16 17:24:44.000000 dfsync-0.4.2/dfsync/pycode/generate_pytest.py
+-rw-r--r--   0        0        0     1822 2023-07-08 13:05:08.349161 dfsync-0.4.2/dfsync/pycode/oai.py
+-rw-r--r--   0        0        0     2674 2023-06-02 11:17:40.000000 dfsync-0.4.2/dfsync/pycode/prompts.py
+-rw-r--r--   0        0        0      212 2023-07-08 13:05:57.874746 dfsync-0.4.2/dfsync/pycode/search.py
+-rw-r--r--   0        0        0     1830 2023-05-18 09:18:10.000000 dfsync-0.4.2/dfsync/pycode/test_generate_data.py
+-rw-r--r--   0        0        0     4879 2023-05-20 08:26:16.000000 dfsync-0.4.2/dfsync/pycode/tokens.py
+-rw-r--r--   0        0        0     3193 2023-05-20 11:11:17.000000 dfsync-0.4.2/dfsync/pycode/util.py
+-rw-r--r--   0        0        0     4269 2023-07-26 02:24:53.086605 dfsync-0.4.2/dfsync/scrape_anm.py
+-rw-r--r--   0        0        0      982 2023-07-26 01:41:23.893303 dfsync-0.4.2/dfsync/scrape_reord.py
+-rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.2/dfsync/transactions.py
+-rw-r--r--   0        0        0      630 2023-08-05 14:12:09.256450 dfsync-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 dfsync-0.4.2/PKG-INFO
```

### Comparing `dfsync-0.4.1/dfsync/backends/kube.py` & `dfsync-0.4.2/dfsync/backends/kube.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/backends/kube_exec.py` & `dfsync-0.4.2/dfsync/backends/kube_exec.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,18 +42,25 @@
     with open(f"dfsync-{kube_container}.log", "a") as f:
         container_cmd = get_container_command()
         cmd = [*kubectl_cmd, *container_cmd]
         cmd_str = " ".join(cmd)
         print(f"[{pod_name}] Running: {cmd_str}", file=f, flush=True)
         try:
             subprocess.check_call(cmd)
+            return 0
+
+        except subprocess.CalledProcessError as e:
+            err = str(e) or type(e)
+            print(f"[{pod_name}] Error: {err}", file=f, flush=True)
+            return e.returncode
 
         except Exception as e:
             err = str(e) or type(e)
             print(f"[{pod_name}] Error: {err}", file=f, flush=True)
+            return 1
 
         finally:
             print(f"[{pod_name}] Exiting", file=f, flush=True)
 
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

### Comparing `dfsync-0.4.1/dfsync/char_ui.py` & `dfsync-0.4.2/dfsync/char_ui.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/chcli.py` & `dfsync-0.4.2/dfsync/chcli.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/check_dns.py` & `dfsync-0.4.2/dfsync/check_dns.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/config.py` & `dfsync-0.4.2/dfsync/config.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/distribution.py` & `dfsync-0.4.2/dfsync/distribution.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/exp.py` & `dfsync-0.4.2/dfsync/exp.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/filters.py` & `dfsync-0.4.2/dfsync/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def _black_check(self, src_file_path):
         try:
             with open(src_file_path, "r") as f:
                 contents = f.read()
                 black.format_file_contents(contents, fast=False, mode=black.FileMode())
             return False
 
-        except black.report.NothingChanged as e:
+        except (FileNotFoundError, PermissionError, black.report.NothingChanged) as e:
             return False
 
         except Exception as e:
             message = str(e) or type(e).__name__
             echo(f"Rejected {src_file_path}, {message}")
             return True
```

### Comparing `dfsync-0.4.1/dfsync/generate.py` & `dfsync-0.4.2/dfsync/generate.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/kube_credentials.py` & `dfsync-0.4.2/dfsync/kube_credentials.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/monitor.py` & `dfsync-0.4.2/dfsync/monitor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,86 @@
 import click
 import os
 import os.path
 import sys
 import time
 import logging
+import queue
 
 from click_default_group import DefaultGroup
+from contextlib import contextmanager
 from functools import partial
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 from dfsync.backends import rsync_backend, kube_backend
 from dfsync.distribution import get_installed_version, get_latest_version, is_older_version, AsyncVersionChecker
 from dfsync.filters import add_user_ignored_patterns_filter, ALL_FILTERS
 from dfsync.config import read_config
 from dfsync.char_ui import KeyController
 from dfsync.kube_credentials import contextualize_kube_credentials, update_local_kube_config
+from dfsync.lib import ControlledThreadedOperation, thread_manager
 
 logging.basicConfig(level=logging.WARN)
 
 BACKENDS = {
     # File sync backends
     "rsync": rsync_backend,
     "kube": kube_backend,
 }
 
 
 class IgnoreEvent(Exception):
     pass
 
 
-class FileChangedEventHandler(FileSystemEventHandler):
-    def __init__(self, backend: str = "log", watched_dir: str = ".", input_controller: KeyController = None, **kwargs):
+class FileChangedEventHandler(ControlledThreadedOperation, FileSystemEventHandler):
+    def __init__(
+        self,
+        backend: str = "log",
+        watched_dir: str = ".",
+        all_watched_dirs: list = None,
+        input_controller: KeyController = None,
+        **kwargs,
+    ):
+        super().__init__()
         self.filters = [*ALL_FILTERS]
 
         self.backend = backend
         self.backend_options = kwargs
         self.raised_exception = False
+        self.watched_dir = watched_dir
         self.abs_watched_dir = os.path.abspath(watched_dir)
         self.input_controller = input_controller
+        self.events = queue.Queue(maxsize=10000)
+        self.full_sync_threashold = 3
+        self.all_watched_dirs = all_watched_dirs if all_watched_dirs is not None else [watched_dir]
 
     def _log_backend(self, event):
         logging.info(event)
 
+    @contextmanager
+    def _input_lock(self):
+        if self.input_controller is None:
+            yield self
+        else:
+            with self.input_controller.getch_lock():
+                yield self
+
+    @contextmanager
+    def terminal_lock(self):
+        try:
+            with self._input_lock():
+                yield self
+        except IgnoreEvent:
+            pass
+        except:
+            self.raised_exception = True
+            raise
+
     def _sync(self, event):
         # It seems like in some contexts, event.src_path will be an absolute path
         # and in some other contexts, it will be a relative path
 
         src_file_path = self._get_path_relative_to_watched_dir(event.src_path, self.abs_watched_dir)
         self.backend.sync(
             src_file_path=src_file_path,
@@ -74,32 +108,75 @@
             if not rel_path.startswith("."):
                 rel_path = os.path.join(".", rel_path)
 
             return rel_path
         except ValueError as e:
             raise IgnoreEvent() from e
 
-    def _propagate_event(self, event):
-        for file_filter in self.filters:
-            if file_filter(event=event) is False:
-                return
-        self._sync(event)
+    def _drain_queue(self, timeout=0.5):
+        event = self.events.get(block=True, timeout=timeout)
+        latest_events = {event.src_path: event}
+        try:
+            # Allow a bit of time for the queue to fill
+            if self.events.qsize() == 0:
+                time.sleep(0.25)
+            # Started filling? allow a little bit more time
+            if self.events.qsize() > 0:
+                time.sleep(0.4)
+
+            # Start draining
+            while self.events.qsize() > 0:
+                event = self.events.get_nowait()
+                # Only keep the latest event for a given file path
+                latest_events[event.src_path] = event
+
+        except queue.Empty:
+            pass
+        finally:
+            return latest_events.values()
+
+    def _filter_events(self, latest_events, stop_threashold=None):
+        sync_events = []
+        for event in latest_events:
+            filtered = False
+            for file_filter in self.filters:
+                with self.terminal_lock():
+                    if file_filter(event=event) is False:
+                        filtered = True
+                        break
+            if not filtered:
+                sync_events.append(event)
+            if stop_threashold is not None and len(sync_events) > stop_threashold:
+                return sync_events
+
+        return sync_events
+
+    def run(self):
+        while self._running:
+            try:
+                latest_events = self._drain_queue()
+                sync_events = self._filter_events(latest_events, stop_threashold=self.full_sync_threashold)
+                if len(sync_events) >= self.full_sync_threashold:
+                    with self.terminal_lock():
+                        self.backend.sync_project(self.all_watched_dirs, **self.backend_options)
+                else:
+                    for event in sync_events:
+                        with self.terminal_lock():
+                            self._sync(event)
+            except queue.Empty:
+                time.sleep(0.001)
 
     def catch_all_handler(self, event):
         try:
-            if self.input_controller is None:
-                self._propagate_event(event)
-            else:
-                with self.input_controller.getch_lock():
-                    self._propagate_event(event)
-        except IgnoreEvent:
+            # Add sync event to the sync queue
+            self.events.put(event)
+        except queue.Full:
+            # It's acceptable for events to be rejected from the queue
+            # because a busy queue will trigger a full-sync
             pass
-        except:
-            self.raised_exception = True
-            raise
 
     def on_moved(self, event):
         self.catch_all_handler(event)
 
     def on_created(self, event):
         self.catch_all_handler(event)
 
@@ -252,28 +329,29 @@
     checker = AsyncVersionChecker()
     controller = KeyController()
 
     handlers = []
     observer = Observer()
     for p in paths:
         event_handler = FileChangedEventHandler(
-            backend_engine, watched_dir=p, input_controller=controller, **backend_options
+            backend_engine, watched_dir=p, all_watched_dirs=paths, input_controller=controller, **backend_options
         )
         handlers.append(event_handler)
+        event_handler.start()
         observer.schedule(event_handler, os.path.abspath(p), recursive=True)
 
     controller.on_key(
         "f",
         description="to trigger a full sync",
         action=partial(backend_engine.sync_project, paths, **backend_options),
     )
     controller.on_key(
         "x",
         description="to exit",
-        action=partial(controller.stop, "Exiting."),
+        action=partial(thread_manager.stop, "Exiting."),
     )
 
     try:
         backend_engine.on_monitor_start(src_file_paths=paths, **backend_options)
         click.echo("Watching dir(s): '{}'; press [Ctrl-C] to exit\n".format("', '".join(paths)))
         observer.start()
 
@@ -291,24 +369,24 @@
             with controller.getch_lock():
                 if checker.should_emit_upgrade_warning:
                     checker.set_emitted_upgrade_warning()
                     click.echo(checker.get_upgrade_warning())
             controller.raise_exceptions()
 
     except KeyboardInterrupt:
-        controller.stop()
+        thread_manager.stop()
         click.echo("Received [Ctrl-C], exiting.")
 
     except:
-        controller.stop()
+        thread_manager.stop()
         raise
 
     finally:
         observer.stop()
-        checker.stop()
+        thread_manager.stop()
         backend_engine.on_monitor_exit(**backend_options)
         if observer.ident is not None:
             # only join the observer if it was previously started
             observer.join()
 
 
 if __name__ == "__main__":
```

### Comparing `dfsync-0.4.1/dfsync/pycode/__init__.py` & `dfsync-0.4.2/dfsync/pycode/__init__.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/bpe.py` & `dfsync-0.4.2/dfsync/pycode/bpe.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/generate_data.py` & `dfsync-0.4.2/dfsync/pycode/generate_data.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/generate_docstring.py` & `dfsync-0.4.2/dfsync/pycode/generate_docstring.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/generate_expansion.py` & `dfsync-0.4.2/dfsync/pycode/generate_expansion.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/generate_func.py` & `dfsync-0.4.2/dfsync/pycode/generate_func.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/generate_pytest.py` & `dfsync-0.4.2/dfsync/pycode/generate_pytest.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/oai.py` & `dfsync-0.4.2/dfsync/pycode/oai.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/prompts.py` & `dfsync-0.4.2/dfsync/pycode/prompts.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/test_generate_data.py` & `dfsync-0.4.2/dfsync/pycode/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/tokens.py` & `dfsync-0.4.2/dfsync/pycode/tokens.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/pycode/util.py` & `dfsync-0.4.2/dfsync/pycode/util.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/scrape_anm.py` & `dfsync-0.4.2/dfsync/scrape_anm.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/scrape_reord.py` & `dfsync-0.4.2/dfsync/scrape_reord.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/dfsync/transactions.py` & `dfsync-0.4.2/dfsync/transactions.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.1/pyproject.toml` & `dfsync-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfsync"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Mihai Balint <balint.mihai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 watchdog = "^2.0.2"
 gitpython = "^3.1.14"
```

### Comparing `dfsync-0.4.1/PKG-INFO` & `dfsync-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsync
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Mihai Balint
 Author-email: balint.mihai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

