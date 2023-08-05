# Comparing `tmp/hashbeaf-1.0.0.tar.gz` & `tmp/hashbeaf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hashbeaf/hashbeaf/dist/.tmp-32eo7jlh/hashbeaf-1.0.0.tar", last modified: Sun Jul  2 07:56:09 2023, max compression
+gzip compressed data, was "/home/runner/work/hashbeaf/hashbeaf/dist/.tmp-ws163wec/hashbeaf-1.1.0.tar", last modified: Sat Aug  5 09:49:02 2023, max compression
```

## Comparing `hashbeaf-1.0.0.tar` & `hashbeaf-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/src/hashbeaf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/src/hashbeaf/hashbeaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/src/hashbeaf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/src/hashbeaf/words.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/src/hashbeaf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:56:09.000000 hashbeaf-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 07:56:00.000000 hashbeaf-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/src/hashbeaf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/src/hashbeaf/hashbeaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/src/hashbeaf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/src/hashbeaf/words.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/src/hashbeaf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:49:02.000000 hashbeaf-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/tests/test_hashbeaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-05 09:48:54.000000 hashbeaf-1.1.0/tests/test_words.py
```

### Comparing `hashbeaf-1.0.0/LICENSE` & `hashbeaf-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashbeaf-1.0.0/PKG-INFO` & `hashbeaf-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashbeaf
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple utility to create user-specified git commit hashes
 Author-email: Cedric Nugteren <web@cedricnugteren.nl>
 Project-URL: Homepage, https://github.com/cnugteren/hashbeaf
 Project-URL: Bug Tracker, https://github.com/cnugteren/hashbeaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,37 +42,43 @@
 (...)
 ```
 And voila, we have `c0de2c4`, our HashBeaf'ed commit hash!
 
 
 ## Want to try it yourself?
 
-Install it with `pip install hashbeaf`, navigate to your own git repository, make a commit, and then run either:
+Install it with:
+```bash
+pip install hashbeaf
+```
+Then navigate to your own git repository, make a commit, and then run either:
 ```bash
 hashbeaf
 ```
 to use a default list of nice 'words', or something like this for a custom 'word':
 ```bash
 hashbeaf c0de
 ```
 See `hashbeaf --help` for more information.
+There is also a `hb` alias if you don't want to type 8 characters.
 
 If you think it is too much work to run this after each commit, you can also install a git post-commit hook for your repository.
 Modify `post-commit` to point to the right absolute path (and customize it further as needed), and simple copy it to `your_repo/.git/hooks`.
 On the next commit hashbeaf should run automatically.
 
 Need some inspiration?
 Check out the [default words list](src/hashbeaf/words.py) for nice commit hashes, or see more on [Wikipedia here](https://en.wikipedia.org/wiki/Hexspeak) and [here](https://en.wikipedia.org/wiki/Magic_number_(programming)#Magic_debug_values).
 
 
 ## Implementation details
 
 The algorithm is inspired by [beautify_git_hash](https://github.com/vog/beautify_git_hash), a slightly outdated tool that achieves the same thing.
 
 HashBeaf is implemented in Python and requires version 3.7 or newer.
+It has been tested on Linux but might run on other operation systems.
 
 HashBeaf works as follows.
 A commit hash in git is computed based on the commit details, which include the commit message, author time and committer time.
 If we modify any of those, we get a new commit hash.
 With HashBeaf we set the author time and committer time to some time in the near future, compute a new hash, and if the hash starts with any of the user supplied 'words', we amend the previous commit by running something like:
 ```bash
 GIT_COMMITTER_DATE=$(some_commit_time) git commit --amend -C HEAD --date=$(some_author_time)
@@ -92,11 +98,9 @@
 
 
 ## Feature wish list
 
 Missing a feature?
 Soon there will be also:
 
