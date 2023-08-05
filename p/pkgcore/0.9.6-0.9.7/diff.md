# Comparing `tmp/pkgcore-0.9.6.tar.gz` & `tmp/pkgcore-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pkgcore-0.9.6.tar", last modified: Fri Sep 22 21:29:28 2017, max compression
+gzip compressed data, was "dist/pkgcore-0.9.7.tar", last modified: Wed Sep 27 08:53:49 2017, max compression
```

## Comparing `pkgcore-0.9.6.tar` & `pkgcore-0.9.7.tar`

### file list

```diff
@@ -1,469 +1,469 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3255 2017-09-22 21:27:50.000000 pkgcore-0.9.6/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    17992 2017-09-22 21:27:50.000000 pkgcore-0.9.6/GPL2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/ebuild/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13318 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/cpv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4283 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/resolver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14470 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/filter_env.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26692 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/profiles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6395 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/digest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26736 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33335 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31472 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/atom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22710 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/triggers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8790 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/ebuild_built.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1635 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19971 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/repo_objs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22923 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/formatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9116 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/portageq.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4038 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/pkg_updates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25678 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/domain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23934 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/portage_conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9936 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/restricts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14770 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/eapi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      981 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11573 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/inspect_profile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14516 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/ebuild_src.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4610 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/eclass_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38114 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/ebd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12685 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/conditionals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20104 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ebuild/misc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/fetch/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1775 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fetch/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4579 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fetch/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6211 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fetch/custom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3787 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fetch/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      616 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/log.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4100 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1091 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/mutated.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9130 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/conditionals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/virtual.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2791 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/package/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/vdb/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6191 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/vdb/repo_ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4918 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/vdb/contents.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8136 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/vdb/ondisk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/vdb/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/repository/
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/syncable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/configured.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16723 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/prototype.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/multiplex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/visibility.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/wrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/virtual.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3549 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/repository/misc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/operations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5198 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/observer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9740 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/format.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9055 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/repo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9592 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/domain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4736 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/operations/regen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5945 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/dhcpformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21602 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/central.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5777 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2753 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/domain.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/cparser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3905 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2515 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/mke2fsformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23642 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/config/basics.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/merge/
--rw-rw-r--   0 travis    (2000) travis    (2000)    30623 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/merge/triggers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/merge/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16271 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/merge/engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/merge/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/merge/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/system/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5086 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/system/libtool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/system/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/_verinfo.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/sync/
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/darcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1445 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/bzr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2092 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/svn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/git_svn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1304 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/hg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8332 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/rsync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7284 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/sync/cvs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/resolver/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10652 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2898 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/pigeonholes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5217 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/choice_point.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33012 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/resolver/plan.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/fs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8413 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/tar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13242 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/contents.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7722 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/livefs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10108 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10921 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/fs/ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1452 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/os_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11752 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/gpg.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/ospkg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3218 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ospkg/deb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      977 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ospkg/triggers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/ospkg/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/ebuild/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3667 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_eclass_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12408 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4194 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_digest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6468 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_filter_env.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3626 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12862 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_conditionals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56730 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_profiles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37862 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_formatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6313 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_portage_conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_repo_objs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26225 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_atom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13596 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_cpv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18296 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/ebuild/test_ebuild_src.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_py3k_eq_hash_inheritance.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/fetch/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4059 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fetch/test_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4500 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fetch/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fetch/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1353 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/package/test_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1890 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/package/test_mutated.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2395 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/package/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/package/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/repository/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/repository/test_visibility.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10447 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/repository/test_prototype.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2605 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/repository/test_multiplex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/repository/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_del_usage.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/test_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1859 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/test_cparser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9826 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/test_dhcpformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19797 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/test_basics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32383 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/test_central.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/config/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/merge/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5236 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/merge/test_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23816 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/merge/test_triggers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/merge/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1199 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/merge/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/sync/
--rw-rw-r--   0 travis    (2000) travis    (2000)      874 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_git_svn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      868 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_darcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      840 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_hg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_rsync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1828 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_cvs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_bzr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      665 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/test_svn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/sync/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/resolver/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2192 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/resolver/test_pigeonholes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3254 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/resolver/test_choice_point.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1055 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/resolver/test_plan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/resolver/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/fs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      955 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/fs_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7426 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/test_fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13261 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/test_contents.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9485 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/test_ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5534 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/fs/test_livefs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      399 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_slot_shadowing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9804 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      413 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_source_hygene.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/interfaces/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/interfaces/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/cache/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6149 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/cache/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      732 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/cache/test_flat_hash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/cache/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2280 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/cache/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      858 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_filter_env.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1789 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pmerge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12030 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pconfig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pclonecache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2335 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pquery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8006 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pmaint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pplugincache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pclean.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/scripts/test_pebuild.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/test_gpg.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/pkgsets/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3998 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/pkgsets/test_filelist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/pkgsets/test_glsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/pkgsets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/pkgsets/test_installed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3551 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9324 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/util/test_parserestrict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7887 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/util/test_commandline.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/test/restrictions/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_restriction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14039 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1328 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_delegated.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7762 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_boolean.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7274 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/restrictions/test_packages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4248 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/test/misc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/cache/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5099 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/cache/flat_hash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1031 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/cache/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/cache/fs_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6869 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/cache/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9879 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/cache/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/filter_env.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36079 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pmerge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pebuild.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12823 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pclean.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19529 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pmaint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13855 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pinspect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37863 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pquery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pclonecache.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1378 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pplugincache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15461 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/scripts/pconfig.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/pkgsets/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/filelist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8843 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/glsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/installed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1269 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/live_rebuild_set.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/pkgsets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/const.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)      856 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/builtin_configurables.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/builtin_formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      372 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/pkgcore_fsops_default.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      890 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/pkgcore_formatters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      229 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/pkgcore_syncers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      424 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/plugins/pkgcore_triggers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6474 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/parserestrict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1539 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/file_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/packages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/thread_pool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/repo_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21864 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/commandline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/util/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/binpkg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4807 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/binpkg/repo_ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13106 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/binpkg/repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10126 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/binpkg/remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/binpkg/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9685 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/binpkg/xpak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/pkgcore/restrictions/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11051 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/packages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5103 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/restriction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20374 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1452 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/delegated.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21248 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/boolean.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgcore/restrictions/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2017-09-22 21:27:50.000000 pkgcore-0.9.6/tox.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2017-09-22 21:27:50.000000 pkgcore-0.9.6/config/make.globals
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2017-09-22 21:27:50.000000 pkgcore-0.9.6/config/repos.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2017-09-22 21:27:50.000000 pkgcore-0.9.6/BSD
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2525 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pebuild.1
--rw-rw-r--   0 travis    (2000) travis    (2000)     9332 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pclean.1
--rw-rw-r--   0 travis    (2000) travis    (2000)     2293 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pclonecache.1
--rw-rw-r--   0 travis    (2000) travis    (2000)    16280 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pkgcore.5
--rw-rw-r--   0 travis    (2000) travis    (2000)     9595 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pconfig.1
--rw-rw-r--   0 travis    (2000) travis    (2000)    13634 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pquery.1
--rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pplugincache.1
--rw-rw-r--   0 travis    (2000) travis    (2000)    47691 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pinspect.1
--rw-rw-r--   0 travis    (2000) travis    (2000)    11030 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pmaint.1
--rw-rw-r--   0 travis    (2000) travis    (2000)     9588 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/pmerge.1
--rw-rw-r--   0 travis    (2000) travis    (2000)     2327 2017-09-22 21:29:28.000000 pkgcore-0.9.6/man/filter-env.1
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2017-09-22 21:27:50.000000 pkgcore-0.9.6/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)      749 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/bmh_search.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/bmh_search.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11660 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/depset.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    28379 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/atom.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    16691 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/filter_env.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    23964 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/cpv.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    17138 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/restrictions.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3758 2017-09-22 21:27:50.000000 pkgcore-0.9.6/src/misc.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12251 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/ebuild-daemon.bash
--rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/exit-handling.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)    17900 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/ebuild.lib
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2174 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/generate_global_func_list.bash
--rwxrwxr-x   0 travis    (2000) travis    (2000)      895 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/generate_eapi_func_list.bash
--rw-rw-r--   0 travis    (2000) travis    (2000)     5516 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/ebuild-env-utils.lib
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/
--rw-rw-r--   0 travis    (2000) travis    (2000)      244 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/3
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/4
--rw-rw-r--   0 travis    (2000) travis    (2000)      399 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/6
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/0
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/1
--rw-rw-r--   0 travis    (2000) travis    (2000)      323 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/5
--rw-rw-r--   0 travis    (2000) travis    (2000)      244 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2017-09-22 21:29:04.000000 pkgcore-0.9.6/ebd/funcnames/global
--rw-rw-r--   0 travis    (2000) travis    (2000)     1735 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/ebuild-daemon.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)    11279 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/isolated-functions.lib
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/eapi/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/5.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)      660 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/4.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)      901 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/2.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)      986 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/0.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/1.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)     3508 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/6.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)     4287 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/depend.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)      901 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/3.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)    15469 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/eapi/common.lib
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/4/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       92 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/4/docompress
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/4/dohard -> ../internals/banned
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/4/dosed -> ../internals/banned
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/6/
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/6/dohtml -> ../internals/deprecated
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/5/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      186 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/5/doheader
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/5/newheader -> ../internals/_generic_new
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/common/
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dosbin -> dobin
--rwxrwxr-x   0 travis    (2000) travis    (2000)      565 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doexe
--rwxrwxr-x   0 travis    (2000) travis    (2000)      191 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dodir
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newinitd -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      496 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/domo
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newexe -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      185 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doconfd
--rwxrwxr-x   0 travis    (2000) travis    (2000)      408 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dobin
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newsbin -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      274 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/fowners
--rwxrwxr-x   0 travis    (2000) travis    (2000)      382 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doinfo
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newlib.a -> ../internals/_generic_new
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newconfd -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      184 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doenvd
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3406 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/pkgcore-ebuild-helper
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1235 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doman
--rwxrwxr-x   0 travis    (2000) travis    (2000)      471 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dohard
--rwxrwxr-x   0 travis    (2000) travis    (2000)      231 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/emake
--rwxrwxr-x   0 travis    (2000) travis    (2000)      274 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/fperms
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1612 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/prepalldocs
--rwxrwxr-x   0 travis    (2000) travis    (2000)      295 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/prepallstrip
--rwxrwxr-x   0 travis    (2000) travis    (2000)      940 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dodoc
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dolib.a -> dolib
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dosym -> dohard
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1739 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/prepinfo
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1805 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/prepman
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dolib.so -> dolib
--rwxrwxr-x   0 travis    (2000) travis    (2000)      193 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doinitd
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newbin -> ../internals/_generic_new
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newdoc -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2559 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/prepstrip
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1174 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/doins
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newins -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      600 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/keepdir
--rwxrwxr-x   0 travis    (2000) travis    (2000)      234 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dohtml
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newlib.so -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      503 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dosed
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newenvd -> ../internals/_generic_new
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/newman -> ../internals/_generic_new
--rwxrwxr-x   0 travis    (2000) travis    (2000)      658 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/common/dolib
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/ebd/helpers/internals/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      116 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/banned
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2745 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/prepall
--rwxrwxr-x   0 travis    (2000) travis    (2000)      405 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/deprecated
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6077 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/_raw_dohtml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      563 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/prepallman
--rwxrwxr-x   0 travis    (2000) travis    (2000)      601 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/helpers/internals/_generic_new
--rw-rw-r--   0 travis    (2000) travis    (2000)     8336 2017-09-22 21:27:50.000000 pkgcore-0.9.6/ebd/ebuild-default-functions.lib
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2017-09-22 21:27:50.000000 pkgcore-0.9.6/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9050 2017-09-22 21:27:50.000000 pkgcore-0.9.6/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2017-09-22 21:27:50.000000 pkgcore-0.9.6/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)     4668 2017-09-22 21:29:28.000000 pkgcore-0.9.6/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/shell/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/shell/zsh/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8927 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/zsh/pkgcore.zsh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/shell/zsh/completion/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26042 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/zsh/completion/_pkgcore
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/pkgcore.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/shell/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      425 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/bin/pkgcore-sh-helper
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1391 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/bin/psite
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/shell/bash/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2017-09-22 21:27:50.000000 pkgcore-0.9.6/shell/bash/pkgcore.bash
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/bin/
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/filter-env -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pconfig -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pebuild -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pplugincache -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pquery -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pmaint -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pclonecache -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pclean -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pmerge -> ../pkgcore/scripts/__init__.py
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/bin/pinspect -> ../pkgcore/scripts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41098 2017-09-22 21:27:50.000000 pkgcore-0.9.6/pkgdist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101881 2017-09-22 21:27:50.000000 pkgcore-0.9.6/NEWS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/doc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      231 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/man.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/doc/man/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14413 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/man/pkgcore.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4400 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/man/pquery.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/man/pmerge.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9916 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5174 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      832 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/api.rst
-lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/news.rst -> ../NEWS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/doc/dev-notes/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23013 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/hacking.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/tackling-domain.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    22813 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/heapy.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/doc/dev-notes/formats/
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/formats/cpan.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1132 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/formats/dpkg.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      620 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/fs-ops.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3726 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/eapi.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/plugins.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3953 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/TODO.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    16230 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/config.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1344 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/tests.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      940 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/changes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4662 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/portage-differences.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/doc/dev-notes/framework/
--rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/framework/intro.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1310 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/harring-notes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/feature-breakdown.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/developing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7620 2017-09-22 21:27:50.000000 pkgcore-0.9.6/doc/dev-notes/commandline.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2017-09-22 21:27:50.000000 pkgcore-0.9.6/AUTHORS
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-22 21:29:28.000000 pkgcore-0.9.6/examples/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1650 2017-09-22 21:27:50.000000 pkgcore-0.9.6/examples/pkg_info.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2549 2017-09-22 21:27:50.000000 pkgcore-0.9.6/examples/changed_use.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3290 2017-09-22 21:27:50.000000 pkgcore-0.9.6/examples/report_pkg_changes.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1566 2017-09-22 21:27:50.000000 pkgcore-0.9.6/examples/repo_list.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      856 2017-09-22 21:27:50.000000 pkgcore-0.9.6/examples/identify-installed-non-split-debug-pkgs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3255 2017-09-27 08:52:54.000000 pkgcore-0.9.7/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17992 2017-09-27 08:52:54.000000 pkgcore-0.9.7/GPL2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      804 2017-09-27 08:52:54.000000 pkgcore-0.9.7/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      789 2017-09-27 08:52:54.000000 pkgcore-0.9.7/config/make.globals
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2017-09-27 08:52:54.000000 pkgcore-0.9.7/config/repos.conf
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2017-09-27 08:52:54.000000 pkgcore-0.9.7/BSD
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/man/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2525 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pebuild.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9332 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pclean.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2293 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pclonecache.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16280 2017-09-27 08:53:49.000000 pkgcore-0.9.7/man/pkgcore.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9595 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pconfig.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13634 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pquery.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pplugincache.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47691 2017-09-27 08:53:49.000000 pkgcore-0.9.7/man/pinspect.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11030 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pmaint.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9588 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/pmerge.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2327 2017-09-27 08:53:48.000000 pkgcore-0.9.7/man/filter-env.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2017-09-27 08:52:54.000000 pkgcore-0.9.7/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/ebuild/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13318 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/cpv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4283 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/resolver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14470 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/filter_env.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26677 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/profiles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6395 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/digest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26736 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33335 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31472 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/atom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22710 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/triggers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8790 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/ebuild_built.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1635 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19971 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/repo_objs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22923 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/formatter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9116 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/portageq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4038 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/pkg_updates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25678 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/domain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23922 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/portage_conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9936 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/restricts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14770 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/eapi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      981 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/const.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11573 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/inspect_profile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14516 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/ebuild_src.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4610 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/eclass_cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38114 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/ebd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12685 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/conditionals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20104 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ebuild/misc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/fetch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1775 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fetch/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4579 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fetch/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6211 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fetch/custom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3787 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fetch/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      616 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/log.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4100 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1091 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/mutated.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9130 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/conditionals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/virtual.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2791 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/package/base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/vdb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6191 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/vdb/repo_ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4937 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/vdb/contents.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8136 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/vdb/ondisk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/vdb/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/repository/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/syncable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/configured.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16723 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/prototype.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7522 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/multiplex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2555 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/visibility.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/wrapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/virtual.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3549 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/repository/misc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/operations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5198 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/observer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9740 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/format.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9055 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/repo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9592 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/domain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4736 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/operations/regen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5945 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/dhcpformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21602 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/central.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5777 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2753 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/domain.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/cparser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3905 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2515 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/mke2fsformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23642 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/config/basics.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/merge/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30623 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/merge/triggers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/merge/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16271 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/merge/engine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/merge/const.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/merge/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/system/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5086 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/system/libtool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/system/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/_verinfo.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/sync/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      771 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/darcs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1445 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/bzr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2092 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/svn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/git_svn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1304 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/hg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8332 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/rsync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7284 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/sync/cvs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/resolver/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10652 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/state.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2898 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/pigeonholes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5217 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/choice_point.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33012 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/resolver/plan.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/fs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8413 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/tar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13242 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/contents.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7722 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/livefs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10108 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/fs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10921 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/fs/ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1452 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/os_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11752 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/gpg.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/ospkg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3218 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ospkg/deb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      977 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ospkg/triggers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/ospkg/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3667 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_eclass_cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12408 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4194 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_digest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6468 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_filter_env.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3626 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12862 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_conditionals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56730 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_profiles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40659 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_formatter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7744 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_portage_conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_repo_objs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26225 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_atom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13596 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_cpv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18296 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/ebuild/test_ebuild_src.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_py3k_eq_hash_inheritance.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/fetch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4059 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fetch/test_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4500 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fetch/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fetch/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1353 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/package/test_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1890 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/package/test_mutated.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2395 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/package/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/package/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/repository/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2250 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/repository/test_visibility.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10447 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/repository/test_prototype.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2605 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/repository/test_multiplex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/repository/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_del_usage.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/test_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1859 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/test_cparser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9826 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/test_dhcpformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19797 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/test_basics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32383 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/test_central.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/config/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/merge/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5236 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/merge/test_engine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23816 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/merge/test_triggers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/merge/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1199 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/merge/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/sync/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      874 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_git_svn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      868 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_darcs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      840 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_hg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_rsync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1828 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_cvs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      755 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_bzr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      665 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/test_svn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      362 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/sync/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/resolver/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2192 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/resolver/test_pigeonholes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3254 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/resolver/test_choice_point.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1055 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/resolver/test_plan.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/resolver/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/fs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      955 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/fs_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7426 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/test_fs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13261 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/test_contents.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9485 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/test_ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5534 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/fs/test_livefs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      399 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_slot_shadowing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9804 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      413 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_source_hygene.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/interfaces/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/interfaces/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/cache/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6149 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/cache/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      732 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/cache/test_flat_hash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/cache/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2280 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/cache/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      858 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_filter_env.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1789 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pmerge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12030 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pconfig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pclonecache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2335 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pquery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8006 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pmaint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pplugincache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pclean.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/scripts/test_pebuild.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/test_gpg.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/pkgsets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3998 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_filelist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_glsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/pkgsets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_installed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3551 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9324 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/util/test_parserestrict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7887 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/util/test_commandline.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_restriction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14039 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1328 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_delegated.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7762 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_boolean.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7274 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/restrictions/test_packages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4248 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/test/misc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/cache/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5099 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/cache/flat_hash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1031 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/cache/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/cache/fs_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6869 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/cache/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9879 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/cache/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/filter_env.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36079 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pmerge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pebuild.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12823 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pclean.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19529 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pmaint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13855 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pinspect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37863 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pquery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pclonecache.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1278 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pplugincache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15461 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/scripts/pconfig.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/filelist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8843 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/glsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      536 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/system.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/installed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1269 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/live_rebuild_set.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/pkgsets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/const.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      856 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/builtin_configurables.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/builtin_formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      372 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/pkgcore_fsops_default.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      890 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/pkgcore_formatters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      229 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/pkgcore_syncers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      424 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/plugins/pkgcore_triggers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6474 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/parserestrict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1539 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/file_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/packages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/thread_pool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/repo_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21864 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/commandline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/util/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/binpkg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4807 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/binpkg/repo_ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13106 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/binpkg/repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10126 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/binpkg/remote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/binpkg/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9685 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/binpkg/xpak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/src/pkgcore/restrictions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11051 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/packages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5103 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/restriction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20374 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1452 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/delegated.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21248 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/boolean.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/pkgcore/restrictions/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      749 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/bmh_search.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      235 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/bmh_search.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11660 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/depset.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28379 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/atom.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16691 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/filter_env.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23964 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/cpv.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17138 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/restrictions.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3758 2017-09-27 08:52:54.000000 pkgcore-0.9.7/src/misc.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12251 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/ebuild-daemon.bash
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4171 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/exit-handling.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17900 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/ebuild.lib
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2174 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/generate_global_func_list.bash
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      895 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/generate_eapi_func_list.bash
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5516 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/ebuild-env-utils.lib
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      244 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/3
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/4
+-rw-rw-r--   0 travis    (2000) travis    (2000)      399 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/6
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/0
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      323 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/5
+-rw-rw-r--   0 travis    (2000) travis    (2000)      244 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2017-09-27 08:53:23.000000 pkgcore-0.9.7/ebd/funcnames/global
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1735 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/ebuild-daemon.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11279 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/isolated-functions.lib
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/eapi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/5.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      660 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/4.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      901 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/2.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      986 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/0.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/1.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3508 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/6.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4287 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/depend.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      901 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/3.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15469 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/eapi/common.lib
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/4/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       92 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/4/docompress
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/4/dohard -> ../internals/banned
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/4/dosed -> ../internals/banned
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/6/
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/6/dohtml -> ../internals/deprecated
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/5/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      186 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/5/doheader
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/5/newheader -> ../internals/_generic_new
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/common/
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dosbin -> dobin
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      565 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doexe
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      191 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dodir
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newinitd -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      496 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/domo
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newexe -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      185 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doconfd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      408 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dobin
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newsbin -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      274 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/fowners
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      382 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doinfo
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newlib.a -> ../internals/_generic_new
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newconfd -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      184 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doenvd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3406 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/pkgcore-ebuild-helper
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1235 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doman
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      471 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dohard
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      231 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/emake
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      274 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/fperms
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1612 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/prepalldocs
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      295 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/prepallstrip
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      940 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dodoc
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dolib.a -> dolib
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dosym -> dohard
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1739 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/prepinfo
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1805 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/prepman
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dolib.so -> dolib
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      193 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doinitd
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newbin -> ../internals/_generic_new
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newdoc -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2559 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/prepstrip
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1174 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/doins
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newins -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      600 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/keepdir
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      234 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dohtml
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newlib.so -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      503 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dosed
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newenvd -> ../internals/_generic_new
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/newman -> ../internals/_generic_new
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      658 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/common/dolib
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/ebd/helpers/internals/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      116 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/banned
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2745 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/prepall
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      405 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/deprecated
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6077 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/_raw_dohtml
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      563 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/prepallman
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      601 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/helpers/internals/_generic_new
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8336 2017-09-27 08:52:54.000000 pkgcore-0.9.7/ebd/ebuild-default-functions.lib
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2017-09-27 08:52:54.000000 pkgcore-0.9.7/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9362 2017-09-27 08:52:54.000000 pkgcore-0.9.7/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2017-09-27 08:52:54.000000 pkgcore-0.9.7/.coveragerc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4668 2017-09-27 08:53:49.000000 pkgcore-0.9.7/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/shell/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/shell/zsh/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8927 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/zsh/pkgcore.zsh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/shell/zsh/completion/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26042 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/zsh/completion/_pkgcore
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/pkgcore.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/shell/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      425 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/bin/pkgcore-sh-helper
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1391 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/bin/psite
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/shell/bash/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2017-09-27 08:52:54.000000 pkgcore-0.9.7/shell/bash/pkgcore.bash
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/bin/
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/filter-env -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pconfig -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pebuild -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pplugincache -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pquery -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pmaint -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pclonecache -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pclean -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pmerge -> ../src/pkgcore/scripts/__init__.py
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/bin/pinspect -> ../src/pkgcore/scripts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43974 2017-09-27 08:52:54.000000 pkgcore-0.9.7/pkgdist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102363 2017-09-27 08:52:54.000000 pkgcore-0.9.7/NEWS.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/doc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      231 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/man.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/doc/man/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14413 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/man/pkgcore.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4400 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/man/pquery.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/man/pmerge.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9802 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5256 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      832 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/api.rst
+lrwxrwxrwx   0 travis    (2000) travis    (2000)        0 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/news.rst -> ../NEWS.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/doc/dev-notes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23013 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/hacking.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/tackling-domain.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22813 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/heapy.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/doc/dev-notes/formats/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/formats/cpan.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1132 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/formats/dpkg.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      620 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/fs-ops.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3726 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/eapi.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4584 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/plugins.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3953 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/TODO.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16230 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/config.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1344 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/tests.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      940 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/changes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4662 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/portage-differences.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/doc/dev-notes/framework/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/framework/intro.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1310 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/harring-notes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/feature-breakdown.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/developing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7620 2017-09-27 08:52:54.000000 pkgcore-0.9.7/doc/dev-notes/commandline.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2017-09-27 08:52:54.000000 pkgcore-0.9.7/AUTHORS
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 08:53:49.000000 pkgcore-0.9.7/examples/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1650 2017-09-27 08:52:54.000000 pkgcore-0.9.7/examples/pkg_info.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2549 2017-09-27 08:52:54.000000 pkgcore-0.9.7/examples/changed_use.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3290 2017-09-27 08:52:54.000000 pkgcore-0.9.7/examples/report_pkg_changes.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1566 2017-09-27 08:52:54.000000 pkgcore-0.9.7/examples/repo_list.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      856 2017-09-27 08:52:54.000000 pkgcore-0.9.7/examples/identify-installed-non-split-debug-pkgs.py
```

### Comparing `pkgcore-0.9.6/README.rst` & `pkgcore-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/GPL2` & `pkgcore-0.9.7/GPL2`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/cpv.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/cpv.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/resolver.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/resolver.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/filter_env.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/filter_env.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/profiles.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,20 +186,20 @@
         repo_config = self.repoconfig
         if repo_config is not None and 'portage-2' in repo_config.profile_formats:
             l = []
             for repo_id, separator, path in (x.partition(':') for x in data):
                 if separator:
                     if repo_id:
                         try:
-                            repo_config = self._repo_map[repo_id]
+                            location = self._repo_map[repo_id]
                         except KeyError:
                             raise ValueError("unknown repository name: %r" % repo_id)
                         except TypeError:
                             raise ValueError("repo mapping is unset")
-                    l.append(abspath(pjoin(repo_config.location, 'profiles', path)))
+                    l.append(abspath(pjoin(location, 'profiles', path)))
                 else:
                     l.append(abspath(pjoin(self.path, repo_id)))
             return tuple(l)
         return tuple(abspath(pjoin(self.path, x)) for x in data)
 
     @klass.jit_attr
     def parents(self):
```

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/digest.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/digest.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/repository.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/repository.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/processor.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/processor.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/atom.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/atom.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/triggers.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/triggers.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/ebuild_built.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/ebuild_built.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/errors.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/repo_objs.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/repo_objs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/formatter.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/formatter.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/portageq.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/portageq.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/pkg_updates.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/pkg_updates.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/domain.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/domain.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/portage_conf.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/portage_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,23 +299,23 @@
         dict: global repo settings
         dict: repo settings
     """
     defaults = {}
     repos = {}
 
     for fp in sorted_scan(os.path.realpath(path), follow_symlinks=True, nonexistent=True):
+        config = ConfigParser()
         try:
             with open(fp) as f:
-                config = ConfigParser()
                 config.read_file(f)
         except EnvironmentError as e:
             if e.errno == errno.EACCES:
                 raise_from(errors.PermissionDeniedError(fp))
             raise_from(errors.ParsingError("repos.conf: '%s'" % (fp,), exception=e))
-        except configparser.ParsingError as e:
+        except ConfigParser.exceptions as e:
             raise_from(errors.ParsingError("repos.conf: '%s'" % (fp,), exception=e))
 
         defaults_data = config.defaults()
         if defaults_data and defaults:
             logger.warning("repos.conf: parsing '%s': overriding DEFAULT section", fp)
         defaults.update(defaults_data)
 
@@ -470,15 +470,15 @@
     repo_map = {}
 
     for repo_name, repo_opts in repos_conf.iteritems():
         repo_path = repo_opts['location']
 
         # XXX: Hack for portage-2 profile format support.
         repo_config = RepoConfig(repo_path, repo_name)
-        repo_map[repo_config.repo_id] = repo_config
+        repo_map[repo_config.repo_id] = repo_path
 
         # repo configs
         repo_conf = {
             'class': 'pkgcore.ebuild.repo_objs.RepoConfig',
             'config_name': repo_name,
             'location': repo_path,
             'syncer': 'sync:' + repo_name,
```

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/restricts.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/restricts.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/eapi.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/eapi.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/const.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/const.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/inspect_profile.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/inspect_profile.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/ebuild_src.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/ebuild_src.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/eclass_cache.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/eclass_cache.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/ebd.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/ebd.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/conditionals.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/conditionals.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ebuild/misc.py` & `pkgcore-0.9.7/src/pkgcore/ebuild/misc.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fetch/errors.py` & `pkgcore-0.9.7/src/pkgcore/fetch/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fetch/__init__.py` & `pkgcore-0.9.7/src/pkgcore/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fetch/custom.py` & `pkgcore-0.9.7/src/pkgcore/fetch/custom.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fetch/base.py` & `pkgcore-0.9.7/src/pkgcore/fetch/base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/log.py` & `pkgcore-0.9.7/src/pkgcore/log.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/errors.py` & `pkgcore-0.9.7/src/pkgcore/package/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/metadata.py` & `pkgcore-0.9.7/src/pkgcore/package/metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/mutated.py` & `pkgcore-0.9.7/src/pkgcore/package/mutated.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/conditionals.py` & `pkgcore-0.9.7/src/pkgcore/package/conditionals.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/virtual.py` & `pkgcore-0.9.7/src/pkgcore/package/virtual.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/package/base.py` & `pkgcore-0.9.7/src/pkgcore/package/base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/vdb/repo_ops.py` & `pkgcore-0.9.7/src/pkgcore/vdb/repo_ops.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/vdb/contents.py` & `pkgcore-0.9.7/src/pkgcore/vdb/contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pkgcore.fs.contents import contentsSet
 
 demandload(
     'errno',
     'os',
     'stat',
     'snakeoil.chksum:get_handler',
-    'snakeoil.fileutils:readlines_ascii',
+    'snakeoil.fileutils:readlines_utf8',
     'pkgcore:os_data',
 )
 
 
 class LookupFsDev(fs.fsDev):
 
     __slots__ = ()
@@ -72,17 +72,18 @@
                 raise TypeError("fsFile objects need to be strict")
 
         contentsSet.add(self, obj)
 
     def _get_fd(self, write=False):
         if isinstance(self._source, basestring):
             if write:
-                return AtomicWriteFile(self._source, uid=os_data.root_uid,
+                return AtomicWriteFile(
+                    self._source, uid=os_data.root_uid,
                     gid=os_data.root_gid, perms=0644)
-            return readlines_ascii(self._source, True)
+            return readlines_utf8(self._source, True)
         fobj = self._source.text_fileobj(writable=write)
         if write:
             fobj.seek(0, 0)
             fobj.truncate(0)
         return fobj
 
     def flush(self):
```

### Comparing `pkgcore-0.9.6/pkgcore/vdb/ondisk.py` & `pkgcore-0.9.7/src/pkgcore/vdb/ondisk.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/configured.py` & `pkgcore-0.9.7/src/pkgcore/repository/configured.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/prototype.py` & `pkgcore-0.9.7/src/pkgcore/repository/prototype.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/multiplex.py` & `pkgcore-0.9.7/src/pkgcore/repository/multiplex.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/errors.py` & `pkgcore-0.9.7/src/pkgcore/repository/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/visibility.py` & `pkgcore-0.9.7/src/pkgcore/repository/visibility.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/wrapper.py` & `pkgcore-0.9.7/src/pkgcore/repository/wrapper.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/virtual.py` & `pkgcore-0.9.7/src/pkgcore/repository/virtual.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/util.py` & `pkgcore-0.9.7/src/pkgcore/repository/util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/repository/misc.py` & `pkgcore-0.9.7/src/pkgcore/repository/misc.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/observer.py` & `pkgcore-0.9.7/src/pkgcore/operations/observer.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/format.py` & `pkgcore-0.9.7/src/pkgcore/operations/format.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/repo.py` & `pkgcore-0.9.7/src/pkgcore/operations/repo.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/domain.py` & `pkgcore-0.9.7/src/pkgcore/operations/domain.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/__init__.py` & `pkgcore-0.9.7/src/pkgcore/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/operations/regen.py` & `pkgcore-0.9.7/src/pkgcore/operations/regen.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/dhcpformat.py` & `pkgcore-0.9.7/src/pkgcore/config/dhcpformat.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/central.py` & `pkgcore-0.9.7/src/pkgcore/config/central.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/errors.py` & `pkgcore-0.9.7/src/pkgcore/config/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/domain.py` & `pkgcore-0.9.7/src/pkgcore/config/domain.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/cparser.py` & `pkgcore-0.9.7/src/pkgcore/config/cparser.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/__init__.py` & `pkgcore-0.9.7/src/pkgcore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/mke2fsformat.py` & `pkgcore-0.9.7/src/pkgcore/config/mke2fsformat.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/config/basics.py` & `pkgcore-0.9.7/src/pkgcore/config/basics.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/merge/triggers.py` & `pkgcore-0.9.7/src/pkgcore/merge/triggers.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/merge/errors.py` & `pkgcore-0.9.7/src/pkgcore/merge/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/merge/engine.py` & `pkgcore-0.9.7/src/pkgcore/merge/engine.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/system/libtool.py` & `pkgcore-0.9.7/src/pkgcore/system/libtool.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/darcs.py` & `pkgcore-0.9.7/src/pkgcore/sync/darcs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/git.py` & `pkgcore-0.9.7/src/pkgcore/sync/git.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/bzr.py` & `pkgcore-0.9.7/src/pkgcore/sync/bzr.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/svn.py` & `pkgcore-0.9.7/src/pkgcore/sync/svn.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/git_svn.py` & `pkgcore-0.9.7/src/pkgcore/sync/git_svn.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/hg.py` & `pkgcore-0.9.7/src/pkgcore/sync/hg.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/rsync.py` & `pkgcore-0.9.7/src/pkgcore/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/base.py` & `pkgcore-0.9.7/src/pkgcore/sync/base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/sync/cvs.py` & `pkgcore-0.9.7/src/pkgcore/sync/cvs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/resolver/state.py` & `pkgcore-0.9.7/src/pkgcore/resolver/state.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/resolver/pigeonholes.py` & `pkgcore-0.9.7/src/pkgcore/resolver/pigeonholes.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/resolver/choice_point.py` & `pkgcore-0.9.7/src/pkgcore/resolver/choice_point.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/resolver/util.py` & `pkgcore-0.9.7/src/pkgcore/resolver/util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/resolver/plan.py` & `pkgcore-0.9.7/src/pkgcore/resolver/plan.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fs/tar.py` & `pkgcore-0.9.7/src/pkgcore/fs/tar.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fs/contents.py` & `pkgcore-0.9.7/src/pkgcore/fs/contents.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fs/livefs.py` & `pkgcore-0.9.7/src/pkgcore/fs/livefs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fs/fs.py` & `pkgcore-0.9.7/src/pkgcore/fs/fs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/fs/ops.py` & `pkgcore-0.9.7/src/pkgcore/fs/ops.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/os_data.py` & `pkgcore-0.9.7/src/pkgcore/os_data.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/plugin.py` & `pkgcore-0.9.7/src/pkgcore/plugin.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/gpg.py` & `pkgcore-0.9.7/src/pkgcore/gpg.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ospkg/deb.py` & `pkgcore-0.9.7/src/pkgcore/ospkg/deb.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/ospkg/triggers.py` & `pkgcore-0.9.7/src/pkgcore/ospkg/triggers.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_eclass_cache.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_eclass_cache.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_repository.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_repository.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_digest.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_digest.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_filter_env.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_filter_env.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_misc.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_misc.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_conditionals.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_profiles.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_profiles.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_formatter.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,39 +119,53 @@
     def test_end(self):
         # Sub-classes should override this if they print something in end()
         self.formatter.format(FakeOp(FakeMutatedPkg('dev-util/diffball-1.1')))
         self.fakeout.resetstream()
         self.formatter.end()
         self.assertOut(suffix=())
 
+
 class TestBasicFormatter(BaseFormatterTest, TestCase):
+
     formatterClass = BasicFormatter
-    def test_op(self):
+
+    def test_install(self):
         # Make sure we ignore versions...
         self.formatter.format(FakeOp(FakeMutatedPkg('dev-util/diffball-1.1')))
         self.assertOut('dev-util/diffball')
 
+    def test_reinstall(self):
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.4'),
+            FakeMutatedPkg('app-arch/bzip2-1.0.4')))
+        self.assertOut('app-arch/bzip2')
+
+
 class TestPkgcoreFormatter(BaseFormatterTest, TestCase):
+
     formatterClass = PkgcoreFormatter
-    def test_op(self):
-        # This basically just tests string methods
-        self.formatter.format(
-            FakeOp(FakeEbuildSrc('dev-util/diffball-1.2'),
-                FakeMutatedPkg('dev-util/diffball-1.1')))
-        self.assertOut(
-            "replace dev-util/diffball-1.1, "
-            "dev-util/diffball-1.2")
 
+    def test_install(self):
         self.formatter.format(FakeOp(FakeEbuildSrc('dev-util/diffball-1.0')))
         self.assertOut("add     dev-util/diffball-1.0")
 
+    def test_install_repo(self):
         self.formatter.format(FakeOp(FakeEbuildSrc('dev-util/diffball-1.0',
             repo=FakeRepo(repo_id='gentoo', location='/var/gentoo/repos/gentoo'))))
         self.assertOut("add     dev-util/diffball-1.0::gentoo")
 
+    def test_reinstall(self):
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('dev-util/diffball-1.2'),
+                FakeMutatedPkg('dev-util/diffball-1.1')))
+        self.assertOut(
+            "replace dev-util/diffball-1.1, "
+            "dev-util/diffball-1.2")
+
+    def test_reinstall_repo(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('dev-util/diffball-1.2',
                    repo=FakeRepo(repo_id='gentoo', location='/var/gentoo/repos/gentoo')),
                 FakeMutatedPkg('dev-util/diffball-1.1')))
         self.assertOut(
             "replace dev-util/diffball-1.1, "
             "dev-util/diffball-1.2::gentoo")
@@ -254,14 +268,39 @@
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/gzip-1.6'),
             FakeMutatedPkg('app-arch/gzip-1.6')))
         self.fakeout.resetstream()
         self.formatter.end()
         self.assertEnd('\nTotal: 2 packages (2 reinstalls)')
 
+    def test_end_all_ops_order(self):
+        # new
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/pkga-1.0.3-r6')))
+        # new slot
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/pkgb-1.0.3-r6', slot='1')))
+        # downgrade
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/pkgc-1.0.3-r6'),
+            FakeMutatedPkg('app-arch/pkgc-1.0.4')))
+        # upgrade
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/pkgd-1.0.4'),
+            FakeMutatedPkg('app-arch/pkgd-1.0.3-r6')))
+        # reinstall
+        self.formatter.format(
+            FakeOp(FakeEbuildSrc('app-arch/pkge-1.0.4'),
+            FakeMutatedPkg('app-arch/pkge-1.0.4')))
+
+        self.fakeout.resetstream()
+        self.formatter.end()
+        self.assertEnd(
+            '\nTotal: 5 packages (1 new, 1 upgrade, 1 downgrade, 1 in new slot, 1 reinstall)')
+
 
 class TestPaludisFormatter(CountingFormatterTest, TestCase):
     formatterClass = PaludisFormatter
 
     def setUp(self):
         BaseFormatterTest.setUp(self)
         self.repo = FakeRepo(repo_id='gentoo', location='/var/gentoo/repos/gentoo')
@@ -295,15 +334,15 @@
         self.formatter.format(
             FakeOp(self.FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut("* ", Color('fg', 'blue'), "app-arch/bzip2", "-1.0.3-r6", "::gentoo ",
             Color('fg', 'blue'), "{:0} ", Color('fg', 'yellow'), "[R] ",
             Color('fg', 'red'), "-static")
 
-    def test_iuse_stripped(self):
+    def test_iuse_defaults(self):
         self.formatter.format(
             FakeOp(self.FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', eapi='1', iuse=['+static', '-junk'], use=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut("* ", Color('fg', 'blue'), "app-arch/bzip2", "-1.0.3-r6", "::gentoo ",
             Color('fg', 'blue'), "{:0} ", Color('fg', 'yellow'), "[R] ",
             Color('fg', 'red'), "-junk ", Color('fg', 'green'), "static")
 
@@ -319,15 +358,17 @@
         self.formatter.format(
             FakeOp(self.FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static', 'bootstrap'], use=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut("* ", Color('fg', 'blue'), "app-arch/bzip2", "-1.0.3-r6", "::gentoo ",
             Color('fg', 'blue'), "{:0} ", Color('fg', 'yellow'), "[R] ",
             Color('fg', 'red'), "-bootstrap ", Color('fg', 'green'), "static")
 
+
 class TestPortageFormatter(BaseFormatterTest, TestCase):
+
     formatterClass = PortageFormatter
 
     def setUp(self):
         pkg = FakeMutatedPkg('app-arch/bzip2-1.0.1-r1', slot='0')
         masked_atom = atom('>=app-arch/bzip2-2.0')
         self.repo1 = FakeRepo(repo_id='gentoo', location='/var/gentoo/repos/gentoo', masks=(masked_atom,))
         self.repo2 = FakeRepo(repo_id='repo2', location='/var/gentoo/repos/repo2')
@@ -414,32 +455,43 @@
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
             ' USE="', Color('fg', 'yellow'), Bold(), '-static', Reset(), '%"')
 
-    def test_iuse_stripped(self):
+    def test_iuse_defaults(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', eapi='1', iuse=['+static', '-junk'], use=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
             ' USE="', Color('fg', 'yellow'), Bold(), 'static', Reset(), "%* ",
             Color('fg', 'yellow'), Bold(), '-junk', Reset(), '%"')
 
-    def test_use(self):
-        self.formatter.format(
-            FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
-            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
+    def test_use_enabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static']),
+        ))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
-            ' USE="', Color('fg', 'yellow'), Bold(), 'static', Reset(), '%*"')
+            ' USE="', Color('fg', 'green'), Bold(), 'static', Reset(), '*"')
+
+    def test_use_disabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static']),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
+        ))
+        self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
+            '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
+            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
+            ' USE="', Color('fg', 'green'), Bold(), '-static', Reset(), '*"')
 
     def test_multiuse(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static', 'bootstrap'], use=['static']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
@@ -451,47 +503,66 @@
         self.formatter.format(FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', slot='1')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '  ', Color('fg', 'green'), Bold(), 'N', Reset(), Color('fg', 'green'), Bold(),
             'S', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
             ' ', Color('fg', 'blue'), Bold(), '[1.0.1-r1]', Reset())
 
-    def test_fetch_restrict(self):
-        # no fetchables
+    def test_fetch_restrict_no_fetchables(self):
         self.formatter.format(FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', restrict='fetch')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '  ', Color('fg', 'green'), Bold(), 'N', Reset(),
             ' ', Color('fg', 'green'), Bold(), 'f', Reset(), '   ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset())
 
-        # TODO: add tests for fetch restricted ebuilds with required fetchables
-        # for both pre-fetched and missing fetchables cases
-
-    def test_changed_use(self):
-        self.formatter.format(
-            FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static', 'bootstrap'], use=['static']),
-            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static'])))
+    # TODO
+    def test_fetch_restrict_missing_fetchables(self):
+        pass
+
+    # TODO
+    def test_fetch_restrict_prefetched_fetchables(self):
+        pass
+
+    def test_added_iuse_disabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['bootstrap']),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6'),
+        ))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
             ' USE="', Color('fg', 'yellow'), Bold(), '-bootstrap', Reset(), '%"')
-        self.formatter.format(
-            FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6',
-                iuse=['static', 'bootstrap', 'perl', 'foobar', 'rice'],
-                use=['static', 'rice']),
-            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6',
-                iuse=['bootstrap', 'foobar', 'rice', 'kazaam'],
-                use=['foobar'])))
+
+    def test_added_iuse_enabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6'),
+        ))
+        self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
+            '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
+            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
+            ' USE="', Color('fg', 'yellow'), Bold(), 'static', Reset(), '%*"')
+
+    def test_dropped_iuse_disabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6'),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['bootstrap']),
+        ))
+        self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
+            '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
+            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset())
+
+    def test_dropped_iuse_enabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6'),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
+        ))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
-            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(), ' USE="',
-            Color('fg', 'green'), Bold(), 'rice', Reset(), '* ',
-            Color('fg', 'yellow'), Bold(), 'static', Reset(), '%* ',
-            Color('fg', 'green'), Bold(), '-foobar', Reset(), '* ',
-            Color('fg', 'yellow'), Bold(), '-perl', Reset(), '%"')
+            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset())
 
     def test_use_expand(self):
         self.formatter = self.newFormatter(use_expand=set(["foo", "bar"]))
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6',
                 iuse=['foo_static', 'foo_bootstrap', 'bar_baz'],
                 use=['foo_static', 'bar_baz']),
@@ -574,32 +645,31 @@
 
     def newFormatter(self, **kwargs):
         kwargs.setdefault("verbose", True)
         kwargs.setdefault("unstable_arch", "~amd64")
         kwargs.setdefault("domain_settings", {"ACCEPT_KEYWORDS": ("amd64",)})
         return TestPortageFormatter.newFormatter(self, **kwargs)
 
-    def test_install_symbols(self):
-        # unkeyworded
+    def test_install_symbol_unkeyworded(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', repo=self.repo1, keywords=())))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '  ', Color('fg', 'green'), Bold(), 'N', Reset(), '    ',
             Color('fg', 'red'), Bold(), '*', Reset(), '] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6%s' % self.repo_id(self.repo1), Reset())
 
-        # unstable arch
+    def test_install_symbol_unstable(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', repo=self.repo1, keywords=('~amd64',))))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '  ', Color('fg', 'green'), Bold(), 'N', Reset(), '    ',
             Color('fg', 'yellow'), Bold(), '~', Reset(), '] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6%s' % self.repo_id(self.repo1), Reset())
 
-        # masked
+    def test_install_symbol_masked(self):
         self.formatter.format(
            FakeOp(FakeEbuildSrc('app-arch/bzip2-2.1', repo=self.repo1)))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
            '  ', Color('fg', 'green'), Bold(), 'N', Reset(), '    ',
            Color('fg', 'red'), Bold(), '#', Reset(), '] ',
            Color('fg', 'green'), 'app-arch/bzip2-2.1%s' % self.repo_id(self.repo1), Reset())
 
@@ -669,23 +739,35 @@
         self.formatter.format(FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', slot='2', subslot='foo')))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '  ', Color('fg', 'green'), Bold(), 'N', Reset(), Color('fg', 'green'), Bold(),
             'S', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6:2/foo', Reset(),
             ' ', Color('fg', 'blue'), Bold(), '[1.0.1-r1:0]', Reset())
 
-    def test_changed_use(self):
-        self.formatter.format(
-            FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6', iuse=['static', 'bootstrap'], use=['static']),
-            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static'])))
+    def test_dropped_iuse_disabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6'),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['bootstrap']),
+        ))
         self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
             '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
             Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
-            ' USE="', Color('fg', 'red'), Bold(), 'static', Reset(), ' ',
-            Color('fg', 'yellow'), Bold(), '-bootstrap', Reset(), '%"')
+            ' USE="(', Color('fg', 'yellow'), Bold(), '-bootstrap', Reset(), '%)"')
+
+    def test_dropped_iuse_enabled(self):
+        self.formatter.format(FakeOp(
+            FakeEbuildSrc('app-arch/bzip2-1.0.3-r6'),
+            FakeMutatedPkg('app-arch/bzip2-1.0.3-r6', iuse=['static'], use=['static']),
+        ))
+        self.assertOut('[', Color('fg', 'green'), 'ebuild', Reset(),
+            '   ', Color('fg', 'yellow'), Bold(), 'R', Reset(), '    ] ',
+            Color('fg', 'green'), 'app-arch/bzip2-1.0.3-r6', Reset(),
+            ' USE="(', Color('fg', 'yellow'), Bold(), '-static', Reset(), '%*)"')
+
+    def test_changed_use(self):
         self.formatter.format(
             FakeOp(FakeEbuildSrc('app-arch/bzip2-1.0.3-r6',
                 iuse=['static', 'bootstrap', 'perl', 'foobar', 'rice'],
                 use=['static', 'rice']),
             FakeMutatedPkg('app-arch/bzip2-1.0.3-r6',
                 iuse=['bootstrap', 'foobar', 'rice', 'kazaam'],
                 use=['foobar'])))
```

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_portage_conf.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_portage_conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright: 2015 Tim Harder
 # License: GPL2/BSD
 
+import binascii
 import os
 import shutil
 import stat
 from tempfile import NamedTemporaryFile
 import textwrap
 
 from snakeoil.osutils import pjoin
@@ -101,14 +102,21 @@
                 errors.PermissionDeniedError, load_repos_conf, f.name)
 
         # blank file
         with NamedTemporaryFile() as f:
             self.assertRaises(
                 errors.ConfigurationError, load_repos_conf, f.name)
 
+        # garbage file
+        with NamedTemporaryFile() as f:
+            f.write(binascii.b2a_hex(os.urandom(10)))
+            f.flush()
+            self.assertRaises(
+                errors.ConfigurationError, load_repos_conf, f.name)
+
         # missing location parameter
         with NamedTemporaryFile() as f:
             f.write(textwrap.dedent('''\
                 [foo]
                 sync-uri = git://foo.git''').encode())
             f.flush()
             self.assertRaises(
@@ -122,14 +130,31 @@
                 location = /var/gentoo/repos/foo
                 [gentoo]
                 location = /var/gentoo/repos/gentoo''').encode())
             f.flush()
             defaults, repos = load_repos_conf(f.name)
             self.assertEqual(0, repos['foo']['priority'])
 
+        # overriding defaults in the same file throws an exception from configparser
+        with NamedTemporaryFile() as f:
+            f.write(textwrap.dedent('''\
+                [DEFAULT]
+                main-repo = gentoo
+                [DEFAULT]
+                main-repo = foo
+
+                [foo]
+                priority = foo
+                location = /var/gentoo/repos/foo
+                [gentoo]
+                location = /var/gentoo/repos/gentoo''').encode())
+            f.flush()
+            self.assertRaises(
+                errors.ConfigurationError, load_repos_conf, f.name)
+
         # undefined main repo with 'gentoo' missing
         with NamedTemporaryFile() as f:
             f.write(textwrap.dedent('''\
                 [foo]
                 location = /var/gentoo/repos/foo''').encode())
             f.flush()
             self.assertRaises(
@@ -143,14 +168,29 @@
                 [gentoo]
                 location = /var/gentoo/repos/gentoo''').encode())
             f.flush()
             defaults, repos = load_repos_conf(f.name)
             self.assertEqual('gentoo', defaults['main-repo'])
             self.assertEqual(['foo', 'gentoo'], repos.keys())
 
+        # TODO: check for logger output?
+        # overriding defaults in the same file throws an exception from configparser
+        with NamedTemporaryFile() as f:
+            f.write(textwrap.dedent('''\
+                [DEFAULT]
+                main-repo = foo
+                [foo]
+                priority = 3
+                location = /var/gentoo/repos/gentoo
+                [foo]
+                location = /var/gentoo/repos/foo''').encode())
+            f.flush()
+            self.assertRaises(
+                errors.ConfigurationError, load_repos_conf, f.name)
+
     def test_load_repos_conf_dir(self):
         # repo priority sorting and dir/symlink scanning
 
         repos_conf_dir = pjoin(self.dir, 'repos.conf')
         os.mkdir(repos_conf_dir)
         repos_conf_sym = pjoin(self.dir, 'repos.conf.sym')
         os.symlink(repos_conf_dir, repos_conf_sym)
```

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_repo_objs.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_repo_objs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_atom.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_atom.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_cpv.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_cpv.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/ebuild/test_ebuild_src.py` & `pkgcore-0.9.7/src/pkgcore/test/ebuild/test_ebuild_src.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fetch/test_init.py` & `pkgcore-0.9.7/src/pkgcore/test/fetch/test_init.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fetch/test_base.py` & `pkgcore-0.9.7/src/pkgcore/test/fetch/test_base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/package/test_metadata.py` & `pkgcore-0.9.7/src/pkgcore/test/package/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/package/test_mutated.py` & `pkgcore-0.9.7/src/pkgcore/test/package/test_mutated.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/package/test_base.py` & `pkgcore-0.9.7/src/pkgcore/test/package/test_base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/repository/test_visibility.py` & `pkgcore-0.9.7/src/pkgcore/test/repository/test_visibility.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/repository/test_prototype.py` & `pkgcore-0.9.7/src/pkgcore/test/repository/test_prototype.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/repository/test_multiplex.py` & `pkgcore-0.9.7/src/pkgcore/test/repository/test_multiplex.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/config/test_init.py` & `pkgcore-0.9.7/src/pkgcore/test/config/test_init.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/config/test_cparser.py` & `pkgcore-0.9.7/src/pkgcore/test/config/test_cparser.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/config/test_dhcpformat.py` & `pkgcore-0.9.7/src/pkgcore/test/config/test_dhcpformat.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/config/test_basics.py` & `pkgcore-0.9.7/src/pkgcore/test/config/test_basics.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/config/test_central.py` & `pkgcore-0.9.7/src/pkgcore/test/config/test_central.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/merge/test_engine.py` & `pkgcore-0.9.7/src/pkgcore/test/merge/test_engine.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/merge/test_triggers.py` & `pkgcore-0.9.7/src/pkgcore/test/merge/test_triggers.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/merge/util.py` & `pkgcore-0.9.7/src/pkgcore/test/merge/util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_git_svn.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_git_svn.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_git.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_git.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_darcs.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_darcs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_hg.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_hg.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_rsync.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_base.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_cvs.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_cvs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_bzr.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_bzr.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/sync/test_svn.py` & `pkgcore-0.9.7/src/pkgcore/test/sync/test_svn.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/resolver/test_pigeonholes.py` & `pkgcore-0.9.7/src/pkgcore/test/resolver/test_pigeonholes.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/resolver/test_choice_point.py` & `pkgcore-0.9.7/src/pkgcore/test/resolver/test_choice_point.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/resolver/test_plan.py` & `pkgcore-0.9.7/src/pkgcore/test/resolver/test_plan.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fs/fs_util.py` & `pkgcore-0.9.7/src/pkgcore/test/fs/fs_util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fs/test_fs.py` & `pkgcore-0.9.7/src/pkgcore/test/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fs/test_contents.py` & `pkgcore-0.9.7/src/pkgcore/test/fs/test_contents.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fs/test_ops.py` & `pkgcore-0.9.7/src/pkgcore/test/fs/test_ops.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/fs/test_livefs.py` & `pkgcore-0.9.7/src/pkgcore/test/fs/test_livefs.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/test_plugin.py` & `pkgcore-0.9.7/src/pkgcore/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/cache/test_base.py` & `pkgcore-0.9.7/src/pkgcore/test/cache/test_base.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/cache/test_flat_hash.py` & `pkgcore-0.9.7/src/pkgcore/test/cache/test_flat_hash.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/cache/util.py` & `pkgcore-0.9.7/src/pkgcore/test/cache/util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_filter_env.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_filter_env.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/helpers.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/helpers.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pmerge.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pmerge.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pconfig.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pconfig.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pclonecache.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pclonecache.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pquery.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pquery.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pmaint.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pmaint.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pclean.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pclean.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/scripts/test_pebuild.py` & `pkgcore-0.9.7/src/pkgcore/test/scripts/test_pebuild.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/test_gpg.py` & `pkgcore-0.9.7/src/pkgcore/test/test_gpg.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/pkgsets/test_filelist.py` & `pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_filelist.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/pkgsets/test_glsa.py` & `pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_glsa.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/pkgsets/test_installed.py` & `pkgcore-0.9.7/src/pkgcore/test/pkgsets/test_installed.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/__init__.py` & `pkgcore-0.9.7/src/pkgcore/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/util/test_parserestrict.py` & `pkgcore-0.9.7/src/pkgcore/test/util/test_parserestrict.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/util/test_commandline.py` & `pkgcore-0.9.7/src/pkgcore/test/util/test_commandline.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_restriction.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_restriction.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_values.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_values.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_util.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_delegated.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_delegated.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_boolean.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_boolean.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/restrictions/test_packages.py` & `pkgcore-0.9.7/src/pkgcore/test/restrictions/test_packages.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/test/misc.py` & `pkgcore-0.9.7/src/pkgcore/test/misc.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/cache/flat_hash.py` & `pkgcore-0.9.7/src/pkgcore/cache/flat_hash.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/cache/errors.py` & `pkgcore-0.9.7/src/pkgcore/cache/errors.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/cache/fs_template.py` & `pkgcore-0.9.7/src/pkgcore/cache/fs_template.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/cache/metadata.py` & `pkgcore-0.9.7/src/pkgcore/cache/metadata.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/cache/__init__.py` & `pkgcore-0.9.7/src/pkgcore/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/filter_env.py` & `pkgcore-0.9.7/src/pkgcore/scripts/filter_env.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pmerge.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pmerge.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pebuild.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pebuild.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pclean.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pclean.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pmaint.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pmaint.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pinspect.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pinspect.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pquery.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pquery.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pclonecache.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pclonecache.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/__init__.py` & `pkgcore-0.9.7/src/pkgcore/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,23 @@
         script = import_module(script_module)
     except ImportError as e:
         sys.stderr.write('Failed importing: %s!\n' % str(e))
         sys.stderr.write(
             'Verify that pkgcore and its deps are properly installed '
             'and/or PYTHONPATH is set correctly for python %s.\n' %
             ('.'.join(map(str, sys.version_info[:3])),))
-        if '--debug' in sys.argv:
+        if '--debug' in sys.argv[1:]:
             raise
         sys.stderr.write('Add --debug to the commandline for a traceback.\n')
         sys.exit(1)
 
     tool = Tool(script.argparser)
     ret = tool()
     raise SystemExit(ret)
 
 
 if __name__ == '__main__':
-    # we're in a git repo or tarball so add the base dir to the system path
-    repo_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    if not os.path.exists(os.path.join(repo_dir, 'setup.py')):
-        raise SystemExit('unknown repo hierarchy, %r should be repo root' % repo_dir)
-    sys.path.insert(0, repo_dir)
+    # We're in a git repo or tarball so add the src dir to the system path.
+    # Note that this assumes a certain module layout.
+    src_dir = os.path.realpath(__file__).rsplit(os.path.sep, 3)[0]
+    sys.path.insert(0, src_dir)
     run(os.path.basename(__file__))
```

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pplugincache.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pplugincache.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/scripts/pconfig.py` & `pkgcore-0.9.7/src/pkgcore/scripts/pconfig.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/pkgsets/filelist.py` & `pkgcore-0.9.7/src/pkgcore/pkgsets/filelist.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/pkgsets/glsa.py` & `pkgcore-0.9.7/src/pkgcore/pkgsets/glsa.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/pkgsets/system.py` & `pkgcore-0.9.7/src/pkgcore/pkgsets/system.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/pkgsets/installed.py` & `pkgcore-0.9.7/src/pkgcore/pkgsets/installed.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/pkgsets/live_rebuild_set.py` & `pkgcore-0.9.7/src/pkgcore/pkgsets/live_rebuild_set.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/const.py` & `pkgcore-0.9.7/src/pkgcore/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     if allow_environment_override:
         result = os.environ.get("PKGCORE_OVERRIDE_%s" % attr, result)
     if is_tuple:
         result = tuple(result)
     return result
 
 
-_reporoot = osp.dirname(osp.dirname(osp.realpath(__file__)))
+_reporoot = osp.realpath(__file__).rsplit(os.path.sep, 3)[0]
 DATA_PATH = _GET_CONST('DATA_PATH', _reporoot, allow_environment_override=True)
 LIBDIR_PATH = _GET_CONST('LIBDIR_PATH', _reporoot)
 CONFIG_PATH = _GET_CONST('CONFIG_PATH', '%(DATA_PATH)s/config')
 PATH_FORCED_PREPEND = _GET_CONST('INJECTED_BIN_PATH', ('%(DATA_PATH)s/bin',))
 CP_BINARY = _GET_CONST('CP_BINARY', '/bin/cp')
```

### Comparing `pkgcore-0.9.6/pkgcore/plugins/builtin_configurables.py` & `pkgcore-0.9.7/src/pkgcore/plugins/builtin_configurables.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/plugins/pkgcore_formatters.py` & `pkgcore-0.9.7/src/pkgcore/plugins/pkgcore_formatters.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/util/parserestrict.py` & `pkgcore-0.9.7/src/pkgcore/util/parserestrict.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/util/file_type.py` & `pkgcore-0.9.7/src/pkgcore/util/file_type.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/util/thread_pool.py` & `pkgcore-0.9.7/src/pkgcore/util/thread_pool.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/util/commandline.py` & `pkgcore-0.9.7/src/pkgcore/util/commandline.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/binpkg/repo_ops.py` & `pkgcore-0.9.7/src/pkgcore/binpkg/repo_ops.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/binpkg/repository.py` & `pkgcore-0.9.7/src/pkgcore/binpkg/repository.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/binpkg/remote.py` & `pkgcore-0.9.7/src/pkgcore/binpkg/remote.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/binpkg/xpak.py` & `pkgcore-0.9.7/src/pkgcore/binpkg/xpak.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/packages.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/packages.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/restriction.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/restriction.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/values.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/values.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/delegated.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/delegated.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/boolean.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/boolean.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgcore/restrictions/util.py` & `pkgcore-0.9.7/src/pkgcore/restrictions/util.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/config/make.globals` & `pkgcore-0.9.7/config/make.globals`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/BSD` & `pkgcore-0.9.7/BSD`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/man/pebuild.1` & `pkgcore-0.9.7/man/pebuild.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PEBUILD" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PEBUILD" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pebuild \- low-level ebuild utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pclean.1` & `pkgcore-0.9.7/man/pclean.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PCLEAN" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PCLEAN" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pclean \- system cleaning utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pclonecache.1` & `pkgcore-0.9.7/man/pclonecache.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PCLONECACHE" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PCLONECACHE" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pclonecache \- repository cache clone utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pkgcore.5` & `pkgcore-0.9.7/man/pkgcore.5`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PKGCORE" "5" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PKGCORE" "5" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pkgcore \- a framework for package management
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pconfig.1` & `pkgcore-0.9.7/man/pconfig.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PCONFIG" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PCONFIG" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pconfig \- configuration querying utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pquery.1` & `pkgcore-0.9.7/man/pquery.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PQUERY" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PQUERY" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pquery \- package querying interface
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pplugincache.1` & `pkgcore-0.9.7/man/pplugincache.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PPLUGINCACHE" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PPLUGINCACHE" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pplugincache \- plugin cache update utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pinspect.1` & `pkgcore-0.9.7/man/pinspect.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PINSPECT" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PINSPECT" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pinspect \- repository inspection interface
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pmaint.1` & `pkgcore-0.9.7/man/pmaint.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PMAINT" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PMAINT" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pmaint \- system/repository maintenance utility
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/pmerge.1` & `pkgcore-0.9.7/man/pmerge.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PMERGE" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "PMERGE" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 pmerge \- package merging and unmerging interface
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/man/filter-env.1` & `pkgcore-0.9.7/man/filter-env.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "FILTER-ENV" "1" "Sep 22, 2017" "0.9.6" "pkgcore"
+.TH "FILTER-ENV" "1" "Sep 27, 2017" "0.9.7" "pkgcore"
 .SH NAME
 filter-env \- filter a bash environment dump
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `pkgcore-0.9.6/src/bmh_search.c` & `pkgcore-0.9.7/src/bmh_search.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/depset.c` & `pkgcore-0.9.7/src/depset.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/atom.c` & `pkgcore-0.9.7/src/atom.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/filter_env.c` & `pkgcore-0.9.7/src/filter_env.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/cpv.c` & `pkgcore-0.9.7/src/cpv.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/restrictions.c` & `pkgcore-0.9.7/src/restrictions.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/src/misc.c` & `pkgcore-0.9.7/src/misc.c`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/ebuild-daemon.bash` & `pkgcore-0.9.7/ebd/ebuild-daemon.bash`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/exit-handling.lib` & `pkgcore-0.9.7/ebd/exit-handling.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/ebuild.lib` & `pkgcore-0.9.7/ebd/ebuild.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/generate_global_func_list.bash` & `pkgcore-0.9.7/ebd/generate_global_func_list.bash`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/generate_eapi_func_list.bash` & `pkgcore-0.9.7/ebd/generate_eapi_func_list.bash`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/ebuild-env-utils.lib` & `pkgcore-0.9.7/ebd/ebuild-env-utils.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/funcnames/global` & `pkgcore-0.9.7/ebd/funcnames/global`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/ebuild-daemon.lib` & `pkgcore-0.9.7/ebd/ebuild-daemon.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/isolated-functions.lib` & `pkgcore-0.9.7/ebd/isolated-functions.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/5.lib` & `pkgcore-0.9.7/ebd/eapi/5.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/4.lib` & `pkgcore-0.9.7/ebd/eapi/4.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/2.lib` & `pkgcore-0.9.7/ebd/eapi/2.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/0.lib` & `pkgcore-0.9.7/ebd/eapi/0.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/6.lib` & `pkgcore-0.9.7/ebd/eapi/6.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/depend.lib` & `pkgcore-0.9.7/ebd/eapi/depend.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/3.lib` & `pkgcore-0.9.7/ebd/eapi/3.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/eapi/common.lib` & `pkgcore-0.9.7/ebd/eapi/common.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/doexe` & `pkgcore-0.9.7/ebd/helpers/common/doexe`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/pkgcore-ebuild-helper` & `pkgcore-0.9.7/ebd/helpers/common/pkgcore-ebuild-helper`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/doman` & `pkgcore-0.9.7/ebd/helpers/common/doman`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/prepalldocs` & `pkgcore-0.9.7/ebd/helpers/common/prepalldocs`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/dodoc` & `pkgcore-0.9.7/ebd/helpers/common/dodoc`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/prepinfo` & `pkgcore-0.9.7/ebd/helpers/common/prepinfo`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/prepman` & `pkgcore-0.9.7/ebd/helpers/common/prepman`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/prepstrip` & `pkgcore-0.9.7/ebd/helpers/common/prepstrip`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/doins` & `pkgcore-0.9.7/ebd/helpers/common/doins`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/keepdir` & `pkgcore-0.9.7/ebd/helpers/common/keepdir`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/common/dolib` & `pkgcore-0.9.7/ebd/helpers/common/dolib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/internals/prepall` & `pkgcore-0.9.7/ebd/helpers/internals/prepall`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/internals/_raw_dohtml` & `pkgcore-0.9.7/ebd/helpers/internals/_raw_dohtml`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/internals/prepallman` & `pkgcore-0.9.7/ebd/helpers/internals/prepallman`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/helpers/internals/_generic_new` & `pkgcore-0.9.7/ebd/helpers/internals/_generic_new`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/ebd/ebuild-default-functions.lib` & `pkgcore-0.9.7/ebd/ebuild-default-functions.lib`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/setup.py` & `pkgcore-0.9.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import os
 import subprocess
 import sys
 
 from distutils import log
 from distutils.errors import DistutilsExecError
 from distutils.util import byte_compile
-from setuptools import setup, find_packages
+from setuptools import setup
 
 import pkgdist
+pkgdist_setup, pkgdist_cmds = pkgdist.setup()
 
 # These offsets control where we install the pkgcore config files and the EBD
 # bits relative to the install-data path given to the install subcmd.
 DATA_INSTALL_OFFSET = 'share/pkgcore'
 CONFIG_INSTALL_OFFSET = os.path.join(DATA_INSTALL_OFFSET, 'config')
 LIBDIR_INSTALL_OFFSET = 'lib/pkgcore'
 EBD_INSTALL_OFFSET = os.path.join(LIBDIR_INSTALL_OFFSET, 'ebd')
@@ -108,51 +109,65 @@
     path = os.path.join(python_base, "pkgcore", "_const.py")
     try:
         os.makedirs(os.path.dirname(path))
     except OSError as e:
         if e.errno != errno.EEXIST:
             raise
     log.info("writing lookup config to %r" % path)
+
     with open(path, "w") as f:
         os.chmod(path, 0o644)
-        f.write("INSTALL_PREFIX=%r\n" % install_prefix)
-        f.write("DATA_PATH=%r\n" %
-                os.path.join(install_prefix, DATA_INSTALL_OFFSET))
-        f.write("CONFIG_PATH=%r\n" %
-                os.path.join(install_prefix, CONFIG_INSTALL_OFFSET))
-        f.write("LIBDIR_PATH=%r\n" %
-                os.path.join(install_prefix, LIBDIR_INSTALL_OFFSET))
-        f.write("EBD_PATH=%r\n" %
-                os.path.join(install_prefix, EBD_INSTALL_OFFSET))
-
-        # This is added to suppress the default behaviour of looking
-        # within the repo for a bin subdir.
-        f.write("INJECTED_BIN_PATH=%r\n" % (tuple(injected_bin_path),))
-
-        # Static paths for various utilities.
-        from snakeoil import process
-        required_progs = ('bash', 'cp')
-        try:
-            for prog in required_progs:
-                prog_path = process.find_binary(prog)
-                f.write("%s_BINARY=%r\n" % (prog.upper(), prog_path))
-        except process.CommandNotFound:
-            raise DistutilsExecError(
-                "generating lookup config failed: required utility %r missing from PATH" % (prog,))
-
-        extra_progs = ('sandbox',)
-        for prog in extra_progs:
+        # write more dynamic _const file for wheel installs
+        if install_prefix != os.path.abspath(sys.prefix):
+            import textwrap
+            f.write(textwrap.dedent("""\
+                import os.path as osp
+                import sys
+
+                from snakeoil import process
+
+                INSTALL_PREFIX = osp.abspath(sys.prefix)
+                DATA_PATH = osp.join(INSTALL_PREFIX, {!r})
+                CONFIG_PATH = osp.join(INSTALL_PREFIX, {!r})
+                LIBDIR_PATH = osp.join(INSTALL_PREFIX, {!r})
+                EBD_PATH = osp.join(INSTALL_PREFIX, {!r})
+                INJECTED_BIN_PATH = ()
+                CP_BINARY = process.find_binary('cp')
+            """.format(
+                DATA_INSTALL_OFFSET, CONFIG_INSTALL_OFFSET,
+                LIBDIR_INSTALL_OFFSET, EBD_INSTALL_OFFSET)))
+        else:
+            f.write("INSTALL_PREFIX=%r\n" % install_prefix)
+            f.write("DATA_PATH=%r\n" %
+                    os.path.join(install_prefix, DATA_INSTALL_OFFSET))
+            f.write("CONFIG_PATH=%r\n" %
+                    os.path.join(install_prefix, CONFIG_INSTALL_OFFSET))
+            f.write("LIBDIR_PATH=%r\n" %
+                    os.path.join(install_prefix, LIBDIR_INSTALL_OFFSET))
+            f.write("EBD_PATH=%r\n" %
+                    os.path.join(install_prefix, EBD_INSTALL_OFFSET))
+
+            # This is added to suppress the default behaviour of looking
+            # within the repo for a bin subdir.
+            f.write("INJECTED_BIN_PATH=%r\n" % (tuple(injected_bin_path),))
+
+            # Static paths for various utilities.
+            from snakeoil import process
+            required_progs = ('cp',)
             try:
-                prog_path = process.find_binary(prog)
+                for prog in required_progs:
+                    prog_path = process.find_binary(prog)
+                    f.write("%s_BINARY=%r\n" % (prog.upper(), prog_path))
             except process.CommandNotFound:
-                prog_path = ''
-            f.write("%s_BINARY=%r\n" % (prog.upper(), prog_path))
+                raise DistutilsExecError(
+                    "generating lookup config failed: required utility %r missing from PATH" % (prog,))
 
-    byte_compile([path], prefix=python_base)
-    byte_compile([path], optimize=2, prefix=python_base)
+            f.close()
+            byte_compile([path], prefix=python_base)
+            byte_compile([path], optimize=2, prefix=python_base)
 
 
 class test(pkgdist.test):
     """test wrapper to enforce testing against built version."""
 
     def run(self):
         # This is fairly hacky, but is done to ensure that the tests
@@ -184,52 +199,43 @@
                 'src/filter_env.c', 'src/bmh_search.c']),
         pkgdist.OptionalExtension(
             'pkgcore.restrictions._restrictions', ['src/restrictions.c']),
         pkgdist.OptionalExtension(
             'pkgcore.ebuild._misc', ['src/misc.c']),
     ])
 
-cmdclass = {
+cmdclass = pkgdist_cmds
+cmdclass.update({
     'sdist': sdist,
     'build': pkgdist.build,
     'build_py': pkgdist.build_py2to3,
     'build_ext': pkgdist.build_ext,
-    'build_scripts': pkgdist.build_scripts,
-    'build_man': pkgdist.build_man,
-    'build_docs': pkgdist.build_docs,
     'test': test,
     'install': install,
-    'install_man': pkgdist.install_man,
-    'install_docs': pkgdist.install_docs,
-}
-command_options = {}
+})
 
 setup(
-    name=pkgdist.MODULE,
-    version=pkgdist.version(),
     description='package managing framework',
-    long_description=pkgdist.readme(),
     url='https://github.com/pkgcore/pkgcore',
     license='BSD/GPLv2',
     author='Brian Harring, Tim Harder',
     author_email='pkgcore-dev@googlegroups.com',
-    packages=find_packages(),
-    install_requires=pkgdist.install_requires(),
-    scripts=os.listdir('bin'),
     data_files=list(chain(
         pkgdist.data_mapping(EBD_INSTALL_OFFSET, 'ebd'),
         pkgdist.data_mapping(CONFIG_INSTALL_OFFSET, 'config'),
         pkgdist.data_mapping('share/zsh/site-functions', 'shell/zsh/completion'),
         pkgdist.data_mapping(
             os.path.join(LIBDIR_INSTALL_OFFSET, 'shell'), 'shell',
             skip=glob.glob('shell/*/completion')),
     )),
-    ext_modules=extensions, cmdclass=cmdclass, command_options=command_options,
+    ext_modules=extensions,
+    cmdclass=cmdclass,
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
     ],
+    **pkgdist_setup
 )
```

### Comparing `pkgcore-0.9.6/PKG-INFO` & `pkgcore-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pkgcore
-Version: 0.9.6
+Version: 0.9.7
 Summary: package managing framework
 Home-page: https://github.com/pkgcore/pkgcore
 Author: Brian Harring, Tim Harder
 Author-email: pkgcore-dev@googlegroups.com
 License: BSD/GPLv2
 Description: |pypi| |test| |coverage| |docs|
```

### Comparing `pkgcore-0.9.6/shell/zsh/pkgcore.zsh` & `pkgcore-0.9.7/shell/zsh/pkgcore.zsh`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/shell/zsh/completion/_pkgcore` & `pkgcore-0.9.7/shell/zsh/completion/_pkgcore`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/shell/pkgcore.sh` & `pkgcore-0.9.7/shell/pkgcore.sh`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/shell/bin/psite` & `pkgcore-0.9.7/shell/bin/psite`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/shell/bash/pkgcore.bash` & `pkgcore-0.9.7/shell/bash/pkgcore.bash`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/pkgdist.py` & `pkgcore-0.9.7/pkgdist.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 A collection of distutils extensions adding things like automatic 2to3
 translation, a test runner, and working around broken stdlib extensions CFLAG
 passing in distutils.
 
 Specifically, this module is only meant to be imported in setup.py scripts.
 """
 
