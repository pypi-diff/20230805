# Comparing `tmp/gsb-0.0.2rc1.tar.gz` & `tmp/gsb-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsb-0.0.2rc1.tar", last modified: Wed Jul 26 21:55:58 2023, max compression
+gzip compressed data, was "gsb-0.0.2rc2.tar", last modified: Sat Aug  5 19:46:48 2023, max compression
```

## Comparing `gsb-0.0.2rc1.tar` & `gsb-0.0.2rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/onboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/rewind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/gsb/test/test_rewind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/gsb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 21:55:58.000000 gsb-0.0.2rc1/gsb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-26 21:55:58.198759 gsb-0.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-26 21:55:49.000000 gsb-0.0.2rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:46:48.074455 gsb-0.0.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-05 19:46:48.074455 gsb-0.0.2rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:46:48.078455 gsb-0.0.2rc2/gsb/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-05 19:46:48.078455 gsb-0.0.2rc2/gsb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/onboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/rewind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:46:48.074455 gsb-0.0.2rc2/gsb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/gsb/test/test_rewind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:46:48.074455 gsb-0.0.2rc2/gsb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 19:46:48.000000 gsb-0.0.2rc2/gsb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-05 19:46:48.078455 gsb-0.0.2rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-08-05 19:46:40.000000 gsb-0.0.2rc2/versioneer.py
```

### Comparing `gsb-0.0.2rc1/LICENSE` & `gsb-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/PKG-INFO` & `gsb-0.0.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsb
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: Game Save Backups: A Git-Based Tool for Managing Your Save States
 Home-page: https://github.com/OpenBagTwo/gsb
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `gsb-0.0.2rc1/README.md` & `gsb-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/_git.py` & `gsb-0.0.2rc2/gsb/_git.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         The initialized git repository
 
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
-    LOGGER.debug("git init %s", repo_root)
     return _repo(repo_root, new=True)
 
 
 def _repo(repo_root: Path, new: bool = False) -> pygit2.Repository:
     """Load a git repository from the specified location
 
     Parameters
@@ -63,14 +62,15 @@
     """
     repo_root = repo_root.expanduser().resolve()
     if not repo_root.exists():
         raise FileNotFoundError(f"{repo_root} does not exist")
     if not repo_root.is_dir():
         raise NotADirectoryError(f"{repo_root} is not a directory")
     if new:
+        LOGGER.debug("git init %s", repo_root)
         return pygit2.init_repository(repo_root, initial_head="gsb")
     try:
         return pygit2.Repository(repo_root)
     except pygit2.GitError as maybe_no_git:
         if "repository not found" in str(maybe_no_git).lower():
             raise FileNotFoundError(maybe_no_git) from maybe_no_git
         raise  # pragma: no cover
@@ -128,17 +128,19 @@
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
     patterns = list(patterns)
+    LOGGER.debug(
+        "git add %s",
+        " ".join([repr(pattern) for pattern in patterns]),
+    )
     repo.index.add_all(patterns)
-    for pattern in patterns:
-        LOGGER.debug("git add %s", pattern)
     repo.index.write()
     return repo.index
 
 
 def force_add(repo_root: Path, files: Iterable[Path]) -> pygit2.Index:
     """Forcibly add specific files, overriding .gitignore, equivalent to running
     `git add <file> --force`
@@ -163,16 +165,16 @@
         If one of the specified paths is a directory
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
     for path in files:
         try:
-            repo.index.add(path)
             LOGGER.debug("git add --force %s", path)
+            repo.index.add(path)
         except OSError as maybe_file_not_found:  # pragma: no cover
             if "No such file or directory" in str(maybe_file_not_found):
                 raise FileNotFoundError(maybe_file_not_found) from maybe_file_not_found
             raise  # pragma: no cover
         except pygit2.GitError as maybe_directory:  # pragma: no cover
             if "is a directory" in str(maybe_directory):
                 raise IsADirectoryError(maybe_directory) from maybe_directory
@@ -263,18 +265,19 @@
     author = pygit2.Signature(config["user.name"], config["user.email"])
     if _committer is None:
         committer = pygit2.Signature(
             config["committer.name"], config["committer.email"]
         )
     else:
         committer = pygit2.Signature(*_committer)
+
+    LOGGER.debug("git commit -m %s", message)
     commit_id = repo.create_commit(
         ref, author, committer, message, repo.index.write_tree(), parents
     )
-    LOGGER.debug("git commit -m %s", message)
     return Commit.from_pygit2(repo[commit_id])
 
 
 def log(repo_root: Path) -> Generator[Commit, None, None]:
     """Return metadata about commits such as you'd get by running `git log`
 
     Parameters
@@ -415,33 +418,36 @@
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
 
     config = _config()
     if _tagger is None:
-        tagger = pygit2.Signature(config["committer.name"], config["committer.email"])
+        tagger = pygit2.Signature(
+            config["committer.name"],
+            config["committer.email"],
+        )
     else:
         tagger = pygit2.Signature(*_tagger)
 
     if annotation:
         if not annotation.endswith("\n"):
             annotation += "\n"
 
+        LOGGER.debug("git tag %s -am %s", tag_name, annotation)
         repo.create_tag(
             tag_name,
             repo.head.target,
             pygit2.GIT_OBJ_COMMIT,
             tagger,
             annotation,
         )
-        LOGGER.debug("git tag %s -am %s", tag_name, annotation)
     else:
-        repo.create_reference(f"refs/tags/{tag_name}", repo.head.target)
         LOGGER.debug("git tag %s", tag_name)
+        repo.create_reference(f"refs/tags/{tag_name}", repo.head.target)
 
     return Tag.from_repo_reference(tag_name, repo)
 
     # PSA: pygit2.AlreadyExistsError subclasses ValueError
 
 
 def get_tags(repo_root: Path, annotated_only: bool) -> list[Tag]:
@@ -464,22 +470,51 @@
     Raises
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     """
     repo = _repo(repo_root)
     tags: list[Tag] = []
+    LOGGER.debug("git tag")
     for reference in repo.references.iterator(pygit2.GIT_REFERENCES_TAGS):
         parsed_tag = Tag.from_repo_reference(reference, repo)
         if parsed_tag.annotation or not annotated_only:
             tags.append(parsed_tag)
-    LOGGER.debug("git tag")
     return sorted(tags)
 
 
+def _resolve_reference(reference: str, repo: pygit2.Repository) -> pygit2.Object:
+    """Attempt to resolve a reference
+
+    Parameters
+    ----------
+    reference : str
+        The reference to resolve
+    repo : Repository
+        The git repository
+
+    Returns
+    -------
+    pygit2.Object
+        The resolved reference
+
+    Raises
+    ------
+    ValueError
+        If the specified revision does not exist
+    """
+    try:
+        LOGGER.debug("git show %s", reference)
+        return repo.revparse_single(reference)
+    except KeyError as no_rev:
+        raise ValueError(
+            f"Could not find a revision named {repr(reference)}"
+        ) from no_rev
+
+
 def show(repo_root: Path, reference: str) -> Commit | Tag:
     """Get information about a specified revision, similar to the output you'd
     get from running `git show <commit-hash-or-tag-name>`.
 
     Parameters
     ----------
     repo_root : Path
@@ -496,21 +531,15 @@
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     ValueError
         If the specified revision does not exist
     """
     repo = _repo(repo_root)
-    try:
-        revision = repo.revparse_single(reference)
-        LOGGER.debug("git show %s", reference)
-    except KeyError as no_rev:
-        raise ValueError(
-            f"Could not find a revision named {repr(reference)}"
-        ) from no_rev
+    revision = _resolve_reference(reference, repo)
     if revision.type == pygit2.GIT_OBJ_TAG:
         return Tag.from_repo_reference(str(revision.id), repo)
     if revision.type == pygit2.GIT_OBJ_COMMIT:
         return Commit.from_pygit2(revision)
     raise TypeError(  # pragma: no cover
         f"Object of type {revision.type} is not a valid revision"
     )
@@ -537,16 +566,67 @@
     ------
     OSError
         If `repo_root` does not exist, is not a directory or cannot be accessed
     ValueError
         If the specified revision does not exist
     """
     repo = _repo(repo_root)
-    try:
-        reference = repo.revparse_single(reference).id
-    except KeyError as no_rev:
-        raise ValueError(
-            f"Could not find a revision named {repr(reference)}"
-        ) from no_rev
+
+    # make sure revision exists
+    reference = _resolve_reference(reference, repo).id
 
     LOGGER.debug(f"git reset --{'hard' if hard else 'soft'} %s", reference)
     repo.reset(reference, pygit2.GIT_RESET_HARD if hard else pygit2.GIT_RESET_SOFT)
+
+
+def checkout_files(repo_root: Path, reference: str, paths: Iterable[Path]) -> None:
+    """Check out the versions of the specified files that existed at the specified
+    revision, equivalent to running
+    `git reset <revision> -- <paths...> && git checkout <revision> -- <paths...>`
+
+    Parameters
+    ----------
+    repo_root : Path
+        The root directory of the git repo
+    reference : str
+        A unique descriptor of the tag or commit
+    paths : list of Paths
+        The files to reset
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    OSError
+        If `repo_root` does not exist, is not a directory or cannot be accessed
+    ValueError
+        If the specified revision does not exist
+    """
+    repo = _repo(repo_root)
+
+    revision = _resolve_reference(reference, repo)
+    if isinstance(revision, pygit2.Tag):
+        return checkout_files(repo_root, str(revision.target), paths)
+
+    paths = list(paths)
+
+    for path in paths:
+        LOGGER.debug(f"git reset %s -- %s", reference, path)
+        try:
+            repo.index.remove(path)
+        except OSError:
+            pass  # possible that the file no longer exists
+        try:
+            past_file = revision.tree[path]
+            repo.index.add(pygit2.IndexEntry(path, past_file.id, past_file.filemode))
+        except KeyError:
+            pass  # possible that the file doesn't exist at the time of the revision
+
+    repo.index.write()
+    LOGGER.debug(
+        f"git checkout %s -- %s",
+        reference,
+        " ".join((repr(str(path)) for path in paths)),
+    )
+    repo.checkout(strategy=pygit2.GIT_CHECKOUT_FORCE, paths=paths)
```

