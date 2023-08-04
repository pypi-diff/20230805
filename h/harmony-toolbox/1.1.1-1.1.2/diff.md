# Comparing `tmp/harmony_toolbox-1.1.1.tar.gz` & `tmp/harmony_toolbox-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony_toolbox-1.1.1.tar", last modified: Thu Jul 27 19:40:36 2023, max compression
+gzip compressed data, was "harmony_toolbox-1.1.2.tar", last modified: Fri Aug  4 20:04:01 2023, max compression
```

## Comparing `harmony_toolbox-1.1.1.tar` & `harmony_toolbox-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:36.075226 harmony_toolbox-1.1.1/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/LICENSE
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/MANIFEST.in
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-27 19:40:36.076226 harmony_toolbox-1.1.1/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/README.md
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/pyproject.toml
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.1.1/requirements.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-07-27 19:40:36.084222 harmony_toolbox-1.1.1/setup.cfg
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/setup.py
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:35.566121 harmony_toolbox-1.1.1/src/
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:35.872225 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/SOURCES.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/dependency_links.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:36.034226 harmony_toolbox-1.1.1/src/toolbox/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.1.1/src/toolbox/__init__.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-07-27 19:37:57.000000 harmony_toolbox-1.1.1/src/toolbox/config.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    49984 2023-07-27 18:03:40.000000 harmony_toolbox-1.1.1/src/toolbox/library.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    31224 2023-07-27 17:44:47.000000 harmony_toolbox-1.1.1/src/toolbox/toolbox.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 20:04:01.981562 harmony_toolbox-1.1.2/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.2/LICENSE
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.2/MANIFEST.in
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-04 20:04:01.982563 harmony_toolbox-1.1.2/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.2/README.md
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.2/pyproject.toml
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.1.2/requirements.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-08-04 20:04:01.989565 harmony_toolbox-1.1.2/setup.cfg
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.2/setup.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 20:04:01.564628 harmony_toolbox-1.1.2/src/
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 20:04:01.816834 harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-04 20:04:01.000000 harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-08-04 20:04:01.000000 harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-08-04 20:04:01.000000 harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-08-04 20:04:01.000000 harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 20:04:01.948869 harmony_toolbox-1.1.2/src/toolbox/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.1.2/src/toolbox/__init__.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-08-04 19:22:49.000000 harmony_toolbox-1.1.2/src/toolbox/config.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    49277 2023-08-04 19:36:44.000000 harmony_toolbox-1.1.2/src/toolbox/library.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    32807 2023-08-04 19:59:21.000000 harmony_toolbox-1.1.2/src/toolbox/toolbox.py
```

### Comparing `harmony_toolbox-1.1.1/LICENSE` & `harmony_toolbox-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.1.1/PKG-INFO` & `harmony_toolbox-1.1.2/src/harmony_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: harmony_toolbox
-Version: 1.1.1
+Name: harmony-toolbox
+Version: 1.1.2
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.1.1/README.md` & `harmony_toolbox-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.1.1/setup.cfg` & `harmony_toolbox-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = harmony_toolbox
-version = 1.1.1
+version = 1.1.2
 author = EasyNode.PRO
 author_email = support@easynode.pro
 description = Harmony ONE Validator Node Toolbox and Easy Setup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-node-pro/harmony-toolbox
 project_urls =
```

### Comparing `harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/PKG-INFO` & `harmony_toolbox-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: harmony-toolbox
-Version: 1.1.1
+Name: harmony_toolbox
+Version: 1.1.2
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.1.1/src/toolbox/config.py` & `harmony_toolbox-1.1.2/src/toolbox/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     except requests.exceptions.RequestException as x:
         print(type(x), x)
         result = "0.0.0.0"
     return result
 
 
 class EnvironmentVariables:
-    easy_version = "1.1.1"
+    easy_version = "1.1.2"
     server_host_name = socket.gethostname()
     user_home_dir = path.expanduser("~")
     dotenv_file = f"{user_home_dir}/.easynode.env"
     active_user = path.split(user_home_dir)[-1]
     harmony_dir = environ.get("HARMONY_DIR") or f"{user_home_dir}/harmony"
     bls_key_file = path.join(harmony_dir, "blskey.pass")
     hmy_app = path.join(harmony_dir, "hmy")
```

### Comparing `harmony_toolbox-1.1.1/src/toolbox/library.py` & `harmony_toolbox-1.1.2/src/toolbox/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         )
         print_stars()
         raise SystemExit(0)
 
 
 # Install Harmony ONE
 def install_hmy():
