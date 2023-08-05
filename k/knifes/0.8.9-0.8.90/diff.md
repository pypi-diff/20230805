# Comparing `tmp/knifes-0.8.9.tar.gz` & `tmp/knifes-0.8.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knifes-0.8.9.tar", last modified: Thu Nov  3 11:19:21 2022, max compression
+gzip compressed data, was "knifes-0.8.90.tar", last modified: Fri Aug  4 10:49:26 2023, max compression
```

## Comparing `knifes-0.8.9.tar` & `knifes-0.8.90.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.636872 knifes-0.8.9/
--rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:19:21.636726 knifes-0.8.9/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.9/README.md
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.635679 knifes-0.8.9/knifes/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)      134 2022-08-09 07:31:37.000000 knifes-0.8.9/knifes/_settings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.9/knifes/aes.py
--rw-r--r--   0 hwei       (501) staff       (20)      606 2022-08-09 10:00:32.000000 knifes-0.8.9/knifes/alarm.py
--rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/auth.py
--rw-r--r--   0 hwei       (501) staff       (20)      487 2022-02-16 01:56:36.000000 knifes-0.8.9/knifes/constants.py
--rw-r--r--   0 hwei       (501) staff       (20)     6160 2022-08-31 09:51:36.000000 knifes-0.8.9/knifes/decorators.py
--rw-r--r--   0 hwei       (501) staff       (20)     5201 2022-11-03 11:18:34.000000 knifes-0.8.9/knifes/deploy.py
--rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.9/knifes/digests.py
--rw-r--r--   0 hwei       (501) staff       (20)      368 2022-09-25 02:42:32.000000 knifes-0.8.9/knifes/envconfig.py
--rw-r--r--   0 hwei       (501) staff       (20)      200 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/file.py
--rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.9/knifes/jsons.py
--rw-r--r--   0 hwei       (501) staff       (20)      559 2022-09-25 02:41:33.000000 knifes-0.8.9/knifes/logging.py
--rw-r--r--   0 hwei       (501) staff       (20)      849 2022-07-04 09:50:15.000000 knifes-0.8.9/knifes/misc.py
--rw-r--r--   0 hwei       (501) staff       (20)      866 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/randoms.py
--rw-r--r--   0 hwei       (501) staff       (20)     1792 2022-02-12 10:43:59.000000 knifes-0.8.9/knifes/results.py
--rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.9/knifes/roar.py
--rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/shell.py
--rw-r--r--   0 hwei       (501) staff       (20)     1563 2022-08-09 10:02:01.000000 knifes-0.8.9/knifes/sms.py
--rw-r--r--   0 hwei       (501) staff       (20)      994 2022-10-25 10:02:34.000000 knifes-0.8.9/knifes/strings.py
--rw-r--r--   0 hwei       (501) staff       (20)     1154 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/times.py
--rw-r--r--   0 hwei       (501) staff       (20)     2714 2022-10-22 06:06:43.000000 knifes-0.8.9/knifes/urls.py
--rw-r--r--   0 hwei       (501) staff       (20)     4333 2022-01-21 03:14:54.000000 knifes-0.8.9/knifes/useragent.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2022-11-03 11:19:21.636540 knifes-0.8.9/knifes.egg-info/
--rw-r--r--   0 hwei       (501) staff       (20)      765 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      576 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/SOURCES.txt
--rw-r--r--   0 hwei       (501) staff       (20)        1 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/dependency_links.txt
--rw-r--r--   0 hwei       (501) staff       (20)       27 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/requires.txt
--rw-r--r--   0 hwei       (501) staff       (20)        7 2022-11-03 11:19:21.000000 knifes-0.8.9/knifes.egg-info/top_level.txt
--rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.9/pyproject.toml
--rw-r--r--   0 hwei       (501) staff       (20)       38 2022-11-03 11:19:21.636925 knifes-0.8.9/setup.cfg
--rw-r--r--   0 hwei       (501) staff       (20)      900 2022-11-03 11:19:10.000000 knifes-0.8.9/setup.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.150734 knifes-0.8.90/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-04 10:49:26.150575 knifes-0.8.90/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.8.90/README.md
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.149607 knifes-0.8.90/knifes/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.8.90/knifes/aes.py
+-rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.8.90/knifes/alarm.py
+-rw-r--r--   0 hwei       (501) staff       (20)      740 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/auth.py
+-rw-r--r--   0 hwei       (501) staff       (20)      502 2023-07-29 10:19:19.000000 knifes-0.8.90/knifes/constants.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7208 2023-07-31 13:37:02.000000 knifes-0.8.90/knifes/decorators.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7567 2023-06-14 01:08:29.000000 knifes-0.8.90/knifes/deploy.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.8.90/knifes/digests.py
+-rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.8.90/knifes/envconfig.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1649 2022-11-17 08:15:03.000000 knifes-0.8.90/knifes/file.py
+-rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.8.90/knifes/getui.py
+-rw-r--r--   0 hwei       (501) staff       (20)      732 2022-03-13 09:06:03.000000 knifes-0.8.90/knifes/jsons.py
+-rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.8.90/knifes/logging.py
+-rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.8.90/knifes/media.py
+-rw-r--r--   0 hwei       (501) staff       (20)      924 2023-02-21 04:17:56.000000 knifes-0.8.90/knifes/misc.py
+-rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.8.90/knifes/operators.py
+-rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.8.90/knifes/package.py
+-rw-r--r--   0 hwei       (501) staff       (20)      863 2023-07-31 13:36:03.000000 knifes-0.8.90/knifes/randoms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1895 2023-07-30 11:26:01.000000 knifes-0.8.90/knifes/results.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.8.90/knifes/roar.py
+-rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.8.90/knifes/shell.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.8.90/knifes/sms.py
+-rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.8.90/knifes/strings.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1335 2023-07-31 13:41:32.000000 knifes-0.8.90/knifes/times.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.8.90/knifes/urls.py
+-rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.8.90/knifes/useragent.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-08-04 10:49:26.150369 knifes-0.8.90/knifes.egg-info/
+-rw-r--r--   0 hwei       (501) staff       (20)      766 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      626 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/SOURCES.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        1 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/dependency_links.txt
+-rw-r--r--   0 hwei       (501) staff       (20)       27 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/requires.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        7 2023-08-04 10:49:26.000000 knifes-0.8.90/knifes.egg-info/top_level.txt
+-rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.8.90/pyproject.toml
+-rw-r--r--   0 hwei       (501) staff       (20)       38 2023-08-04 10:49:26.150782 knifes-0.8.90/setup.cfg
+-rw-r--r--   0 hwei       (501) staff       (20)      901 2023-08-04 10:49:11.000000 knifes-0.8.90/setup.py
```

### Comparing `knifes-0.8.9/PKG-INFO` & `knifes-0.8.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.9
+Version: 0.8.90
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.9/knifes/aes.py` & `knifes-0.8.90/knifes/aes.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.9/knifes/auth.py` & `knifes-0.8.90/knifes/auth.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.9/knifes/deploy.py` & `knifes-0.8.90/knifes/deploy.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,53 +13,111 @@
 PIDFile={PIDFile}
 ExecStart={ExecStart}
 
 [Install]
 WantedBy=multi-user.target"""
 
 
-def print_help(project_dir):
+def print_help(project_dir, app_name):
     print('reload      --reload gunicorn\n'
           'start       --start gunicorn\n'
           'log n       --read gunicorn last log\n'
           'modules     --install modules\n'
           'knifes      --force install latest knifes\n'
-          'autostart    --autostart at boot\n\n'
+          'pull        --pull latest code\n'
+          'autostart   --autostart at boot\n'
+          'celery [start | restart | stop]\n'
+          'celerybeat [start | restart | stop]\n\n'
+          f'systemctl status {app_name}.gunicorn.service\n\n'
           'activate virtual environment cmd:\n\n'
-          'source {}venv/bin/activate'.format(project_dir))
+          f'source {project_dir}venv/bin/activate')
 
 
-def main_script(chdir, logdir, app_name):
+def main_script(chdir, logdir, app_name, project_name=None):
+    if not project_name:
+        project_name = app_name
+
     args = sys.argv[1:]
     if not args:
-        print_help(chdir)
+        print_help(chdir, app_name)
     elif args[0] == 'reload':
         reload_gunicorn(chdir, logdir)
     elif args[0] == 'modules':
         install_modules(chdir)
+    elif args[0] == 'pull':
+        pull_latest_code(chdir)
     elif args[0] == 'log':
         line_count = 10 if len(args) == 1 else args[1]
         read_last_log(logdir, line_count)
     elif args[0] == 'start':
         start_gunicorn(chdir, logdir, app_name)
     elif args[0] == 'knifes':
         install_latest_knifes(chdir)
     elif args[0] == 'autostart':
         autostart_at_boot(chdir, logdir, app_name)
+    elif args[0] == 'celery':
+        celery(chdir, logdir, project_name, args[1], False)
+    elif args[0] == 'celerybeat':
+        celery(chdir, logdir, project_name, args[1], True)
     else:
-        print_help(chdir)
+        print_help(chdir, app_name)
+
+
+def celery(project_dir, log_dir, project_name, operate, is_beat=False):
+    if operate not in ('restart', 'stop', 'start'):
+        print_err('not supported operate, only supports [start | restart | stop]')
+        return
+
+    type_ = 'beat' if is_beat else 'worker'
+    pid_file = f'{log_dir}celery_{type_}.pid'
+    log_file = f'{log_dir}celery_{type_}{"" if is_beat else "%I"}.log'
+
+    # stop
+    if operate in ('restart', 'stop'):
+        pid = read_file(pid_file).strip()
+        if not pid:
+            print_err(f'restart/stop {type_} failed，pid not exists:{pid_file}')
+            return
+        exec_shell(f'kill -KILL {pid}')
+        print_succ(f'stopped old {type_} process: {pid}')
+
+    # start new process
+    if operate in ('restart', 'start'):
+        cmd = f'cd {project_dir} && venv/bin/celery -A {project_name} {type_} --pidfile={pid_file} --logfile={log_file} --loglevel=INFO --detach'
+        if not is_beat:
+            cmd += ' --concurrency=1'
+        # 判断是否已启动
+        succ, err = exec_shell(f"pgrep -f '{cmd}'")
+        if succ:
+            print_err('it is currently started, please restart it through the restart command')
+            return
+        succ, err = exec_shell(cmd)
+        print_succ(succ)
+        print_err(err)
+        time.sleep(1)
+        print_succ(f'new {type_} process: {read_file(pid_file).strip()}')
 
 
 def install_latest_knifes(project_dir):
     cmd = 'source {}venv/bin/activate && pip install knifes --index-url https://pypi.python.org/simple -U'.format(project_dir)
     succ, err = exec_shell(cmd)
     print_succ(succ)
     print_err(err)
 
 
+def pull_latest_code(project_dir):
+    cmd = f'cd {project_dir} && git pull origin master'
+    ret = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    if ret.returncode != 0:
+        print_err(ret.stderr.decode())
+        raise SystemExit
+    print_succ(ret.stdout.decode())
+    print_succ(ret.stderr.decode())  # warning message
+
+
 def install_modules(project_dir):
     cmd = 'source {}venv/bin/activate && pip install -r {}requirements.txt'.format(project_dir, project_dir)
     ret = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     if ret.returncode != 0:
         print_err(ret.stderr.decode())
         raise SystemExit
     print_succ(ret.stdout.decode())
@@ -91,14 +149,15 @@
 
     ret = subprocess.run(f'systemctl daemon-reload && systemctl enable {app_name}.gunicorn.service', shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     if ret.returncode != 0:
         print_err(ret.stderr.decode())
         print_err('设置开机自启动失败')
         raise SystemExit
     print_succ(ret.stdout.decode())
+    print_succ(ret.stderr.decode())  # warning message
     print_succ('已设置开机自启动')
 
 
 
 def start_gunicorn(project_dir, log_dir, app_name):
     """
     调用前先在project目录下创建venv环境,如:
@@ -126,14 +185,15 @@
     read_last_log(log_dir, 6)
 
     # 配置开机启动
     autostart_at_boot(project_dir, log_dir, app_name)
 
 
 def reload_gunicorn(project_dir, log_dir):
+    pull_latest_code(project_dir)
     install_modules(project_dir)
 
     pid_file = f'{log_dir}pid.pid'
     pid = read_file(pid_file).strip()
     if not pid:
         print_err(f'重启gunicorn失败,pid不存在:{pid_file}')
     exec_shell('kill -HUP {}'.format(pid))
```

### Comparing `knifes-0.8.9/knifes/digests.py` & `knifes-0.8.90/knifes/digests.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.9/knifes/jsons.py` & `knifes-0.8.90/knifes/jsons.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.9/knifes/misc.py` & `knifes-0.8.90/knifes/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import TypeVar
 from django.http import HttpRequest
-import logging
 T = TypeVar('T')
 
 
 def get_client_ip(request):
     x_forwarded_for = request.META.get('HTTP_X_FORWARDED_FOR')
     if x_forwarded_for:
         ip = x_forwarded_for.split(',')[0]
@@ -14,20 +13,23 @@
 
 
 def get_request_param_strip_spaces(request: HttpRequest, key):
     value = request.POST.get(key, request.GET.get(key))
     return value.strip() if value else value
 
 
