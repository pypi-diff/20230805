# Comparing `tmp/fusepyng-1.0.7.tar.gz` & `tmp/fusepyng-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fusepyng-1.0.7.tar", last modified: Wed Oct 24 01:05:19 2018, max compression
+gzip compressed data, was "fusepyng-2.0.0.tar", last modified: Fri Aug  4 23:00:30 2023, max compression
```

## Comparing `fusepyng-1.0.7.tar` & `fusepyng-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2018-10-24 01:05:19.000000 fusepyng-1.0.7/
--rw-r--r--   0 rian      (1000) rian      (1000)       59 2018-10-24 01:05:19.000000 fusepyng-1.0.7/setup.cfg
--rw-r--r--   0 rian      (1000) rian      (1000)     1074 2018-10-24 01:04:47.000000 fusepyng-1.0.7/README.rst
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2018-10-24 01:05:19.000000 fusepyng-1.0.7/fusepyng.egg-info/
--rw-r--r--   0 rian      (1000) rian      (1000)        1 2018-10-24 01:05:19.000000 fusepyng-1.0.7/fusepyng.egg-info/dependency_links.txt
--rw-r--r--   0 rian      (1000) rian      (1000)      178 2018-10-24 01:05:19.000000 fusepyng-1.0.7/fusepyng.egg-info/SOURCES.txt
--rw-r--r--   0 rian      (1000) rian      (1000)     1941 2018-10-24 01:05:19.000000 fusepyng-1.0.7/fusepyng.egg-info/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)        9 2018-10-24 01:05:19.000000 fusepyng-1.0.7/fusepyng.egg-info/top_level.txt
--rw-r--r--   0 rian      (1000) rian      (1000)       16 2016-03-31 03:30:14.000000 fusepyng-1.0.7/MANIFEST.in
--rw-r--r--   0 rian      (1000) rian      (1000)      928 2018-10-24 01:05:10.000000 fusepyng-1.0.7/setup.py
--rw-r--r--   0 rian      (1000) rian      (1000)     1941 2018-10-24 01:05:19.000000 fusepyng-1.0.7/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)    44745 2018-10-24 01:04:50.000000 fusepyng-1.0.7/fusepyng.py
--rw-r--r--   0 rian      (1000) rian      (1000)     1074 2018-10-24 01:04:47.000000 fusepyng-1.0.7/README
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2023-08-04 23:00:30.277869 fusepyng-2.0.0/
+-rw-r--r--   0 rian      (1000) rian      (1000)      731 2023-08-03 03:49:50.000000 fusepyng-2.0.0/LICENSE
+-rw-r--r--   0 rian      (1000) rian      (1000)       16 2023-08-03 03:49:50.000000 fusepyng-2.0.0/MANIFEST.in
+-rw-r--r--   0 rian      (1000) rian      (1000)      719 2023-08-04 23:00:30.277869 fusepyng-2.0.0/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)      166 2023-08-04 22:59:35.000000 fusepyng-2.0.0/README.rst
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2023-08-04 23:00:30.277869 fusepyng-2.0.0/fusepyng.egg-info/
+-rw-r--r--   0 rian      (1000) rian      (1000)      719 2023-08-04 23:00:30.000000 fusepyng-2.0.0/fusepyng.egg-info/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)      179 2023-08-04 23:00:30.000000 fusepyng-2.0.0/fusepyng.egg-info/SOURCES.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)        1 2023-08-04 23:00:30.000000 fusepyng-2.0.0/fusepyng.egg-info/dependency_links.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)        9 2023-08-04 23:00:30.000000 fusepyng-2.0.0/fusepyng.egg-info/top_level.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)    44964 2023-08-04 22:59:35.000000 fusepyng-2.0.0/fusepyng.py
+-rw-r--r--   0 rian      (1000) rian      (1000)       38 2023-08-04 23:00:30.277869 fusepyng-2.0.0/setup.cfg
+-rw-r--r--   0 rian      (1000) rian      (1000)      832 2023-08-04 22:59:35.000000 fusepyng-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fusepyng-1.0.7/setup.py` & `fusepyng-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 #!/usr/bin/env python
 
 from __future__ import with_statement
 
 from setuptools import setup
 
