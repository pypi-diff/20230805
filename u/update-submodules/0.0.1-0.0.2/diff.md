# Comparing `tmp/update-submodules-0.0.1.tar.gz` & `tmp/update-submodules-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-submodules-0.0.1.tar", last modified: Sat Aug  5 12:45:26 2023, max compression
+gzip compressed data, was "update-submodules-0.0.2.tar", last modified: Sat Aug  5 14:31:50 2023, max compression
```

## Comparing `update-submodules-0.0.1.tar` & `update-submodules-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:45:26.169921 update-submodules-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 12:45:26.169921 update-submodules-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-08-05 12:45:11.000000 update-submodules-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:45:26.169921 update-submodules-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-05 12:45:11.000000 update-submodules-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:45:26.169921 update-submodules-0.0.1/update_submodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:45:11.000000 update-submodules-0.0.1/update_submodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-05 12:45:11.000000 update-submodules-0.0.1/update_submodules/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-05 12:45:11.000000 update-submodules-0.0.1/update_submodules/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-05 12:45:11.000000 update-submodules-0.0.1/update_submodules/meta_branch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:45:26.169921 update-submodules-0.0.1/update_submodules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 12:45:26.000000 update-submodules-0.0.1/update_submodules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:31:50.981642 update-submodules-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 14:31:50.981642 update-submodules-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-08-05 14:31:37.000000 update-submodules-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:31:50.981642 update-submodules-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-05 14:31:37.000000 update-submodules-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:31:50.977642 update-submodules-0.0.2/update_submodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 14:31:37.000000 update-submodules-0.0.2/update_submodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-05 14:31:37.000000 update-submodules-0.0.2/update_submodules/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-05 14:31:37.000000 update-submodules-0.0.2/update_submodules/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-05 14:31:37.000000 update-submodules-0.0.2/update_submodules/meta_branch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:31:50.981642 update-submodules-0.0.2/update_submodules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 14:31:50.000000 update-submodules-0.0.2/update_submodules.egg-info/top_level.txt
```

### Comparing `update-submodules-0.0.1/README.md` & `update-submodules-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # update-submodules
- Update a repo's submodules without cloning it (using the GitHub API)
- - [Python library](#python-library)
- - [GitHub Action](#github-action)
+Update a repo's submodules without cloning it (using the GitHub API)
 
-## Python Library <a id="python-library"></a>
+ - [Python library](#python-library): `update-submodules` [![PyPI badge: "update-submodules" library](https://img.shields.io/pypi/v/update-submodules.svg)](https://pypi.python.org/pypi/update-submodules)
+     - [Update submodules directly via the GitHub API](#github-update-modules)
+     - [Update submodules in cloned repositories (including "bare" clones)](#git-update-submodules)
+ - [GitHub Action: `runsascoded/update-submodules@v1`](#github-action)
+     - [Default branches](#default-branches)
+     - [Overriding branches/refs](#non-default-branches)
+     - [Step output: new commit SHA](#output)
+     - [Step summary](#step-summary)
+
+## Python Library: `update-submodules` <a id="python-library"></a>
 ```bash
 pip install update-submodules
 ```
-### Update submodules directly via the GitHub API
+### Update submodules directly via the GitHub API <a id="github-update-modules"></a>
 ```bash
 github-update-submodules --help
 # Usage: github-update-submodules [OPTIONS] [REF_STRS]...
 #
 #   Update submodules in a GitHub repository, using the API / without cloning
 #   the repository.
 #
@@ -40,15 +47,15 @@
 #   -R, --repository TEXT           Repository name (with owner, e.g.
 #                                   "owner/repo"), defaults to
 #                                   $GITHUB_REPOSITORY then `gh repo view --json
 #                                   nameWithOwner`
 #   --help                          Show this message and exit.
 ```
 
-### Update submodules in cloned repositories (including "bare" clones)
+### Update submodules in cloned repositories (including "bare" clones) <a id="git-update-submodules"></a>
 If your repository is already cloned (including "bare" clones), `git-update-submodules` works similarly (including `push`ing):
 ```bash
 git-update-submodules --help
 # Usage: git-update-submodules [OPTIONS] [REF_STRS]...
 #
 #   Update submodules in a locally-cloned Git repository.
 #
@@ -75,60 +82,65 @@
 #   -v, --verbose       1x: print tree, commit SHAs; 2x: also print `git`
 #                       commands as they are run; 3x: print `git ls-tree` output
 #                       for new commit
 #   --help              Show this message and exit.
 ```
 This also works on repos hosted outside GitHub.
 
-## GitHub Action <a id="github-action"></a>
-Example usage:
+## GitHub Action: `runsascoded/update-submodules@v1` <a id="github-action"></a>
+`github-update-submodules` is also available as a GitHub Action (see [`action.yml`](action.yml)).
+
+### Default branches <a id="default-branches"></a>
+Update all submodules in current `$GITHUB_REPOSITORY`'s default branch to point to the latest SHA's on their respective default branches:
 ```yaml
 steps:
-  # Update the current $GITHUB_REPOSITORY's default branch to contain the latest SHA on each submodule's default branch
   - uses: runsascoded/update-submodules@v1
     with:
       token: ${{ secrets.GITHUB_TOKEN }}
 ```
 
-Specific refs can be provided per-submodule, and non-default branches can be updated:
+### Overriding branches/refs <a id="non-default-branches"></a>
+The parent-repo branch to update is configurable, as are the specific refs to update each submodule to:
 ```yaml
 steps:
   - uses: runsascoded/update-submodules@v1
     with:
-      # Specific branch/tag for 2 submodules, `develop` branch for others
-      refs: submodule1=main submodule2:refs/tags/v1.0.0 develop
-      # Update a non-HEAD branch
+      # Update a non-default branch
       branch: develop
+      # Specific branch/tag for 2 submodules, fall back to the `develop` branch for all others
+      refs: submodule1=main submodule2:refs/tags/v1.0.0 develop
       token: ${{ secrets.GITHUB_TOKEN }}
 ```
 
+### Step output: new commit SHA <a id="output"></a>
 If the action creates a commit (containing newly-updated submodules), the commit's SHA is stored as an "output":
 ```yaml
 steps:
   - uses: runsascoded/update-submodules@v1
     id: update
     with:
       token: ${{ secrets.GITHUB_TOKEN }}
   - run: echo "Pushed new commit ${{ steps.update.outputs.sha }} with updated submodules"
 ```
 
+### Step summary <a id="step-summary"></a>
+
 The Action also prints a summary on the workflow "summary" page, like:
-[![](screenshots/rc.png)](https://github.com/runsascoded/.rc/actions/runs/5755454755)
-([from runsascoded/.rc](https://github.com/runsascoded/.rc/blob/server/.github/workflows/update-branches.yml))
+[![](screenshots/rc.png)](https://github.com/runsascoded/.rc/actions/runs/5771027368)
+([from runsascoded/.rc](https://github.com/runsascoded/.rc/blob/server/.github/workflows/update-branches.yml#L10-L15))
 
 or:
 [![](screenshots/test.png)](https://github.com/runsascoded/update-submodules/actions/runs/5757404520)
 ([from `.github/workflows/test.yml`](./.github/workflows/test.yml))
 
 ## Similar Projects / Links
 I looked at the following libraries and examples, but they mostly require cloning the repo, which I wanted to avoid:
 
-- https://github.blog/2020-12-21-get-up-to-speed-with-partial-clone-and-shallow-clone/
-- https://github.com/robherley/shallow-fetch-sha
-- https://github.com/marketplace/actions/github-action-submodule-updates
 - https://thenewstack.io/how-to-trigger-github-actions-on-submodule-updates/
 - https://stackoverflow.com/questions/64407333/using-github-actions-to-automatically-update-the-repos-submodules
 - https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#package-ecosystem
+- https://github.blog/2020-12-21-get-up-to-speed-with-partial-clone-and-shallow-clone/
+- https://github.com/robherley/shallow-fetch-sha
 
 ### Github Actions
 - https://github.com/marketplace/actions/submodule-branch-check
 - https://github.com/marketplace/actions/github-action-submodule-updates
```

### Comparing `update-submodules-0.0.1/update_submodules/git.py` & `update-submodules-0.0.2/update_submodules/git.py`

 * *Files identical despite different names*

### Comparing `update-submodules-0.0.1/update_submodules/github.py` & `update-submodules-0.0.2/update_submodules/github.py`

 * *Files identical despite different names*

### Comparing `update-submodules-0.0.1/update_submodules/meta_branch.py` & `update-submodules-0.0.2/update_submodules/meta_branch.py`

 * *Files identical despite different names*