+def get_param_values_from_request(request, *param_names):
+    values = []
+    for param in param_names:
+        values.append(request.POST.get(param, request.GET.get(param)))
+    return tuple(values)
+
+
 def get_object_or_None(T, **kwargs) -> T:
     objs = T.objects.filter(**kwargs)
     return objs[0] if objs else None
 
 
 def get_value_or_None(T, **kwargs) -> T:
     objs = T.objects.filter(**kwargs).values()
     return objs[0] if objs else None
 
-
-class OnlyDebugLevel(logging.Filter):
-    def filter(self, record):
-        return record.levelname == 'DEBUG'
```

### Comparing `knifes-0.8.9/knifes/randoms.py` & `knifes-0.8.90/knifes/randoms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import random
 import string
-from knifes.digests import md5
 from knifes import times
 import uuid
 
 id_alphabet = string.ascii_uppercase + string.digits
 
 
 def random_str(length=4):
     return ''.join(random.choices(string.ascii_lowercase + string.digits, k=length))
 
 
-# 16位唯一的
+# 32位唯一的字符串
 def make_unique_str():
-    return md5(str(uuid.uuid1()))
+    return str(uuid.uuid4()).replace('-', '')
 
 
 # 碰撞概率极小的(唯一的)随机ID
 # 建议长度 >= 10
 def random_str_id(length=10):