-with open('README') as readme:
+with open('README.rst') as readme:
     documentation = readme.read()
 
 setup(
     name = 'fusepyng',
-    version='1.0.7',
+    version='2.0.0',
     description = 'Simple ctypes bindings for FUSE',
     long_description = documentation,
     author = 'Giorgos Verigakis',
     author_email = 'verigak@gmail.com',
     maintainer = 'Rian Hunter',
     maintainer_email = 'rian@alum.mit.edu',
     license = 'ISC',
     py_modules=['fusepyng'],
-    url = 'http://github.com/rianhunter/fusepyng',
 
     classifiers = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: ISC License (ISCL)',
         'Operating System :: MacOS',
         'Operating System :: POSIX',
         'Operating System :: Unix',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 3',
         'Topic :: System :: Filesystems',
     ]
 )
```

### Comparing `fusepyng-1.0.7/fusepyng.py` & `fusepyng-2.0.0/fusepyng.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,85 +23,83 @@
 
 from ctypes.util import find_library
 from platform import machine, system
 from signal import signal, SIGINT, SIG_DFL, SIGTERM
 from stat import S_IFDIR
 from traceback import print_exc
 
+import typing
 
-try:
-    from functools import partial
-except ImportError:
-    # http://docs.python.org/library/functools.html#functools.partial
-    def partial(func, *args, **keywords):
-        def newfunc(*fargs, **fkeywords):
-            newkeywords = keywords.copy()
-            newkeywords.update(fkeywords)
-            return func(*(args + fargs), **newkeywords)
-
-        newfunc.func = func
-        newfunc.args = args
-        newfunc.keywords = keywords
-        return newfunc
+from functools import partial
 
 try:
     basestring
 except NameError:
     basestring = str
 
 log = logging.getLogger("fuse")
 _system = system()
 _machine = machine()
 
-if _system == 'Windows':
-    # NOTE:
-    #
-    # sizeof(long)==4 on Windows 32-bit and 64-bit
-    # sizeof(long)==4 on Cygwin 32-bit and ==8 on Cygwin 64-bit
-    #
-    # We have to fix up c_long and c_ulong so that it matches the
-    # Cygwin (and UNIX) sizes when run on Windows.
-    import sys
-    if sys.maxsize > 0xffffffff:
-        c_win_long = ctypes.c_int64
-        c_win_ulong = ctypes.c_uint64
-    else:
-        c_win_long = ctypes.c_int32
-        c_win_ulong = ctypes.c_uint32
+# NOTE:
+#
+# sizeof(long)==4 on Windows 32-bit and 64-bit
+# sizeof(long)==4 on Cygwin 32-bit and ==8 on Cygwin 64-bit
+#
+# We have to fix up c_long and c_ulong so that it matches the
+# Cygwin (and UNIX) sizes when run on Windows.
+import sys
+
+c_win_long: typing.Type
+c_win_ulong: typing.Type
+
+if sys.maxsize > 0xffffffff:
+    c_win_long = ctypes.c_int64
+    c_win_ulong = ctypes.c_uint64
+else:
+    c_win_long = ctypes.c_int32
+    c_win_ulong = ctypes.c_uint32
+
+class c_win_timespec(ctypes.Structure):
+    _fields_ = [('tv_sec', c_win_long), ('tv_nsec', c_win_long)]
+
+c_openbsd_time_t = ctypes.c_int64
+class c_openbsd_timespec(ctypes.Structure):
+    _fields_ = [('tv_sec', c_openbsd_time_t), ('tv_nsec', ctypes.c_long)]
+
+class c_std_timespec(ctypes.Structure):
+    _fields_ = [('tv_sec', ctypes.c_long), ('tv_nsec', ctypes.c_long)]
 
+c_timespec: typing.Type
 if _system == 'Windows' or _system.startswith('CYGWIN'):
-    class c_timespec(ctypes.Structure):
-        _fields_ = [('tv_sec', c_win_long), ('tv_nsec', c_win_long)]
+    c_timespec = c_win_timespec
 elif _system == 'OpenBSD':
-    c_time_t = ctypes.c_int64
-    class c_timespec(ctypes.Structure):
-        _fields_ = [('tv_sec', c_time_t), ('tv_nsec', ctypes.c_long)]
+    c_timespec = c_openbsd_timespec
 else:
-    class c_timespec(ctypes.Structure):
-        _fields_ = [('tv_sec', ctypes.c_long), ('tv_nsec', ctypes.c_long)]
+    c_timespec = c_std_timespec
 
 class c_utimbuf(ctypes.Structure):
     _fields_ = [('actime', c_timespec), ('modtime', c_timespec)]
 
+FuseFieldsType = typing.List[typing.Union[typing.Tuple[str, typing.Type], typing.Tuple[str, typing.Type, int]]]
+
 class c_stat(ctypes.Structure):
+    _fields_: typing.ClassVar[FuseFieldsType]
     pass    # Platform dependent
 
 _libfuse_path = os.environ.get('FUSE_LIBRARY_PATH')
 if not _libfuse_path:
     if _system == 'Darwin':
         # libfuse dependency
         _libiconv = ctypes.CDLL(find_library('iconv'), ctypes.RTLD_GLOBAL)
 
         _libfuse_path = (find_library('fuse4x') or find_library('osxfuse') or
                          find_library('fuse'))
     elif _system == 'Windows':
-        try:
-            import _winreg as reg
-        except ImportError:
-            import winreg as reg
+        import winreg as reg
         def Reg32GetValue(rootkey, keyname, valname):
             key, val = None, None
             try:
                 key = reg.OpenKey(rootkey, keyname, 0, reg.KEY_READ | reg.KEY_WOW64_32KEY)
                 val = str(reg.QueryValueEx(key, valname)[0])
             except WindowsError:
                 pass
@@ -119,34 +117,52 @@
     raise EnvironmentError('Unable to find libfuse')
 else:
     _libfuse = ctypes.CDLL(_libfuse_path)
 
 if _system == 'Darwin' and hasattr(_libfuse, 'macfuse_version'):
     _system = 'Darwin-MacFuse'
 
+c_dev_t: typing.Type
+c_fsblkcnt_t: typing.Type
+c_fsfilcnt_t: typing.Type
+c_gid_t: typing.Type
+c_mode_t: typing.Type
+c_off_t: typing.Type
+c_pid_t: typing.Type
+c_uid_t: typing.Type
 
 if _system in ('Darwin', 'Darwin-MacFuse', 'FreeBSD'):
     ENOTSUP = 45
 
     c_dev_t = ctypes.c_int32
     c_fsblkcnt_t = ctypes.c_ulong
     c_fsfilcnt_t = ctypes.c_ulong
     c_gid_t = ctypes.c_uint32
     c_mode_t = ctypes.c_uint16
     c_off_t = ctypes.c_int64
     c_pid_t = ctypes.c_int32
     c_uid_t = ctypes.c_uint32
-    setxattr_t = ctypes.CFUNCTYPE(
-        ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
-        ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t, ctypes.c_int,
-        ctypes.c_uint32)
-    getxattr_t = ctypes.CFUNCTYPE(
-        ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
-        ctypes.POINTER(ctypes.c_byte),
-        ctypes.c_size_t, ctypes.c_uint32)
+    if _system == 'FreeBSD':
+        setxattr_t = ctypes.CFUNCTYPE(
+            ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
+            ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t, ctypes.c_int)
+
+        getxattr_t = ctypes.CFUNCTYPE(
+            ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
+            ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t)
+    else:
+        setxattr_t = ctypes.CFUNCTYPE(
+            ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
+            ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t, ctypes.c_int,
+            ctypes.c_uint32)
+
+        getxattr_t = ctypes.CFUNCTYPE(
+            ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
+            ctypes.POINTER(ctypes.c_byte),
+            ctypes.c_size_t, ctypes.c_uint32)
     if _system == 'Darwin':
         c_stat._fields_ = [
             ('st_dev', c_dev_t),
             ('st_mode', c_mode_t),
             ('st_nlink', ctypes.c_uint16),
             ('st_ino', ctypes.c_uint64),
             ('st_uid', c_uid_t),
@@ -386,129 +402,142 @@
         ('st_flags', ctypes.c_uint32),
         ('st_gen', ctypes.c_uint32),
         ('st_birthtimespec', c_timespec),
     ]
 else:
     raise NotImplementedError('%s is not supported.' % _system)
 