-1. A pypi version that you can install as `pip install hashbeaf`.
-2. More tests
-3. More documentation
-4. More error checking
+1. More documentation
+2. More error checking
```

### Comparing `hashbeaf-1.0.0/README.md` & `hashbeaf-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,37 +28,43 @@
 (...)
 ```
 And voila, we have `c0de2c4`, our HashBeaf'ed commit hash!
 
 
 ## Want to try it yourself?
 
-Install it with `pip install hashbeaf`, navigate to your own git repository, make a commit, and then run either:
+Install it with:
+```bash
+pip install hashbeaf
+```
+Then navigate to your own git repository, make a commit, and then run either:
 ```bash
 hashbeaf
 ```
 to use a default list of nice 'words', or something like this for a custom 'word':
 ```bash
 hashbeaf c0de
 ```
 See `hashbeaf --help` for more information.
+There is also a `hb` alias if you don't want to type 8 characters.
 
 If you think it is too much work to run this after each commit, you can also install a git post-commit hook for your repository.
 Modify `post-commit` to point to the right absolute path (and customize it further as needed), and simple copy it to `your_repo/.git/hooks`.
 On the next commit hashbeaf should run automatically.
 
 Need some inspiration?
 Check out the [default words list](src/hashbeaf/words.py) for nice commit hashes, or see more on [Wikipedia here](https://en.wikipedia.org/wiki/Hexspeak) and [here](https://en.wikipedia.org/wiki/Magic_number_(programming)#Magic_debug_values).
 
 
 ## Implementation details
 
 The algorithm is inspired by [beautify_git_hash](https://github.com/vog/beautify_git_hash), a slightly outdated tool that achieves the same thing.
 
 HashBeaf is implemented in Python and requires version 3.7 or newer.
+It has been tested on Linux but might run on other operation systems.
 
 HashBeaf works as follows.
 A commit hash in git is computed based on the commit details, which include the commit message, author time and committer time.
 If we modify any of those, we get a new commit hash.
 With HashBeaf we set the author time and committer time to some time in the near future, compute a new hash, and if the hash starts with any of the user supplied 'words', we amend the previous commit by running something like:
 ```bash
 GIT_COMMITTER_DATE=$(some_commit_time) git commit --amend -C HEAD --date=$(some_author_time)
@@ -78,11 +84,9 @@
 
 
 ## Feature wish list
 
 Missing a feature?
 Soon there will be also:
 
-1. A pypi version that you can install as `pip install hashbeaf`.
-2. More tests
-3. More documentation
-4. More error checking
+1. More documentation
+2. More error checking
```

### Comparing `hashbeaf-1.0.0/pyproject.toml` & `hashbeaf-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hashbeaf"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Cedric Nugteren", email="web@cedricnugteren.nl" },
 ]
 description = "A simple utility to create user-specified git commit hashes"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -25,8 +25,9 @@
 "Homepage" = "https://github.com/cnugteren/hashbeaf"
 "Bug Tracker" = "https://github.com/cnugteren/hashbeaf/issues"
 
 [tool.black]
 line-length = 100
 
 [tool.pytype]
-inputs = ["src", "tests"]
+# TODO: Add 'tests' folder for checking
+inputs = ["src"]
```

### Comparing `hashbeaf-1.0.0/src/hashbeaf/hashbeaf.py` & `hashbeaf-1.1.0/src/hashbeaf/hashbeaf.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,36 +7,45 @@
 
 logger = logging.getLogger(__name__)
 
 
 def _commit_data_modify_increment(
     commit_data: str, author_increment: int, commit_increment: int
 ) -> Tuple[str, str, str]:
+    if "author " not in commit_data or "committer " not in commit_data:
+        raise RuntimeError(f"Received unexpected commmit-data: {commit_data}")
     lines = commit_data.split("\n")
-    author_data_split = lines[2].split(" ")
-    commit_data_split = lines[3].split(" ")
+    line_offset = [i for i, line in enumerate(lines) if line.startswith("author ")][0]
+    author_data_split = lines[line_offset].split(" ")
+    commit_data_split = lines[line_offset + 1].split(" ")
     author_timestamp = int(author_data_split[-2]) + author_increment
     commit_timestamp = int(commit_data_split[-2]) + commit_increment
     author_time_full = f"{author_timestamp} {author_data_split[-1]}"
     commit_time_full = f"{commit_timestamp} {commit_data_split[-1]}"
     author_line = " ".join([*author_data_split[:-2], author_time_full])
     commit_line = " ".join([*commit_data_split[:-2], commit_time_full])