-    id = get_short_code_from_num(times.current_milli_time())
-    if len(id) < length:
-        return ''.join(random.choices(id_alphabet, k=length - len(id))) + id
-    elif len(id) > length:
-        return id[0:length]
+    id_ = get_short_code_from_num(times.current_milli_time())
+    if len(id_) < length:
+        return ''.join(random.choices(id_alphabet, k=length - len(id_))) + id_
+    elif len(id_) > length:
+        return id_[0:length]
     else:
-        return id
+        return id_
 
 
 def get_short_code_from_num(num):
     code = ''
     while num > 0:
         index = num % 36
         num = (num - index) // 36
```

### Comparing `knifes-0.8.9/knifes/results.py` & `knifes-0.8.90/knifes/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,49 +16,45 @@
 
     @classmethod
     def get_by_code(cls, code) -> Optional[BaseErrorEnum]:
         return next(filter(lambda x: x.code == code, cls.__members__.values()), None)
 
 
 class ApiResult:
-    code = 200
-    succ = True
-    msg = ''
-    msg_detail = ''
-    data = None
+    def __init__(self, code, *, msg=None, msg_detail=None, data=None):
+        self.code = code
+        self.succ = (code == 200)
+        self.msg = msg
+        self.msg_detail = msg_detail
+        self.data = data
 
     @classmethod
     def fail(cls, msg, code=400, msg_detail=None):
-        ret = ApiResult()
-        ret.succ = False
-        ret.code = code
-        ret.msg = msg
-        ret.msg_detail = msg_detail
-        return ret
+        return ApiResult(code, msg=msg, msg_detail=msg_detail)
 
     @classmethod
     def succ(cls, data=None):
-        ret = ApiResult()
-        ret.code = 200
-        ret.succ = True
-        ret.data = data
-        return ret
+        return ApiResult(200, data=data)
 
     @classmethod
     def succResponse(cls, data=None):
         return JsonResponse(cls.succ(data), encoder=ObjectEncoder, safe=False)
 
     @classmethod
     def failResponse(cls, msg, code=400, msg_detail=None):
         return JsonResponse(cls.fail(msg, code=code, msg_detail=msg_detail), encoder=ObjectEncoder, safe=False)
 
     @classmethod
     def errorResponse(cls, error_enum: BaseErrorEnum, msg_detail=None):
         return JsonResponse(cls.fail(error_enum.msg, code=error_enum.code, msg_detail=msg_detail), encoder=ObjectEncoder, safe=False)
 
     @classmethod
-    def tokenInvalid(cls, msg=_('请先登录')):
-        return cls.failResponse(msg, code=300)
-
-    @classmethod
     def missingParam(cls, msg=_('缺少参数')):
         return cls.failResponse(msg)