+c_freebsd_fsblkcnt_t = ctypes.c_uint64
+c_freebsd_fsfilcnt_t = ctypes.c_uint64
+class c_freebsd_statvfs(ctypes.Structure):
+    _fields_ = [
+        ('f_bavail', c_freebsd_fsblkcnt_t),
+        ('f_bfree', c_freebsd_fsblkcnt_t),
+        ('f_blocks', c_freebsd_fsblkcnt_t),
+        ('f_favail', c_freebsd_fsfilcnt_t),
+        ('f_ffree', c_freebsd_fsfilcnt_t),
+        ('f_files', c_freebsd_fsfilcnt_t),
+        ('f_bsize', ctypes.c_ulong),
+        ('f_flag', ctypes.c_ulong),
+        ('f_frsize', ctypes.c_ulong)]
 
-if _system == 'FreeBSD':
-    c_fsblkcnt_t = ctypes.c_uint64
-    c_fsfilcnt_t = ctypes.c_uint64
-    setxattr_t = ctypes.CFUNCTYPE(
-        ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
-        ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t, ctypes.c_int)
+class c_win_statvfs(ctypes.Structure):
+    _fields_ = [
+        ('f_bsize', c_win_ulong),
+        ('f_frsize', c_win_ulong),
+        ('f_blocks', c_fsblkcnt_t),
+        ('f_bfree', c_fsblkcnt_t),
+        ('f_bavail', c_fsblkcnt_t),
+        ('f_files', c_fsfilcnt_t),
+        ('f_ffree', c_fsfilcnt_t),
+        ('f_favail', c_fsfilcnt_t),
+        ('f_fsid', c_win_ulong),
+        ('f_flag', c_win_ulong),
+        ('f_namemax', c_win_ulong)]
 
-    getxattr_t = ctypes.CFUNCTYPE(
-        ctypes.c_int, ctypes.c_char_p, ctypes.c_char_p,
-        ctypes.POINTER(ctypes.c_byte), ctypes.c_size_t)
+class c_std_statvfs(ctypes.Structure):
+    _fields_ = [
+        ('f_bsize', ctypes.c_ulong),
+        ('f_frsize', ctypes.c_ulong),
+        ('f_blocks', c_fsblkcnt_t),
+        ('f_bfree', c_fsblkcnt_t),
+        ('f_bavail', c_fsblkcnt_t),
+        ('f_files', c_fsfilcnt_t),
+        ('f_ffree', c_fsfilcnt_t),
+        ('f_favail', c_fsfilcnt_t),
+        ('f_fsid', ctypes.c_ulong),
+        # ('unused', ctypes.c_int),
+        ('f_flag', ctypes.c_ulong),
+        ('f_namemax', ctypes.c_ulong)]
 
-    class c_statvfs(ctypes.Structure):
-        _fields_ = [
-            ('f_bavail', c_fsblkcnt_t),
-            ('f_bfree', c_fsblkcnt_t),
-            ('f_blocks', c_fsblkcnt_t),
-            ('f_favail', c_fsfilcnt_t),
-            ('f_ffree', c_fsfilcnt_t),
-            ('f_files', c_fsfilcnt_t),
-            ('f_bsize', ctypes.c_ulong),
-            ('f_flag', ctypes.c_ulong),
-            ('f_frsize', ctypes.c_ulong)]
+c_statvfs: typing.Type
+if _system == 'FreeBSD':
+    c_statvfs = c_freebsd_statvfs
 elif _system == 'Windows' or _system.startswith('CYGWIN'):
-    class c_statvfs(ctypes.Structure):
-        _fields_ = [
-            ('f_bsize', c_win_ulong),
-            ('f_frsize', c_win_ulong),
-            ('f_blocks', c_fsblkcnt_t),
-            ('f_bfree', c_fsblkcnt_t),
-            ('f_bavail', c_fsblkcnt_t),
-            ('f_files', c_fsfilcnt_t),
-            ('f_ffree', c_fsfilcnt_t),
-            ('f_favail', c_fsfilcnt_t),
-            ('f_fsid', c_win_ulong),
-            ('f_flag', c_win_ulong),
-            ('f_namemax', c_win_ulong)]
+    c_statvfs = c_win_statvfs
 else:
-    class c_statvfs(ctypes.Structure):
-        _fields_ = [
-            ('f_bsize', ctypes.c_ulong),
-            ('f_frsize', ctypes.c_ulong),
-            ('f_blocks', c_fsblkcnt_t),
-            ('f_bfree', c_fsblkcnt_t),
-            ('f_bavail', c_fsblkcnt_t),
-            ('f_files', c_fsfilcnt_t),
-            ('f_ffree', c_fsfilcnt_t),
-            ('f_favail', c_fsfilcnt_t),
-            ('f_fsid', ctypes.c_ulong),
-            # ('unused', ctypes.c_int),
-            ('f_flag', ctypes.c_ulong),
-            ('f_namemax', ctypes.c_ulong)]
+    c_statvfs = c_std_statvfs
+
+class fuse_file_info_win(ctypes.Structure):
+    _fields_ = [
+        ('flags', ctypes.c_int),
+        ('fh_old', ctypes.c_int),
+        ('writepage', ctypes.c_int),
+        ('direct_io', ctypes.c_uint, 1),
+        ('keep_cache', ctypes.c_uint, 1),
+        ('flush', ctypes.c_uint, 1),
+        ('padding', ctypes.c_uint, 29),
+        ('fh', ctypes.c_uint64),
+        ('lock_owner', ctypes.c_uint64)]
 
+class fuse_file_info_openbsd(ctypes.Structure):
+    _fields_ = [
+        ('flags', ctypes.c_int32),
+        ('fh_old', ctypes.c_uint32),
+        ('writepage', ctypes.c_int32),
+        ('direct_io', ctypes.c_uint32, 1),
+        ('keep_cache', ctypes.c_uint32, 1),
+        ('flush', ctypes.c_uint32, 1),
+        ('nonseekable', ctypes.c_uint32, 1),
+        ('padding', ctypes.c_uint32, 27),
+        ('flock_release', ctypes.c_uint32, 1),
+        ('fh', ctypes.c_uint64),
+        ('lock_owner', ctypes.c_uint64)]
+
+class fuse_file_info_std(ctypes.Structure):
+    _fields_ = [
+        ('flags', ctypes.c_int),
+        ('fh_old', ctypes.c_ulong),
+        ('writepage', ctypes.c_int),
+        ('direct_io', ctypes.c_uint, 1),
+        ('keep_cache', ctypes.c_uint, 1),
+        ('flush', ctypes.c_uint, 1),
+        ('nonseekable', ctypes.c_uint, 1),
+        ('flock_release', ctypes.c_uint, 1),
+        ('padding', ctypes.c_uint, 27),
+        ('fh', ctypes.c_uint64),
+        ('lock_owner', ctypes.c_uint64)]
+
+fuse_file_info: typing.Type
 if _system == 'Windows' or _system.startswith('CYGWIN'):
-    class fuse_file_info(ctypes.Structure):
-        _fields_ = [
-            ('flags', ctypes.c_int),
-            ('fh_old', ctypes.c_int),
-            ('writepage', ctypes.c_int),
-            ('direct_io', ctypes.c_uint, 1),
-            ('keep_cache', ctypes.c_uint, 1),
-            ('flush', ctypes.c_uint, 1),
-            ('padding', ctypes.c_uint, 29),
-            ('fh', ctypes.c_uint64),
-            ('lock_owner', ctypes.c_uint64)]
+    fuse_file_info = fuse_file_info_win
 elif _system == "OpenBSD":
-    class fuse_file_info(ctypes.Structure):
-        _fields_ = [
-            ('flags', ctypes.c_int32),
-            ('fh_old', ctypes.c_uint32),
-            ('writepage', ctypes.c_int32),
-            ('direct_io', ctypes.c_uint32, 1),
-            ('keep_cache', ctypes.c_uint32, 1),
-            ('flush', ctypes.c_uint32, 1),
-            ('nonseekable', ctypes.c_uint32, 1),
-            ('padding', ctypes.c_uint32, 27),
-            ('flock_release', ctypes.c_uint32, 1),
-            ('fh', ctypes.c_uint64),
-            ('lock_owner', ctypes.c_uint64)]
+    fuse_file_info = fuse_file_info_openbsd
 else:
-    class fuse_file_info(ctypes.Structure):
-        _fields_ = [
-            ('flags', ctypes.c_int),
-            ('fh_old', ctypes.c_ulong),
-            ('writepage', ctypes.c_int),
-            ('direct_io', ctypes.c_uint, 1),
-            ('keep_cache', ctypes.c_uint, 1),
-            ('flush', ctypes.c_uint, 1),
-            ('nonseekable', ctypes.c_uint, 1),
-            ('flock_release', ctypes.c_uint, 1),
-            ('padding', ctypes.c_uint, 27),
-            ('fh', ctypes.c_uint64),
-            ('lock_owner', ctypes.c_uint64)]
+    fuse_file_info = fuse_file_info_std
+
+class fuse_context_openbsd(ctypes.Structure):
+    _fields_ = [
+        ('fuse', ctypes.c_void_p),
+        ('uid', c_uid_t),
+        ('gid', c_gid_t),
+        ('pid', c_pid_t),
+        ('private_data', ctypes.c_void_p),
+        ('umask', c_mode_t),
+    ]
+
+class fuse_context_std(ctypes.Structure):
+    _fields_ = [
+        ('fuse', ctypes.c_void_p),
+        ('uid', c_uid_t),
+        ('gid', c_gid_t),
+        ('pid', c_pid_t),
+        ('private_data', ctypes.c_void_p)]
 
+fuse_context: typing.Type
 if _system == "OpenBSD":
-    class fuse_context(ctypes.Structure):
-        _fields_ = [
-            ('fuse', ctypes.c_voidp),
-            ('uid', c_uid_t),
-            ('gid', c_gid_t),
-            ('pid', c_pid_t),
-            ('private_data', ctypes.c_voidp),
-            ('umask', c_mode_t),
-        ]
+    fuse_context = fuse_context_openbsd
 else:
-    class fuse_context(ctypes.Structure):
-        _fields_ = [
-            ('fuse', ctypes.c_voidp),
-            ('uid', c_uid_t),
-            ('gid', c_gid_t),
-            ('pid', c_pid_t),
-            ('private_data', ctypes.c_voidp)]
+    fuse_context = fuse_context_std
 
 _libfuse.fuse_get_context.restype = ctypes.POINTER(fuse_context)
 
+bmap_ret_t: typing.Type
+extra_fields: FuseFieldsType
+
 if _system == "OpenBSD":
     bmap_ret_t = ctypes.c_uint64
     extra_fields = []
 else:
     bmap_ret_t = ctypes.c_ulonglong
     extra_fields = [
         ('flag_nullpath_ok', ctypes.c_uint, 1),
@@ -518,23 +547,23 @@
 
         ('ioctl', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.c_uint, ctypes.c_void_p,
             ctypes.POINTER(fuse_file_info), ctypes.c_uint, ctypes.c_void_p)),
     ]
 
 class fuse_operations(ctypes.Structure):
-    _fields_ = [
+    _core_fields: FuseFieldsType = [
         ('getattr', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(c_stat))),
 
         ('readlink', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(ctypes.c_byte),
             ctypes.c_size_t)),
 
-        ('getdir', ctypes.c_voidp),    # Deprecated, use readdir
+        ('getdir', ctypes.c_void_p),    # Deprecated, use readdir
 
         ('mknod', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, c_mode_t, c_dev_t)),
 
         ('mkdir', ctypes.CFUNCTYPE(ctypes.c_int, ctypes.c_char_p, c_mode_t)),
         ('unlink', ctypes.CFUNCTYPE(ctypes.c_int, ctypes.c_char_p)),
         ('rmdir', ctypes.CFUNCTYPE(ctypes.c_int, ctypes.c_char_p)),
@@ -552,15 +581,15 @@
 
         ('chown', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, c_uid_t, c_gid_t)),
 
         ('truncate', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, c_off_t)),
 
-        ('utime', ctypes.c_voidp),     # Deprecated, use utimens
+        ('utime', ctypes.c_void_p),     # Deprecated, use utimens
         ('open', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(fuse_file_info))),
 
         ('read', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(ctypes.c_byte),
             ctypes.c_size_t, c_off_t, ctypes.POINTER(fuse_file_info))),
 