-    modified_commit_data = "\n".join([lines[0], lines[1], author_line, commit_line, *lines[4:]])
+    modified_commit_data = "\n".join(
+        [*lines[:line_offset], author_line, commit_line, *lines[line_offset + 2 :]]  # noqa: E203
+    )
     return modified_commit_data, author_time_full, commit_time_full
 
 
+def _get_commit_data_original() -> str:
+    return run_command("git cat-file commit HEAD")
+
+
 def hashbeaf_main(words: List[str], max_minutes_in_future: int) -> None:
     words = [word.lower() for word in words]
     for word in words:
         if not ishex(word):
             raise RuntimeError(
                 f"User input '{word}' contains non-hexadecimal characters, aborting."
             )
 
-    commit_data_original = run_command("git cat-file commit HEAD")
+    commit_data_original = _get_commit_data_original()
     for commit_increment in range(max_minutes_in_future * 60):
         for author_increment in range(commit_increment + 1):
             (commit_data, author_time_full, commit_time_full) = _commit_data_modify_increment(
                 commit_data_original, author_increment, commit_increment
             )
             new_hash = get_hash(commit_data)
             for word in words:
```

### Comparing `hashbeaf-1.0.0/src/hashbeaf/utils.py` & `hashbeaf-1.1.0/src/hashbeaf/utils.py`

 * *Files identical despite different names*

### Comparing `hashbeaf-1.0.0/src/hashbeaf.egg-info/PKG-INFO` & `hashbeaf-1.1.0/src/hashbeaf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashbeaf
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple utility to create user-specified git commit hashes
 Author-email: Cedric Nugteren <web@cedricnugteren.nl>
 Project-URL: Homepage, https://github.com/cnugteren/hashbeaf
 Project-URL: Bug Tracker, https://github.com/cnugteren/hashbeaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,37 +42,43 @@
 (...)
 ```
 And voila, we have `c0de2c4`, our HashBeaf'ed commit hash!
 
 
 ## Want to try it yourself?
 
-Install it with `pip install hashbeaf`, navigate to your own git repository, make a commit, and then run either:
+Install it with:
+```bash
+pip install hashbeaf
+```
+Then navigate to your own git repository, make a commit, and then run either:
 ```bash
 hashbeaf
 ```
 to use a default list of nice 'words', or something like this for a custom 'word':
 ```bash
 hashbeaf c0de
 ```
 See `hashbeaf --help` for more information.
+There is also a `hb` alias if you don't want to type 8 characters.
 
 If you think it is too much work to run this after each commit, you can also install a git post-commit hook for your repository.
 Modify `post-commit` to point to the right absolute path (and customize it further as needed), and simple copy it to `your_repo/.git/hooks`.
 On the next commit hashbeaf should run automatically.
 
 Need some inspiration?
 Check out the [default words list](src/hashbeaf/words.py) for nice commit hashes, or see more on [Wikipedia here](https://en.wikipedia.org/wiki/Hexspeak) and [here](https://en.wikipedia.org/wiki/Magic_number_(programming)#Magic_debug_values).
 
 
 ## Implementation details
 
 The algorithm is inspired by [beautify_git_hash](https://github.com/vog/beautify_git_hash), a slightly outdated tool that achieves the same thing.
 
 HashBeaf is implemented in Python and requires version 3.7 or newer.
+It has been tested on Linux but might run on other operation systems.
 
 HashBeaf works as follows.
 A commit hash in git is computed based on the commit details, which include the commit message, author time and committer time.
 If we modify any of those, we get a new commit hash.
 With HashBeaf we set the author time and committer time to some time in the near future, compute a new hash, and if the hash starts with any of the user supplied 'words', we amend the previous commit by running something like:
 ```bash
 GIT_COMMITTER_DATE=$(some_commit_time) git commit --amend -C HEAD --date=$(some_author_time)
@@ -92,11 +98,9 @@
 
 
 ## Feature wish list
 
 Missing a feature?
 Soon there will be also:
 
-1. A pypi version that you can install as `pip install hashbeaf`.
-2. More tests
-3. More documentation
-4. More error checking
+1. More documentation
+2. More error checking
```

