# Comparing `tmp/ghast_scanner-1.4.6.tar.gz` & `tmp/ghast_scanner-1.4.7.tar.gz`

## Comparing `ghast_scanner-1.4.6.tar` & `ghast_scanner-1.4.7.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.pylintrc
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/__about__.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/colors.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/requirements.txt
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.github/workflows/ghast-scan.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-create-or-approves-pr-using-curl.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-creates-or-approves-pr-using-gh-cli.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-creates-or-approves-pr-using-gh-script.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-remote-script.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/__init__.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/analyzer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/analyzer_test.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/regex.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/images/ghast-stdout.png
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/LICENSE
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/README.md
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/.pylintrc
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/__about__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/colors.py
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/requirements.txt
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/.github/workflows/ghast-scan.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-create-or-approves-pr-using-curl.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-creates-or-approves-pr-using-gh-cli.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-creates-or-approves-pr-using-gh-script.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-remote-script.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/analyzer/__init__.py
+-rw-r--r--   0        0        0    15796 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/analyzer/analyzer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/analyzer/regex.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/LICENSE
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/README.md
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 ghast_scanner-1.4.7/PKG-INFO
```

### Comparing `ghast_scanner-1.4.6/action.yml` & `ghast_scanner-1.4.7/action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-name: "actions-security-analyzer"
-description: "Scan your GitHub actions folder for common security vulnerabilities"
+name: "ghast-scanner"
+description: "Scan your GitHub actions and environment for common security vulnerabilities"
 author: "bin3xish477"
 branding:
   icon: "shield"
   color: "green"
 inputs:
   dir:
     description: "path to directory with GitHub Actions files to scan"
```

### Comparing `ghast_scanner-1.4.6/colors.py` & `ghast_scanner-1.4.7/colors.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/main.py` & `ghast_scanner-1.4.7/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,17 @@
             if dir_.is_dir() and dir_.exists():
                 if verbose:
                     print(
                         f"{Colors.LIGHT_GRAY}INFO{Colors.END} "
                         f"Scanning {Colors.UNDERLINE}{dir_}{Colors.END} directory..."
                     )
                 for action in dir_.iterdir():
-                    print(f"File: {Colors.BOLD}{str(action).rsplit(sep, maxsplit=1)[-1]}{Colors.END}")
+                    print(
+                        f"FILE => {Colors.BOLD}{Colors.UNDERLINE}{str(action).rsplit(sep, maxsplit=1)[-1]}{Colors.END}"
+                    )
                     if action.is_file and action.suffix in (".yml", ".yaml"):
                         with action.open("r") as action_file:
                             action_dict = safe_load(action_file)
                             if not analyzer.run_checks(action=action_dict):
                                 failed_actions.append(action)
                             else:
                                 if verbose:
```

### Comparing `ghast_scanner-1.4.6/.github/workflows/ghast-scan.yml` & `ghast_scanner-1.4.7/.github/workflows/ghast-scan.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
   RunGhast:
     runs-on: ubuntu-latest
     steps:
       - name: "Checkout repo"
         uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
       - name: "Run Ghast"
-        uses: "bin3xish477/ghast@ee733379e314d44f1a960a70339ee5e5d19e404d"
+        uses: "bin3xish477/ghast@591140d3068c278519062744c180bd3198b7394c"
         with:
           dir: "./actions/"
           verbose: true
           #no-summary: true
           #ignore-checks: ''
           #ignore-warnings: true
         continue-on-error: true # adding this since this workflow is always expected to fail
```

### Comparing `ghast_scanner-1.4.6/actions/action-create-or-approves-pr-using-curl.yml` & `ghast_scanner-1.4.7/actions/action-create-or-approves-pr-using-curl.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `ghast_scanner-1.4.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/analyzer/analyzer.py` & `ghast_scanner-1.4.7/analyzer/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """analyzer.py contains all the INFOic related to analyzing GitHub Actions"""
 
 from re import search, DOTALL
+from pathlib import Path
 from colors import Colors
 
 import analyzer.regex
 
 
 class Analyzer:
     """Analyzer contains all the checks that will run
@@ -27,20 +28,25 @@
             "_check_for_cache_action_usage": {"level": "WARN"},
             "_check_for_dangerous_write_permissions": {"level": "FAIL"},
             "_check_for_inline_script": {"level": "WARN"},
             "_check_for_pull_request_target": {"level": "FAIL"},
             "_check_for_script_injection": {"level": "FAIL"},
             "_check_for_self_hosted_runners": {"level": "WARN"},
             "_check_for_aws_configure_credentials_non_oidc": {"level": "WARN"},
-            "_check_for_pull_request_create_or_approve": {"level": "FAIL"},
+            "_check_for_create_or_approve_pull_request": {"level": "FAIL"},
             "_check_for_remote_script": {"level": "WARN"},
         }
+        self.auxiliary_checks = [
+            "_check_for_codeowners_file",
+        ]
         self.action = {}
         self.jobs = {}
 
+        self._run_aux_checks()
+
     def _print_failed_check_msg(self, check: str, level: str):
         color = None
         if level == "FAIL":
             color = Colors.RED
         elif level == "WARN":
             color = Colors.LIGHT_GREEN
         print(
@@ -269,15 +275,15 @@
                                     print(
                                         f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step not using OIDC with `configure-aws-credentials`"
                                     )
                         if passed:
                             passed = False
         return passed
 
-    def _check_for_pull_request_create_or_approve(self) -> bool:
+    def _check_for_create_or_approve_pull_request(self) -> bool:
         passed = True
 
         def __print_msg(job: str, step: dict):
             if self.verbose:
                 if "name" in step:
                     print(
                         f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') has a step('{step['name']}') that creates or approves a pull request"
@@ -305,14 +311,36 @@
                             script = step["with"]["script"]
                             match = search(analyzer.regex.GITHUB_SCRIPT_CREATE_APPROVE_PR, script, flags=DOTALL)
                             if match:
                                 __print_msg(job, step)
                                 passed = False
         return passed
 
+    # ==================================================================
+    # ======================== Auxiliary Checks ========================
+    # ==================================================================
+
+    def _check_for_codeowners_file(self) -> bool:
+        if not Path(".github/workflows/CODEOWNERS").exists():
+            print(
+                f"{Colors.LIGHT_BLUE}AUXI{Colors.END} missing CODEOWNERS file"
+                "which can provide additional protections for your workflow files"
+            )
+        else:
+            if self.verbose:
+                print(f"{Colors.LIGHT_BLUE}AUXI{Colors.END} found CODEOWNERS file")
+
+    def _run_aux_checks(self) -> None:
+        """Runs auxiliary checks which are checks for security-related
+        configurations/properties/mechanisms that contribute to more secure
+        GitHub Actions workflows.
+        """
+        for check in self.auxiliary_checks:
+            Analyzer.__dict__[check](self)
+
     def get_checks(self) -> list:
         """Returns list containing available checks.
 
         Returns:
             list: list() of available checks.
         """
         return [*self.checks.keys()]
@@ -340,9 +368,8 @@
                     continue
                 if not Analyzer.__dict__[check](self):
                     fail_checks.append(check)
                     if passed_all_checks:
                         passed_all_checks = False
             for check in fail_checks:
                 self._print_failed_check_msg(check, self.checks[check]["level"])
-
         return passed_all_checks
```