### Comparing `gsb-0.0.2rc1/gsb/backup.py` & `gsb-0.0.2rc2/gsb/backup.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/cli.py` & `gsb-0.0.2rc2/gsb/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,26 +171,31 @@
         kwargs["limit"] = limit
     if since is not None:
         kwargs["since"] = since
 
     history_.get_history(path_as_arg or repo_root, **kwargs)
 
 
+@click.option(
+    "--include_gsb_settings",
+    is_flag=True,
+    help="Also revert the GSB configuration files (including .gitignore)",
+)
 @click.argument(
     "revision",
     type=str,
     required=False,
 )
 @_subcommand_init
-def rewind(repo_root: Path, revision: str | None):
+def rewind(repo_root: Path, revision: str | None, include_gsb_settings: bool):
     """Restore a backup to the specified REVISION."""
     if revision is None:
         revision = _prompt_for_revision(repo_root)
     try:
-        rewind_.restore_backup(repo_root, revision)
+        rewind_.restore_backup(repo_root, revision, not include_gsb_settings)
     except ValueError as whats_that:
         LOGGER.error(whats_that)
         sys.exit(1)
 
 
 def _prompt_for_revision(repo_root) -> str:
     """Select a revision from a prompt"""
```

### Comparing `gsb-0.0.2rc1/gsb/history.py` & `gsb-0.0.2rc2/gsb/history.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/logging.py` & `gsb-0.0.2rc2/gsb/logging.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/manifest.py` & `gsb-0.0.2rc2/gsb/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,12 +123,12 @@
     dumped = ""
     for key, value in manifest.items():
         dumped += f"{key} = "
         if isinstance(value, str):
             # it's honestly shocking how often I rely on json.dump for str escaping
             dumped += f"{json.dumps(value)}\n"
         else:
-            dumped += "[\n"
+            dumped += "["
             for entry in sorted(set(value)):
-                dumped += f"    {json.dumps(entry)},"
-            dumped += "]\n"
+                dumped += f"\n    {json.dumps(entry)},"
+            dumped += "\n]\n"
     return dumped
```

### Comparing `gsb-0.0.2rc1/gsb/onboard.py` & `gsb-0.0.2rc2/gsb/onboard.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/rewind.py` & `gsb-0.0.2rc2/gsb/rewind.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 
 from . import _git, backup
 from .logging import IMPORTANT
 
 LOGGER = logging.getLogger(__name__)
 
 
-def restore_backup(repo_root: Path, revision: str) -> str:
+def restore_backup(repo_root: Path, revision: str, keep_gsb_files: bool = True) -> str:
     """Rewind to a previous backup state and create a new backup
 
     Parameters
     ----------
     repo_root : Path
         The directory containing the GSB-managed repo
     revision : str
         The commit hash or tag name of the backup to restore
+    keep_gsb_files : bool, optional
+        By default, `.gsb_manifest` and `.gitignore` *will not* be restored
+        (that is, the latest versions will be kept). To override this behavior,
+        pass in `keep_gsb_files = False`.
 
     Returns
     -------
     str
         The tag name of the new restored backup
 
     Notes
@@ -41,9 +45,10 @@
     )
     orig_head = backup.create_backup(
         repo_root, f"Backing up state before rewinding to {revision}"
     )
 
     _git.reset(repo_root, revision, hard=True)
     _git.reset(repo_root, orig_head, hard=False)
-
+    if keep_gsb_files:
+        _git.checkout_files(repo_root, orig_head, backup.REQUIRED_FILES)
     return backup.create_backup(repo_root, f"Restored to {revision}")
```

### Comparing `gsb-0.0.2rc1/gsb/test/conftest.py` & `gsb-0.0.2rc2/gsb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/test/test_backup.py` & `gsb-0.0.2rc2/gsb/test/test_backup.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/test/test_history.py` & `gsb-0.0.2rc2/gsb/test/test_history.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/gsb/test/test_init.py` & `gsb-0.0.2rc2/gsb/test/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,21 @@
     def test_init_adds_save_contents(self, root):
         (root / "game.sav").write_text("poke\n")
         _ = onboard.create_repo(root, "game.sav")
         index = _git.ls_files(root)
         expected = {root / "game.sav", root / MANIFEST_NAME, root / ".gitignore"}
         assert expected == expected.intersection(index)
 
+    def test_pattern_with_no_matches_does_not_error(self, root):
+        (root / "game.sav").write_text("poke\n")
+        _ = onboard.create_repo(root, "save.game")
+        index = _git.ls_files(root)
+        expected = {root / MANIFEST_NAME, root / ".gitignore"}
+        assert expected == expected.intersection(index)
+
     def test_initial_add_respects_gitignore(self, root):
         (root / ".dot_dot").write_text("dash\n")
         _ = onboard.create_repo(root, ignore=[".*"])
         index = _git.ls_files(root)
 
         assert (root / ".dot_dot") not in index
```

### Comparing `gsb-0.0.2rc1/gsb/test/test_rewind.py` & `gsb-0.0.2rc2/gsb/test/test_rewind.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """Tests for restoring backups"""
 import subprocess
 
 import pytest
 
 from gsb import _git, backup, history, onboard, rewind
+from gsb.manifest import MANIFEST_NAME
 
 
 @pytest.fixture
 def repo(tmp_path, patch_tag_naming):
     my_game_data = tmp_path / "best game ever"
     my_save_data = my_game_data / "save" / "data.txt"
     my_save_data.parent.mkdir(parents=True)
     my_save_data.touch()
+    _git.init(my_game_data)
+    _git.add(my_game_data, my_save_data.name)
+    _git.commit(
+        my_game_data,
+        "Back when the world was new",
+        _committer=("Old Man", "old@man"),
+    )
     onboard.create_repo(my_game_data, "save")
 
     for i in range(10):
         my_save_data.write_text(f"{i}\n")
         if i % 2 == 0:
             (my_save_data.parent / ".boop").touch()
             (my_save_data.parent / ".beep").unlink(missing_ok=True)
@@ -93,14 +101,53 @@
         assert (
             "restore"
             in next(iter(history.get_history(repo, tagged_only=False)))[
                 "description"
             ].lower()
         )
 
+    def test_gsb_manifest_and_gitignore_are_not_rewound(self, repo):
+        with (repo / ".gitignore").open("a") as ignore:
+            ignore.write("nothingtosee\n")
+        with (repo / MANIFEST_NAME).open("a") as manifest:
+            manifest.write("# it's a comment\n")
+
+        rewind.restore_backup(repo, "gsb2023.07.10")
+
+        with pytest.raises(ValueError, match="othing to"):
+            _git.add(repo, ["saves"])
+            _git.commit(repo, "Test")
+
+        assert "nothingtosee" in (repo / ".gitignore").read_text().splitlines()
+        assert "# it's a comment" in (repo / MANIFEST_NAME).read_text().splitlines()
+
+    def test_gsb_manifest_and_gitignore_can_be_rewound(self, repo):
+        with (repo / ".gitignore").open("a") as ignore:
+            ignore.write("nothingtosee\n")
+        with (repo / MANIFEST_NAME).open("a") as manifest:
+            manifest.write("# it's a comment\n")
+
+        rewind.restore_backup(repo, "gsb2023.07.10", keep_gsb_files=False)
+
+        with pytest.raises(ValueError, match="othing to"):
+            _git.add(repo, ["saves"])
+            _git.commit(repo, "Test")
+
+        assert "nothingtosee" not in (repo / ".gitignore").read_text()
+        assert "# it's a comment" not in (repo / MANIFEST_NAME).read_text()
+
+    def test_can_rewind_to_pre_gsb_state(self, repo):
+        first_commit = history.get_history(
+            repo, tagged_only=False, include_non_gsb=True
+        )[-1]
+
+        rewind.restore_backup(repo, first_commit["identifier"])
+
+        assert (repo / MANIFEST_NAME).exists()
+
 
 class TestCLI:
     def test_no_args_initiates_prompt_in_cwd(self, repo):
         result = subprocess.run(
             ["gsb", "rewind"], cwd=repo, capture_output=True, input="q\n".encode()
         )
 
@@ -127,15 +174,15 @@
             ["gsb", "rewind", "gsb2023.07.12"], cwd=repo, capture_output=True
         )
 
         assert (repo / "save" / "data.txt").read_text() == "3\n"
 
     @pytest.mark.parametrize("how", ("short", "full"))
     def test_restoring_to_commit(self, repo, how):
-        some_commit = list(_git.log(repo))[-4].hash
+        some_commit = list(_git.log(repo))[-5].hash
         if how == "short":
             some_commit = some_commit[:8]
 
         _ = subprocess.run(
             ["gsb", "rewind", some_commit],
             cwd=repo,
             capture_output=True,
@@ -216,7 +263,19 @@
         something = repo / "file"
         something.touch()
         _git.init(repo)
 
         result = subprocess.run(["gsb", "rewind"], cwd=repo, capture_output=True)
         assert result.returncode == 1
         assert "No revisions found" in result.stderr.decode().strip().splitlines()[-1]
+
+    def test_force_rewind_of_required_files(self, repo):
+        with (repo / MANIFEST_NAME).open("a") as manifest:
+            manifest.write("# it's a comment\n")
+
+        _ = subprocess.run(
+            ["gsb", "rewind", "gsb2023.07.12", "--include_gsb_settings"],
+            cwd=repo,
+            capture_output=False,
+        )
+
+        assert "# it's a comment" not in (repo / MANIFEST_NAME).read_text()
```

### Comparing `gsb-0.0.2rc1/gsb.egg-info/PKG-INFO` & `gsb-0.0.2rc2/gsb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsb
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: Game Save Backups: A Git-Based Tool for Managing Your Save States
 Home-page: https://github.com/OpenBagTwo/gsb
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `gsb-0.0.2rc1/setup.py` & `gsb-0.0.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `gsb-0.0.2rc1/versioneer.py` & `gsb-0.0.2rc2/versioneer.py`

 * *Files identical despite different names*

