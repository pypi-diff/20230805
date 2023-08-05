# Comparing `tmp/py3status_amdfan-0.1.7.tar.gz` & `tmp/py3status_amdfan-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3status_amdfan-0.1.7.tar", max compression
+gzip compressed data, was "py3status_amdfan-0.1.8.tar", max compression
```

## Comparing `py3status_amdfan-0.1.7.tar` & `py3status_amdfan-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2021-04-10 23:07:50.266458 py3status_amdfan-0.1.7/LICENSE
--rw-r--r--   0        0        0     1907 2021-12-01 00:57:46.858655 py3status_amdfan-0.1.7/README.md
--rw-r--r--   0        0        0     1114 2022-12-31 20:34:31.821072 py3status_amdfan-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2021-03-06 23:15:12.096058 py3status_amdfan-0.1.7/src/py3status_amdfan/__init__.py
--rw-r--r--   0        0        0     1006 2021-04-10 23:15:22.852560 py3status_amdfan-0.1.7/src/py3status_amdfan/fan_monitor.py
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 py3status_amdfan-0.1.7/setup.py
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 py3status_amdfan-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-04-10 23:07:50.266458 py3status_amdfan-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1907 2021-12-01 00:57:46.858655 py3status_amdfan-0.1.8/README.md
+-rw-r--r--   0        0        0     1096 2023-03-08 01:39:57.266344 py3status_amdfan-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-03-06 23:15:12.096058 py3status_amdfan-0.1.8/src/py3status_amdfan/__init__.py
+-rw-r--r--   0        0        0     1006 2021-04-10 23:15:22.852560 py3status_amdfan-0.1.8/src/py3status_amdfan/fan_monitor.py
+-rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 py3status_amdfan-0.1.8/setup.py
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 py3status_amdfan-0.1.8/PKG-INFO
```

### Comparing `py3status_amdfan-0.1.7/LICENSE` & `py3status_amdfan-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py3status_amdfan-0.1.7/README.md` & `py3status_amdfan-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `py3status_amdfan-0.1.7/pyproject.toml` & `py3status_amdfan-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py3status-amdfan"
-version = "0.1.7"
+version = "0.1.8"
 description = "py3status monitor to show amdgpu fan speeds and temp"
 authors = ["mcgillij <mcgillivray.jason@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mcgillij/py3status-amdfan"
 repository = "https://github.com/mcgillij/py3status-amdfan"
 documentation = "https://github.com/mcgillij/py3status-amdfan"
@@ -22,18 +22,18 @@
 
 [tool.poetry.plugins."py3status"]
 module = "py3status_amdfan.fan_monitor"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 py3status = "^3.47"
-amdfan = "^0.1.21"
+amdfan = "^0.1.22"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-pylint = "^2.15.9"
-flake8 = "^6.0.0"
+black = "*"
+pylint = "*"
+flake8 = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py3status_amdfan-0.1.7/src/py3status_amdfan/fan_monitor.py` & `py3status_amdfan-0.1.8/src/py3status_amdfan/fan_monitor.py`

 * *Files identical despite different names*

### Comparing `py3status_amdfan-0.1.7/setup.py` & `py3status_amdfan-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['py3status_amdfan']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['amdfan>=0.1.21,<0.2.0', 'py3status>=3.47,<4.0']
+['amdfan>=0.1.22,<0.2.0', 'py3status>=3.47,<4.0']
 
 entry_points = \
 {'py3status': ['module = py3status_amdfan.fan_monitor']}
 
 setup_kwargs = {
     'name': 'py3status-amdfan',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'py3status monitor to show amdgpu fan speeds and temp',
     'long_description': '# py3status-amdfan\nPython module for monitoring fan RPMs and temperature for `amdgpu` cards in **i3wm** using py3status.\n\n[![Downloads](https://static.pepy.tech/personalized-badge/py3status-amdfan?period=total&units=international_system&left_color=blue&right_color=green&left_text=Downloads)](https://pepy.tech/project/py3status-amdfan)\n\n## Screenshot\n![Status Bar with py3status_amdfan](https://raw.githubusercontent.com/mcgillij/py3status-amdfan/main/images/py3status-amdfan.png)\n\n## Prerequisites\n\n* i3\n* py3status\n* [amdfan](https://github.com/mcgillij/amdfan)\n* poetry (if installing from git)\n\n## Installation\n\n### From Git\n\n``` bash\ngit clone https://github.com/mcgillij/py3status-amdfan.git\ncd py3status-amdfan && poetry install\nmkdir -p ~/.i3/py3status && cd ~/.i3/py3status\nln -s <PATH_TO_CLONED_REPO>/src/py3status_amdfan/fan_monitor.py ./\n```\n\n### With Pip, Pipenv or Poetry\n\n``` bash\npip install py3status-amdfan amdfan\npipenv install py3status-amdfan amdfan\npoetry add py3status-amdfan amdfan && poetry install\n```\n\n### With `yay`\n\n``` bash\nyay -S py3status-amdfan amdfan\n```\n\n### Building Arch package w/PKGBUILD\n\n``` bash\ngit clone https://aur.archlinux.org/py3status-amdfan.git\ncd py3status-amdfan.git\nmakechrootpkg -c -r $HOME/$CHROOT\n```\n\n### Installing built Arch package\n\n``` bash\nsudo pacman -U --asdeps py3status-amdfan-*-any.pkg.tar.zst\n```\n\n## Configuration\n\nNext you will need to add the services you want to monitor, and optionally choose some appropriate emoji\'s.\nYou can also configure actions to open up your browser when you click on the icon, which I find pretty handy.\n\n**~/.config/i3/i3status.conf**\n\n```bash\n...\norder += "fan_monitor"\norder += "clock"\norder += "mail"\n...\n```\n\n## Configuration Options\n\nYou can pass in the following configuration options:\n\n* cache_timeout\n* format\n\n## Restart i3\n\nOnce the package is installed and configured you just need to restart i3.\n',
     'author': 'mcgillij',
     'author_email': 'mcgillivray.jason@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mcgillij/py3status-amdfan',
```

### Comparing `py3status_amdfan-0.1.7/PKG-INFO` & `py3status_amdfan-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3status-amdfan
-Version: 0.1.7
+Version: 0.1.8
 Summary: py3status monitor to show amdgpu fan speeds and temp
 Home-page: https://github.com/mcgillij/py3status-amdfan
 License: MIT
 Keywords: amdgpu,monitor,fan,i3,py3status
 Author: mcgillij
 Author-email: mcgillivray.jason@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -14,15 +14,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: Window Managers
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: amdfan (>=0.1.21,<0.2.0)
+Requires-Dist: amdfan (>=0.1.22,<0.2.0)
 Requires-Dist: py3status (>=3.47,<4.0)
 Project-URL: Documentation, https://github.com/mcgillij/py3status-amdfan
 Project-URL: Repository, https://github.com/mcgillij/py3status-amdfan
 Description-Content-Type: text/markdown
 
 # py3status-amdfan
 Python module for monitoring fan RPMs and temperature for `amdgpu` cards in **i3wm** using py3status.
```