+
+    @classmethod
+    def unauthorized(cls, msg=_('请先登录')):
+        return cls.failResponse(msg, code=401)
+
+    @classmethod
+    def tokenInvalid(cls, msg=_('请先登录')):    # TODO 废弃
+        return cls.failResponse(msg, code=300)
```

### Comparing `knifes-0.8.9/knifes/roar.py` & `knifes-0.8.90/knifes/roar.py`

 * *Files identical despite different names*

### Comparing `knifes-0.8.9/knifes/sms.py` & `knifes-0.8.90/knifes/sms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from tencentcloud.common import credential
 from tencentcloud.common.profile.client_profile import ClientProfile
 from tencentcloud.common.profile.http_profile import HttpProfile
 from tencentcloud.sms.v20210111 import sms_client, models
 from typing import List
-from knifes._settings import settings
-exceed_limit_codes = ["LimitExceeded.PhoneNumberDailyLimit", "LimitExceeded.PhoneNumberOneHourLimit", "LimitExceeded.PhoneNumberSameContentDailyLimit", "LimitExceeded.PhoneNumberThirtySecondLimit"]
+from django.conf import settings
+import re
+pattern_china_mainland_phone_number = re.compile(r'^1\d{10}$')
+exceed_limit_codes = ['LimitExceeded.PhoneNumberDailyLimit', 'LimitExceeded.PhoneNumberOneHourLimit', 'LimitExceeded.PhoneNumberSameContentDailyLimit', 'LimitExceeded.PhoneNumberThirtySecondLimit']
+incorrect_number_codes = ['InvalidParameterValue.IncorrectPhoneNumber']
 
 
-class LimitExceededError(Exception):
+class SmsError(Exception):
     pass
 
 
-class SendFailedError(Exception):
+class LimitExceededError(SmsError):
+    pass
+
+
+class IncorrectNumberError(SmsError):
+    pass
+
+
+class SendFailedError(SmsError):
     pass
 
 
 def send_sms_msg_by_tencent_cloud(sign_name, phone, template_id, template_param_list: List[str] = None):
     if template_param_list is None:
         template_param_list = []
     cred = credential.Credential(settings.TENCENT_CLOUD_SMS_SECRET_ID, settings.TENCENT_CLOUD_SMS_SECRET_KEY)
@@ -30,9 +41,17 @@
     req.TemplateId = template_id
     req.TemplateParamSet = template_param_list
 
     resp = client.SendSms(req)
     code = resp.SendStatusSet[0].Code
     if code in exceed_limit_codes:
         raise LimitExceededError('该手机号短信发送频率太高，请稍后重试~')
+    if code in incorrect_number_codes:
+        raise IncorrectNumberError('手机号格式错误')
     if code != 'Ok':
         raise SendFailedError('发送失败，请重试！')
+
+
+def is_china_mainland_phone_number(phone):
+    return True if re.match(pattern_china_mainland_phone_number, str(phone)) else False
+
+
```

### Comparing `knifes-0.8.9/knifes/strings.py` & `knifes-0.8.90/knifes/strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-def desensitizePhone(phone):
-    """
-    废弃
-    """
-    return '****'.join([phone[:3], phone[7:]])
-
-
 # 手机号脱敏
 def blur_phone(phone):
     if not phone or len(phone) < 11:
         return phone
     return phone[:3] + '****' + phone[7:]
```

### Comparing `knifes-0.8.9/knifes/times.py` & `knifes-0.8.90/knifes/times.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from datetime import datetime, timedelta, date, time
 import time as time_module
 
+SECONDS_PER_DAY = int(timedelta(days=1).total_seconds())
+SECONDS_PER_HOUR = int(timedelta(hours=1).total_seconds())
+SECONDS_PER_MINUTE = int(timedelta(minutes=1).total_seconds())
+
 
 def to_timestamp(val: datetime, unit='second'):
     if not val:
         return None
     if unit == 'millisecond':
         return int(val.timestamp()) * 1000
     return int(val.timestamp())
