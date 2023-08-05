# Comparing `tmp/amdfan-0.1.8.tar.gz` & `tmp/amdfan-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amdfan-0.1.8.tar", last modified: Sat Apr 10 22:57:49 2021, max compression
+gzip compressed data, was "amdfan-0.1.9.tar", last modified: Sun Apr 11 00:18:42 2021, max compression
```

## Comparing `amdfan-0.1.8.tar` & `amdfan-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    18092 2021-02-10 21:17:30.562814 amdfan-0.1.8/LICENSE
--rw-r--r--   0        0        0     6434 2021-04-09 01:24:26.885501 amdfan-0.1.8/README.md
--rw-r--r--   0        0        0     1161 2021-04-10 19:52:57.628468 amdfan-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-10 21:07:11.880338 amdfan-0.1.8/src/amdfan/__init__.py
--rwxr-xr-x   0        0        0    12211 2021-04-10 22:40:53.249365 amdfan-0.1.8/src/amdfan/amdfan.py
--rw-r--r--   0        0        0      136 2021-02-12 22:00:12.935069 amdfan-0.1.8/src/amdfan/amdfan.service
--rw-r--r--   0        0        0     7552 2021-04-10 22:57:49.941683 amdfan-0.1.8/setup.py
--rw-r--r--   0        0        0     7696 2021-04-10 22:57:49.941890 amdfan-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    18092 2021-02-10 21:17:30.562814 amdfan-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6434 2021-04-09 01:24:26.885501 amdfan-0.1.9/README.md
+-rw-r--r--   0        0        0     1161 2021-04-11 00:18:16.839798 amdfan-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-04-10 22:58:20.978751 amdfan-0.1.9/src/amdfan/__init__.py
+-rwxr-xr-x   0        0        0    12211 2021-04-10 22:58:20.978751 amdfan-0.1.9/src/amdfan/amdfan.py
+-rw-r--r--   0        0        0      136 2021-04-10 22:58:20.978751 amdfan-0.1.9/src/amdfan/amdfan.service
+-rw-r--r--   0        0        0     7552 2021-04-11 00:18:42.523576 amdfan-0.1.9/setup.py
+-rw-r--r--   0        0        0     7696 2021-04-11 00:18:42.523784 amdfan-0.1.9/PKG-INFO
```

### Comparing `amdfan-0.1.8/LICENSE` & `amdfan-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amdfan-0.1.8/README.md` & `amdfan-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amdfan-0.1.8/pyproject.toml` & `amdfan-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amdfan"
-version = "0.1.8"
+version = "0.1.9"
 description = "Fan monitor and controller for AMD gpus in Linux"
 authors = ["mcgillij <mcgillivray.jason@gmail.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://mcgillij.dev/pages/amdfan.html"
 repository = "https://github.com/mcgillij/amdfan"
 documentation = "https://mcgillij.dev/pages/amdfan.html"
@@ -23,16 +23,16 @@
 
 include = [ "LICENSE", ]
 
 [tool.poetry.dependencies]
 python = "^3.7 || ^3.8 || ^3.9"
 numpy = "^1.20.1"
 PyYAML = "^5.4.1"
-rich = "^9.10.0"
 click = "^7.1.2"
+rich = "^10.1.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.6.0"
 flake8 = "^3.8.4"
 black = "^20.8b1"
 pytest = "^6.2.2"
```

### Comparing `amdfan-0.1.8/src/amdfan/amdfan.py` & `amdfan-0.1.9/src/amdfan/amdfan.py`

 * *Files identical despite different names*

### Comparing `amdfan-0.1.8/setup.py` & `amdfan-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.4.1,<6.0.0',
  'click>=7.1.2,<8.0.0',
  'numpy>=1.20.1,<2.0.0',
- 'rich>=9.10.0,<10.0.0']
+ 'rich>=10.1.0,<11.0.0']
 
 entry_points = \
 {'console_scripts': ['amdfan = amdfan.amdfan:cli']}
 
 setup_kwargs = {
     'name': 'amdfan',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Fan monitor and controller for AMD gpus in Linux',
     'long_description': '# AmdFan\n![Python package](https://github.com/mcgillij/amdfan/workflows/Python%20package/badge.svg)\n[![Downloads](https://static.pepy.tech/personalized-badge/amdfan?period=total&units=international_system&left_color=blue&right_color=green&left_text=PyPi%20Downloads)](https://pepy.tech/project/amdfan)\n\nIs a fork of amdgpu-fan, with security updates and added functionality.\n\n## Why fork?\n\n* alternatives abandoned\n* lacking required features\n* security fixes not addressed\n* basic functionality not working\n\n### Amdgpu_fan abandoned\n\nAs of a couple years ago, and isn’t applying any security fixes to their project or improvements. There were also some bugs that bothered me with the project when I tried to get it up and running.\nFeatures missing\n\nThere are a number of features that I wanted, but weren’t available.\n\n* Thresholds allow temperature range before changing fan speed\n* Frequency setting to allow better control\n* Monitoring to be able to see real-time fan speeds and temperature\n\n### Security Fixes\n\nThere are some un-addressed pull requests for some recent YAML vulnerabilities that are still present in the old amdgpu_fan project, that I’ve addressed in this fork.\n\n### Basic functionality\n\nSetting the card to system managed using the amdgpu_fan pegs your GPU fan at 100%, instead of allowing the system to manage the fan settings. I fixed that bug as well in this release.\n\nThese are all addressed in Amdfan, and as long as I’ve still got some AMD cards I intend to at least maintain this for myself. And anyone’s able to help out since this is open source. I would have liked to just contribute these fixes to the main project, but it’s now inactive.\n\n# Documentation\n## Usage\n\n``` bash\nUsage: amdfan.py [OPTIONS]\n\nOptions:\n  --daemon         Run as daemon applying the fan curve\n  --monitor        Run as a monitor showing temp and fan speed\n  --manual         Manually set the fan speed value of a card\n  --configuration  Prints out the default configuration for you to use\n  --service        Prints out the amdfan.service file to use with systemd\n  --help           Show this message and exit.\n```\n\n## Daemon\n\nAmdfan is also runnable as a systemd service, with the provided ```amdfan.service```.\n\n## Monitor\n\nYou can use Amdfan to monitor your AMD video cards using the ```--monitor``` flag.\n\n![screenshot](https://raw.githubusercontent.com/mcgillij/amdfan/main/images/screenshot.png)\n\n## Manual\n\nAlternatively if you don\'t want to set a fan curve, you can just apply a fan setting manually. \nAlso allows you to revert the fan control to the systems default behavior by using the "auto" parameter.\n![screenshot](https://raw.githubusercontent.com/mcgillij/amdfan/main/images/manual.png)\n\n## Configuration\n\nThis will dump out the default configuration that would get generated for `/etc/amdfan.yml` when you first run it as a service. This allows you to configure the settings prior to running it as a daemon if you wish.\n\nRunning `amdfan --configuration` will output the following block to STDOUT.\n\n``` bash\n#Fan Control Matrix.\n# [<Temp in C>,<Fanspeed in %>]\nspeed_matrix:\n- [4, 4]\n- [30, 33]\n- [45, 50]\n- [60, 66]\n- [65, 69]\n- [70, 75]\n- [75, 89]\n- [80, 100]\n\n# Current Min supported value is 4 due to driver bug\n#\n# Optional configuration options\n#\n# Allows for some leeway +/- temp, as to not constantly change fan speed\n# threshold: 4\n#\n# Frequency will change how often we probe for the temp\n# frequency: 5\n#\n# While frequency and threshold are optional, I highly recommend finding\n# settings that work for you. I\'ve included the defaults I use above.\n#\n# cards:\n# can be any card returned from `ls /sys/class/drm | grep "^card[[:digit:]]$"`\n# - card0\n```\nYou can use this to generate your configuration by doing ``amdfan --configuration > amdfan.yml``, you can then modify the settings and place it in ``/etc/amdfan.yml`` for when you would like to run it as a service.\n\n## Service\n\nThis is just a convenience method for dumping out the `amdfan.service` that would get installed if you used a package manager to install amdfan. Useful if you installed the module via `pip`, `pipenv` or `poetry`.\n\nRunning `amdfan --service` will output the following block to STDOUT.\n\n``` bash\n[Unit]\nDescription=amdfan controller\n\n[Service]\nExecStart=/usr/bin/amdfan --daemon\nRestart=always\n\n[Install]\nWantedBy=multi-user.target\n```\n\n# Note\n\nMonitoring fan speeds and temperatures can run with regular user permissions.\n`root` permissions are required for changing the settings / running as a daemon.\n\n# Recommended settings\n\nBelow is the settings that I use on my machines to control the fan curve without too much fuss, but you should find a frequency and threshold setting that works for your workloads.\n\n`/etc/amdfan.yml`\n``` bash\nspeed_matrix:\n- [4, 4]\n- [30, 33]\n- [45, 50]\n- [60, 66]\n- [65, 69]\n- [70, 75]\n- [75, 89]\n- [80, 100]\n\nthreshold: 4\nfrequency: 5\n```\n\n## Installing the systemd service\nIf you installed via the AUR, the service is already installed, and you just need to *start/enable* it. If you installed via pip/pipenv or poetry, you can generate your systemd service file with the following command.\n\n``` bash\namdfan --service > amdfan.service && sudo mv amdfan.service /usr/lib/systemd/system/\n```\n\n## Starting the systemd service\n\nTo run the service, you can run the following commands to **start/enable** the service.\n\n``` bash\nsudo systemctl start amdfan\nsudo systemctl enable amdfan\n```\n\nAfter you\'ve started it, you may want to edit the settings found in `/etc/amdfan.yml`. Once your happy with those, you can restart amdfan with the following command.\n\n``` bash\nsudo systemctl restart amdfan\n```\n\n## Checking the status\nYou can check the systemd service status with the following command:\n\n``` bash\nsystemctl status amdfan\n```\n\n\n## Building Arch AUR package\n\nBuilding the Arch package assumes you already have a chroot env setup to build packages.\n\n```bash\ngit clone https://aur.archlinux.org/amdfan.git\ncd amdfan/\nmakechrootpkg -c -r $HOME/$CHROOT\n```\n\n## Installing the Arch package\n\n``` bash\nsudo pacman -U --asdeps amdfan-*-any.pkg.tar.zst\n```\n\n# Installing from PyPi\nYou can also install amdfan from pypi using something like poetry.\n\n``` bash\npoetry init\npoetry add amdfan\npoetry run amdfan --help\n```\n\n# Building Python package\nRequires [poetry](https://python-poetry.org/) to be installed\n\n``` bash\ngit clone git@github.com:mcgillij/amdfan.git\ncd amdfan/\npoetry build\n```\n',
     'author': 'mcgillij',
     'author_email': 'mcgillivray.jason@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://mcgillij.dev/pages/amdfan.html',
```

### Comparing `amdfan-0.1.8/PKG-INFO` & `amdfan-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amdfan
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fan monitor and controller for AMD gpus in Linux
 Home-page: https://mcgillij.dev/pages/amdfan.html
 License: GPL-2.0-only
 Keywords: fan,gpu,temp,monitor,amd
 Author: mcgillij
 Author-email: mcgillivray.jason@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -21,15 +21,15 @@
 Classifier: Topic :: System :: Boot :: Init
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: numpy (>=1.20.1,<2.0.0)
-Requires-Dist: rich (>=9.10.0,<10.0.0)
+Requires-Dist: rich (>=10.1.0,<11.0.0)
 Project-URL: Documentation, https://mcgillij.dev/pages/amdfan.html
 Project-URL: Repository, https://github.com/mcgillij/amdfan
 Description-Content-Type: text/markdown
 
 # AmdFan
 ![Python package](https://github.com/mcgillij/amdfan/workflows/Python%20package/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/amdfan?period=total&units=international_system&left_color=blue&right_color=green&left_text=PyPi%20Downloads)](https://pepy.tech/project/amdfan)
```