-    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
-    os.system(f"curl -LO https://harmony.one/hmycli && mv hmycli hmy && chmod +x hmy")
+    os.chdir(f"{environ.get('HARMONY_DIR')}")
+    process_command(f"curl -LO https://harmony.one/hmycli && mv hmycli hmy && chmod +x hmy")
     print_stars()
     print("* hmy application installed.")
 
 
 # Code to update the harmony.conf after an upgrade and other text files.
 def update_text_file(fileName, originalText, newText):
     with open(fileName, "r") as f:
@@ -143,27 +143,27 @@
     return
 
 
 def pull_harmony_update(harmony_dir, harmony_conf):
     arch = os.uname().machine
     os.chdir(f"{harmony_dir}")
     if environ.get("NETWORK") == "testnet":
-        os.system("curl -LO https://harmony.one/binary_testnet && mv binary_testnet harmony && chmod +x harmony")
-        os.system("./harmony config dump --network testnet harmony.conf")
+        process_command("curl -LO https://harmony.one/binary_testnet && mv binary_testnet harmony && chmod +x harmony")
+        process_command("./harmony config dump --network testnet harmony.conf")
     if environ.get("NETWORK") == "mainnet":
         if arch.startswith("arm"):
-            os.system("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
+            process_command("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
         if arch == "x86_64":
-            os.system("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
-        os.system("./harmony config dump harmony.conf")
+            process_command("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
+        process_command("./harmony config dump harmony.conf")
     update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     update_text_file(harmony_conf, " DisablePrivateIPScan = false", " DisablePrivateIPScan = true")
     print_stars()
     print("* harmony.conf MaxKeys modified to 13 & DisablePrivateIPScan set to true.")
-    if os.path.isfile(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
+    if os.path.isfile(f"{environ.get('HARMONY_DIR')}/blskey.pass"):
         update_text_file(harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
         print("* blskey.pass found, updated harmony.conf")
     print_stars()
     print(f"* Harmony {environ.get('NETWORK')} application installed & ~/harmony/harmony.conf created. ")
     return
 
 
@@ -204,26 +204,27 @@
         folders["harmony3"] = port
         print(f"* Found ~/harmony3 folder, on port {port}")
     print_stars()
     return folders
 
 
 def validator_stats_output(folders) -> None:
+    config = EnvironmentVariables()
     # Get server stats & wallet balances
     load_1, load_5, load_15 = os.getloadavg()
     sign_percentage = get_sign_pct()
     total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
     # Print Menu
     print_stars()
     print(
         f"{Fore.GREEN}* harmony-toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{EnvironmentVariables.easy_version}{Style.RESET_ALL}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*"
     )
     print_stars()
     print(
-        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {EnvironmentVariables.server_host_name} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {EnvironmentVariables.server_host_name} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
     for folder in folders:
         harmony_service_status(folder)
     print(
         f"* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current user home dir free space: {Fore.CYAN}{free_space_check(EnvironmentVariables.user_home_dir): >6}{Fore.GREEN}"
     )
     print(
@@ -331,15 +332,15 @@
         validator_wallet = environ.get("VALIDATOR_WALLET")
         return validator_wallet
 
 
 def get_db_size(harmony_dir, our_shard) -> str:
     harmony_db_size = subprocess.getoutput(f"du -h {harmony_dir}/harmony_db_{our_shard}")
     harmony_db_size = harmony_db_size.rstrip("\t")
-    countTrim = len(os.environ.get("HARMONY_DIR")) + 13
+    countTrim = len(environ.get("HARMONY_DIR")) + 13
     return harmony_db_size[:-countTrim]
 
 
 def recovery_type():
     print_stars()
     print("* Wallet Recovery Type!                                                                     *")
     print_stars()
@@ -353,50 +354,50 @@
     terminal_menu = TerminalMenu(
         menu_options, title="* Which type of restore method would you like to use for your validator wallet?"
     )
     results = terminal_menu.show()
     passphrase_set()
     if results == 0:
         # Mnemonic Recovery Here
-        os.system(
+        process_command(
             f"{environ.get('HARMONY_DIR')}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
         )
         print_stars()
         set_wallet_env()
     elif results == 1:
         # Private Key Recovery Here
         print("* Private key recovery requires your private information in the command itself.")
         private = input("* Please enter your private key to restore your wallet: ")
-        os.system(
+        process_command(
             f"{environ.get('HARMONY_DIR')}/hmy keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
         )
         print_stars()
         set_wallet_env()
 
 
 def passphrase_status():
     load_var_file(EnvironmentVariables.dotenv_file)
     if os.path.exists(EnvironmentVariables.hmy_wallet_store):
         passphrase_set()
         set_var(
             EnvironmentVariables.dotenv_file,
             "PASS_SWITCH",
-            f"--passphrase-file {os.environ.get('HARMONY_DIR')}/passphrase.txt",
+            f"--passphrase-file {environ.get('HARMONY_DIR')}/passphrase.txt",
         )
     else:
         set_var(EnvironmentVariables.dotenv_file, "PASS_SWITCH", "--passphrase")
     load_var_file(EnvironmentVariables.dotenv_file)
 
 
 def passphrase_set():
     if os.path.exists(f"{environ.get('HARMONY_DIR')}/passphrase.txt"):
         return
     import getpass
 
-    print(f"* Setup {os.environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.")
+    print(f"* Setup {environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.")
     print_stars()
     # take input
     while True:
         print("* ")
         password_1 = getpass.getpass(
             prompt="* Please set a wallet password for this node\n* Enter your password now: ", stream=None
         )
@@ -508,29 +509,21 @@
     print("* Edit ~/.easynode.env and add your wallet address on a new line like this example:         *")
     print("* VALIDATOR_WALLET='one1thisisjustanexamplewalletreplaceme'                                 *")
     print_stars()
     raise SystemExit(0)
 
 
 def get_validator_info():
-    if environ.get("NETWORK") == "mainnet":
-        endpoint = len(EnvironmentVariables.rpc_endpoints)
-    if environ.get("NETWORK") == "testnet":
-        endpoint = len(EnvironmentVariables.rpc_endpoints_test)
-    current = 0
-    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
+    config = EnvironmentVariables()
     validator_data = -1
-
-    while current < max_tries:
-        try:
-            validator_data = staking.get_validator_information(environ.get("VALIDATOR_WALLET"), endpoint)
-            return validator_data
-        except Exception:
-            current += 1
-            continue
+    try:
+        validator_data = staking.get_validator_information(environ.get("VALIDATOR_WALLET"), config.working_rpc_endpoint)
+        return validator_data
+    except Exception:
+        current += 1
 
     return validator_data
 
 
 def current_price():
     try:
         response = requests.get(EnvironmentVariables.onePriceURL, timeout=5)
@@ -548,55 +541,37 @@
     rpc_endpoint = config.working_rpc_endpoint
     wallet_balance = get_wallet_balance_by_endpoint(rpc_endpoint, wallet_addr)
     if wallet_balance is not None:
         return wallet_balance
 
 
 def get_wallet_balance_by_endpoint(endpoint, wallet_addr):
-    current = 0
-    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     get_balance = 0
 
-    while current < max_tries:
-        try:
-            get_balance = pyhmy.numbers.convert_atto_to_one(account.get_balance(wallet_addr, endpoint))
-            return get_balance
-        except Exception:
-            current += 1
-            continue
+    try:
+        get_balance = pyhmy.numbers.convert_atto_to_one(account.get_balance(wallet_addr, endpoint))
+        return get_balance
+    except Exception:
+        return get_balance
 
-    return get_balance
 
 
 def get_rewards_balance(endpoint, wallet_addr):
-    endpoints_count = len(endpoint)
-
-    for i in range(endpoints_count):
-        wallet_balance = get_rewards_balance_by_endpoint(endpoint[i], wallet_addr)
-
-        if wallet_balance >= 0:
-            return wallet_balance
-
-    raise ConnectionError("Couldn't fetch RPC data for current epoch.")
-
-
-def get_rewards_balance_by_endpoint(endpoint, wallet_addr):
-    current = 0
-    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
     totalRewards = 0
-
     try:
         validator_rewards = staking.get_delegations_by_delegator(wallet_addr, endpoint)
-    except Exception:
+    except (Exception, ConnectionError) as e:
         return totalRewards
 
     for i in validator_rewards:
         totalRewards = totalRewards + i["reward"]
     totalRewards = pyhmy.numbers.convert_atto_to_one(totalRewards)
-    return totalRewards
+    
+    if totalRewards >= 0:
+        return totalRewards
 
 
 def save_json(fn: str, data: dict) -> dict:
     with open(fn, "w") as j:
         dump(data, j, indent=4)
 
 
@@ -786,114 +761,117 @@
                 f"* Are you sure you want to isntall into the already existing folder {answer}? (YES/NO) "
             )
             if question:
                 set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
             else:
                 install_harmony()
         set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
-        os.system(f"sudo mkdir -p {os.environ.get('HARMONY_DIR')}")
-        os.system(f"sudo chown {EnvironmentVariables.active_user} {os.environ.get('HARMONY_DIR')}")
+        process_command(f"sudo mkdir -p {environ.get('HARMONY_DIR')}")
+        process_command(f"sudo chown {EnvironmentVariables.active_user} {environ.get('HARMONY_DIR')}")
     print_stars()
     print("* Creating all Harmony Files & Folders")
-    os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
+    process_command(f"mkdir -p {environ.get('HARMONY_DIR')}/.hmy/blskeys")
 
     # Setup folders now that symlink exists or we know we're using ~/harmony
     if not os.path.isdir(f"{EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/"):
-        os.system(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
-    if not os.path.isdir(f"{os.environ.get('HARMONY_DIR')}/.hmy/blskeys"):
+        process_command(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
+    if not os.path.isdir(f"{environ.get('HARMONY_DIR')}/.hmy/blskeys"):
         print("* Creating all Harmony Files & Folders")
-        os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
+        process_command(f"mkdir -p {environ.get('HARMONY_DIR')}/.hmy/blskeys")
     # Change to ~/harmony folder
-    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
+    os.chdir(f"{environ.get('HARMONY_DIR')}")
     print_stars()
     # Install hmy
     install_hmy()
     print_stars()
     # Install harmony
-    pull_harmony_update(os.environ.get("HARMONY_DIR"), f"{os.environ.get('HARMONY_DIR')}/harmony.conf")
+    pull_harmony_update(environ.get("HARMONY_DIR"), f"{environ.get('HARMONY_DIR')}/harmony.conf")
     # install hmy files
     print("* Installing rclone application & rclone configuration files")
     print_stars()
     # check for working rclone site and download
     try:
-        os.system("curl https://rclone.org/install.sh | sudo bash")
+        process_command("curl https://rclone.org/install.sh | sudo bash")
     except (ValueError, KeyError, TypeError):
         result = ask_yes_no(
             "* rclone site is offline, we can install rclone from the Ubuntu repo as a workaround, do you want to continue? (Y/N): "
         )
         if result:
             # If rclone curl is down, install rclone with apt instead
             subprocess.run("sudo apt install rclone -y")
 
-    os.system(
+    process_command(
         f"mkdir -p {EnvironmentVariables.user_home_dir}/.config/rclone && cp {EnvironmentVariables.toolbox_location}/src/bin/rclone.conf {EnvironmentVariables.user_home_dir}/.config/rclone/"
     )
     print_stars()
     # Setup the harmony service file
     print("* Customizing, Moving & Enabling your harmony.service systemd file")
+    
+    # Set initial file for customization
     service_file_path = f"{EnvironmentVariables.toolbox_location}/src/bin/harmony.service"
     
     # Read the service file
     with open(service_file_path, 'r') as file:
         filedata = file.read()
 
     # Replace the paths with the value of HARMONY_DIR
-    harmony_dir = os.environ.get("HARMONY_DIR")
+    harmony_dir = environ.get("HARMONY_DIR")
     if harmony_dir:
         filedata = filedata.replace('WorkingDirectory=/home/serviceharmony/harmony', f'WorkingDirectory={harmony_dir}')
         filedata = filedata.replace('ExecStart=/home/serviceharmony/harmony/harmony -c harmony.conf', f'ExecStart={harmony_dir}/harmony -c harmony.conf')
 
     # Write the file out again
     with open('harmony.service', 'w') as file:
         file.write(filedata)
 
     # Move the modified service file into place, change the permissions and enable the service
+    # Update these steps in the future to use a dynamic harmony.service name?
     subprocess.run(['sudo', 'mv', 'harmony.service', '/etc/systemd/system/harmony.service'], check=True)
     subprocess.run(['sudo', 'chmod', 'a-x', '/etc/systemd/system/harmony.service'], check=True)
     subprocess.run(['sudo', 'systemctl', 'enable', 'harmony.service'], check=True)
 
 
 # Database Downloader
 def clone_shards():
     # Move to ~/harmony
-    os.chdir(f"{os.environ.get('HARMONY_DIR')}")
+    os.chdir(f"{environ.get('HARMONY_DIR')}")
 
     if environ.get("SHARD") != "0":
         # If we're not on shard 0, download the numbered shard DB here.
         print(f"* Now cloning shard {environ.get('SHARD')}")
         print_stars()
-        os.system(
-            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {os.environ.get('HARMONY_DIR')}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
+        process_command(
+            f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {environ.get('HARMONY_DIR')}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
         )
         print_stars()
         print(f"* Shard {environ.get('SHARD')} completed.\n* Shard 0 will be created when you start your service.")
         print_stars()
     else:
         # If we're on shard 0, grab the snap DB here.
         print("* Now cloning Shard 0, kick back and relax for awhile...")
         print_stars()
-        os.system(
-            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {os.environ.get('HARMONY_DIR')}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
+        process_command(
+            f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {environ.get('HARMONY_DIR')}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
         )
 
 
 # is this used?
 def set_mounted_point():
     # First let's make sure your volume is mounted
     totalDir = len(os.listdir("/mnt"))
     if totalDir > 0:
         volumeMountPath = os.listdir("/mnt")
         myVolumePath = "/mnt/" + str(volumeMountPath[0])
         myLongHmyPath = myVolumePath + "/harmony"
     else:
-        myVolumePath = os.environ.get("HARMONY_DIR")
+        myVolumePath = environ.get("HARMONY_DIR")
     if totalDir == 1:
         dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", myLongHmyPath)
     else:
-        dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{os.environ.get('HARMONY_DIR')}")
+        dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{environ.get('HARMONY_DIR')}")
 
 
 def finish_node_install():
     load_var_file(EnvironmentVariables.dotenv_file)
     print_stars()
     print(
         "* Installation is completed"
@@ -1166,15 +1144,15 @@
         Fore.RED
         + "WARNING: YOU WILL MISS BLOCKS WHILE YOU REBOOT YOUR ENTIRE SERVER.\n\n"
         + "Reconnect after a few moments & Run the Validator Toolbox Menu again with: python3 ~/harmony-toolbox/start.py\n"
         + Fore.WHITE
         + "Are you sure you would like to proceed with rebooting your server?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
-        os.system("sudo reboot")
+        process_command("sudo reboot")
     else:
         print("Invalid option.")
 
 
 def finish_node():
     print(
         "* Thanks for using Easy Node Toolbox - Making everything Easy Mode!"
```

### Comparing `harmony_toolbox-1.1.1/src/toolbox/toolbox.py` & `harmony_toolbox-1.1.2/src/toolbox/toolbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     recover_wallet,
     refreshing_stats_message,
     passphrase_status
 )
 
 
 def parse_flags(parser):
+    config = EnvironmentVariables()
     print_stars()
     # Add the arguments
     parser.add_argument(
         "-s",
         "--stats",
         action="store_true",
         help="Run your stats if Harmony is installed and running.",
@@ -95,93 +96,117 @@
         update_harmony_app()
 
     if args.stats:
         run_multistats()
         finish_node()
 
     if args.collect:
-        rewards_collector(EnvironmentVariables.hmy_app, True)
+        rewards_collector(config.working_rpc_endpoint)
         finish_node()
 
     if args.collect_send:
-        rewards_collector(EnvironmentVariables.hmy_app, True, True)
+        rewards_collector(config.working_rpc_endpoint, True)
         finish_node()
 
 
 def run_multistats():
     refreshing_stats_message()
     folders = get_folders()
     validator_stats_output(folders)
     return
 
 
 def collect_rewards(networkCall):
-    os.system(
+    process_command(
         f"{networkCall} staking collect-rewards --delegator-addr {environ.get('VALIDATOR_WALLET')} --gas-price 100 {environ.get('PASS_SWITCH')}"
     )
 
 
 def send_rewards(networkCall, sendAmount, rewards_wallet):
-    os.system(
+    process_command(
         f"{networkCall} transfer --amount {sendAmount} --from {environ.get('VALIDATOR_WALLET')} --from-shard 0 --to {rewards_wallet} --to-shard 0 --gas-price 100 {environ.get('PASS_SWITCH')}"
     )
+    
+    
+def send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet, bypass = False):
+    if bypass == False:
+        print("*\n*\n")
+        print_stars()
+        print("\n* Send your Harmony ONE Rewards?")
+        print_stars()
+        question = ask_yes_no(
+            f"* You have {validator_wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
+        )
+        if question == False: 
+            print("*\n*\n* Skipping sending of rewards.\n")
+            return
+    print(f"*\n*\n* Sending {suggested_send} $ONE Rewards to {rewards_wallet}, awaiting confirmation...\n")
+    send_rewards(EnvironmentVariables.hmy_app, suggested_send, rewards_wallet)
+    validator_wallet_balance = get_wallet_balance(validator_wallet)
+    rewards_wallet_balance = get_wallet_balance(rewards_wallet)
+    print(f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*")
+    print(f"*\n*\n* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*\n*")
+    return
+
+
+def rewards_sender(
+    rewards_wallet=environ.get("REWARDS_WALLET"),
+    validator_wallet=environ.get("VALIDATOR_WALLET"),
+) -> None:
+    validator_wallet_balance = get_wallet_balance(validator_wallet)
+    suggested_send = validator_wallet_balance - int(environ.get("GAS_RESERVE"))
+    if suggested_send >= 1:
+        send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet)
+    else:
+        print("*\n* Wallet balance is less than your gas reservation, please try again later.\n*\n")
+    validator_wallet_balance = get_wallet_balance(validator_wallet)
+    rewards_wallet_balance = get_wallet_balance(rewards_wallet)
+    print(f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*\n* Current Rewards Wallet Balance: {rewards_wallet_balance}\n*\n*")
+    return
 
 
 def rewards_collector(
     rpc,
     bypass=False,
-    send_out_rewards=False,
     rewards_wallet=environ.get("REWARDS_WALLET"),
     validator_wallet=environ.get("VALIDATOR_WALLET"),
 ) -> None:
+    print_stars()
     print("* Harmony ONE Rewards Collection")
     print_stars()
     if bypass == False:
         question = ask_yes_no(
             f"*\n* For your validator wallet {validator_wallet}\n* You have {get_rewards_balance(rpc, validator_wallet)} $ONE pending.\n* Would you like to collect your rewards on the Harmony mainnet? (YES/NO) "
         )
-        bypass = True
-    if bypass:
+        if question:
+            bypass = True
+        else:
+            print("*\n*\n* Skipping collection of rewards.\n")
+    if bypass == True:
         collect_rewards(EnvironmentVariables.hmy_app)
         print_stars()
         print(
             Fore.GREEN + f"* mainnet rewards for {validator_wallet} have been collected." + Style.RESET_ALL + Fore.GREEN
         )
         print_stars()
-    else:
-        return
-    wallet_balance = get_wallet_balance(validator_wallet)
-    suggested_send = wallet_balance - int(environ.get("GAS_RESERVE"))
+    validator_wallet_balance = get_wallet_balance(validator_wallet)
+    suggested_send = validator_wallet_balance - int(environ.get("GAS_RESERVE"))
     if suggested_send >= 1:
-        if send_rewards == False:
-            print("*\n*\n")
-            print_stars()
-            print("\n* Send your Harmony ONE Rewards?")
-            print_stars()
-            question = ask_yes_no(
-                f"* You have {wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
-            )
-            if question:
-                send_out_rewards = True
-        if send_out_rewards:
-            print("*\n*\n")
-            print_stars()
-            print("\n* Sending your Harmony ONE Rewards, awaiting confirmation...")
-            print_stars()
-            send_rewards(EnvironmentVariables.hmy_app, suggested_send, rewards_wallet)
-        wallet_balance = get_wallet_balance(validator_wallet)
-        print(f"*\n*\n* Current Wallet Balance: {wallet_balance} $ONE\n*\n*")
-        return
+        send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet, bypass)
     else:
-        wallet_balance = get_wallet_balance(validator_wallet)
-        print(f"*\n*\n* Current Wallet Balance: {wallet_balance} $ONE\n*\n*")
-        return
+        validator_wallet_balance = get_wallet_balance(validator_wallet)
+        rewards_wallet_balance = get_wallet_balance(rewards_wallet)
+        print(f"*\n*\n* Balance too low to send to rewards wallet\n")
+        print(f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*")
+        print(f"* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*\n*")
+    return
 
 
 def menu_topper_regular(software_versions) -> None:
+    config = EnvironmentVariables()
     # Get stats & balances
     try:
         load_1, load_5, load_15 = os.getloadavg()
         sign_percentage = get_sign_pct()
         total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
         remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
     except (ValueError, KeyError, TypeError) as e:
@@ -189,15 +214,15 @@
     # Print Menu
     print_stars()
     print(
         f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
     )
     print_stars()
     print(
-        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
     harmony_service_status(environ.get("SERVICE_NAME", "harmony"))
     print(
         f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(os.environ.get("HARMONY_DIR")): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
     )
     print_stars()
     if environ.get("SHARD") != "0":
@@ -325,27 +350,29 @@
 
 def drive_check() -> None:
     server_drive_check(EnvironmentVariables.dotenv_file, os.environ.get("HARMONY_DIR"))
     return
 
 
 def run_check_balance() -> None:
-    menu_check_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET"))
+    config = EnvironmentVariables()
+    menu_check_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET"))
 
 
 def bingo_checker():
-    os.system(f"grep BINGO {os.environ.get('HARMONY_DIR')}/latest/zerolog-harmony.log | tail -10")
+    process_command(f"grep BINGO {os.environ.get('HARMONY_DIR')}/latest/zerolog-harmony.log | tail -10")
     print_stars()
     print("* Press enter to return to the main menu.")
     print_stars()
     input()
 
 
 def run_rewards_collector() -> None:
-    rewards_collector(EnvironmentVariables.hmy_app)
+    config = EnvironmentVariables()
+    rewards_collector(config.working_rpc_endpoint)
     return
 
 
 def safety_defaults() -> None:
     # default settings section
     set_var(EnvironmentVariables.dotenv_file, "EASY_VERSION", EnvironmentVariables.easy_version)
     if environ.get("GAS_RESERVE") is None:
@@ -436,19 +463,19 @@
 
 
 def run_regular_node(software_versions) -> None:
     menu_options = {
         0: finish_node,
         1: refreshing_stats_message,
         2: menu_active_bls,
-        3: coming_soon,
+        3: bingo_checker,
         4: run_rewards_collector,
-        5: bingo_checker,
-        6: coming_soon,
-        7: set_rewards_wallet,
+        5: rewards_sender,
+        6: set_rewards_wallet,
+        7: coming_soon,
         8: menu_service_stop_start,
         9: menu_service_restart,
         10: harmony_binary_upgrade,
         11: hmy_cli_upgrade,
         12: menu_ubuntu_updates,
         13: drive_check,
         14: tmi_server_info,
@@ -506,90 +533,99 @@
                 print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
                 input()
                 start_regular_node()
 
 
 def service_menu_option() -> None:
-    status = os.system("systemctl is-active --quiet harmony")
+    status = process_command("systemctl is-active --quiet harmony")
     if status == 0:
         print(
             f"*   8 - {Fore.RED}Stop Harmony Service      {Fore.GREEN}- {Fore.YELLOW}{Back.RED}WARNING: You will miss blocks while stopped!   {Style.RESET_ALL}{Fore.GREEN}"
         )
         print(
             f"*   9 - Restart Harmony Service   - {Back.RED}{Fore.YELLOW}WARNING: You will miss blocks during a restart!{Style.RESET_ALL}{Fore.GREEN}"
         )
     else:
         print(f"*   8 - Start Harmony Service")
+    return
 
 
+def rewards_sender_option() -> None:
+    if environ.get("REWARDS_WALLET"):
+        print("*   5 - Send Wallet Balance       - Send your wallet balance - saved gas to rewards wallet")
+        print("*   6 - Set Rewards Wallet        - Update your saved wallet or gas reserve")   
+    else:
+        print("*   6 - Set Rewards Wallet        - Set up a one1 wallet address to send rewards when using option #4")   
+    return
+
 def make_backup_dir() -> str:
     folder_name = f'{os.environ.get("HARMONY_DIR")}/harmony_backup/{datetime.now().strftime("%Y%m%d%H%M")}'
-    os.system(f"mkdir -p {folder_name}")
+    process_command(f"mkdir -p {folder_name}")
     return folder_name
 
 
 def hmy_cli_upgrade():
     question = ask_yes_no(
         "* Are you sure you would like to proceed with updating the Harmony CLI file?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         folder_name = make_backup_dir()
-        os.system(f"cp {environ.get('HARMONY_DIR')}/hmy {folder_name}")
+        process_command(f"cp {environ.get('HARMONY_DIR')}/hmy {folder_name}")
         print_stars()
         install_hmy()
         print_stars()
         print("Harmony cli has been updated to: ")
-        os.system(f"{environ.get('HARMONY_DIR')}/hmy version")
+        process_command(f"{environ.get('HARMONY_DIR')}/hmy version")
         print_stars()
         set_var(EnvironmentVariables.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
         input("* Update completed, press ENTER to return to the main menu. ")
 
 
 def update_harmony_app():
     os.chdir(f"{os.environ.get('HARMONY_DIR')}")
     print_stars()
     print("Currently installed version: ")
-    os.system("./harmony -V")
+    process_command("./harmony -V")
     folder_name = make_backup_dir()
-    os.system(
+    process_command(
         f"cp {os.environ.get('HARMONY_DIR')}/harmony {os.environ.get('HARMONY_DIR')}/harmony.conf {folder_name}"
     )
     print_stars()
     print("Downloading current harmony binary file from harmony.one: ")
     print_stars()
     pull_harmony_update(
         os.environ.get("HARMONY_DIR"), EnvironmentVariables.harmony_conf
     )
     print_stars()
     print("Updated version: ")
-    os.system("./harmony -V")
+    process_command("./harmony -V")
     if environ.get("SHARD") != "0":
         size = 0
         for path, dirs, files in os.walk(f"{os.environ.get('HARMONY_DIR')}/harmony_db_0"):
             for f in files:
                 fp = os.path.join(path, f)
                 size += os.path.getsize(fp)
             if size >= 400000000:
                 question = ask_yes_no(
                     Fore.WHITE
                     + "* Are you sure you would like to proceed with upgrading and trimming database 0?\n\nType 'Yes' or 'No' to continue"
                 )
                 if question:
-                    os.system("sudo service harmony stop")
-                    os.system(
+                    process_command("sudo service harmony stop")
+                    process_command(
                         f"mv {os.environ.get('HARMONY_DIR')}/harmony_db_0 {os.environ.get('HARMONY_DIR')}/harmony_db_0_old"
                     )
-                    os.system("sudo service harmony start")
-                    os.system(f"rm -r {os.environ.get('HARMONY_DIR')}/harmony_db_0_old")
+                    process_command("sudo service harmony start")
+                    process_command(f"rm -r {os.environ.get('HARMONY_DIR')}/harmony_db_0_old")
                 else:
                     print("Skipping removal of 0, but it's no longer required, fyi!")
             else:
                 print("Your database 0 is already trimmed, enjoy!")
-    os.system("sudo service harmony restart")
+    process_command("sudo service harmony restart")
     print_stars()
     print("Harmony Service is restarting, waiting 10 seconds for restart.")
     set_var(EnvironmentVariables.dotenv_file, "HARMONY_UPGRADE_AVAILABLE", "False")
     time.sleep(10)
 
 
 def menu_validator_stats():
@@ -666,31 +702,31 @@
         + "* Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         update_harmony_app()
 
 
 def menu_service_stop_start() -> str:
-    status = os.system("systemctl is-active --quiet harmony")
+    status = process_command("systemctl is-active --quiet harmony")
     if status != 0:
-        os.system("sudo service harmony start")
+        process_command("sudo service harmony start")
         print()
         print("* Harmony Service Has Been Started.")
         print()
         input("* Press ENTER to return to the main menu.")
     else:
         question = ask_yes_no(
             "*********\n"
             + Fore.RED
             + "* WARNING: YOU WILL MISS BLOCKS IF YOU STOP THE HARMONY SERVICE.\n\n"
             + Fore.WHITE
             + "* Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
         )
         if question:
-            os.system("sudo service harmony stop")
+            process_command("sudo service harmony stop")
             print()
             print(
                 "* Harmony Service Has Been Stopped. "
                 + Fore.RED
                 + "YOU ARE MISSING BLOCKS ON THIS NODE."
                 + Style.RESET_ALL
                 + Fore.GREEN
@@ -704,15 +740,15 @@
         "*********\n"
         + Fore.RED
         + "WARNING: YOU WILL MISS BLOCKS UNTIL RESTART IS COMPLETED & SYNC CATCHES UP!\n\n"
         + Fore.WHITE
         + "Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
-        os.system("sudo service harmony restart")
+        process_command("sudo service harmony restart")
         print()
         print("* The Harmony Service Has Been Restarted")
         input("* Press ENTER to return to the main menu.")
 
 
 def menu_active_bls() -> str:
     validator_wallet = environ.get("VALIDATOR_WALLET")
@@ -773,35 +809,15 @@
         f"* The Mainnet Wallet Balance is: {total_balance} Harmony ONE Coins\n* The Testnet Wallet Balance is: {total_balance_test} Harmony ONE Test Coins"
     )
     print_stars()
     input("* Press ENTER to continue.")
 
 
 def get_current_epoch():
-    if environ.get("NETWORK") == "mainnet":
-        endpoints_count = len(EnvironmentVariables.rpc_endpoints)
-    if environ.get("NETWORK") == "testnet":
-        endpoints_count = len(EnvironmentVariables.rpc_endpoints_test)
-
-    for i in range(endpoints_count):
-        current_epoch = get_current_epochByEndpoint(EnvironmentVariables.rpc_endpoints[i])
-
-        if current_epoch != -1:
-            return current_epoch
+    config = EnvironmentVariables()
     current_epoch = 0
-    return current_epoch
-
-
-def get_current_epochByEndpoint(endpoint):
-    current = 0
-    max_tries = EnvironmentVariables.rpc_endpoints_max_connection_retries
-    current_epoch = -1
-
-    while current < max_tries:
-        try:
-            current_epoch = blockchain.get_current_epoch(endpoint)
-            return current_epoch
-        except Exception:
-            current += 1
-            continue
-
-    return current_epoch
+    try:
+        current_epoch = blockchain.get_current_epoch(config.working_rpc_endpoint)
+        return current_epoch
+    except Exception as e:
+        print(f"* Error getting current epoch: {e}")
+        return current_epoch
```