+from contextlib import contextmanager
 import copy
 import errno
 import io
 import math
 from multiprocessing import cpu_count
 import operator
 import os
@@ -23,14 +24,15 @@
 import subprocess
 import sys
 import textwrap
 
 os.environ["SNAKEOIL_DEMANDLOAD_PROTECTION"] = 'n'
 os.environ["SNAKEOIL_DEMANDLOAD_WARN"] = 'n'
 
+from setuptools import find_packages
 from setuptools.command import install as dst_install
 
 from distutils import log
 from distutils.core import Command, Extension
 from distutils.errors import DistutilsExecError
 from distutils.command import (
     sdist as dst_sdist, build_ext as dst_build_ext, build_py as dst_build_py,
@@ -90,16 +92,16 @@
     if moduledir is None:
         raise ValueError('No main module found')
 
     return moduledir
 
 
 # determine the main module we're being used to package
-MODULEDIR = find_moduledir() 
-MODULEDIRNAME = os.path.dirname(MODULEDIR)
+MODULEDIR = find_moduledir()
+PACKAGEDIR = os.path.dirname(MODULEDIR)
 MODULE = os.path.basename(MODULEDIR)
 
 
 def version(moduledir=MODULEDIR):
     """Determine a module's version.
 
     Based on the assumption that a module defines __version__.
@@ -133,28 +135,75 @@
                 pass
             else:
                 raise
 
     return None
 
 
-def install_requires(topdir=TOPDIR):
-    """Determine a project's runtime dependencies."""
+def setup():
+    """Parameters and commands for setuptools."""
+    params = {
+        'name': MODULE,
+        'version': version(),
+        'long_description': readme(),
+        'packages': find_packages(PACKAGEDIR),
+        'package_dir': {'':os.path.basename(PACKAGEDIR)},
+        'install_requires': install_requires(),
+    }
+
+    cmds = {
+        'sdist': sdist,
+    }
+
+    # check for scripts
+    if os.path.exists(os.path.join(TOPDIR, 'bin')):
+        params['scripts'] = os.listdir('bin')
+        cmds['build_scripts'] = build_scripts
+
+    # check for docs
+    if os.path.exists(os.path.join(TOPDIR, 'doc')):
+        cmds['build_docs'] = build_docs
+        cmds['install_docs'] = install_docs
+
+    # check for man pages
+    if os.path.exists(os.path.join(TOPDIR, 'doc', 'man')):
+        cmds['build_man'] = build_man
+        cmds['install_man'] = install_man
+
+    return params, cmds
+
+
+def _requires(path):
+    """Determine a project's various dependencies from requirements files."""
     try:
-        with io.open(os.path.join(topdir, 'requirements', 'release.txt')) as f:
+        with io.open(path) as f:
             return f.read().splitlines()
     except IOError as e:
         if e.errno == errno.ENOENT:
             pass
         else:
             raise
-
     return None
 
 
+def build_requires():
+    """Determine a project's build dependencies."""
+    return _requires(os.path.join(TOPDIR, 'requirements', 'build.txt'))
+
+
+def install_requires():
+    """Determine a project's runtime dependencies."""
+    return _requires(os.path.join(TOPDIR, 'requirements', 'install.txt'))
+
+
+def test_requires():
+    """Determine a project's test dependencies."""
+    return _requires(os.path.join(TOPDIR, 'requirements', 'test.txt'))
+
+
 def get_file_paths(path):
     """Get list of all file paths under a given path."""
     for root, dirs, files in os.walk(path):
         for f in files:
             yield os.path.join(root, f)[len(path):].lstrip('/')
 
 
@@ -264,15 +313,16 @@
 
     def generate_verinfo(self, base_dir):
         """Generate project version module.
 
         This is used by the --version option in interactive programs among
         other things.
         """
-        from snakeoil.version import get_git_version
+        with syspath(PACKAGEDIR, MODULE == 'snakeoil'):
+            from snakeoil.version import get_git_version
         log.info('generating _verinfo')
         data = get_git_version(base_dir)
         if not data:
             return
         path = os.path.join(base_dir, '_verinfo.py')
         with open(path, 'w') as f:
             f.write('version_info=%r' % (data,))
@@ -281,15 +331,17 @@
         """Create and populate the directory tree that is put in source tars.
 
         This copies or hardlinks "normal" source files that should go
         into the release and adds generated files that should not
         exist in a working tree.
         """
 
-        if 'build_man' in self.distribution.cmdclass:
+        # don't build man pages when running under tox
+        if ('build_man' in self.distribution.cmdclass and
+                not os.path.basename(os.environ.get('_', '')) == 'tox'):
             build_man = self.reinitialize_command('build_man')
             build_man.ensure_finalized()
             self.run_command('build_man')
             shutil.copytree(os.path.join(os.getcwd(), build_man.content_search_path[0]),
                             os.path.join(base_dir, build_man.content_search_path[1]))
 
         dst_sdist.sdist.make_release_tree(self, base_dir, files)
@@ -330,15 +382,16 @@
         dst_build_py.build_py.finalize_options(self)
 
     def _run_generate_verinfo(self, rebuilds=None):
         ver_path = self.get_module_outfile(
             self.build_lib, (MODULE,), '_verinfo')
         # this should check mtime...
         if not os.path.exists(ver_path):
-            from snakeoil.version import get_git_version
+            with syspath(PACKAGEDIR, MODULE == 'snakeoil'):
+                from snakeoil.version import get_git_version
             log.info('generating _verinfo')
             with open(ver_path, 'w') as f:
                 f.write("version_info=%r" % (get_git_version('.'),))
             self.byte_compile([ver_path])
             if rebuilds is not None:
                 rebuilds.append((ver_path, os.lstat(ver_path).st_mtime))
 
@@ -374,15 +427,16 @@
                 yield trg_path, new_mtime
 
     def _inner_run(self, rebuilds):
         pass
 
     def get_py2to3_converter(self, options=None, proc_count=0):
         from lib2to3 import refactor as ref_mod
-        from snakeoil.dist import caching_2to3
+        with syspath(PACKAGEDIR, MODULE == 'snakeoil'):
+            from snakeoil.dist import caching_2to3
 
         if proc_count == 0:
             proc_count = cpu_count()
 
         assert proc_count >= 1
 
         if proc_count > 1 and not caching_2to3.multiprocessing_available:
@@ -456,22 +510,35 @@
         log.info("starting 3to2 conversion; this may take a while...")
         run_3to2([x[0] for x in py2k_rebuilds], fixer_names=fixer_names)
         for path, mtime in py2k_rebuilds:
             os.utime(path, (-1, mtime))
         log.info("completed py2k conversions")
 
 
+def generate_html():
+    """Generate html docs for the project."""
+    from snakeoil.dist.generate_docs import generate_html
+    generate_html(TOPDIR, PACKAGEDIR, MODULE)
+
+
+def generate_man():
+    """Generate man pages for the project."""
+    from snakeoil.dist.generate_docs import generate_man
+    generate_man(TOPDIR, PACKAGEDIR, MODULE)
+
+
 class build_man(Command):
     """Build man pages.
 
     Override the module search path before running sphinx. This fixes
     generating man pages for scripts that need to import modules generated via
     2to3 or other conversions instead of straight from the build directory.
     """
 
+    description = "build man pages"
     user_options = [
         ("force", "f", "force build as needed"),
     ]
     content_search_path = ('build/sphinx/man', 'man')
 
     def initialize_options(self):
         self.force = False
@@ -490,33 +557,30 @@
     def run(self):
         if self.force or not self.skip():
             # Use a built version for the man page generation process that
             # imports script modules.
             build_py = self.reinitialize_command('build_py')
             build_py.ensure_finalized()
             self.run_command('build_py')
-            syspath = sys.path[:]
-            sys.path.insert(0, os.path.abspath(build_py.build_lib))
-
-            # generate man page content for scripts we create
-            if 'build_scripts' in self.distribution.cmdclass:
-                from snakeoil.dist.generate_docs import generate_man
-                generate_man(MODULE, TOPDIR)
-
-            # generate man pages
-            build_sphinx = self.reinitialize_command('build_sphinx')
-            build_sphinx.builder = 'man'
-            build_sphinx.ensure_finalized()
-            self.run_command('build_sphinx')
-            sys.path = syspath
+            with syspath(os.path.abspath(build_py.build_lib)):
+                # generate man page content for scripts we create
+                if 'build_scripts' in self.distribution.cmdclass:
+                    generate_man()
+
+                # generate man pages
+                build_sphinx = self.reinitialize_command('build_sphinx')
+                build_sphinx.builder = 'man'
+                build_sphinx.ensure_finalized()
+                self.run_command('build_sphinx')
 
 
 class build_docs(build_man):
     """Build html docs."""
 
+    description = "build HTML documentation"
     user_options = [
         ("force", "f", "force build as needed"),
     ]
     content_search_path = ('build/sphinx/html', 'html')
 
     def initialize_options(self):
         self.force = False
@@ -526,16 +590,15 @@
 
     def run(self):
         if self.force or not self.skip():
             # generate man pages -- html versions of man pages are provided
             self.run_command('build_man')
 
             # generate API docs
-            from snakeoil.dist.generate_docs import generate_html
-            generate_html(MODULE, TOPDIR)
+            generate_html()
 
             # generate html docs -- allow build_sphinx cmd to run again
             build_sphinx = self.reinitialize_command('build_sphinx')
             build_sphinx.builder = 'html'
             build_sphinx.ensure_finalized()
             self.run_command('build_sphinx')
 
@@ -702,14 +765,15 @@
             self.enable_html_docs = False
 
 
 class install_docs(Command):
     """Install html documentation."""
 
     content_search_path = build_docs.content_search_path
+    description = "install HTML documentation"
     user_options = [
         ('path=', None, "final path to install to; else it's calculated"),
         ('build-dir=', None, "build directory"),
     ]
     build_command = 'build_docs'
 
     def initialize_options(self):
@@ -784,14 +848,15 @@
         # Py3k compatibility- force list so behaviour is the same.
         return list(self.content.values())
 
 
 class install_man(install_docs):
     """Install man pages."""
 
+    description = "install man pages"
     content_search_path = build_man.content_search_path
     build_command = 'build_man'
 
     def calculate_install_path(self):
         return os.path.join(self.prefix, 'share', 'man')
 
     def _map_paths(self, content):
@@ -838,14 +903,15 @@
     """Run our unit tests in a built copy.
 
     Based on code from setuptools.
     """
 
     blacklist = frozenset()
 
+    description = "run unit tests in a built copy"
     user_options = [
         ("inplace", "i", "do building/testing in place"),
         ("skip-rebuilding", "s", "skip rebuilds. primarily for development"),
         ("disable-fork", None, "disable forking of the testloader; primarily for debugging.  "
                                "Automatically set in jython, disabled for cpython/unladen-swallow."),
         ("namespaces=", "t", "run only tests matching these namespaces.  "
                              "comma delimited"),
@@ -924,14 +990,15 @@
         if retval:
             raise DistutilsExecError("tests failed; return %i" % (retval,))
 
 
 class pytest(Command):
     """Run tests using pytest."""
 
+    description = "run unit tests in a built copy using pytest"
     user_options = [
         ('pytest-args=', 'a', 'arguments to pass to py.test'),
         ('coverage', 'c', 'generate coverage info'),
         ('skip-build', 's', 'skip building the module'),
         ('test-dir=', 'd', 'directory to source tests from'),
         ('report=', 'r', 'generate and/or show a coverage report'),
         ('jobs=', 'j', 'run X parallel tests at once'),
@@ -1009,26 +1076,27 @@
             build_py = self.reinitialize_command('build_py')
             build_ext.ensure_finalized()
             build_py.ensure_finalized()
             self.run_command('build_ext')
             self.run_command('build_py')
             builddir = os.path.abspath(build_py.build_lib)
 
-        sys.path.insert(0, builddir)
-        from snakeoil.contexts import chdir
-        # Change the current working directory to the builddir during testing
-        # so coverage paths are correct.
-        with chdir(builddir):
-            ret = pytest.main(self.test_args)
+        with syspath(builddir):
+            from snakeoil.contexts import chdir
+            # Change the current working directory to the builddir during testing
+            # so coverage paths are correct.
+            with chdir(builddir):
+                ret = pytest.main(self.test_args)
         sys.exit(ret)
 
 
 class pylint(Command):
     """Run pylint on a module."""
 
+    description = "run pylint on a module"
     user_options = [
         ('errors-only', 'E', 'Check only errors with pylint'),
         ('output-format=', 'f', 'Change the output format'),
     ]
 
     def initialize_options(self):
         self.errors_only = False
@@ -1119,15 +1187,16 @@
 
     @cache_check('_sanity_check')
     @print_check('Performing basic C toolchain sanity check', 'works', 'broken')
     def _sanity_check(self):
         return self.try_link("int main(int argc, char *argv[]) { return 0; }")
 
     def run(self):
-        from snakeoil.pickling import dump, load
+        with syspath(PACKAGEDIR, MODULE == 'snakeoil'):
+            from snakeoil.pickling import dump, load
 
         # try to load the cached results
         try:
             with open(self.cache_path, 'rb') as f:
                 cache_db = load(f)
         except (OSError, IOError):
             cache_db = {}
@@ -1167,12 +1236,33 @@
     def check_struct_member(self, typename, member, headers=None, include_dirs=None, lang="c"):
         """Check whether typename (must be struct or union) has the named member."""
         return self.try_compile(
             'int main() { %s x; (void) x.%s; return 0; }'
             % (typename, member), headers, include_dirs, lang)
 
 
+# directly copied from snakeoil.contexts
+@contextmanager
+def syspath(path, condition=True, position=0):
+    """Context manager that mangles sys.path and then reverts on exit.
+
+    Args:
+        path: The directory path to add to sys.path.
+        condition: Optional boolean that decides whether sys.path is mangled or
+            not, defaults to being enabled.
+        position: Optional integer that is the place where the path is inserted
+            in sys.path, defaults to prepending.
+    """
+    syspath = sys.path[:]
+    if condition:
+        sys.path.insert(position, path)
+    try:
+        yield
+    finally:
+        sys.path = syspath
+
+
 # yes these are in snakeoil.compatibility; we can't rely on that module however
 # since snakeoil source is in 2k form, but this module is 2k/3k compatible.
 # in other words, it could be invoked by py3k to translate snakeoil to py3k
 is_py3k = sys.version_info >= (3, 0)
 is_jython = 'java' in getattr(sys, 'getPlatform', lambda: '')().lower()
```

### Comparing `pkgcore-0.9.6/NEWS.rst` & `pkgcore-0.9.7/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 =============
 Release Notes
 =============
 
 --------------------------
+pkgcore 0.9.7 (2017-09-27)
+--------------------------
+
+- Use a more dynamic pkgcore._const for wheel-based installs instead of the
+  static version used when installing directly to a system. Using a static
+  version can't be done because the final paths aren't known until the wheel is
+  installed on the target system.
+
+- Fix merging pkgs with non-ascii filenames with python3. Previously pmerge
+  would crash when writing the contents file to the vdb.
+
+--------------------------
 pkgcore 0.9.6 (2017-09-22)
 --------------------------
 
 - Fix building and deploying wheels.
 
 --------------------------
 pkgcore 0.9.5 (2017-09-22)
```

### Comparing `pkgcore-0.9.6/doc/man/pkgcore.rst` & `pkgcore-0.9.7/doc/man/pkgcore.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/man/pquery.rst` & `pkgcore-0.9.7/doc/man/pquery.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/man/pmerge.rst` & `pkgcore-0.9.7/doc/man/pmerge.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/conf.py` & `pkgcore-0.9.7/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 libdir = os.path.abspath(os.path.join('..', 'build', 'lib'))
 if os.path.exists(libdir):
     sys.path.insert(0, libdir)
 sys.path.insert(1, os.path.abspath('..'))
-
-from pkgcore import __version__, const
-from snakeoil.dist.generate_docs import generate_man, generate_html
+import pkgdist
 
 on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
@@ -52,24 +50,24 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'pkgcore'
+project = pkgdist.MODULE
 authors = ''
 copyright = '2006-2017, pkgcore contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = __version__
+version = pkgdist.version()
 # The full version, including alpha/beta/rc tags.
 release = 'trunk'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
@@ -101,16 +99,16 @@
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
 #modindex_common_prefix = []
 
 # auto-generate required files for RTD build environment
 if on_rtd:
-    generate_man(project, const.DATA_PATH)
-    generate_html(project, const.DATA_PATH)
+    pkgdist.generate_man()
+    pkgdist.generate_html()
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinxdoc'
```

### Comparing `pkgcore-0.9.6/doc/Makefile` & `pkgcore-0.9.7/doc/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 PYTHONPATH    = ../
 PYTHON        = python
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
 BUILDDIR      = $(CURDIR)/_build
+TOPDIR        = ..
+PACKAGEDIR    = ../src
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 MAINSPHINXOPTS   = $(PAPEROPT_$(PAPER)) $(SPHINXOPTS)
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(MAINSPHINXOPTS) .
 # note this should probably just check for sphinx.domains in sys.modules w/in the demandload instead..
@@ -41,15 +43,15 @@
 	@echo "  linkcheck  to check all external links for integrity"
 	@echo "  doctest    to run all doctests embedded in the documentation (if enabled)"
 
 clean:
 	-rm -rf $(BUILDDIR) api generated
 
 html:
-	$(PYTHON) -m snakeoil.dist.generate_docs --html ../ pkgcore
+	$(PYTHON) -m snakeoil.dist.generate_docs --html $(TOPDIR) $(PACKAGEDIR) pkgcore
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 dirhtml:
 	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) $(BUILDDIR)/dirhtml
 	@echo
@@ -114,15 +116,15 @@
 
 text:
 	$(SPHINXBUILD) -b text $(ALLSPHINXOPTS) $(BUILDDIR)/text
 	@echo
 	@echo "Build finished. The text files are in $(BUILDDIR)/text."
 
 man:
-	$(PYTHON) -m snakeoil.dist.generate_docs --man ../ pkgcore
+	$(PYTHON) -m snakeoil.dist.generate_docs --man $(TOPDIR) $(PACKAGEDIR) pkgcore
 	$(SPHINXBUILD) -b man $(ALLSPHINXOPTS) $(BUILDDIR)/man
 	@for file in man/*; do \
 		[ -L "$${file}" ] && rm -f "$${file}" || continue; \
 	done
 	@echo
 	@echo "Build finished. The manual pages are in $(BUILDDIR)/man."
```

### Comparing `pkgcore-0.9.6/doc/index.rst` & `pkgcore-0.9.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/hacking.rst` & `pkgcore-0.9.7/doc/dev-notes/hacking.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/tackling-domain.rst` & `pkgcore-0.9.7/doc/dev-notes/tackling-domain.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/heapy.rst` & `pkgcore-0.9.7/doc/dev-notes/heapy.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/formats/dpkg.rst` & `pkgcore-0.9.7/doc/dev-notes/formats/dpkg.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/fs-ops.rst` & `pkgcore-0.9.7/doc/dev-notes/fs-ops.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/eapi.rst` & `pkgcore-0.9.7/doc/dev-notes/eapi.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/plugins.rst` & `pkgcore-0.9.7/doc/dev-notes/plugins.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/TODO.rst` & `pkgcore-0.9.7/doc/dev-notes/TODO.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/config.rst` & `pkgcore-0.9.7/doc/dev-notes/config.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/tests.rst` & `pkgcore-0.9.7/doc/dev-notes/tests.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/changes.rst` & `pkgcore-0.9.7/doc/dev-notes/changes.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/portage-differences.rst` & `pkgcore-0.9.7/doc/dev-notes/portage-differences.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/framework/intro.rst` & `pkgcore-0.9.7/doc/dev-notes/framework/intro.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/harring-notes.rst` & `pkgcore-0.9.7/doc/dev-notes/harring-notes.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/feature-breakdown.rst` & `pkgcore-0.9.7/doc/dev-notes/feature-breakdown.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/developing.rst` & `pkgcore-0.9.7/doc/dev-notes/developing.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/doc/dev-notes/commandline.rst` & `pkgcore-0.9.7/doc/dev-notes/commandline.rst`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/examples/pkg_info.py` & `pkgcore-0.9.7/examples/pkg_info.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/examples/changed_use.py` & `pkgcore-0.9.7/examples/changed_use.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/examples/report_pkg_changes.py` & `pkgcore-0.9.7/examples/report_pkg_changes.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/examples/repo_list.py` & `pkgcore-0.9.7/examples/repo_list.py`

 * *Files identical despite different names*

### Comparing `pkgcore-0.9.6/examples/identify-installed-non-split-debug-pkgs.py` & `pkgcore-0.9.7/examples/identify-installed-non-split-debug-pkgs.py`

 * *Files identical despite different names*