@@ -42,8 +46,8 @@
         t = int(t)
     return datetime.fromtimestamp(t // 1000)
 
 
 def fromtimestamp_in_sec(t) -> datetime:
     if not isinstance(t, int):
         t = int(t)
-    return datetime.fromtimestamp(t)
+    return datetime.fromtimestamp(t)
```

### Comparing `knifes-0.8.9/knifes/urls.py` & `knifes-0.8.90/knifes/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib import parse
 import mimetypes
-from knifes.constants import MediaType
+from knifes.media import MediaType, extension_to_media_type_dict
 from typing import Optional, Union
 import validators
+import os
 
 
 def get_url_from_text(text):
     if not text:
         return text
     start_index = text.rfind('http://')
     if start_index == -1:
@@ -56,36 +57,47 @@
 
 # 目前支持video、audio、image类型，其他返回None
 # fixed bug for 'http://v.example.com/o0/000bH9u0lx07TQ0OHwmA01041200Onth0E010.mp4?label=mp4_hd&template=852x480.28.0&ori=0&ps=1CwnkDw1GXwCQx&Expires=1645114865&ssig=8QbZXUCE85&KID=unistore,video'
 def guess_media_type(url) -> Optional[MediaType]:
     url_without_query = url[:url.index('?')] if '?' in url else url
     mimetype, _ = mimetypes.guess_type(url_without_query)
     if not mimetype:
-        return None
+        return extension_to_media_type_dict.get(get_extension(url_without_query.lower()))
+    if mimetype in ('application/x-mpegurl', 'application/vnd.apple.mpegurl'):   # .m3u8
+        return MediaType.VIDEO
     try:
         return MediaType(mimetype.split('/')[0])
     except:
         return None
 
 
-def parse_query(url, _key=None) -> Union[dict, str, None]:
+def parse_query(url, key_=None) -> Union[dict, str, None]:
     query_dict = dict(parse.parse_qsl(parse.urlparse(url).query))
-    return query_dict.get(_key) if _key else query_dict
+    return query_dict.get(key_) if key_ else query_dict
 
 
-def parse_path(url, _index: int = None) -> Union[list, str, None]:
+def parse_path(url, index_: int = None) -> Union[list, str, None]:
     path_list = parse.urlparse(url).path.strip('/').split('/')
-    if _index is not None:
-        return path_list[_index] if len(path_list) > _index else None
+    if index_ is not None:
+        return path_list[index_] if len(path_list) > index_ else None
     return path_list
 
 
+def parse_url(url) -> (str, list, dict):
+    """return (netloc、path_list, query_dict)"""
+    parsed = parse.urlparse(url)
+    return parsed.netloc, parsed.path.strip('/').split('/'), dict(parse.parse_qsl(parsed.query))
+
+
 def sanitize_url(url, scheme='http'):
     """ Prepend protocol-less URLs with `http:` scheme in order to mitigate
     the number of unwanted failures due to missing protocol
     """
     if not url:
         return url
     if url.startswith('//'):
         return f'{scheme}:{url}'
     return url
 
+
+def get_extension(url):
+    return os.path.splitext(parse.urlparse(url).path)[1]
```

### Comparing `knifes-0.8.9/knifes/useragent.py` & `knifes-0.8.90/knifes/useragent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import random
 
+default = 'Mozilla/5.0'
+
 _pc = [
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36',
     'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2866.71 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/52.0.2762.73 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2656.18 Safari/537.36',
     'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:77.0) Gecko/20190101 Firefox/77.0',
@@ -48,11 +50,10 @@
     return _mobile[0]
 
 
 def random_mobile_ua():
     return random.choice(_mobile)
 
 
-def ua_headers(useragent):
-    return {'user-agent': useragent}
-
+def ua_headers(useragent=None):
+    return {'User-Agent': default if useragent is None else useragent}
```

### Comparing `knifes-0.8.9/knifes.egg-info/PKG-INFO` & `knifes-0.8.90/knifes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.8.9
+Version: 0.8.90
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.8.9/knifes.egg-info/SOURCES.txt` & `knifes-0.8.90/knifes.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 README.md
 pyproject.toml
 setup.py
 knifes/__init__.py
-knifes/_settings.py
 knifes/aes.py
 knifes/alarm.py
 knifes/auth.py
 knifes/constants.py
 knifes/decorators.py
 knifes/deploy.py
 knifes/digests.py
 knifes/envconfig.py
 knifes/file.py
+knifes/getui.py
 knifes/jsons.py
 knifes/logging.py
+knifes/media.py
 knifes/misc.py
+knifes/operators.py
+knifes/package.py
 knifes/randoms.py
 knifes/results.py
 knifes/roar.py
 knifes/shell.py
 knifes/sms.py
 knifes/strings.py
 knifes/times.py
```

### Comparing `knifes-0.8.9/setup.py` & `knifes-0.8.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knifes",
-    version="0.8.9",
+    version="0.8.90",
     author="knifes",
     author_email="author@example.com",
     description="Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     classifiers=[
```