@@ -593,30 +622,30 @@
 
         ('opendir', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(fuse_file_info))),
 
         ('readdir', ctypes.CFUNCTYPE(
             ctypes.c_int,
             ctypes.c_char_p,
-            ctypes.c_voidp,
+            ctypes.c_void_p,
             ctypes.CFUNCTYPE(
-                ctypes.c_int, ctypes.c_voidp, ctypes.c_char_p,
+                ctypes.c_int, ctypes.c_void_p, ctypes.c_char_p,
                 ctypes.POINTER(c_stat), c_off_t),
             c_off_t,
             ctypes.POINTER(fuse_file_info))),
 
         ('releasedir', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(fuse_file_info))),
 
         ('fsyncdir', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.c_int,
             ctypes.POINTER(fuse_file_info))),
 
-        ('init', ctypes.CFUNCTYPE(ctypes.c_voidp, ctypes.c_voidp)),
-        ('destroy', ctypes.CFUNCTYPE(ctypes.c_voidp, ctypes.c_voidp)),
+        ('init', ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p)),
+        ('destroy', ctypes.CFUNCTYPE(ctypes.c_void_p, ctypes.c_void_p)),
 
         ('access', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.c_int)),
 
         ('create', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, c_mode_t,
             ctypes.POINTER(fuse_file_info))),
@@ -627,23 +656,25 @@
 
         ('fgetattr', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(c_stat),
             ctypes.POINTER(fuse_file_info))),
 
         ('lock', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(fuse_file_info),
-            ctypes.c_int, ctypes.c_voidp)),
+            ctypes.c_int, ctypes.c_void_p)),
 
         ('utimens', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.POINTER(c_utimbuf))),
 
         ('bmap', ctypes.CFUNCTYPE(
             ctypes.c_int, ctypes.c_char_p, ctypes.c_size_t,
             ctypes.POINTER(bmap_ret_t))),
-    ] + extra_fields
+    ]
+
+    _fields_ = _core_fields + extra_fields
 
 if _system == "OpenBSD":
     def fuse_main_real(argc, argv, fuse_ops_v, sizeof_fuse_ops, ctx_p):
         return _libfuse.fuse_main(argc, argv, fuse_ops_v, ctx_p)
 else:
     fuse_main_real =_libfuse.fuse_main_real
 
@@ -690,19 +721,16 @@
     if _system == "OpenBSD":
         os.kill(os.getpid(), SIGTERM)
         return
 
     fuse_ptr = ctypes.c_void_p(_libfuse.fuse_get_context().contents.fuse)
     _libfuse.fuse_exit(fuse_ptr)
 
-
-class FuseOSError(OSError):
-    def __init__(self, errno):
-        super(FuseOSError, self).__init__(errno, os.strerror(errno))
-
+def FuseOSError(errno):
+    return OSError(errno, os.strerror(errno))
 
 class FUSE(object):
     '''
     This class is the lower level interface and should not be subclassed under
     normal use. Its methods are called by fuse.
 
     Assumes API version 2.6 or later.
@@ -710,14 +738,16 @@
 
     OPTIONS = (
         ('foreground', '-f'),
         ('debug', '-d'),
         ('nothreads', '-s'),
     )
 
+    __deletable__ = ['operations']
+
     def __init__(self, operations, mountpoint, raw_fi=False, encoding='utf-8',
                  **kwargs):
 
         '''
         Setting raw_fi to True will cause FUSE to pass the fuse_file_info
         class as is to Operations, instead of just the fh field.
 
@@ -1321,17 +1351,17 @@
         raise FuseOSError(errno.EROFS)
 
 
 class LoggingMixIn:
     log = logging.getLogger('fuse.log-mixin')
 
     def __call__(self, op, path, *args):
-        self.log.debug('-> %s %s %s', op, path, repr(args))
+        self.log.debug('-> %s %s %r', op, path, args)
         ret = '[Unhandled Exception]'
         try:
             ret = getattr(self, op)(path, *args)
             return ret
         except OSError as e:
-            ret = str(e)
+            ret = e
             raise
         finally:
-            self.log.debug('<- %s %s', op, repr(ret))
+            self.log.debug('<- %s %r', op, ret)
```

