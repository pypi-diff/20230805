# Comparing `tmp/mkdocs-git-revision-date-plugin-blame-0.1.5.tar.gz` & `tmp/mkdocs-git-revision-date-plugin-blame-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.5.tar", last modified: Sat Aug  5 20:28:09 2023, max compression
+gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.6.tar", last modified: Sat Aug  5 21:10:39 2023, max compression
```

## Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5.tar` & `mkdocs-git-revision-date-plugin-blame-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.153925 mkdocs-git-revision-date-plugin-blame-0.1.5/
--rw-rw-rw-   0        0        0      378 2023-08-05 20:28:09.152912 mkdocs-git-revision-date-plugin-blame-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.137910 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/
--rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-08-05 20:22:51.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/gitTest.py
--rw-rw-rw-   0        0        0     2648 2023-08-05 19:00:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/plugin.py
--rw-rw-rw-   0        0        0     2155 2023-08-05 20:25:43.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/util.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.150923 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/
--rw-rw-rw-   0        0        0      378 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 20:28:09.153925 mkdocs-git-revision-date-plugin-blame-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-08-05 20:26:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 21:10:39.487079 mkdocs-git-revision-date-plugin-blame-0.1.6/
+-rw-rw-rw-   0        0        0      378 2023-08-05 21:10:39.486078 mkdocs-git-revision-date-plugin-blame-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 21:10:39.456052 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/
+-rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/__init__.py
+-rw-rw-rw-   0        0        0     2283 2023-08-05 21:00:13.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/gitTest.py
+-rw-rw-rw-   0        0        0     2648 2023-08-05 19:00:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/plugin.py
+-rw-rw-rw-   0        0        0     2858 2023-08-05 21:02:01.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/util.py
+drwxrwxrwx   0        0        0        0 2023-08-05 21:10:39.485072 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-08-05 21:10:39.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 21:10:39.487079 mkdocs-git-revision-date-plugin-blame-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-08-05 21:02:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.6/setup.py
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/README.md` & `mkdocs-git-revision-date-plugin-blame-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/gitTest.py` & `mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/gitTest.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,45 +3,58 @@
 import datetime
 
 myRepo = git.repo.Repo("C:/Users/Cody/tuas/wiki")
 
 # print(myRepo.commit('bdea42410c5655e1e9505b3d87099897716987a0').)
 
 # iterator for each blame 'chunk' of the file
-blameIter = myRepo.blame_incremental(myRepo.head, "docs/software/software_home.md")
+blameIter = myRepo.blame_incremental(myRepo.head, "docs/general/repo_guide.md")
 currOutput = myRepo.blame(myRepo.head, "docs/embedded/electronics-diagram.md")
 
 # print each timestamp of the git blame
 
 blameTimes = []
 
 for blame in blameIter:
     rawEpochTime = blame.commit.authored_date # type: ignore (not sure why this gives an error; it works fine)
-    print(rawEpochTime)
     timeSince = datetime.datetime.fromtimestamp(rawEpochTime).strftime('%Y-%m-%d') # add %H:%M:%S for specific time
     blameTimes.append(timeSince)
 
-print(blameTimes)
+# print(blameTimes)
 
 def getMostRecentTime(times):
 
     mostRecentTime = '0000-00-00'
 
+    mostRecentTimeYear = int(mostRecentTime[0:4])
+    mostRecentTimeMonth = int(mostRecentTime[5:7])
+    mostRecentTimeDay = int(mostRecentTime[8:10])
+
     for time in times:
         year = int(time[0:4])
         month = int(time[5:7])
         day = int(time[8:10])
-
-        mostRecentTimeYear = int(mostRecentTime[0:4])
-        mostRecentTimeMonth = int(mostRecentTime[5:7])
-        mostRecentTimeDay = int(mostRecentTime[8:10])
+        # print(year)
 
         if year > mostRecentTimeYear:
+            # print('yes')
             mostRecentTime = time
         elif (year == mostRecentTimeYear and month > mostRecentTimeMonth):
             mostRecentTime = time
-        elif (year == mostRecentTimeYear and month == mostRecentTimeMonth and mostRecentTimeDay > mostRecentTimeDay):
+        elif (year == mostRecentTimeYear and month == mostRecentTimeMonth and day > mostRecentTimeDay):
             mostRecentTime = time
 
-    return mostRecentTime
+        mostRecentTimeYear = int(mostRecentTime[0:4])
+        mostRecentTimeMonth = int(mostRecentTime[5:7])
+        mostRecentTimeDay = int(mostRecentTime[8:10])
+
+    # print(mostRecentTimeYear)
+
+    # have to do this case because windows can't use the %-d strftime code. %e is the windows equivalent,
+    #   but instead of actually removing the 0 padding, it prepends the number with a space, leaving some awkward gaps when the number has 2 digits.
+    #   tldr; gg windows sucks
+    if (mostRecentTimeDay < 10):
+        return datetime.date(mostRecentTimeYear,mostRecentTimeMonth,mostRecentTimeDay).strftime("%B%e, %Y")
+
+    return datetime.date(mostRecentTimeYear,mostRecentTimeMonth,mostRecentTimeDay).strftime("%B %d, %Y")
 
 print('most recent time:', getMostRecentTime(blameTimes))
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/plugin.py` & `mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/util.py` & `mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,25 +28,36 @@
         for blame in blameIter:
             rawEpochTime = blame.commit.authored_date # type: ignore (not sure why this gives an error; it works fine)
             timeSince = datetime.datetime.fromtimestamp(rawEpochTime).strftime('%Y-%m-%d') # add %H:%M:%S for specific time
             blameTimes.append(timeSince)
 
         mostRecentTime = '0000-00-00'
 
+        mostRecentTimeYear = int(mostRecentTime[0:4])
+        mostRecentTimeMonth = int(mostRecentTime[5:7])
+        mostRecentTimeDay = int(mostRecentTime[8:10])
+
         # find most recent blame (to be displayed as last updated)
         for time in blameTimes:
             year = int(time[0:4])
             month = int(time[5:7])
             day = int(time[8:10])
 
-            mostRecentTimeYear = int(mostRecentTime[0:4])
-            mostRecentTimeMonth = int(mostRecentTime[5:7])
-            mostRecentTimeDay = int(mostRecentTime[8:10])
-
             if year > mostRecentTimeYear:
                 mostRecentTime = time
             elif (year == mostRecentTimeYear and month > mostRecentTimeMonth):
                 mostRecentTime = time
             elif (year == mostRecentTimeYear and month == mostRecentTimeMonth and day > mostRecentTimeDay):
                 mostRecentTime = time
 
-        return mostRecentTime
+            mostRecentTimeYear = int(mostRecentTime[0:4])
+            mostRecentTimeMonth = int(mostRecentTime[5:7])
+            mostRecentTimeDay = int(mostRecentTime[8:10])
+
+
+        # have to do this case because windows can't use the %-d strftime code. %e is the windows equivalent,
+        #   but instead of actually removing the 0 padding, it prepends the number with a space, leaving some awkward gaps when the number has 2 digits.
+        #   tldr; gg windows sucks
+        if (mostRecentTimeDay < 10):
+            return datetime.date(mostRecentTimeYear,mostRecentTimeMonth,mostRecentTimeDay).strftime("%B%e, %Y")
+
+        return datetime.date(mostRecentTimeYear,mostRecentTimeMonth,mostRecentTimeDay).strftime("%B %d, %Y")
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt` & `mkdocs-git-revision-date-plugin-blame-0.1.6/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.5/setup.py` & `mkdocs-git-revision-date-plugin-blame-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-git-revision-date-plugin-blame',
-    version='0.1.5',
+    version='0.1.6',
     description='MkDocs plugin for setting revision date from git per markdown file using blame.',
     keywords='mkdocs git meta yaml frontmatter',
     url='https://github.com/codyprupp/mkdocs-git-revision-date-plugin',
     author='Cody Rupp',
     author_email='crupp@ucsd.edu',
     license='MIT',
     license_files = ('LICENSE'),
```