### Comparing `ghast_scanner-1.4.6/analyzer/analyzer_test.py` & `ghast_scanner-1.4.7/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/analyzer/regex.py` & `ghast_scanner-1.4.7/analyzer/regex.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/.gitignore` & `ghast_scanner-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/LICENSE` & `ghast_scanner-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/README.md` & `ghast_scanner-1.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ghast
 
-GHAST (GitHub Actions Static Analysis Tool) is a tool to analyze the security posture of your GitHub Actions.
+GHAST (GitHub Actions Static Analysis Tool) is a tool to analyze the security posture of your GitHub Actions and its surronding environment for common security vulnerabilities or missing security configuration.
+
+<img width="936" alt="image" src="https://github.com/bin3xish477/ghast/assets/44281620/721432ca-7944-40b4-803d-8c3cb866996e">
 
-![ghast-stdout](/images/ghast-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
 pip install ghast-scanner
@@ -37,15 +38,15 @@
 jobs:
   RunGhast:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run Ghast"
-      uses: "bin3xish477/ghast@ee733379e314d44f1a960a70339ee5e5d19e404d"
+      uses: "bin3xish477/ghast@591140d3068c278519062744c180bd3198b7394c"
       with:
         dir: "./actions/"
         verbose: true
         no-summary: true
         ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
 ```
 
@@ -83,15 +84,15 @@
 
     - This checks attempts to identify the usage of self-hosted runners. Self-hosted runners are dangerous because if the Action is compromised it may allow a threat actor to gain access to on premise environment or establish persistence mechanisms on a server you own/rent.
 
 9. Name: `check_for_aws_configure_credentials_non_oidc`, Level: `WARN`
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
-10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
+10. Name: `check_for_create_or_approve_pull_request`, Level: `WARN`
 
     - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
 
 11. Name: `check_for_remote_script`, Level: `WARN`
 
     - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
 ### References
```

### Comparing `ghast_scanner-1.4.6/pyproject.toml` & `ghast_scanner-1.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.6/PKG-INFO` & `ghast_scanner-1.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghast-scanner
-Version: 1.4.6
+Version: 1.4.7
 Summary: Analyze the security posture of your GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/ghast#readme
 Project-URL: Issues, https://github.com/bin3xish477/ghast/issues
 Project-URL: Source, https://github.com/bin3xish477/ghast
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -23,17 +23,18 @@
 Requires-Dist: pluggy==1.2.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: pyyaml==6.0
 Description-Content-Type: text/markdown
 
 # ghast
 
-GHAST (GitHub Actions Static Analysis Tool) is a tool to analyze the security posture of your GitHub Actions.
+GHAST (GitHub Actions Static Analysis Tool) is a tool to analyze the security posture of your GitHub Actions and its surronding environment for common security vulnerabilities or missing security configuration.
+
+<img width="936" alt="image" src="https://github.com/bin3xish477/ghast/assets/44281620/721432ca-7944-40b4-803d-8c3cb866996e">
 
-![ghast-stdout](/images/ghast-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
 pip install ghast-scanner
@@ -64,15 +65,15 @@
 jobs:
   RunGhast:
     runs-on: ubuntu-latest
     steps:
     - name: "Checkout repo"
       uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
     - name: "Run Ghast"
-      uses: "bin3xish477/ghast@ee733379e314d44f1a960a70339ee5e5d19e404d"
+      uses: "bin3xish477/ghast@591140d3068c278519062744c180bd3198b7394c"
       with:
         dir: "./actions/"
         verbose: true
         no-summary: true
         ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
 ```
 
@@ -110,15 +111,15 @@
 
     - This checks attempts to identify the usage of self-hosted runners. Self-hosted runners are dangerous because if the Action is compromised it may allow a threat actor to gain access to on premise environment or establish persistence mechanisms on a server you own/rent.
 
 9. Name: `check_for_aws_configure_credentials_non_oidc`, Level: `WARN`
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
-10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
+10. Name: `check_for_create_or_approve_pull_request`, Level: `WARN`
 
     - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
 
 11. Name: `check_for_remote_script`, Level: `WARN`
 
     - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
 ### References
```

